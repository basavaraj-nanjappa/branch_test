## Test core branches

```
Initial commits in main branch
tag main branch as rel-base-r01 (usually previous branch)
Create integration-rel-r01 fromt the main branch
Start a new sprint rel-r01-s01 on integration branch integration-rel-r01
    Create epic-01
        feat-sw-e01-f01
            commit 1
            commit 2
            commit 3
            raise PR to epic-01 and merge
        feat-sw-e01-f02
            commit 1
            commit 2
            raise PR to epic-01 and merge
    Create feat-sw-df01
        commit 1
        commit 2
        commit 3
        commit 4
        commit 5
        Riase PR to integration branch integration-rel-r01 and merge
    Create hotfix-SW-x01
        commit 1
        commit 2
        Raise PR to main and merge
        Release
        Raise PR to integration branch integration-rel-r01 and merge
End of sprint, Code-freeze
	tag integration branch for the codefreez
	create new release branch off the main release-rel-r01-date01
	raise PR from integration branch integration-rel-r01 to release branch and merge
	raise PR from release branch release-rel-r01-date01 to main branch and merge
	tag main branch for the new release release-rel-r01-date01

------------

Start a new sprint rel-r01-s02
    changes to epic-01
        rebase epic-01 with changes from integration branch integration-rel-r01
        Create 
            commit 1        
        commit 1
        commit 2
        Checkout feat-sw-e01-f03
            commit 2
            raise PR to epic-01 and merge
        Create feat-sw-e01-f04
            commit 1
            commit 2
            raise PR to epic-01 and merge
        raise PR to merge to integration branch integration-rel-r01 and merge
    Create epic-02
        commit 1
        create feat-sw-e02-f01
            commit 1
            commit 2
            raise PR to epic-02 and merge
        create feat-sw-e02-f02
            commit 1
            commit 2
            commit 3
            raise PR to epic-02 and merge
        rebase from integration branch integration-rel-r01
        raise PR to integration branch integration-rel-r01 and merge
    Create feat-sw-df02
        commit 1
        commit 2
        commit 3
    Create feat-sw-df03
        commit 1
        commit 2
        commit 3
        commit 4
        commit 5
End of sprint, Code-freeze
	tag integration branch for the codefreez
	create new release branch off the main release-rel-r01-date02
	raise PR from integration branch integration-rel-r01 to release branch and merge
    Fix to release
        emulate a fix to release by create a new feature branch off the integration branch
        crreate feat-sw-df03
            commit 1
            commit 2
            raise PR to integration branch integration-rel-r01 and merge
	raise PR from release branch release-rel-r01-date02 to main branch and merge
	tag main branch for the new release release-r01-date02
    

```