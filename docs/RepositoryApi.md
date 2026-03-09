# RepositoryApi

All URIs are relative to */api/v1*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**acceptRepoTransfer**](RepositoryApi.md#acceptRepoTransfer) | **POST** /repos/{owner}/{repo}/transfer/accept | Accept a repo transfer |
| [**actionRun**](RepositoryApi.md#actionRun) | **GET** /repos/{owner}/{repo}/actions/runs/{run_id} | Get an action run |
| [**createCurrentUserRepo**](RepositoryApi.md#createCurrentUserRepo) | **POST** /user/repos | Create a repository |
| [**createFork**](RepositoryApi.md#createFork) | **POST** /repos/{owner}/{repo}/forks | Fork a repository |
| [**createRepoVariable**](RepositoryApi.md#createRepoVariable) | **POST** /repos/{owner}/{repo}/actions/variables/{variablename} | Create a repo-level variable |
| [**deleteRepoSecret**](RepositoryApi.md#deleteRepoSecret) | **DELETE** /repos/{owner}/{repo}/actions/secrets/{secretname} | Delete a secret in a repository |
| [**deleteRepoVariable**](RepositoryApi.md#deleteRepoVariable) | **DELETE** /repos/{owner}/{repo}/actions/variables/{variablename} | Delete a repo-level variable |
| [**dispatchWorkflow**](RepositoryApi.md#dispatchWorkflow) | **POST** /repos/{owner}/{repo}/actions/workflows/{workflowfilename}/dispatches | Dispatches a workflow |
| [**generateRepo**](RepositoryApi.md#generateRepo) | **POST** /repos/{template_owner}/{template_repo}/generate | Create a repository using a template |
| [**getAnnotatedTag**](RepositoryApi.md#getAnnotatedTag) | **GET** /repos/{owner}/{repo}/git/tags/{sha} | Gets the tag object of an annotated tag (not lightweight tags) |
| [**getBlob**](RepositoryApi.md#getBlob) | **GET** /repos/{owner}/{repo}/git/blobs/{sha} | Gets the blob of a repository. |
| [**getBlobs**](RepositoryApi.md#getBlobs) | **GET** /repos/{owner}/{repo}/git/blobs | Gets multiple blobs of a repository. |
| [**getRepoVariable**](RepositoryApi.md#getRepoVariable) | **GET** /repos/{owner}/{repo}/actions/variables/{variablename} | Get a repo-level variable |
| [**getRepoVariablesList**](RepositoryApi.md#getRepoVariablesList) | **GET** /repos/{owner}/{repo}/actions/variables | Get repo-level variables list |
| [**getTree**](RepositoryApi.md#getTree) | **GET** /repos/{owner}/{repo}/git/trees/{sha} | Gets the tree of a repository. |
| [**listActionRuns**](RepositoryApi.md#listActionRuns) | **GET** /repos/{owner}/{repo}/actions/runs | List a repository&#39;s action runs |
| [**listActionTasks**](RepositoryApi.md#listActionTasks) | **GET** /repos/{owner}/{repo}/actions/tasks | List a repository&#39;s action tasks |
| [**listForks**](RepositoryApi.md#listForks) | **GET** /repos/{owner}/{repo}/forks | List a repository&#39;s forks |
| [**rejectRepoTransfer**](RepositoryApi.md#rejectRepoTransfer) | **POST** /repos/{owner}/{repo}/transfer/reject | Reject a repo transfer |
| [**repoAddCollaborator**](RepositoryApi.md#repoAddCollaborator) | **PUT** /repos/{owner}/{repo}/collaborators/{collaborator} | Add a collaborator to a repository |
| [**repoAddFlag**](RepositoryApi.md#repoAddFlag) | **PUT** /repos/{owner}/{repo}/flags/{flag} | Add a flag to a repository |
| [**repoAddPushMirror**](RepositoryApi.md#repoAddPushMirror) | **POST** /repos/{owner}/{repo}/push_mirrors | Set up a new push mirror in a repository |
| [**repoAddTeam**](RepositoryApi.md#repoAddTeam) | **PUT** /repos/{owner}/{repo}/teams/{team} | Add a team to a repository |
| [**repoAddTopic**](RepositoryApi.md#repoAddTopic) | **PUT** /repos/{owner}/{repo}/topics/{topic} | Add a topic to a repository |
| [**repoApplyDiffPatch**](RepositoryApi.md#repoApplyDiffPatch) | **POST** /repos/{owner}/{repo}/diffpatch | Apply diff patch to repository |
| [**repoCancelScheduledAutoMerge**](RepositoryApi.md#repoCancelScheduledAutoMerge) | **DELETE** /repos/{owner}/{repo}/pulls/{index}/merge | Cancel the scheduled auto merge for the given pull request |
| [**repoChangeFiles**](RepositoryApi.md#repoChangeFiles) | **POST** /repos/{owner}/{repo}/contents | Modify multiple files in a repository |
| [**repoCheckCollaborator**](RepositoryApi.md#repoCheckCollaborator) | **GET** /repos/{owner}/{repo}/collaborators/{collaborator} | Check if a user is a collaborator of a repository |
| [**repoCheckFlag**](RepositoryApi.md#repoCheckFlag) | **GET** /repos/{owner}/{repo}/flags/{flag} | Check if a repository has a given flag |
| [**repoCheckTeam**](RepositoryApi.md#repoCheckTeam) | **GET** /repos/{owner}/{repo}/teams/{team} | Check if a team is assigned to a repository |
| [**repoCompareDiff**](RepositoryApi.md#repoCompareDiff) | **GET** /repos/{owner}/{repo}/compare/{basehead} | Get commit comparison information |
| [**repoConvert**](RepositoryApi.md#repoConvert) | **POST** /repos/{owner}/{repo}/convert | Convert a mirror repo to a normal repo. |
| [**repoCreateBranch**](RepositoryApi.md#repoCreateBranch) | **POST** /repos/{owner}/{repo}/branches | Create a branch |
| [**repoCreateBranchProtection**](RepositoryApi.md#repoCreateBranchProtection) | **POST** /repos/{owner}/{repo}/branch_protections | Create a branch protections for a repository |
| [**repoCreateFile**](RepositoryApi.md#repoCreateFile) | **POST** /repos/{owner}/{repo}/contents/{filepath} | Create a file in a repository |
| [**repoCreateHook**](RepositoryApi.md#repoCreateHook) | **POST** /repos/{owner}/{repo}/hooks | Create a hook |
| [**repoCreateKey**](RepositoryApi.md#repoCreateKey) | **POST** /repos/{owner}/{repo}/keys | Add a key to a repository |
| [**repoCreatePullRequest**](RepositoryApi.md#repoCreatePullRequest) | **POST** /repos/{owner}/{repo}/pulls | Create a pull request |
| [**repoCreatePullReview**](RepositoryApi.md#repoCreatePullReview) | **POST** /repos/{owner}/{repo}/pulls/{index}/reviews | Create a review to an pull request |
| [**repoCreatePullReviewComment**](RepositoryApi.md#repoCreatePullReviewComment) | **POST** /repos/{owner}/{repo}/pulls/{index}/reviews/{id}/comments | Add a new comment to a pull request review |
| [**repoCreatePullReviewRequests**](RepositoryApi.md#repoCreatePullReviewRequests) | **POST** /repos/{owner}/{repo}/pulls/{index}/requested_reviewers | Create review requests for a pull request |
| [**repoCreateRelease**](RepositoryApi.md#repoCreateRelease) | **POST** /repos/{owner}/{repo}/releases | Create a release |
| [**repoCreateReleaseAttachment**](RepositoryApi.md#repoCreateReleaseAttachment) | **POST** /repos/{owner}/{repo}/releases/{id}/assets | Create a release attachment |
| [**repoCreateStatus**](RepositoryApi.md#repoCreateStatus) | **POST** /repos/{owner}/{repo}/statuses/{sha} | Create a commit status |
| [**repoCreateTag**](RepositoryApi.md#repoCreateTag) | **POST** /repos/{owner}/{repo}/tags | Create a new git tag in a repository |
| [**repoCreateTagProtection**](RepositoryApi.md#repoCreateTagProtection) | **POST** /repos/{owner}/{repo}/tag_protections | Create a tag protections for a repository |
| [**repoCreateWikiPage**](RepositoryApi.md#repoCreateWikiPage) | **POST** /repos/{owner}/{repo}/wiki/new | Create a wiki page |
| [**repoDelete**](RepositoryApi.md#repoDelete) | **DELETE** /repos/{owner}/{repo} | Delete a repository |
| [**repoDeleteAllFlags**](RepositoryApi.md#repoDeleteAllFlags) | **DELETE** /repos/{owner}/{repo}/flags | Remove all flags from a repository |
| [**repoDeleteAvatar**](RepositoryApi.md#repoDeleteAvatar) | **DELETE** /repos/{owner}/{repo}/avatar | Delete a repository&#39;s avatar |
| [**repoDeleteBranch**](RepositoryApi.md#repoDeleteBranch) | **DELETE** /repos/{owner}/{repo}/branches/{branch} | Delete a specific branch from a repository |
| [**repoDeleteBranchProtection**](RepositoryApi.md#repoDeleteBranchProtection) | **DELETE** /repos/{owner}/{repo}/branch_protections/{name} | Delete a specific branch protection for the repository |
| [**repoDeleteCollaborator**](RepositoryApi.md#repoDeleteCollaborator) | **DELETE** /repos/{owner}/{repo}/collaborators/{collaborator} | Delete a collaborator from a repository |
| [**repoDeleteFile**](RepositoryApi.md#repoDeleteFile) | **DELETE** /repos/{owner}/{repo}/contents/{filepath} | Delete a file in a repository |
| [**repoDeleteFlag**](RepositoryApi.md#repoDeleteFlag) | **DELETE** /repos/{owner}/{repo}/flags/{flag} | Remove a flag from a repository |
| [**repoDeleteGitHook**](RepositoryApi.md#repoDeleteGitHook) | **DELETE** /repos/{owner}/{repo}/hooks/git/{id} | Delete a Git hook in a repository |
| [**repoDeleteHook**](RepositoryApi.md#repoDeleteHook) | **DELETE** /repos/{owner}/{repo}/hooks/{id} | Delete a hook in a repository |
| [**repoDeleteKey**](RepositoryApi.md#repoDeleteKey) | **DELETE** /repos/{owner}/{repo}/keys/{id} | Delete a key from a repository |
| [**repoDeletePullReview**](RepositoryApi.md#repoDeletePullReview) | **DELETE** /repos/{owner}/{repo}/pulls/{index}/reviews/{id} | Delete a specific review from a pull request |
| [**repoDeletePullReviewComment**](RepositoryApi.md#repoDeletePullReviewComment) | **DELETE** /repos/{owner}/{repo}/pulls/{index}/reviews/{id}/comments/{comment} | Delete a pull review comment |
| [**repoDeletePullReviewRequests**](RepositoryApi.md#repoDeletePullReviewRequests) | **DELETE** /repos/{owner}/{repo}/pulls/{index}/requested_reviewers | Cancel review requests for a pull request |
| [**repoDeletePushMirror**](RepositoryApi.md#repoDeletePushMirror) | **DELETE** /repos/{owner}/{repo}/push_mirrors/{name} | Remove a push mirror from a repository by remoteName |
| [**repoDeleteRelease**](RepositoryApi.md#repoDeleteRelease) | **DELETE** /repos/{owner}/{repo}/releases/{id} | Delete a release |
| [**repoDeleteReleaseAttachment**](RepositoryApi.md#repoDeleteReleaseAttachment) | **DELETE** /repos/{owner}/{repo}/releases/{id}/assets/{attachment_id} | Delete a release attachment |
| [**repoDeleteReleaseByTag**](RepositoryApi.md#repoDeleteReleaseByTag) | **DELETE** /repos/{owner}/{repo}/releases/tags/{tag} | Delete a release by tag name |
| [**repoDeleteTag**](RepositoryApi.md#repoDeleteTag) | **DELETE** /repos/{owner}/{repo}/tags/{tag} | Delete a repository&#39;s tag by name |
| [**repoDeleteTagProtection**](RepositoryApi.md#repoDeleteTagProtection) | **DELETE** /repos/{owner}/{repo}/tag_protections/{id} | Delete a specific tag protection for the repository |
| [**repoDeleteTeam**](RepositoryApi.md#repoDeleteTeam) | **DELETE** /repos/{owner}/{repo}/teams/{team} | Delete a team from a repository |
| [**repoDeleteTopic**](RepositoryApi.md#repoDeleteTopic) | **DELETE** /repos/{owner}/{repo}/topics/{topic} | Delete a topic from a repository |
| [**repoDeleteWikiPage**](RepositoryApi.md#repoDeleteWikiPage) | **DELETE** /repos/{owner}/{repo}/wiki/page/{pageName} | Delete a wiki page |
| [**repoDismissPullReview**](RepositoryApi.md#repoDismissPullReview) | **POST** /repos/{owner}/{repo}/pulls/{index}/reviews/{id}/dismissals | Dismiss a review for a pull request |
| [**repoDownloadCommitDiffOrPatch**](RepositoryApi.md#repoDownloadCommitDiffOrPatch) | **GET** /repos/{owner}/{repo}/git/commits/{sha}.{diffType} | Get a commit&#39;s diff or patch |
| [**repoDownloadPullDiffOrPatch**](RepositoryApi.md#repoDownloadPullDiffOrPatch) | **GET** /repos/{owner}/{repo}/pulls/{index}.{diffType} | Get a pull request diff or patch |
| [**repoEdit**](RepositoryApi.md#repoEdit) | **PATCH** /repos/{owner}/{repo} | Edit a repository&#39;s properties. Only fields that are set will be changed. |
| [**repoEditBranchProtection**](RepositoryApi.md#repoEditBranchProtection) | **PATCH** /repos/{owner}/{repo}/branch_protections/{name} | Edit a branch protections for a repository. Only fields that are set will be changed |
| [**repoEditGitHook**](RepositoryApi.md#repoEditGitHook) | **PATCH** /repos/{owner}/{repo}/hooks/git/{id} | Edit a Git hook in a repository |
| [**repoEditHook**](RepositoryApi.md#repoEditHook) | **PATCH** /repos/{owner}/{repo}/hooks/{id} | Edit a hook in a repository |
| [**repoEditPullRequest**](RepositoryApi.md#repoEditPullRequest) | **PATCH** /repos/{owner}/{repo}/pulls/{index} | Update a pull request. If using deadline only the date will be taken into account, and time of day ignored. |
| [**repoEditRelease**](RepositoryApi.md#repoEditRelease) | **PATCH** /repos/{owner}/{repo}/releases/{id} | Update a release |
| [**repoEditReleaseAttachment**](RepositoryApi.md#repoEditReleaseAttachment) | **PATCH** /repos/{owner}/{repo}/releases/{id}/assets/{attachment_id} | Edit a release attachment |
| [**repoEditTagProtection**](RepositoryApi.md#repoEditTagProtection) | **PATCH** /repos/{owner}/{repo}/tag_protections/{id} | Edit a tag protections for a repository. Only fields that are set will be changed |
| [**repoEditWikiPage**](RepositoryApi.md#repoEditWikiPage) | **PATCH** /repos/{owner}/{repo}/wiki/page/{pageName} | Edit a wiki page |
| [**repoGet**](RepositoryApi.md#repoGet) | **GET** /repos/{owner}/{repo} | Get a repository |
| [**repoGetAllCommits**](RepositoryApi.md#repoGetAllCommits) | **GET** /repos/{owner}/{repo}/commits | Get a list of all commits from a repository |
| [**repoGetArchive**](RepositoryApi.md#repoGetArchive) | **GET** /repos/{owner}/{repo}/archive/{archive} | Get an archive of a repository |
| [**repoGetAssignees**](RepositoryApi.md#repoGetAssignees) | **GET** /repos/{owner}/{repo}/assignees | Return all users that have write access and can be assigned to issues |
| [**repoGetBranch**](RepositoryApi.md#repoGetBranch) | **GET** /repos/{owner}/{repo}/branches/{branch} | Retrieve a specific branch from a repository, including its effective branch protection |
| [**repoGetBranchProtection**](RepositoryApi.md#repoGetBranchProtection) | **GET** /repos/{owner}/{repo}/branch_protections/{name} | Get a specific branch protection for the repository |
| [**repoGetByID**](RepositoryApi.md#repoGetByID) | **GET** /repositories/{id} | Get a repository by id |
| [**repoGetCombinedStatusByRef**](RepositoryApi.md#repoGetCombinedStatusByRef) | **GET** /repos/{owner}/{repo}/commits/{ref}/status | Get a commit&#39;s combined status, by branch/tag/commit reference |
| [**repoGetCommitPullRequest**](RepositoryApi.md#repoGetCommitPullRequest) | **GET** /repos/{owner}/{repo}/commits/{sha}/pull | Get the pull request of the commit |
| [**repoGetContents**](RepositoryApi.md#repoGetContents) | **GET** /repos/{owner}/{repo}/contents/{filepath} | Gets the metadata and contents (if a file) of an entry in a repository, or a list of entries if a dir |
| [**repoGetContentsList**](RepositoryApi.md#repoGetContentsList) | **GET** /repos/{owner}/{repo}/contents | Gets the metadata of all the entries of the root dir |
| [**repoGetEditorConfig**](RepositoryApi.md#repoGetEditorConfig) | **GET** /repos/{owner}/{repo}/editorconfig/{filepath} | Get the EditorConfig definitions of a file in a repository |
| [**repoGetGitHook**](RepositoryApi.md#repoGetGitHook) | **GET** /repos/{owner}/{repo}/hooks/git/{id} | Get a Git hook |
| [**repoGetHook**](RepositoryApi.md#repoGetHook) | **GET** /repos/{owner}/{repo}/hooks/{id} | Get a hook |
| [**repoGetIssueConfig**](RepositoryApi.md#repoGetIssueConfig) | **GET** /repos/{owner}/{repo}/issue_config | Returns the issue config for a repo |
| [**repoGetIssueTemplates**](RepositoryApi.md#repoGetIssueTemplates) | **GET** /repos/{owner}/{repo}/issue_templates | Get available issue templates for a repository |
| [**repoGetKey**](RepositoryApi.md#repoGetKey) | **GET** /repos/{owner}/{repo}/keys/{id} | Get a repository&#39;s key by id |
| [**repoGetLanguages**](RepositoryApi.md#repoGetLanguages) | **GET** /repos/{owner}/{repo}/languages | Get languages and number of bytes of code written |
| [**repoGetLatestRelease**](RepositoryApi.md#repoGetLatestRelease) | **GET** /repos/{owner}/{repo}/releases/latest | Gets the most recent non-prerelease, non-draft release of a repository, sorted by created_at |
| [**repoGetNote**](RepositoryApi.md#repoGetNote) | **GET** /repos/{owner}/{repo}/git/notes/{sha} | Get a note corresponding to a single commit from a repository |
| [**repoGetPullRequest**](RepositoryApi.md#repoGetPullRequest) | **GET** /repos/{owner}/{repo}/pulls/{index} | Get a pull request |
| [**repoGetPullRequestByBaseHead**](RepositoryApi.md#repoGetPullRequestByBaseHead) | **GET** /repos/{owner}/{repo}/pulls/{base}/{head} | Get a pull request by base and head |
| [**repoGetPullRequestCommits**](RepositoryApi.md#repoGetPullRequestCommits) | **GET** /repos/{owner}/{repo}/pulls/{index}/commits | Get commits for a pull request |
| [**repoGetPullRequestFiles**](RepositoryApi.md#repoGetPullRequestFiles) | **GET** /repos/{owner}/{repo}/pulls/{index}/files | Get changed files for a pull request |
| [**repoGetPullReview**](RepositoryApi.md#repoGetPullReview) | **GET** /repos/{owner}/{repo}/pulls/{index}/reviews/{id} | Get a specific review for a pull request |
| [**repoGetPullReviewComment**](RepositoryApi.md#repoGetPullReviewComment) | **GET** /repos/{owner}/{repo}/pulls/{index}/reviews/{id}/comments/{comment} | Get a pull review comment |
| [**repoGetPullReviewComments**](RepositoryApi.md#repoGetPullReviewComments) | **GET** /repos/{owner}/{repo}/pulls/{index}/reviews/{id}/comments | Get a specific review for a pull request |
| [**repoGetPushMirrorByRemoteName**](RepositoryApi.md#repoGetPushMirrorByRemoteName) | **GET** /repos/{owner}/{repo}/push_mirrors/{name} | Get push mirror of the repository by remoteName |
| [**repoGetRawFile**](RepositoryApi.md#repoGetRawFile) | **GET** /repos/{owner}/{repo}/raw/{filepath} | Get a file from a repository |
| [**repoGetRawFileOrLFS**](RepositoryApi.md#repoGetRawFileOrLFS) | **GET** /repos/{owner}/{repo}/media/{filepath} | Get a file or it&#39;s LFS object from a repository |
| [**repoGetRelease**](RepositoryApi.md#repoGetRelease) | **GET** /repos/{owner}/{repo}/releases/{id} | Get a release |
| [**repoGetReleaseAttachment**](RepositoryApi.md#repoGetReleaseAttachment) | **GET** /repos/{owner}/{repo}/releases/{id}/assets/{attachment_id} | Get a release attachment |
| [**repoGetReleaseByTag**](RepositoryApi.md#repoGetReleaseByTag) | **GET** /repos/{owner}/{repo}/releases/tags/{tag} | Get a release by tag name |
| [**repoGetRepoPermissions**](RepositoryApi.md#repoGetRepoPermissions) | **GET** /repos/{owner}/{repo}/collaborators/{collaborator}/permission | Get repository permissions for a user |
| [**repoGetReviewers**](RepositoryApi.md#repoGetReviewers) | **GET** /repos/{owner}/{repo}/reviewers | Return all users that can be requested to review in this repo |
| [**repoGetRunnerRegistrationToken**](RepositoryApi.md#repoGetRunnerRegistrationToken) | **GET** /repos/{owner}/{repo}/actions/runners/registration-token | Get a repository&#39;s actions runner registration token |
| [**repoGetSingleCommit**](RepositoryApi.md#repoGetSingleCommit) | **GET** /repos/{owner}/{repo}/git/commits/{sha} | Get a single commit from a repository |
| [**repoGetTag**](RepositoryApi.md#repoGetTag) | **GET** /repos/{owner}/{repo}/tags/{tag} | Get the tag of a repository by tag name |
| [**repoGetTagProtection**](RepositoryApi.md#repoGetTagProtection) | **GET** /repos/{owner}/{repo}/tag_protections/{id} | Get a specific tag protection for the repository |
| [**repoGetWikiPage**](RepositoryApi.md#repoGetWikiPage) | **GET** /repos/{owner}/{repo}/wiki/page/{pageName} | Get a wiki page |
| [**repoGetWikiPageRevisions**](RepositoryApi.md#repoGetWikiPageRevisions) | **GET** /repos/{owner}/{repo}/wiki/revisions/{pageName} | Get revisions of a wiki page |
| [**repoGetWikiPages**](RepositoryApi.md#repoGetWikiPages) | **GET** /repos/{owner}/{repo}/wiki/pages | Get all wiki pages |
| [**repoListActionsSecrets**](RepositoryApi.md#repoListActionsSecrets) | **GET** /repos/{owner}/{repo}/actions/secrets | List an repo&#39;s actions secrets |
| [**repoListActivityFeeds**](RepositoryApi.md#repoListActivityFeeds) | **GET** /repos/{owner}/{repo}/activities/feeds | List a repository&#39;s activity feeds |
| [**repoListAllGitRefs**](RepositoryApi.md#repoListAllGitRefs) | **GET** /repos/{owner}/{repo}/git/refs | Get specified ref or filtered repository&#39;s refs |
| [**repoListBranchProtection**](RepositoryApi.md#repoListBranchProtection) | **GET** /repos/{owner}/{repo}/branch_protections | List branch protections for a repository |
| [**repoListBranches**](RepositoryApi.md#repoListBranches) | **GET** /repos/{owner}/{repo}/branches | List a repository&#39;s branches |
| [**repoListCollaborators**](RepositoryApi.md#repoListCollaborators) | **GET** /repos/{owner}/{repo}/collaborators | List a repository&#39;s collaborators |
| [**repoListFlags**](RepositoryApi.md#repoListFlags) | **GET** /repos/{owner}/{repo}/flags | List a repository&#39;s flags |
| [**repoListGitHooks**](RepositoryApi.md#repoListGitHooks) | **GET** /repos/{owner}/{repo}/hooks/git | List the Git hooks in a repository |
| [**repoListGitRefs**](RepositoryApi.md#repoListGitRefs) | **GET** /repos/{owner}/{repo}/git/refs/{ref} | Get specified ref or filtered repository&#39;s refs |
| [**repoListHooks**](RepositoryApi.md#repoListHooks) | **GET** /repos/{owner}/{repo}/hooks | List the hooks in a repository |
| [**repoListKeys**](RepositoryApi.md#repoListKeys) | **GET** /repos/{owner}/{repo}/keys | List a repository&#39;s keys |
| [**repoListPinnedIssues**](RepositoryApi.md#repoListPinnedIssues) | **GET** /repos/{owner}/{repo}/issues/pinned | List a repo&#39;s pinned issues |
| [**repoListPinnedPullRequests**](RepositoryApi.md#repoListPinnedPullRequests) | **GET** /repos/{owner}/{repo}/pulls/pinned | List a repo&#39;s pinned pull requests |
| [**repoListPullRequests**](RepositoryApi.md#repoListPullRequests) | **GET** /repos/{owner}/{repo}/pulls | List a repo&#39;s pull requests. If a pull request is selected but fails to be retrieved for any reason, it will be a null value in the list of results. |
| [**repoListPullReviews**](RepositoryApi.md#repoListPullReviews) | **GET** /repos/{owner}/{repo}/pulls/{index}/reviews | List all reviews for a pull request |
| [**repoListPushMirrors**](RepositoryApi.md#repoListPushMirrors) | **GET** /repos/{owner}/{repo}/push_mirrors | Get all push mirrors of the repository |
| [**repoListReleaseAttachments**](RepositoryApi.md#repoListReleaseAttachments) | **GET** /repos/{owner}/{repo}/releases/{id}/assets | List release&#39;s attachments |
| [**repoListReleases**](RepositoryApi.md#repoListReleases) | **GET** /repos/{owner}/{repo}/releases | List a repo&#39;s releases |
| [**repoListStargazers**](RepositoryApi.md#repoListStargazers) | **GET** /repos/{owner}/{repo}/stargazers | List a repo&#39;s stargazers |
| [**repoListStatuses**](RepositoryApi.md#repoListStatuses) | **GET** /repos/{owner}/{repo}/statuses/{sha} | Get a commit&#39;s statuses |
| [**repoListStatusesByRef**](RepositoryApi.md#repoListStatusesByRef) | **GET** /repos/{owner}/{repo}/commits/{ref}/statuses | Get a commit&#39;s statuses, by branch/tag/commit reference |
| [**repoListSubscribers**](RepositoryApi.md#repoListSubscribers) | **GET** /repos/{owner}/{repo}/subscribers | List a repo&#39;s watchers |
| [**repoListTagProtection**](RepositoryApi.md#repoListTagProtection) | **GET** /repos/{owner}/{repo}/tag_protections | List tag protections for a repository |
| [**repoListTags**](RepositoryApi.md#repoListTags) | **GET** /repos/{owner}/{repo}/tags | List a repository&#39;s tags |
| [**repoListTeams**](RepositoryApi.md#repoListTeams) | **GET** /repos/{owner}/{repo}/teams | List a repository&#39;s teams |
| [**repoListTopics**](RepositoryApi.md#repoListTopics) | **GET** /repos/{owner}/{repo}/topics | Get list of topics that a repository has |
| [**repoMergePullRequest**](RepositoryApi.md#repoMergePullRequest) | **POST** /repos/{owner}/{repo}/pulls/{index}/merge | Merge a pull request |
| [**repoMigrate**](RepositoryApi.md#repoMigrate) | **POST** /repos/migrate | Migrate a remote git repository |
| [**repoMirrorSync**](RepositoryApi.md#repoMirrorSync) | **POST** /repos/{owner}/{repo}/mirror-sync | Sync a mirrored repository |
| [**repoNewPinAllowed**](RepositoryApi.md#repoNewPinAllowed) | **GET** /repos/{owner}/{repo}/new_pin_allowed | Returns if new Issue Pins are allowed |
| [**repoPullRequestIsMerged**](RepositoryApi.md#repoPullRequestIsMerged) | **GET** /repos/{owner}/{repo}/pulls/{index}/merge | Check if a pull request has been merged |
| [**repoPushMirrorSync**](RepositoryApi.md#repoPushMirrorSync) | **POST** /repos/{owner}/{repo}/push_mirrors-sync | Sync all push mirrored repository |
| [**repoRemoveNote**](RepositoryApi.md#repoRemoveNote) | **DELETE** /repos/{owner}/{repo}/git/notes/{sha} | Removes a note corresponding to a single commit from a repository |
| [**repoReplaceAllFlags**](RepositoryApi.md#repoReplaceAllFlags) | **PUT** /repos/{owner}/{repo}/flags | Replace all flags of a repository |
| [**repoSearch**](RepositoryApi.md#repoSearch) | **GET** /repos/search | Search for repositories |
| [**repoSearchRunJobs**](RepositoryApi.md#repoSearchRunJobs) | **GET** /repos/{owner}/{repo}/actions/runners/jobs | Search for repository&#39;s action jobs according filter conditions |
| [**repoSetNote**](RepositoryApi.md#repoSetNote) | **POST** /repos/{owner}/{repo}/git/notes/{sha} | Set a note corresponding to a single commit from a repository |
| [**repoSigningKey**](RepositoryApi.md#repoSigningKey) | **GET** /repos/{owner}/{repo}/signing-key.gpg | Get signing-key.gpg for given repository |
| [**repoSubmitPullReview**](RepositoryApi.md#repoSubmitPullReview) | **POST** /repos/{owner}/{repo}/pulls/{index}/reviews/{id} | Submit a pending review to an pull request |
| [**repoSyncForkBranch**](RepositoryApi.md#repoSyncForkBranch) | **POST** /repos/{owner}/{repo}/sync_fork/{branch} | Syncs a fork branch with the base branch |
| [**repoSyncForkBranchInfo**](RepositoryApi.md#repoSyncForkBranchInfo) | **GET** /repos/{owner}/{repo}/sync_fork/{branch} | Gets information about syncing a fork branch with the base branch |
| [**repoSyncForkDefault**](RepositoryApi.md#repoSyncForkDefault) | **POST** /repos/{owner}/{repo}/sync_fork | Syncs the default branch of a fork with the base branch |
| [**repoSyncForkDefaultInfo**](RepositoryApi.md#repoSyncForkDefaultInfo) | **GET** /repos/{owner}/{repo}/sync_fork | Gets information about syncing the fork default branch with the base branch |
| [**repoTestHook**](RepositoryApi.md#repoTestHook) | **POST** /repos/{owner}/{repo}/hooks/{id}/tests | Test a push webhook |
| [**repoTrackedTimes**](RepositoryApi.md#repoTrackedTimes) | **GET** /repos/{owner}/{repo}/times | List a repo&#39;s tracked times |
| [**repoTransfer**](RepositoryApi.md#repoTransfer) | **POST** /repos/{owner}/{repo}/transfer | Transfer a repo ownership |
| [**repoUnDismissPullReview**](RepositoryApi.md#repoUnDismissPullReview) | **POST** /repos/{owner}/{repo}/pulls/{index}/reviews/{id}/undismissals | Cancel to dismiss a review for a pull request |
| [**repoUpdateAvatar**](RepositoryApi.md#repoUpdateAvatar) | **POST** /repos/{owner}/{repo}/avatar | Update a repository&#39;s avatar |
| [**repoUpdateBranch**](RepositoryApi.md#repoUpdateBranch) | **PATCH** /repos/{owner}/{repo}/branches/{branch} | Update a branch |
| [**repoUpdateFile**](RepositoryApi.md#repoUpdateFile) | **PUT** /repos/{owner}/{repo}/contents/{filepath} | Update a file in a repository |
| [**repoUpdatePullRequest**](RepositoryApi.md#repoUpdatePullRequest) | **POST** /repos/{owner}/{repo}/pulls/{index}/update | Merge PR&#39;s baseBranch into headBranch |
| [**repoUpdateTopics**](RepositoryApi.md#repoUpdateTopics) | **PUT** /repos/{owner}/{repo}/topics | Replace list of topics for a repository |
| [**repoValidateIssueConfig**](RepositoryApi.md#repoValidateIssueConfig) | **GET** /repos/{owner}/{repo}/issue_config/validate | Returns the validation information for a issue config |
| [**topicSearch**](RepositoryApi.md#topicSearch) | **GET** /topics/search | Search for topics by keyword |
| [**updateRepoSecret**](RepositoryApi.md#updateRepoSecret) | **PUT** /repos/{owner}/{repo}/actions/secrets/{secretname} | Create or Update a secret value in a repository |
| [**updateRepoVariable**](RepositoryApi.md#updateRepoVariable) | **PUT** /repos/{owner}/{repo}/actions/variables/{variablename} | Update a repo-level variable |
| [**userCurrentCheckSubscription**](RepositoryApi.md#userCurrentCheckSubscription) | **GET** /repos/{owner}/{repo}/subscription | Check if the current user is watching a repo |
| [**userCurrentDeleteSubscription**](RepositoryApi.md#userCurrentDeleteSubscription) | **DELETE** /repos/{owner}/{repo}/subscription | Unwatch a repo |
| [**userCurrentPutSubscription**](RepositoryApi.md#userCurrentPutSubscription) | **PUT** /repos/{owner}/{repo}/subscription | Watch a repo |
| [**userTrackedTimes**](RepositoryApi.md#userTrackedTimes) | **GET** /repos/{owner}/{repo}/times/{user} | List a user&#39;s tracked times in a repo |


<a id="acceptRepoTransfer"></a>
# **acceptRepoTransfer**
> Repository acceptRepoTransfer(owner, repo)

Accept a repo transfer

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo to transfer
    String repo = "repo_example"; // String | name of the repo to transfer
    try {
      Repository result = apiInstance.acceptRepoTransfer(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#acceptRepoTransfer");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo to transfer | |
| **repo** | **String**| name of the repo to transfer | |

### Return type

[**Repository**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **202** | Repository |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |

<a id="actionRun"></a>
# **actionRun**
> ActionRun actionRun(owner, repo, runId)

Get an action run

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long runId = 56L; // Long | id of the action run
    try {
      ActionRun result = apiInstance.actionRun(owner, repo, runId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#actionRun");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **runId** | **Long**| id of the action run | |

### Return type

[**ActionRun**](ActionRun.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ActionRun |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="createCurrentUserRepo"></a>
# **createCurrentUserRepo**
> Repository createCurrentUserRepo(body)

Create a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    CreateRepoOption body = new CreateRepoOption(); // CreateRepoOption | 
    try {
      Repository result = apiInstance.createCurrentUserRepo(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#createCurrentUserRepo");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**CreateRepoOption**](CreateRepoOption.md)|  | [optional] |

### Return type

[**Repository**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Repository |  -  |
| **400** | APIError is error format response |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **409** | The repository with the same name already exists. |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="createFork"></a>
# **createFork**
> Repository createFork(owner, repo, body)

Fork a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo to fork
    String repo = "repo_example"; // String | name of the repo to fork
    CreateForkOption body = new CreateForkOption(); // CreateForkOption | 
    try {
      Repository result = apiInstance.createFork(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#createFork");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo to fork | |
| **repo** | **String**| name of the repo to fork | |
| **body** | [**CreateForkOption**](CreateForkOption.md)|  | [optional] |

### Return type

[**Repository**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **202** | Repository |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | The repository with the same name already exists. |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="createRepoVariable"></a>
# **createRepoVariable**
> createRepoVariable(owner, repo, variablename, body)

Create a repo-level variable

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | name of the owner
    String repo = "repo_example"; // String | name of the repository
    String variablename = "variablename_example"; // String | name of the variable
    CreateVariableOption body = new CreateVariableOption(); // CreateVariableOption | 
    try {
      apiInstance.createRepoVariable(owner, repo, variablename, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#createRepoVariable");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| name of the owner | |
| **repo** | **String**| name of the repository | |
| **variablename** | **String**| name of the variable | |
| **body** | [**CreateVariableOption**](CreateVariableOption.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | response when creating a repo-level variable |  -  |
| **204** | response when creating a repo-level variable |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="deleteRepoSecret"></a>
# **deleteRepoSecret**
> deleteRepoSecret(owner, repo, secretname)

Delete a secret in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repository
    String repo = "repo_example"; // String | name of the repository
    String secretname = "secretname_example"; // String | name of the secret
    try {
      apiInstance.deleteRepoSecret(owner, repo, secretname);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#deleteRepoSecret");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repository | |
| **repo** | **String**| name of the repository | |
| **secretname** | **String**| name of the secret | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | delete one secret of the organization |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="deleteRepoVariable"></a>
# **deleteRepoVariable**
> deleteRepoVariable(owner, repo, variablename)

Delete a repo-level variable

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | name of the owner
    String repo = "repo_example"; // String | name of the repository
    String variablename = "variablename_example"; // String | name of the variable
    try {
      apiInstance.deleteRepoVariable(owner, repo, variablename);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#deleteRepoVariable");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| name of the owner | |
| **repo** | **String**| name of the repository | |
| **variablename** | **String**| name of the variable | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | response when deleting a variable |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="dispatchWorkflow"></a>
# **dispatchWorkflow**
> DispatchWorkflowRun dispatchWorkflow(owner, repo, workflowfilename, body)

Dispatches a workflow

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String workflowfilename = "workflowfilename_example"; // String | name of the workflow
    DispatchWorkflowOption body = new DispatchWorkflowOption(); // DispatchWorkflowOption | 
    try {
      DispatchWorkflowRun result = apiInstance.dispatchWorkflow(owner, repo, workflowfilename, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#dispatchWorkflow");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **workflowfilename** | **String**| name of the workflow | |
| **body** | [**DispatchWorkflowOption**](DispatchWorkflowOption.md)|  | [optional] |

### Return type

[**DispatchWorkflowRun**](DispatchWorkflowRun.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | DispatchWorkflowRun is a Workflow Run after dispatching |  -  |
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="generateRepo"></a>
# **generateRepo**
> Repository generateRepo(templateOwner, templateRepo, body)

Create a repository using a template

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String templateOwner = "templateOwner_example"; // String | name of the template repository owner
    String templateRepo = "templateRepo_example"; // String | name of the template repository
    GenerateRepoOption body = new GenerateRepoOption(); // GenerateRepoOption | 
    try {
      Repository result = apiInstance.generateRepo(templateOwner, templateRepo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#generateRepo");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **templateOwner** | **String**| name of the template repository owner | |
| **templateRepo** | **String**| name of the template repository | |
| **body** | [**GenerateRepoOption**](GenerateRepoOption.md)|  | [optional] |

### Return type

[**Repository**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Repository |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | The repository with the same name already exists. |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="getAnnotatedTag"></a>
# **getAnnotatedTag**
> AnnotatedTag getAnnotatedTag(owner, repo, sha)

Gets the tag object of an annotated tag (not lightweight tags)

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | sha of the tag. The Git tags API only supports annotated tag objects, not lightweight tags.
    try {
      AnnotatedTag result = apiInstance.getAnnotatedTag(owner, repo, sha);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#getAnnotatedTag");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| sha of the tag. The Git tags API only supports annotated tag objects, not lightweight tags. | |

### Return type

[**AnnotatedTag**](AnnotatedTag.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | AnnotatedTag |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="getBlob"></a>
# **getBlob**
> GitBlob getBlob(owner, repo, sha)

Gets the blob of a repository.

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | sha of the blob to retrieve
    try {
      GitBlob result = apiInstance.getBlob(owner, repo, sha);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#getBlob");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| sha of the blob to retrieve | |

### Return type

[**GitBlob**](GitBlob.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GitBlob |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="getBlobs"></a>
# **getBlobs**
> List&lt;GitBlob&gt; getBlobs(owner, repo, shas)

Gets multiple blobs of a repository.

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String shas = "shas_example"; // String | a comma separated list of blob-sha (mind the overall URL-length limit of ~2,083 chars)
    try {
      List<GitBlob> result = apiInstance.getBlobs(owner, repo, shas);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#getBlobs");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **shas** | **String**| a comma separated list of blob-sha (mind the overall URL-length limit of ~2,083 chars) | |

### Return type

[**List&lt;GitBlob&gt;**](GitBlob.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GitBlobList |  -  |
| **400** | APIError is error format response |  -  |

<a id="getRepoVariable"></a>
# **getRepoVariable**
> ActionVariable getRepoVariable(owner, repo, variablename)

Get a repo-level variable

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | name of the owner
    String repo = "repo_example"; // String | name of the repository
    String variablename = "variablename_example"; // String | name of the variable
    try {
      ActionVariable result = apiInstance.getRepoVariable(owner, repo, variablename);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#getRepoVariable");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| name of the owner | |
| **repo** | **String**| name of the repository | |
| **variablename** | **String**| name of the variable | |

### Return type

[**ActionVariable**](ActionVariable.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ActionVariable |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="getRepoVariablesList"></a>
# **getRepoVariablesList**
> List&lt;ActionVariable&gt; getRepoVariablesList(owner, repo, page, limit)

Get repo-level variables list

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | name of the owner
    String repo = "repo_example"; // String | name of the repository
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<ActionVariable> result = apiInstance.getRepoVariablesList(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#getRepoVariablesList");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| name of the owner | |
| **repo** | **String**| name of the repository | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;ActionVariable&gt;**](ActionVariable.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | VariableList |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="getTree"></a>
# **getTree**
> GitTreeResponse getTree(owner, repo, sha, recursive, page, perPage)

Gets the tree of a repository.

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | sha of the commit
    Boolean recursive = true; // Boolean | show all directories and files
    Integer page = 56; // Integer | page number; the 'truncated' field in the response will be true if there are still more items after this page, false if the last page
    Integer perPage = 56; // Integer | number of items per page
    try {
      GitTreeResponse result = apiInstance.getTree(owner, repo, sha, recursive, page, perPage);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#getTree");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| sha of the commit | |
| **recursive** | **Boolean**| show all directories and files | [optional] |
| **page** | **Integer**| page number; the &#39;truncated&#39; field in the response will be true if there are still more items after this page, false if the last page | [optional] |
| **perPage** | **Integer**| number of items per page | [optional] |

### Return type

[**GitTreeResponse**](GitTreeResponse.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GitTreeResponse |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="listActionRuns"></a>
# **listActionRuns**
> ListActionRunResponse listActionRuns(owner, repo, page, limit, event, status, runNumber, headSha)

List a repository&#39;s action runs

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results, default maximum page size is 50
    List<String> event = Arrays.asList(); // List<String> | Returns workflow run triggered by the specified events. For example, `push`, `pull_request` or `workflow_dispatch`.
    List<String> status = Arrays.asList(); // List<String> | Returns workflow runs with the check run status or conclusion that is specified. For example, a conclusion can be success or a status can be in_progress. Only Forgejo Actions can set a status of waiting, pending, or requested. 
    Long runNumber = 56L; // Long | Returns the workflow run associated with the run number. 
    String headSha = "headSha_example"; // String | Only returns workflow runs that are associated with the specified head_sha.
    try {
      ListActionRunResponse result = apiInstance.listActionRuns(owner, repo, page, limit, event, status, runNumber, headSha);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#listActionRuns");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results, default maximum page size is 50 | [optional] |
| **event** | [**List&lt;String&gt;**](String.md)| Returns workflow run triggered by the specified events. For example, &#x60;push&#x60;, &#x60;pull_request&#x60; or &#x60;workflow_dispatch&#x60;. | [optional] |
| **status** | [**List&lt;String&gt;**](String.md)| Returns workflow runs with the check run status or conclusion that is specified. For example, a conclusion can be success or a status can be in_progress. Only Forgejo Actions can set a status of waiting, pending, or requested.  | [optional] [enum: unknown, waiting, running, success, failure, cancelled, skipped, blocked] |
| **runNumber** | **Long**| Returns the workflow run associated with the run number.  | [optional] |
| **headSha** | **String**| Only returns workflow runs that are associated with the specified head_sha. | [optional] |

### Return type

[**ListActionRunResponse**](ListActionRunResponse.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ActionRunList |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="listActionTasks"></a>
# **listActionTasks**
> ActionTaskResponse listActionTasks(owner, repo, page, limit)

List a repository&#39;s action tasks

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results, default maximum page size is 50
    try {
      ActionTaskResponse result = apiInstance.listActionTasks(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#listActionTasks");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results, default maximum page size is 50 | [optional] |

### Return type

[**ActionTaskResponse**](ActionTaskResponse.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | TasksList |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | APIConflict is a conflict empty response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="listForks"></a>
# **listForks**
> List&lt;Repository&gt; listForks(owner, repo, page, limit)

List a repository&#39;s forks

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Repository> result = apiInstance.listForks(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#listForks");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;Repository&gt;**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | RepositoryList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="rejectRepoTransfer"></a>
# **rejectRepoTransfer**
> Repository rejectRepoTransfer(owner, repo)

Reject a repo transfer

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo to transfer
    String repo = "repo_example"; // String | name of the repo to transfer
    try {
      Repository result = apiInstance.rejectRepoTransfer(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#rejectRepoTransfer");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo to transfer | |
| **repo** | **String**| name of the repo to transfer | |

### Return type

[**Repository**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Repository |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoAddCollaborator"></a>
# **repoAddCollaborator**
> repoAddCollaborator(owner, repo, collaborator, body)

Add a collaborator to a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String collaborator = "collaborator_example"; // String | username of the collaborator to add
    AddCollaboratorOption body = new AddCollaboratorOption(); // AddCollaboratorOption | 
    try {
      apiInstance.repoAddCollaborator(owner, repo, collaborator, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoAddCollaborator");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **collaborator** | **String**| username of the collaborator to add | |
| **body** | [**AddCollaboratorOption**](AddCollaboratorOption.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoAddFlag"></a>
# **repoAddFlag**
> repoAddFlag(owner, repo, flag)

Add a flag to a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String flag = "flag_example"; // String | name of the flag
    try {
      apiInstance.repoAddFlag(owner, repo, flag);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoAddFlag");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **flag** | **String**| name of the flag | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoAddPushMirror"></a>
# **repoAddPushMirror**
> PushMirror repoAddPushMirror(owner, repo, body)

Set up a new push mirror in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    CreatePushMirrorOption body = new CreatePushMirrorOption(); // CreatePushMirrorOption | 
    try {
      PushMirror result = apiInstance.repoAddPushMirror(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoAddPushMirror");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**CreatePushMirrorOption**](CreatePushMirrorOption.md)|  | [optional] |

### Return type

[**PushMirror**](PushMirror.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PushMirror |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |

<a id="repoAddTeam"></a>
# **repoAddTeam**
> repoAddTeam(owner, repo, team)

Add a team to a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String team = "team_example"; // String | team name
    try {
      apiInstance.repoAddTeam(owner, repo, team);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoAddTeam");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **team** | **String**| team name | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **405** | APIError is error format response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoAddTopic"></a>
# **repoAddTopic**
> repoAddTopic(owner, repo, topic)

Add a topic to a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String topic = "topic_example"; // String | name of the topic to add
    try {
      apiInstance.repoAddTopic(owner, repo, topic);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoAddTopic");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **topic** | **String**| name of the topic to add | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIInvalidTopicsError is error format response to invalid topics |  -  |

<a id="repoApplyDiffPatch"></a>
# **repoApplyDiffPatch**
> FileResponse repoApplyDiffPatch(owner, repo, body)

Apply diff patch to repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    UpdateFileOptions body = new UpdateFileOptions(); // UpdateFileOptions | 
    try {
      FileResponse result = apiInstance.repoApplyDiffPatch(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoApplyDiffPatch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**UpdateFileOptions**](UpdateFileOptions.md)|  | |

### Return type

[**FileResponse**](FileResponse.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | FileResponse |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoCancelScheduledAutoMerge"></a>
# **repoCancelScheduledAutoMerge**
> repoCancelScheduledAutoMerge(owner, repo, index)

Cancel the scheduled auto merge for the given pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request to merge
    try {
      apiInstance.repoCancelScheduledAutoMerge(owner, repo, index);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCancelScheduledAutoMerge");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request to merge | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoChangeFiles"></a>
# **repoChangeFiles**
> FilesResponse repoChangeFiles(owner, repo, body)

Modify multiple files in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    ChangeFilesOptions body = new ChangeFilesOptions(); // ChangeFilesOptions | 
    try {
      FilesResponse result = apiInstance.repoChangeFiles(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoChangeFiles");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**ChangeFilesOptions**](ChangeFilesOptions.md)|  | |

### Return type

[**FilesResponse**](FilesResponse.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | FilesResponse |  -  |
| **403** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | APIConflict is a conflict empty response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **422** | APIError is error format response |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoCheckCollaborator"></a>
# **repoCheckCollaborator**
> repoCheckCollaborator(owner, repo, collaborator)

Check if a user is a collaborator of a repository

If the user is a collaborator, return 204. If the user is not a collaborator, return 404.

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String collaborator = "collaborator_example"; // String | username of the collaborator
    try {
      apiInstance.repoCheckCollaborator(owner, repo, collaborator);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCheckCollaborator");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **collaborator** | **String**| username of the collaborator | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoCheckFlag"></a>
# **repoCheckFlag**
> repoCheckFlag(owner, repo, flag)

Check if a repository has a given flag

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String flag = "flag_example"; // String | name of the flag
    try {
      apiInstance.repoCheckFlag(owner, repo, flag);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCheckFlag");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **flag** | **String**| name of the flag | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoCheckTeam"></a>
# **repoCheckTeam**
> Team repoCheckTeam(owner, repo, team)

Check if a team is assigned to a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String team = "team_example"; // String | team name
    try {
      Team result = apiInstance.repoCheckTeam(owner, repo, team);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCheckTeam");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **team** | **String**| team name | |

### Return type

[**Team**](Team.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Team |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **405** | APIError is error format response |  -  |

<a id="repoCompareDiff"></a>
# **repoCompareDiff**
> Compare repoCompareDiff(owner, repo, basehead)

Get commit comparison information

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String basehead = "basehead_example"; // String | compare two branches or commits
    try {
      Compare result = apiInstance.repoCompareDiff(owner, repo, basehead);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCompareDiff");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **basehead** | **String**| compare two branches or commits | |

### Return type

[**Compare**](Compare.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoConvert"></a>
# **repoConvert**
> Repository repoConvert(owner, repo)

Convert a mirror repo to a normal repo.

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo to convert
    String repo = "repo_example"; // String | name of the repo to convert
    try {
      Repository result = apiInstance.repoConvert(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoConvert");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo to convert | |
| **repo** | **String**| name of the repo to convert | |

### Return type

[**Repository**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Repository |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoCreateBranch"></a>
# **repoCreateBranch**
> Branch repoCreateBranch(owner, repo, body)

Create a branch

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    CreateBranchRepoOption body = new CreateBranchRepoOption(); // CreateBranchRepoOption | 
    try {
      Branch result = apiInstance.repoCreateBranch(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreateBranch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**CreateBranchRepoOption**](CreateBranchRepoOption.md)|  | [optional] |

### Return type

[**Branch**](Branch.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Branch |  -  |
| **403** | The branch is archived or a mirror. |  -  |
| **404** | The old branch does not exist. |  -  |
| **409** | The branch with the same name already exists. |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoCreateBranchProtection"></a>
# **repoCreateBranchProtection**
> BranchProtection repoCreateBranchProtection(owner, repo, body)

Create a branch protections for a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    CreateBranchProtectionOption body = new CreateBranchProtectionOption(); // CreateBranchProtectionOption | 
    try {
      BranchProtection result = apiInstance.repoCreateBranchProtection(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreateBranchProtection");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**CreateBranchProtectionOption**](CreateBranchProtectionOption.md)|  | [optional] |

### Return type

[**BranchProtection**](BranchProtection.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | BranchProtection |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoCreateFile"></a>
# **repoCreateFile**
> FileResponse repoCreateFile(owner, repo, filepath, body)

Create a file in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String filepath = "filepath_example"; // String | path of the file to create
    CreateFileOptions body = new CreateFileOptions(); // CreateFileOptions | 
    try {
      FileResponse result = apiInstance.repoCreateFile(owner, repo, filepath, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreateFile");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **filepath** | **String**| path of the file to create | |
| **body** | [**CreateFileOptions**](CreateFileOptions.md)|  | |

### Return type

[**FileResponse**](FileResponse.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | FileResponse |  -  |
| **403** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | APIConflict is a conflict empty response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **422** | APIError is error format response |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoCreateHook"></a>
# **repoCreateHook**
> Hook repoCreateHook(owner, repo, body)

Create a hook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    CreateHookOption body = new CreateHookOption(); // CreateHookOption | 
    try {
      Hook result = apiInstance.repoCreateHook(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreateHook");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**CreateHookOption**](CreateHookOption.md)|  | [optional] |

### Return type

[**Hook**](Hook.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Hook |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoCreateKey"></a>
# **repoCreateKey**
> DeployKey repoCreateKey(owner, repo, body)

Add a key to a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    CreateKeyOption body = new CreateKeyOption(); // CreateKeyOption | 
    try {
      DeployKey result = apiInstance.repoCreateKey(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreateKey");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**CreateKeyOption**](CreateKeyOption.md)|  | [optional] |

### Return type

[**DeployKey**](DeployKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | DeployKey |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoCreatePullRequest"></a>
# **repoCreatePullRequest**
> PullRequest repoCreatePullRequest(owner, repo, body)

Create a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    CreatePullRequestOption body = new CreatePullRequestOption(); // CreatePullRequestOption | 
    try {
      PullRequest result = apiInstance.repoCreatePullRequest(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreatePullRequest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**CreatePullRequestOption**](CreatePullRequestOption.md)|  | [optional] |

### Return type

[**PullRequest**](PullRequest.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | PullRequest |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | APIError is error format response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **422** | APIValidationError is error format response related to input validation |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoCreatePullReview"></a>
# **repoCreatePullReview**
> PullReview repoCreatePullReview(owner, repo, index, body)

Create a review to an pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    CreatePullReviewOptions body = new CreatePullReviewOptions(); // CreatePullReviewOptions | 
    try {
      PullReview result = apiInstance.repoCreatePullReview(owner, repo, index, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreatePullReview");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **body** | [**CreatePullReviewOptions**](CreatePullReviewOptions.md)|  | |

### Return type

[**PullReview**](PullReview.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullReview |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoCreatePullReviewComment"></a>
# **repoCreatePullReviewComment**
> PullReviewComment repoCreatePullReviewComment(owner, repo, index, id, body)

Add a new comment to a pull request review

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    Long id = 56L; // Long | id of the review
    CreatePullReviewComment body = new CreatePullReviewComment(); // CreatePullReviewComment | 
    try {
      PullReviewComment result = apiInstance.repoCreatePullReviewComment(owner, repo, index, id, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreatePullReviewComment");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **id** | **Long**| id of the review | |
| **body** | **CreatePullReviewComment**|  | |

### Return type

[**PullReviewComment**](PullReviewComment.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullComment |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoCreatePullReviewRequests"></a>
# **repoCreatePullReviewRequests**
> List&lt;PullReview&gt; repoCreatePullReviewRequests(owner, repo, index, body)

Create review requests for a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    PullReviewRequestOptions body = new PullReviewRequestOptions(); // PullReviewRequestOptions | 
    try {
      List<PullReview> result = apiInstance.repoCreatePullReviewRequests(owner, repo, index, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreatePullReviewRequests");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **body** | [**PullReviewRequestOptions**](PullReviewRequestOptions.md)|  | |

### Return type

[**List&lt;PullReview&gt;**](PullReview.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | PullReviewList |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoCreateRelease"></a>
# **repoCreateRelease**
> Release repoCreateRelease(owner, repo, body)

Create a release

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    CreateReleaseOption body = new CreateReleaseOption(); // CreateReleaseOption | 
    try {
      Release result = apiInstance.repoCreateRelease(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreateRelease");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**CreateReleaseOption**](CreateReleaseOption.md)|  | [optional] |

### Return type

[**Release**](Release.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Release |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | APIError is error format response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoCreateReleaseAttachment"></a>
# **repoCreateReleaseAttachment**
> Attachment repoCreateReleaseAttachment(owner, repo, id, name, attachment, externalUrl)

Create a release attachment

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the release
    String name = "name_example"; // String | name of the attachment
    File attachment = new File("/path/to/file"); // File | attachment to upload (this parameter is incompatible with `external_url`)
    String externalUrl = "externalUrl_example"; // String | url to external asset (this parameter is incompatible with `attachment`)
    try {
      Attachment result = apiInstance.repoCreateReleaseAttachment(owner, repo, id, name, attachment, externalUrl);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreateReleaseAttachment");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the release | |
| **name** | **String**| name of the attachment | [optional] |
| **attachment** | **File**| attachment to upload (this parameter is incompatible with &#x60;external_url&#x60;) | [optional] |
| **externalUrl** | **String**| url to external asset (this parameter is incompatible with &#x60;attachment&#x60;) | [optional] |

### Return type

[**Attachment**](Attachment.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: multipart/form-data, application/octet-stream
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Attachment |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |

<a id="repoCreateStatus"></a>
# **repoCreateStatus**
> CommitStatus repoCreateStatus(owner, repo, sha, body)

Create a commit status

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | sha of the commit
    CreateStatusOption body = new CreateStatusOption(); // CreateStatusOption | 
    try {
      CommitStatus result = apiInstance.repoCreateStatus(owner, repo, sha, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreateStatus");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| sha of the commit | |
| **body** | [**CreateStatusOption**](CreateStatusOption.md)|  | [optional] |

### Return type

[**CommitStatus**](CommitStatus.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | CommitStatus |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoCreateTag"></a>
# **repoCreateTag**
> Tag repoCreateTag(owner, repo, body)

Create a new git tag in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    CreateTagOption body = new CreateTagOption(); // CreateTagOption | 
    try {
      Tag result = apiInstance.repoCreateTag(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreateTag");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**CreateTagOption**](CreateTagOption.md)|  | [optional] |

### Return type

[**Tag**](Tag.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Tag |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **405** | APIEmpty is an empty response |  -  |
| **409** | APIConflict is a conflict empty response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **422** | APIValidationError is error format response related to input validation |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoCreateTagProtection"></a>
# **repoCreateTagProtection**
> TagProtection repoCreateTagProtection(owner, repo, body)

Create a tag protections for a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    CreateTagProtectionOption body = new CreateTagProtectionOption(); // CreateTagProtectionOption | 
    try {
      TagProtection result = apiInstance.repoCreateTagProtection(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreateTagProtection");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**CreateTagProtectionOption**](CreateTagProtectionOption.md)|  | [optional] |

### Return type

[**TagProtection**](TagProtection.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | TagProtection |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoCreateWikiPage"></a>
# **repoCreateWikiPage**
> WikiPage repoCreateWikiPage(owner, repo, body)

Create a wiki page

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    CreateWikiPageOptions body = new CreateWikiPageOptions(); // CreateWikiPageOptions | 
    try {
      WikiPage result = apiInstance.repoCreateWikiPage(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoCreateWikiPage");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**CreateWikiPageOptions**](CreateWikiPageOptions.md)|  | [optional] |

### Return type

[**WikiPage**](WikiPage.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | WikiPage |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoDelete"></a>
# **repoDelete**
> repoDelete(owner, repo)

Delete a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo to delete
    String repo = "repo_example"; // String | name of the repo to delete
    try {
      apiInstance.repoDelete(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDelete");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo to delete | |
| **repo** | **String**| name of the repo to delete | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeleteAllFlags"></a>
# **repoDeleteAllFlags**
> repoDeleteAllFlags(owner, repo)

Remove all flags from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      apiInstance.repoDeleteAllFlags(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteAllFlags");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeleteAvatar"></a>
# **repoDeleteAvatar**
> repoDeleteAvatar(owner, repo)

Delete a repository&#39;s avatar

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      apiInstance.repoDeleteAvatar(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteAvatar");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeleteBranch"></a>
# **repoDeleteBranch**
> repoDeleteBranch(owner, repo, branch)

Delete a specific branch from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String branch = "branch_example"; // String | branch to delete
    try {
      apiInstance.repoDeleteBranch(owner, repo, branch);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteBranch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **branch** | **String**| branch to delete | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoDeleteBranchProtection"></a>
# **repoDeleteBranchProtection**
> repoDeleteBranchProtection(owner, repo, name)

Delete a specific branch protection for the repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String name = "name_example"; // String | name of protected branch
    try {
      apiInstance.repoDeleteBranchProtection(owner, repo, name);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteBranchProtection");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **name** | **String**| name of protected branch | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeleteCollaborator"></a>
# **repoDeleteCollaborator**
> repoDeleteCollaborator(owner, repo, collaborator)

Delete a collaborator from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String collaborator = "collaborator_example"; // String | username of the collaborator to delete
    try {
      apiInstance.repoDeleteCollaborator(owner, repo, collaborator);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteCollaborator");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **collaborator** | **String**| username of the collaborator to delete | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoDeleteFile"></a>
# **repoDeleteFile**
> FileDeleteResponse repoDeleteFile(owner, repo, filepath, body)

Delete a file in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String filepath = "filepath_example"; // String | path of the file to delete
    DeleteFileOptions body = new DeleteFileOptions(); // DeleteFileOptions | 
    try {
      FileDeleteResponse result = apiInstance.repoDeleteFile(owner, repo, filepath, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteFile");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **filepath** | **String**| path of the file to delete | |
| **body** | [**DeleteFileOptions**](DeleteFileOptions.md)|  | |

### Return type

[**FileDeleteResponse**](FileDeleteResponse.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | FileDeleteResponse |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIError is error format response |  -  |
| **404** | APIError is error format response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoDeleteFlag"></a>
# **repoDeleteFlag**
> repoDeleteFlag(owner, repo, flag)

Remove a flag from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String flag = "flag_example"; // String | name of the flag
    try {
      apiInstance.repoDeleteFlag(owner, repo, flag);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteFlag");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **flag** | **String**| name of the flag | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeleteGitHook"></a>
# **repoDeleteGitHook**
> repoDeleteGitHook(owner, repo, id)

Delete a Git hook in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String id = "id_example"; // String | id of the hook to get
    try {
      apiInstance.repoDeleteGitHook(owner, repo, id);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteGitHook");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **String**| id of the hook to get | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeleteHook"></a>
# **repoDeleteHook**
> repoDeleteHook(owner, repo, id)

Delete a hook in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the hook to delete
    try {
      apiInstance.repoDeleteHook(owner, repo, id);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteHook");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the hook to delete | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeleteKey"></a>
# **repoDeleteKey**
> repoDeleteKey(owner, repo, id)

Delete a key from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the key to delete
    try {
      apiInstance.repoDeleteKey(owner, repo, id);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteKey");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the key to delete | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeletePullReview"></a>
# **repoDeletePullReview**
> repoDeletePullReview(owner, repo, index, id)

Delete a specific review from a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    Long id = 56L; // Long | id of the review
    try {
      apiInstance.repoDeletePullReview(owner, repo, index, id);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeletePullReview");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **id** | **Long**| id of the review | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeletePullReviewComment"></a>
# **repoDeletePullReviewComment**
> repoDeletePullReviewComment(owner, repo, index, id, comment)

Delete a pull review comment

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    Long id = 56L; // Long | id of the review
    Long comment = 56L; // Long | id of the comment
    try {
      apiInstance.repoDeletePullReviewComment(owner, repo, index, id, comment);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeletePullReviewComment");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **id** | **Long**| id of the review | |
| **comment** | **Long**| id of the comment | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeletePullReviewRequests"></a>
# **repoDeletePullReviewRequests**
> repoDeletePullReviewRequests(owner, repo, index, body)

Cancel review requests for a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    PullReviewRequestOptions body = new PullReviewRequestOptions(); // PullReviewRequestOptions | 
    try {
      apiInstance.repoDeletePullReviewRequests(owner, repo, index, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeletePullReviewRequests");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **body** | [**PullReviewRequestOptions**](PullReviewRequestOptions.md)|  | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoDeletePushMirror"></a>
# **repoDeletePushMirror**
> repoDeletePushMirror(owner, repo, name)

Remove a push mirror from a repository by remoteName

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String name = "name_example"; // String | remote name of the pushMirror
    try {
      apiInstance.repoDeletePushMirror(owner, repo, name);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeletePushMirror");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **name** | **String**| remote name of the pushMirror | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeleteRelease"></a>
# **repoDeleteRelease**
> repoDeleteRelease(owner, repo, id)

Delete a release

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the release to delete
    try {
      apiInstance.repoDeleteRelease(owner, repo, id);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteRelease");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the release to delete | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoDeleteReleaseAttachment"></a>
# **repoDeleteReleaseAttachment**
> repoDeleteReleaseAttachment(owner, repo, id, attachmentId)

Delete a release attachment

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the release
    Long attachmentId = 56L; // Long | id of the attachment to delete
    try {
      apiInstance.repoDeleteReleaseAttachment(owner, repo, id, attachmentId);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteReleaseAttachment");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the release | |
| **attachmentId** | **Long**| id of the attachment to delete | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeleteReleaseByTag"></a>
# **repoDeleteReleaseByTag**
> repoDeleteReleaseByTag(owner, repo, tag)

Delete a release by tag name

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String tag = "tag_example"; // String | tag name of the release to delete
    try {
      apiInstance.repoDeleteReleaseByTag(owner, repo, tag);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteReleaseByTag");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **tag** | **String**| tag name of the release to delete | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoDeleteTag"></a>
# **repoDeleteTag**
> repoDeleteTag(owner, repo, tag)

Delete a repository&#39;s tag by name

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String tag = "tag_example"; // String | name of tag to delete
    try {
      apiInstance.repoDeleteTag(owner, repo, tag);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteTag");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **tag** | **String**| name of tag to delete | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **405** | APIEmpty is an empty response |  -  |
| **409** | APIConflict is a conflict empty response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoDeleteTagProtection"></a>
# **repoDeleteTagProtection**
> repoDeleteTagProtection(owner, repo, id)

Delete a specific tag protection for the repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of protected tag
    try {
      apiInstance.repoDeleteTagProtection(owner, repo, id);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteTagProtection");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of protected tag | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDeleteTeam"></a>
# **repoDeleteTeam**
> repoDeleteTeam(owner, repo, team)

Delete a team from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String team = "team_example"; // String | team name
    try {
      apiInstance.repoDeleteTeam(owner, repo, team);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteTeam");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **team** | **String**| team name | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **405** | APIError is error format response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoDeleteTopic"></a>
# **repoDeleteTopic**
> repoDeleteTopic(owner, repo, topic)

Delete a topic from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String topic = "topic_example"; // String | name of the topic to delete
    try {
      apiInstance.repoDeleteTopic(owner, repo, topic);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteTopic");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **topic** | **String**| name of the topic to delete | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIInvalidTopicsError is error format response to invalid topics |  -  |

<a id="repoDeleteWikiPage"></a>
# **repoDeleteWikiPage**
> repoDeleteWikiPage(owner, repo, pageName)

Delete a wiki page

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String pageName = "pageName_example"; // String | name of the page
    try {
      apiInstance.repoDeleteWikiPage(owner, repo, pageName);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDeleteWikiPage");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **pageName** | **String**| name of the page | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoDismissPullReview"></a>
# **repoDismissPullReview**
> PullReview repoDismissPullReview(owner, repo, index, id, body)

Dismiss a review for a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    Long id = 56L; // Long | id of the review
    DismissPullReviewOptions body = new DismissPullReviewOptions(); // DismissPullReviewOptions | 
    try {
      PullReview result = apiInstance.repoDismissPullReview(owner, repo, index, id, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDismissPullReview");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **id** | **Long**| id of the review | |
| **body** | [**DismissPullReviewOptions**](DismissPullReviewOptions.md)|  | |

### Return type

[**PullReview**](PullReview.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullReview |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoDownloadCommitDiffOrPatch"></a>
# **repoDownloadCommitDiffOrPatch**
> String repoDownloadCommitDiffOrPatch(owner, repo, sha, diffType)

Get a commit&#39;s diff or patch

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | SHA of the commit to get
    String diffType = "diff"; // String | whether the output is diff or patch
    try {
      String result = apiInstance.repoDownloadCommitDiffOrPatch(owner, repo, sha, diffType);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDownloadCommitDiffOrPatch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| SHA of the commit to get | |
| **diffType** | **String**| whether the output is diff or patch | [enum: diff, patch] |

### Return type

**String**

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | APIString is a string response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoDownloadPullDiffOrPatch"></a>
# **repoDownloadPullDiffOrPatch**
> String repoDownloadPullDiffOrPatch(owner, repo, index, diffType, binary)

Get a pull request diff or patch

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request to get
    String diffType = "diff"; // String | whether the output is diff or patch
    Boolean binary = true; // Boolean | whether to include binary file changes. if true, the diff is applicable with `git apply`
    try {
      String result = apiInstance.repoDownloadPullDiffOrPatch(owner, repo, index, diffType, binary);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoDownloadPullDiffOrPatch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request to get | |
| **diffType** | **String**| whether the output is diff or patch | [enum: diff, patch] |
| **binary** | **Boolean**| whether to include binary file changes. if true, the diff is applicable with &#x60;git apply&#x60; | [optional] |

### Return type

**String**

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | APIString is a string response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoEdit"></a>
# **repoEdit**
> Repository repoEdit(owner, repo, body)

Edit a repository&#39;s properties. Only fields that are set will be changed.

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo to edit
    String repo = "repo_example"; // String | name of the repo to edit
    EditRepoOption body = new EditRepoOption(); // EditRepoOption | Properties of a repo that you can edit
    try {
      Repository result = apiInstance.repoEdit(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoEdit");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo to edit | |
| **repo** | **String**| name of the repo to edit | |
| **body** | [**EditRepoOption**](EditRepoOption.md)| Properties of a repo that you can edit | [optional] |

### Return type

[**Repository**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Repository |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoEditBranchProtection"></a>
# **repoEditBranchProtection**
> BranchProtection repoEditBranchProtection(owner, repo, name, body)

Edit a branch protections for a repository. Only fields that are set will be changed

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String name = "name_example"; // String | name of protected branch
    EditBranchProtectionOption body = new EditBranchProtectionOption(); // EditBranchProtectionOption | 
    try {
      BranchProtection result = apiInstance.repoEditBranchProtection(owner, repo, name, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoEditBranchProtection");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **name** | **String**| name of protected branch | |
| **body** | [**EditBranchProtectionOption**](EditBranchProtectionOption.md)|  | [optional] |

### Return type

[**BranchProtection**](BranchProtection.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | BranchProtection |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoEditGitHook"></a>
# **repoEditGitHook**
> GitHook repoEditGitHook(owner, repo, id, body)

Edit a Git hook in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String id = "id_example"; // String | id of the hook to get
    EditGitHookOption body = new EditGitHookOption(); // EditGitHookOption | 
    try {
      GitHook result = apiInstance.repoEditGitHook(owner, repo, id, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoEditGitHook");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **String**| id of the hook to get | |
| **body** | [**EditGitHookOption**](EditGitHookOption.md)|  | [optional] |

### Return type

[**GitHook**](GitHook.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GitHook |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoEditHook"></a>
# **repoEditHook**
> Hook repoEditHook(owner, repo, id, body)

Edit a hook in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | index of the hook
    EditHookOption body = new EditHookOption(); // EditHookOption | 
    try {
      Hook result = apiInstance.repoEditHook(owner, repo, id, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoEditHook");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| index of the hook | |
| **body** | [**EditHookOption**](EditHookOption.md)|  | [optional] |

### Return type

[**Hook**](Hook.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Hook |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoEditPullRequest"></a>
# **repoEditPullRequest**
> PullRequest repoEditPullRequest(owner, repo, index, body)

Update a pull request. If using deadline only the date will be taken into account, and time of day ignored.

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request to edit
    EditPullRequestOption body = new EditPullRequestOption(); // EditPullRequestOption | 
    try {
      PullRequest result = apiInstance.repoEditPullRequest(owner, repo, index, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoEditPullRequest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request to edit | |
| **body** | [**EditPullRequestOption**](EditPullRequestOption.md)|  | [optional] |

### Return type

[**PullRequest**](PullRequest.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | PullRequest |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | APIError is error format response |  -  |
| **412** | APIError is error format response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoEditRelease"></a>
# **repoEditRelease**
> Release repoEditRelease(owner, repo, id, body)

Update a release

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the release to edit
    EditReleaseOption body = new EditReleaseOption(); // EditReleaseOption | 
    try {
      Release result = apiInstance.repoEditRelease(owner, repo, id, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoEditRelease");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the release to edit | |
| **body** | [**EditReleaseOption**](EditReleaseOption.md)|  | [optional] |

### Return type

[**Release**](Release.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Release |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoEditReleaseAttachment"></a>
# **repoEditReleaseAttachment**
> Attachment repoEditReleaseAttachment(owner, repo, id, attachmentId, body)

Edit a release attachment

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the release
    Long attachmentId = 56L; // Long | id of the attachment to edit
    EditAttachmentOptions body = new EditAttachmentOptions(); // EditAttachmentOptions | 
    try {
      Attachment result = apiInstance.repoEditReleaseAttachment(owner, repo, id, attachmentId, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoEditReleaseAttachment");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the release | |
| **attachmentId** | **Long**| id of the attachment to edit | |
| **body** | [**EditAttachmentOptions**](EditAttachmentOptions.md)|  | [optional] |

### Return type

[**Attachment**](Attachment.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Attachment |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |

<a id="repoEditTagProtection"></a>
# **repoEditTagProtection**
> TagProtection repoEditTagProtection(owner, repo, id, body)

Edit a tag protections for a repository. Only fields that are set will be changed

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of protected tag
    EditTagProtectionOption body = new EditTagProtectionOption(); // EditTagProtectionOption | 
    try {
      TagProtection result = apiInstance.repoEditTagProtection(owner, repo, id, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoEditTagProtection");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of protected tag | |
| **body** | [**EditTagProtectionOption**](EditTagProtectionOption.md)|  | [optional] |

### Return type

[**TagProtection**](TagProtection.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | TagProtection |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoEditWikiPage"></a>
# **repoEditWikiPage**
> WikiPage repoEditWikiPage(owner, repo, pageName, body)

Edit a wiki page

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String pageName = "pageName_example"; // String | name of the page
    CreateWikiPageOptions body = new CreateWikiPageOptions(); // CreateWikiPageOptions | 
    try {
      WikiPage result = apiInstance.repoEditWikiPage(owner, repo, pageName, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoEditWikiPage");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **pageName** | **String**| name of the page | |
| **body** | [**CreateWikiPageOptions**](CreateWikiPageOptions.md)|  | [optional] |

### Return type

[**WikiPage**](WikiPage.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | WikiPage |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoGet"></a>
# **repoGet**
> Repository repoGet(owner, repo)

Get a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      Repository result = apiInstance.repoGet(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**Repository**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Repository |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetAllCommits"></a>
# **repoGetAllCommits**
> List&lt;Commit&gt; repoGetAllCommits(owner, repo, sha, path, stat, verification, files, page, limit, not)

Get a list of all commits from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | SHA or branch to start listing commits from (usually 'master')
    String path = "path_example"; // String | filepath of a file/dir
    Boolean stat = true; // Boolean | include diff stats for every commit (disable for speedup, default 'true')
    Boolean verification = true; // Boolean | include verification for every commit (disable for speedup, default 'true')
    Boolean files = true; // Boolean | include a list of affected files for every commit (disable for speedup, default 'true')
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results (ignored if used with 'path')
    String not = "not_example"; // String | commits that match the given specifier will not be listed.
    try {
      List<Commit> result = apiInstance.repoGetAllCommits(owner, repo, sha, path, stat, verification, files, page, limit, not);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetAllCommits");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| SHA or branch to start listing commits from (usually &#39;master&#39;) | [optional] |
| **path** | **String**| filepath of a file/dir | [optional] |
| **stat** | **Boolean**| include diff stats for every commit (disable for speedup, default &#39;true&#39;) | [optional] |
| **verification** | **Boolean**| include verification for every commit (disable for speedup, default &#39;true&#39;) | [optional] |
| **files** | **Boolean**| include a list of affected files for every commit (disable for speedup, default &#39;true&#39;) | [optional] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results (ignored if used with &#39;path&#39;) | [optional] |
| **not** | **String**| commits that match the given specifier will not be listed. | [optional] |

### Return type

[**List&lt;Commit&gt;**](Commit.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | CommitList |  * X-HasMore - True if there is another page <br>  * X-PageCount - Total number of pages <br>  * X-PerPage - Commits per page <br>  * X-Total - Total commit count <br>  * X-Page - The current page <br>  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | EmptyRepository |  -  |

<a id="repoGetArchive"></a>
# **repoGetArchive**
> repoGetArchive(owner, repo, archive)

Get an archive of a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String archive = "archive_example"; // String | the git reference for download with attached archive format (e.g. master.zip)
    try {
      apiInstance.repoGetArchive(owner, repo, archive);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetArchive");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **archive** | **String**| the git reference for download with attached archive format (e.g. master.zip) | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/octet-stream, application/zip, application/gzip

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | success |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetAssignees"></a>
# **repoGetAssignees**
> List&lt;User&gt; repoGetAssignees(owner, repo)

Return all users that have write access and can be assigned to issues

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      List<User> result = apiInstance.repoGetAssignees(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetAssignees");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**List&lt;User&gt;**](User.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | UserList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetBranch"></a>
# **repoGetBranch**
> Branch repoGetBranch(owner, repo, branch)

Retrieve a specific branch from a repository, including its effective branch protection

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String branch = "branch_example"; // String | branch to get
    try {
      Branch result = apiInstance.repoGetBranch(owner, repo, branch);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetBranch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **branch** | **String**| branch to get | |

### Return type

[**Branch**](Branch.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Branch |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetBranchProtection"></a>
# **repoGetBranchProtection**
> BranchProtection repoGetBranchProtection(owner, repo, name)

Get a specific branch protection for the repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String name = "name_example"; // String | name of protected branch
    try {
      BranchProtection result = apiInstance.repoGetBranchProtection(owner, repo, name);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetBranchProtection");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **name** | **String**| name of protected branch | |

### Return type

[**BranchProtection**](BranchProtection.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | BranchProtection |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetByID"></a>
# **repoGetByID**
> Repository repoGetByID(id)

Get a repository by id

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    Long id = 56L; // Long | id of the repo to get
    try {
      Repository result = apiInstance.repoGetByID(id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetByID");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **Long**| id of the repo to get | |

### Return type

[**Repository**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Repository |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetCombinedStatusByRef"></a>
# **repoGetCombinedStatusByRef**
> CombinedStatus repoGetCombinedStatusByRef(owner, repo, ref, page, limit)

Get a commit&#39;s combined status, by branch/tag/commit reference

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String ref = "ref_example"; // String | name of branch/tag/commit
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      CombinedStatus result = apiInstance.repoGetCombinedStatusByRef(owner, repo, ref, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetCombinedStatusByRef");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **ref** | **String**| name of branch/tag/commit | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**CombinedStatus**](CombinedStatus.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | CombinedStatus |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetCommitPullRequest"></a>
# **repoGetCommitPullRequest**
> PullRequest repoGetCommitPullRequest(owner, repo, sha)

Get the pull request of the commit

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | SHA of the commit to get
    try {
      PullRequest result = apiInstance.repoGetCommitPullRequest(owner, repo, sha);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetCommitPullRequest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| SHA of the commit to get | |

### Return type

[**PullRequest**](PullRequest.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullRequest |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetContents"></a>
# **repoGetContents**
> ContentsResponse repoGetContents(owner, repo, filepath, ref)

Gets the metadata and contents (if a file) of an entry in a repository, or a list of entries if a dir

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String filepath = "filepath_example"; // String | path of the dir, file, symlink or submodule in the repo
    String ref = "ref_example"; // String | The name of the commit/branch/tag. Default the repository’s default branch (usually master)
    try {
      ContentsResponse result = apiInstance.repoGetContents(owner, repo, filepath, ref);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetContents");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **filepath** | **String**| path of the dir, file, symlink or submodule in the repo | |
| **ref** | **String**| The name of the commit/branch/tag. Default the repository’s default branch (usually master) | [optional] |

### Return type

[**ContentsResponse**](ContentsResponse.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ContentsResponse |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetContentsList"></a>
# **repoGetContentsList**
> List&lt;ContentsResponse&gt; repoGetContentsList(owner, repo, ref)

Gets the metadata of all the entries of the root dir

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String ref = "ref_example"; // String | The name of the commit/branch/tag. Default the repository’s default branch (usually master)
    try {
      List<ContentsResponse> result = apiInstance.repoGetContentsList(owner, repo, ref);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetContentsList");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **ref** | **String**| The name of the commit/branch/tag. Default the repository’s default branch (usually master) | [optional] |

### Return type

[**List&lt;ContentsResponse&gt;**](ContentsResponse.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ContentsListResponse |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetEditorConfig"></a>
# **repoGetEditorConfig**
> Map&lt;String, String&gt; repoGetEditorConfig(owner, repo, filepath, ref)

Get the EditorConfig definitions of a file in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String filepath = "filepath_example"; // String | filepath of file to get
    String ref = "ref_example"; // String | The name of the commit/branch/tag. Default the repository’s default branch (usually master)
    try {
      Map<String, String> result = apiInstance.repoGetEditorConfig(owner, repo, filepath, ref);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetEditorConfig");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **filepath** | **String**| filepath of file to get | |
| **ref** | **String**| The name of the commit/branch/tag. Default the repository’s default branch (usually master) | [optional] |

### Return type

**Map&lt;String, String&gt;**

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | definitions |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetGitHook"></a>
# **repoGetGitHook**
> GitHook repoGetGitHook(owner, repo, id)

Get a Git hook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String id = "id_example"; // String | id of the hook to get
    try {
      GitHook result = apiInstance.repoGetGitHook(owner, repo, id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetGitHook");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **String**| id of the hook to get | |

### Return type

[**GitHook**](GitHook.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GitHook |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetHook"></a>
# **repoGetHook**
> Hook repoGetHook(owner, repo, id)

Get a hook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the hook to get
    try {
      Hook result = apiInstance.repoGetHook(owner, repo, id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetHook");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the hook to get | |

### Return type

[**Hook**](Hook.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Hook |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetIssueConfig"></a>
# **repoGetIssueConfig**
> IssueConfig repoGetIssueConfig(owner, repo)

Returns the issue config for a repo

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      IssueConfig result = apiInstance.repoGetIssueConfig(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetIssueConfig");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**IssueConfig**](IssueConfig.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | RepoIssueConfig |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetIssueTemplates"></a>
# **repoGetIssueTemplates**
> List&lt;IssueTemplate&gt; repoGetIssueTemplates(owner, repo)

Get available issue templates for a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      List<IssueTemplate> result = apiInstance.repoGetIssueTemplates(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetIssueTemplates");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**List&lt;IssueTemplate&gt;**](IssueTemplate.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | IssueTemplates |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetKey"></a>
# **repoGetKey**
> DeployKey repoGetKey(owner, repo, id)

Get a repository&#39;s key by id

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the key to get
    try {
      DeployKey result = apiInstance.repoGetKey(owner, repo, id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetKey");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the key to get | |

### Return type

[**DeployKey**](DeployKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | DeployKey |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetLanguages"></a>
# **repoGetLanguages**
> Map&lt;String, Long&gt; repoGetLanguages(owner, repo)

Get languages and number of bytes of code written

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      Map<String, Long> result = apiInstance.repoGetLanguages(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetLanguages");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

**Map&lt;String, Long&gt;**

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | LanguageStatistics |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetLatestRelease"></a>
# **repoGetLatestRelease**
> Release repoGetLatestRelease(owner, repo)

Gets the most recent non-prerelease, non-draft release of a repository, sorted by created_at

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      Release result = apiInstance.repoGetLatestRelease(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetLatestRelease");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**Release**](Release.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Release |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetNote"></a>
# **repoGetNote**
> Note repoGetNote(owner, repo, sha, verification, files)

Get a note corresponding to a single commit from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | a git ref or commit sha
    Boolean verification = true; // Boolean | include verification for every commit (disable for speedup, default 'true')
    Boolean files = true; // Boolean | include a list of affected files for every commit (disable for speedup, default 'true')
    try {
      Note result = apiInstance.repoGetNote(owner, repo, sha, verification, files);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetNote");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| a git ref or commit sha | |
| **verification** | **Boolean**| include verification for every commit (disable for speedup, default &#39;true&#39;) | [optional] |
| **files** | **Boolean**| include a list of affected files for every commit (disable for speedup, default &#39;true&#39;) | [optional] |

### Return type

[**Note**](Note.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Note |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoGetPullRequest"></a>
# **repoGetPullRequest**
> PullRequest repoGetPullRequest(owner, repo, index)

Get a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request to get
    try {
      PullRequest result = apiInstance.repoGetPullRequest(owner, repo, index);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetPullRequest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request to get | |

### Return type

[**PullRequest**](PullRequest.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullRequest |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetPullRequestByBaseHead"></a>
# **repoGetPullRequestByBaseHead**
> PullRequest repoGetPullRequestByBaseHead(owner, repo, base, head)

Get a pull request by base and head

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String base = "base_example"; // String | base of the pull request to get
    String head = "head_example"; // String | head of the pull request to get
    try {
      PullRequest result = apiInstance.repoGetPullRequestByBaseHead(owner, repo, base, head);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetPullRequestByBaseHead");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **base** | **String**| base of the pull request to get | |
| **head** | **String**| head of the pull request to get | |

### Return type

[**PullRequest**](PullRequest.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullRequest |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetPullRequestCommits"></a>
# **repoGetPullRequestCommits**
> List&lt;Commit&gt; repoGetPullRequestCommits(owner, repo, index, page, limit, verification, files)

Get commits for a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request to get
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    Boolean verification = true; // Boolean | include verification for every commit (disable for speedup, default 'true')
    Boolean files = true; // Boolean | include a list of affected files for every commit (disable for speedup, default 'true')
    try {
      List<Commit> result = apiInstance.repoGetPullRequestCommits(owner, repo, index, page, limit, verification, files);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetPullRequestCommits");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request to get | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |
| **verification** | **Boolean**| include verification for every commit (disable for speedup, default &#39;true&#39;) | [optional] |
| **files** | **Boolean**| include a list of affected files for every commit (disable for speedup, default &#39;true&#39;) | [optional] |

### Return type

[**List&lt;Commit&gt;**](Commit.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | CommitList |  * X-HasMore - True if there is another page <br>  * X-PageCount - Total number of pages <br>  * X-PerPage - Commits per page <br>  * X-Total - Total commit count <br>  * X-Page - The current page <br>  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetPullRequestFiles"></a>
# **repoGetPullRequestFiles**
> List&lt;ChangedFile&gt; repoGetPullRequestFiles(owner, repo, index, skipTo, whitespace, page, limit)

Get changed files for a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request to get
    String skipTo = "skipTo_example"; // String | skip to given file
    String whitespace = "ignore-all"; // String | whitespace behavior
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<ChangedFile> result = apiInstance.repoGetPullRequestFiles(owner, repo, index, skipTo, whitespace, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetPullRequestFiles");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request to get | |
| **skipTo** | **String**| skip to given file | [optional] |
| **whitespace** | **String**| whitespace behavior | [optional] [enum: ignore-all, ignore-change, ignore-eol, show-all] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;ChangedFile&gt;**](ChangedFile.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ChangedFileList |  * X-HasMore - True if there is another page <br>  * X-PageCount - Total number of pages <br>  * X-PerPage - Commits per page <br>  * X-Total-Count - Total commit count <br>  * X-Page - The current page <br>  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetPullReview"></a>
# **repoGetPullReview**
> PullReview repoGetPullReview(owner, repo, index, id)

Get a specific review for a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    Long id = 56L; // Long | id of the review
    try {
      PullReview result = apiInstance.repoGetPullReview(owner, repo, index, id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetPullReview");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **id** | **Long**| id of the review | |

### Return type

[**PullReview**](PullReview.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullReview |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetPullReviewComment"></a>
# **repoGetPullReviewComment**
> PullReviewComment repoGetPullReviewComment(owner, repo, index, id, comment)

Get a pull review comment

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    Long id = 56L; // Long | id of the review
    Long comment = 56L; // Long | id of the comment
    try {
      PullReviewComment result = apiInstance.repoGetPullReviewComment(owner, repo, index, id, comment);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetPullReviewComment");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **id** | **Long**| id of the review | |
| **comment** | **Long**| id of the comment | |

### Return type

[**PullReviewComment**](PullReviewComment.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullComment |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetPullReviewComments"></a>
# **repoGetPullReviewComments**
> List&lt;PullReviewComment&gt; repoGetPullReviewComments(owner, repo, index, id)

Get a specific review for a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    Long id = 56L; // Long | id of the review
    try {
      List<PullReviewComment> result = apiInstance.repoGetPullReviewComments(owner, repo, index, id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetPullReviewComments");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **id** | **Long**| id of the review | |

### Return type

[**List&lt;PullReviewComment&gt;**](PullReviewComment.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullCommentList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetPushMirrorByRemoteName"></a>
# **repoGetPushMirrorByRemoteName**
> PushMirror repoGetPushMirrorByRemoteName(owner, repo, name)

Get push mirror of the repository by remoteName

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String name = "name_example"; // String | remote name of push mirror
    try {
      PushMirror result = apiInstance.repoGetPushMirrorByRemoteName(owner, repo, name);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetPushMirrorByRemoteName");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **name** | **String**| remote name of push mirror | |

### Return type

[**PushMirror**](PushMirror.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PushMirror |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetRawFile"></a>
# **repoGetRawFile**
> File repoGetRawFile(owner, repo, filepath, ref)

Get a file from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String filepath = "filepath_example"; // String | filepath of the file to get
    String ref = "ref_example"; // String | The name of the commit/branch/tag. Default the repository’s default branch (usually master)
    try {
      File result = apiInstance.repoGetRawFile(owner, repo, filepath, ref);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetRawFile");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **filepath** | **String**| filepath of the file to get | |
| **ref** | **String**| The name of the commit/branch/tag. Default the repository’s default branch (usually master) | [optional] |

### Return type

[**File**](File.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/octet-stream

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Returns raw file content. |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetRawFileOrLFS"></a>
# **repoGetRawFileOrLFS**
> File repoGetRawFileOrLFS(owner, repo, filepath, ref)

Get a file or it&#39;s LFS object from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String filepath = "filepath_example"; // String | filepath of the file to get
    String ref = "ref_example"; // String | The name of the commit/branch/tag. Default the repository’s default branch (usually master)
    try {
      File result = apiInstance.repoGetRawFileOrLFS(owner, repo, filepath, ref);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetRawFileOrLFS");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **filepath** | **String**| filepath of the file to get | |
| **ref** | **String**| The name of the commit/branch/tag. Default the repository’s default branch (usually master) | [optional] |

### Return type

[**File**](File.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/octet-stream

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Returns raw file content. |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetRelease"></a>
# **repoGetRelease**
> Release repoGetRelease(owner, repo, id)

Get a release

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the release to get
    try {
      Release result = apiInstance.repoGetRelease(owner, repo, id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetRelease");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the release to get | |

### Return type

[**Release**](Release.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Release |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetReleaseAttachment"></a>
# **repoGetReleaseAttachment**
> Attachment repoGetReleaseAttachment(owner, repo, id, attachmentId)

Get a release attachment

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the release
    Long attachmentId = 56L; // Long | id of the attachment to get
    try {
      Attachment result = apiInstance.repoGetReleaseAttachment(owner, repo, id, attachmentId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetReleaseAttachment");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the release | |
| **attachmentId** | **Long**| id of the attachment to get | |

### Return type

[**Attachment**](Attachment.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Attachment |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetReleaseByTag"></a>
# **repoGetReleaseByTag**
> Release repoGetReleaseByTag(owner, repo, tag)

Get a release by tag name

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String tag = "tag_example"; // String | tag name of the release to get
    try {
      Release result = apiInstance.repoGetReleaseByTag(owner, repo, tag);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetReleaseByTag");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **tag** | **String**| tag name of the release to get | |

### Return type

[**Release**](Release.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Release |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetRepoPermissions"></a>
# **repoGetRepoPermissions**
> RepoCollaboratorPermission repoGetRepoPermissions(owner, repo, collaborator)

Get repository permissions for a user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String collaborator = "collaborator_example"; // String | username of the collaborator
    try {
      RepoCollaboratorPermission result = apiInstance.repoGetRepoPermissions(owner, repo, collaborator);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetRepoPermissions");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **collaborator** | **String**| username of the collaborator | |

### Return type

[**RepoCollaboratorPermission**](RepoCollaboratorPermission.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | RepoCollaboratorPermission |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetReviewers"></a>
# **repoGetReviewers**
> List&lt;User&gt; repoGetReviewers(owner, repo)

Return all users that can be requested to review in this repo

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      List<User> result = apiInstance.repoGetReviewers(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetReviewers");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**List&lt;User&gt;**](User.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | UserList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetRunnerRegistrationToken"></a>
# **repoGetRunnerRegistrationToken**
> RegistrationToken repoGetRunnerRegistrationToken(owner, repo)

Get a repository&#39;s actions runner registration token

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      RegistrationToken result = apiInstance.repoGetRunnerRegistrationToken(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetRunnerRegistrationToken");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**RegistrationToken**](RegistrationToken.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | RegistrationToken is a string used to register a runner with a server |  -  |

<a id="repoGetSingleCommit"></a>
# **repoGetSingleCommit**
> Commit repoGetSingleCommit(owner, repo, sha, stat, verification, files)

Get a single commit from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | a git ref or commit sha
    Boolean stat = true; // Boolean | include diff stats for every commit (disable for speedup, default 'true')
    Boolean verification = true; // Boolean | include verification for every commit (disable for speedup, default 'true')
    Boolean files = true; // Boolean | include a list of affected files for every commit (disable for speedup, default 'true')
    try {
      Commit result = apiInstance.repoGetSingleCommit(owner, repo, sha, stat, verification, files);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetSingleCommit");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| a git ref or commit sha | |
| **stat** | **Boolean**| include diff stats for every commit (disable for speedup, default &#39;true&#39;) | [optional] |
| **verification** | **Boolean**| include verification for every commit (disable for speedup, default &#39;true&#39;) | [optional] |
| **files** | **Boolean**| include a list of affected files for every commit (disable for speedup, default &#39;true&#39;) | [optional] |

### Return type

[**Commit**](Commit.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Commit |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoGetTag"></a>
# **repoGetTag**
> Tag repoGetTag(owner, repo, tag)

Get the tag of a repository by tag name

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String tag = "tag_example"; // String | name of tag
    try {
      Tag result = apiInstance.repoGetTag(owner, repo, tag);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetTag");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **tag** | **String**| name of tag | |

### Return type

[**Tag**](Tag.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tag |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetTagProtection"></a>
# **repoGetTagProtection**
> TagProtection repoGetTagProtection(owner, repo, id)

Get a specific tag protection for the repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the tag protect to get
    try {
      TagProtection result = apiInstance.repoGetTagProtection(owner, repo, id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetTagProtection");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the tag protect to get | |

### Return type

[**TagProtection**](TagProtection.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | TagProtection |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetWikiPage"></a>
# **repoGetWikiPage**
> WikiPage repoGetWikiPage(owner, repo, pageName)

Get a wiki page

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String pageName = "pageName_example"; // String | name of the page
    try {
      WikiPage result = apiInstance.repoGetWikiPage(owner, repo, pageName);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetWikiPage");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **pageName** | **String**| name of the page | |

### Return type

[**WikiPage**](WikiPage.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | WikiPage |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetWikiPageRevisions"></a>
# **repoGetWikiPageRevisions**
> WikiCommitList repoGetWikiPageRevisions(owner, repo, pageName, page)

Get revisions of a wiki page

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String pageName = "pageName_example"; // String | name of the page
    Integer page = 56; // Integer | page number of results to return (1-based)
    try {
      WikiCommitList result = apiInstance.repoGetWikiPageRevisions(owner, repo, pageName, page);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetWikiPageRevisions");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **pageName** | **String**| name of the page | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |

### Return type

[**WikiCommitList**](WikiCommitList.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | WikiCommitList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoGetWikiPages"></a>
# **repoGetWikiPages**
> List&lt;WikiPageMetaData&gt; repoGetWikiPages(owner, repo, page, limit)

Get all wiki pages

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<WikiPageMetaData> result = apiInstance.repoGetWikiPages(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoGetWikiPages");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;WikiPageMetaData&gt;**](WikiPageMetaData.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | WikiPageList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListActionsSecrets"></a>
# **repoListActionsSecrets**
> List&lt;Secret&gt; repoListActionsSecrets(owner, repo, page, limit)

List an repo&#39;s actions secrets

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repository
    String repo = "repo_example"; // String | name of the repository
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Secret> result = apiInstance.repoListActionsSecrets(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListActionsSecrets");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repository | |
| **repo** | **String**| name of the repository | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;Secret&gt;**](Secret.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SecretList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListActivityFeeds"></a>
# **repoListActivityFeeds**
> List&lt;Activity&gt; repoListActivityFeeds(owner, repo, date, page, limit)

List a repository&#39;s activity feeds

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    LocalDate date = LocalDate.now(); // LocalDate | the date of the activities to be found
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Activity> result = apiInstance.repoListActivityFeeds(owner, repo, date, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListActivityFeeds");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **date** | **LocalDate**| the date of the activities to be found | [optional] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;Activity&gt;**](Activity.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ActivityFeedsList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListAllGitRefs"></a>
# **repoListAllGitRefs**
> List&lt;Reference&gt; repoListAllGitRefs(owner, repo)

Get specified ref or filtered repository&#39;s refs

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      List<Reference> result = apiInstance.repoListAllGitRefs(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListAllGitRefs");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**List&lt;Reference&gt;**](Reference.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ReferenceList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListBranchProtection"></a>
# **repoListBranchProtection**
> List&lt;BranchProtection&gt; repoListBranchProtection(owner, repo)

List branch protections for a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      List<BranchProtection> result = apiInstance.repoListBranchProtection(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListBranchProtection");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**List&lt;BranchProtection&gt;**](BranchProtection.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | BranchProtectionList |  -  |

<a id="repoListBranches"></a>
# **repoListBranches**
> List&lt;Branch&gt; repoListBranches(owner, repo, page, limit)

List a repository&#39;s branches

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Branch> result = apiInstance.repoListBranches(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListBranches");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;Branch&gt;**](Branch.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | BranchList |  -  |

<a id="repoListCollaborators"></a>
# **repoListCollaborators**
> List&lt;User&gt; repoListCollaborators(owner, repo, page, limit)

List a repository&#39;s collaborators

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<User> result = apiInstance.repoListCollaborators(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListCollaborators");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;User&gt;**](User.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | UserList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListFlags"></a>
# **repoListFlags**
> List&lt;String&gt; repoListFlags(owner, repo)

List a repository&#39;s flags

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      List<String> result = apiInstance.repoListFlags(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListFlags");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

**List&lt;String&gt;**

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | StringSlice |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListGitHooks"></a>
# **repoListGitHooks**
> List&lt;GitHook&gt; repoListGitHooks(owner, repo)

List the Git hooks in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      List<GitHook> result = apiInstance.repoListGitHooks(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListGitHooks");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**List&lt;GitHook&gt;**](GitHook.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GitHookList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListGitRefs"></a>
# **repoListGitRefs**
> List&lt;Reference&gt; repoListGitRefs(owner, repo, ref)

Get specified ref or filtered repository&#39;s refs

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String ref = "ref_example"; // String | part or full name of the ref
    try {
      List<Reference> result = apiInstance.repoListGitRefs(owner, repo, ref);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListGitRefs");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **ref** | **String**| part or full name of the ref | |

### Return type

[**List&lt;Reference&gt;**](Reference.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ReferenceList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListHooks"></a>
# **repoListHooks**
> List&lt;Hook&gt; repoListHooks(owner, repo, page, limit)

List the hooks in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Hook> result = apiInstance.repoListHooks(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListHooks");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;Hook&gt;**](Hook.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | HookList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListKeys"></a>
# **repoListKeys**
> List&lt;DeployKey&gt; repoListKeys(owner, repo, keyId, fingerprint, page, limit)

List a repository&#39;s keys

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer keyId = 56; // Integer | the key_id to search for
    String fingerprint = "fingerprint_example"; // String | fingerprint of the key
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<DeployKey> result = apiInstance.repoListKeys(owner, repo, keyId, fingerprint, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListKeys");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **keyId** | **Integer**| the key_id to search for | [optional] |
| **fingerprint** | **String**| fingerprint of the key | [optional] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;DeployKey&gt;**](DeployKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | DeployKeyList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListPinnedIssues"></a>
# **repoListPinnedIssues**
> List&lt;Issue&gt; repoListPinnedIssues(owner, repo)

List a repo&#39;s pinned issues

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      List<Issue> result = apiInstance.repoListPinnedIssues(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListPinnedIssues");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**List&lt;Issue&gt;**](Issue.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | IssueList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListPinnedPullRequests"></a>
# **repoListPinnedPullRequests**
> List&lt;PullRequest&gt; repoListPinnedPullRequests(owner, repo)

List a repo&#39;s pinned pull requests

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      List<PullRequest> result = apiInstance.repoListPinnedPullRequests(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListPinnedPullRequests");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**List&lt;PullRequest&gt;**](PullRequest.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullRequestList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListPullRequests"></a>
# **repoListPullRequests**
> List&lt;PullRequest&gt; repoListPullRequests(owner, repo, state, sort, milestone, labels, poster, page, limit)

List a repo&#39;s pull requests. If a pull request is selected but fails to be retrieved for any reason, it will be a null value in the list of results.

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | Owner of the repo
    String repo = "repo_example"; // String | Name of the repo
    String state = "open"; // String | State of pull request
    String sort = "oldest"; // String | Type of sort
    Long milestone = 56L; // Long | ID of the milestone
    List<Long> labels = Arrays.asList(); // List<Long> | Label IDs
    String poster = "poster_example"; // String | Filter by pull request author
    Integer page = 1; // Integer | Page number of results to return (1-based)
    Integer limit = 56; // Integer | Page size of results
    try {
      List<PullRequest> result = apiInstance.repoListPullRequests(owner, repo, state, sort, milestone, labels, poster, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListPullRequests");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| Owner of the repo | |
| **repo** | **String**| Name of the repo | |
| **state** | **String**| State of pull request | [optional] [default to open] [enum: open, closed, all] |
| **sort** | **String**| Type of sort | [optional] [enum: oldest, recentupdate, recentclose, leastupdate, mostcomment, leastcomment, priority] |
| **milestone** | **Long**| ID of the milestone | [optional] |
| **labels** | [**List&lt;Long&gt;**](Long.md)| Label IDs | [optional] |
| **poster** | **String**| Filter by pull request author | [optional] |
| **page** | **Integer**| Page number of results to return (1-based) | [optional] [default to 1] |
| **limit** | **Integer**| Page size of results | [optional] |

### Return type

[**List&lt;PullRequest&gt;**](PullRequest.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullRequestList |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **500** | APIError is error format response |  -  |

<a id="repoListPullReviews"></a>
# **repoListPullReviews**
> List&lt;PullReview&gt; repoListPullReviews(owner, repo, index, page, limit)

List all reviews for a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<PullReview> result = apiInstance.repoListPullReviews(owner, repo, index, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListPullReviews");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;PullReview&gt;**](PullReview.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullReviewList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListPushMirrors"></a>
# **repoListPushMirrors**
> List&lt;PushMirror&gt; repoListPushMirrors(owner, repo, page, limit)

Get all push mirrors of the repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<PushMirror> result = apiInstance.repoListPushMirrors(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListPushMirrors");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;PushMirror&gt;**](PushMirror.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PushMirrorList |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListReleaseAttachments"></a>
# **repoListReleaseAttachments**
> List&lt;Attachment&gt; repoListReleaseAttachments(owner, repo, id)

List release&#39;s attachments

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the release
    try {
      List<Attachment> result = apiInstance.repoListReleaseAttachments(owner, repo, id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListReleaseAttachments");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the release | |

### Return type

[**List&lt;Attachment&gt;**](Attachment.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | AttachmentList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListReleases"></a>
# **repoListReleases**
> List&lt;Release&gt; repoListReleases(owner, repo, draft, preRelease, q, page, limit)

List a repo&#39;s releases

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Boolean draft = true; // Boolean | filter (exclude / include) drafts, if you dont have repo write access none will show
    Boolean preRelease = true; // Boolean | filter (exclude / include) pre-releases
    String q = "q_example"; // String | Search string
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Release> result = apiInstance.repoListReleases(owner, repo, draft, preRelease, q, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListReleases");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **draft** | **Boolean**| filter (exclude / include) drafts, if you dont have repo write access none will show | [optional] |
| **preRelease** | **Boolean**| filter (exclude / include) pre-releases | [optional] |
| **q** | **String**| Search string | [optional] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;Release&gt;**](Release.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | ReleaseList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListStargazers"></a>
# **repoListStargazers**
> List&lt;User&gt; repoListStargazers(owner, repo, page, limit)

List a repo&#39;s stargazers

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<User> result = apiInstance.repoListStargazers(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListStargazers");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;User&gt;**](User.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | UserList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListStatuses"></a>
# **repoListStatuses**
> List&lt;CommitStatus&gt; repoListStatuses(owner, repo, sha, sort, state, page, limit)

Get a commit&#39;s statuses

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | sha of the commit
    String sort = "oldest"; // String | type of sort
    String state = "pending"; // String | type of state
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<CommitStatus> result = apiInstance.repoListStatuses(owner, repo, sha, sort, state, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListStatuses");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| sha of the commit | |
| **sort** | **String**| type of sort | [optional] [enum: oldest, recentupdate, leastupdate, leastindex, highestindex] |
| **state** | **String**| type of state | [optional] [enum: pending, success, error, failure, warning] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;CommitStatus&gt;**](CommitStatus.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | CommitStatusList |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListStatusesByRef"></a>
# **repoListStatusesByRef**
> List&lt;CommitStatus&gt; repoListStatusesByRef(owner, repo, ref, sort, state, page, limit)

Get a commit&#39;s statuses, by branch/tag/commit reference

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String ref = "ref_example"; // String | name of branch/tag/commit
    String sort = "oldest"; // String | type of sort
    String state = "pending"; // String | type of state
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<CommitStatus> result = apiInstance.repoListStatusesByRef(owner, repo, ref, sort, state, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListStatusesByRef");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **ref** | **String**| name of branch/tag/commit | |
| **sort** | **String**| type of sort | [optional] [enum: oldest, recentupdate, leastupdate, leastindex, highestindex] |
| **state** | **String**| type of state | [optional] [enum: pending, success, error, failure, warning] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;CommitStatus&gt;**](CommitStatus.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | CommitStatusList |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListSubscribers"></a>
# **repoListSubscribers**
> List&lt;User&gt; repoListSubscribers(owner, repo, page, limit)

List a repo&#39;s watchers

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<User> result = apiInstance.repoListSubscribers(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListSubscribers");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;User&gt;**](User.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | UserList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListTagProtection"></a>
# **repoListTagProtection**
> List&lt;TagProtection&gt; repoListTagProtection(owner, repo)

List tag protections for a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      List<TagProtection> result = apiInstance.repoListTagProtection(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListTagProtection");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**List&lt;TagProtection&gt;**](TagProtection.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | TagProtectionList |  -  |

<a id="repoListTags"></a>
# **repoListTags**
> List&lt;Tag&gt; repoListTags(owner, repo, page, limit)

List a repository&#39;s tags

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results, default maximum page size is 50
    try {
      List<Tag> result = apiInstance.repoListTags(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListTags");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results, default maximum page size is 50 | [optional] |

### Return type

[**List&lt;Tag&gt;**](Tag.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | TagList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListTeams"></a>
# **repoListTeams**
> List&lt;Team&gt; repoListTeams(owner, repo)

List a repository&#39;s teams

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      List<Team> result = apiInstance.repoListTeams(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListTeams");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**List&lt;Team&gt;**](Team.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | TeamList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoListTopics"></a>
# **repoListTopics**
> TopicName repoListTopics(owner, repo, page, limit)

Get list of topics that a repository has

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      TopicName result = apiInstance.repoListTopics(owner, repo, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoListTopics");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**TopicName**](TopicName.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | TopicNames |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoMergePullRequest"></a>
# **repoMergePullRequest**
> repoMergePullRequest(owner, repo, index, body)

Merge a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request to merge
    MergePullRequestOption body = new MergePullRequestOption(); // MergePullRequestOption | 
    try {
      apiInstance.repoMergePullRequest(owner, repo, index, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoMergePullRequest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request to merge | |
| **body** | [**MergePullRequestOption**](MergePullRequestOption.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **405** | APIEmpty is an empty response |  -  |
| **409** | APIError is error format response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoMigrate"></a>
# **repoMigrate**
> Repository repoMigrate(body)

Migrate a remote git repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    MigrateRepoOptions body = new MigrateRepoOptions(); // MigrateRepoOptions | 
    try {
      Repository result = apiInstance.repoMigrate(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoMigrate");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**MigrateRepoOptions**](MigrateRepoOptions.md)|  | [optional] |

### Return type

[**Repository**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Repository |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **409** | The repository with the same name already exists. |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoMirrorSync"></a>
# **repoMirrorSync**
> repoMirrorSync(owner, repo)

Sync a mirrored repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo to sync
    String repo = "repo_example"; // String | name of the repo to sync
    try {
      apiInstance.repoMirrorSync(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoMirrorSync");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo to sync | |
| **repo** | **String**| name of the repo to sync | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |

<a id="repoNewPinAllowed"></a>
# **repoNewPinAllowed**
> NewIssuePinsAllowed repoNewPinAllowed(owner, repo)

Returns if new Issue Pins are allowed

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      NewIssuePinsAllowed result = apiInstance.repoNewPinAllowed(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoNewPinAllowed");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**NewIssuePinsAllowed**](NewIssuePinsAllowed.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | RepoNewIssuePinsAllowed |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoPullRequestIsMerged"></a>
# **repoPullRequestIsMerged**
> repoPullRequestIsMerged(owner, repo, index)

Check if a pull request has been merged

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    try {
      apiInstance.repoPullRequestIsMerged(owner, repo, index);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoPullRequestIsMerged");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | pull request has been merged |  -  |
| **404** | pull request has not been merged |  -  |

<a id="repoPushMirrorSync"></a>
# **repoPushMirrorSync**
> repoPushMirrorSync(owner, repo)

Sync all push mirrored repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo to sync
    String repo = "repo_example"; // String | name of the repo to sync
    try {
      apiInstance.repoPushMirrorSync(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoPushMirrorSync");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo to sync | |
| **repo** | **String**| name of the repo to sync | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | APIEmpty is an empty response |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |

<a id="repoRemoveNote"></a>
# **repoRemoveNote**
> repoRemoveNote(owner, repo, sha)

Removes a note corresponding to a single commit from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | a git ref or commit sha
    try {
      apiInstance.repoRemoveNote(owner, repo, sha);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoRemoveNote");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| a git ref or commit sha | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoReplaceAllFlags"></a>
# **repoReplaceAllFlags**
> repoReplaceAllFlags(owner, repo, body)

Replace all flags of a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    ReplaceFlagsOption body = new ReplaceFlagsOption(); // ReplaceFlagsOption | 
    try {
      apiInstance.repoReplaceAllFlags(owner, repo, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoReplaceAllFlags");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**ReplaceFlagsOption**](ReplaceFlagsOption.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoSearch"></a>
# **repoSearch**
> SearchResults repoSearch(q, topic, includeDesc, uid, priorityOwnerId, teamId, starredBy, _private, isPrivate, template, archived, mode, exclusive, sort, order, page, limit)

Search for repositories

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String q = "q_example"; // String | keyword
    Boolean topic = true; // Boolean | Limit search to repositories with keyword as topic
    Boolean includeDesc = true; // Boolean | include search of keyword within repository description
    Long uid = 56L; // Long | search only for repos that the user with the given id owns or contributes to
    Long priorityOwnerId = 56L; // Long | repo owner to prioritize in the results
    Long teamId = 56L; // Long | search only for repos that belong to the given team id
    Long starredBy = 56L; // Long | search only for repos that the user with the given id has starred
    Boolean _private = true; // Boolean | include private repositories this user has access to (defaults to true)
    Boolean isPrivate = true; // Boolean | show only public, private or all repositories (defaults to all)
    Boolean template = true; // Boolean | include template repositories this user has access to (defaults to true)
    Boolean archived = true; // Boolean | show only archived, non-archived or all repositories (defaults to all)
    String mode = "mode_example"; // String | type of repository to search for. Supported values are \"fork\", \"source\", \"mirror\" and \"collaborative\"
    Boolean exclusive = true; // Boolean | if `uid` is given, search only for repos that the user owns
    String sort = "alpha"; // String | sort repos by attribute. Supported values are \"alpha\", \"created\", \"updated\", \"size\", \"git_size\", \"lfs_size\", \"stars\", \"forks\" and \"id\". Default is \"alpha\"
    String order = "asc"; // String | sort order, either \"asc\" (ascending) or \"desc\" (descending). Default is \"asc\", ignored if \"sort\" is not specified.
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      SearchResults result = apiInstance.repoSearch(q, topic, includeDesc, uid, priorityOwnerId, teamId, starredBy, _private, isPrivate, template, archived, mode, exclusive, sort, order, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoSearch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **q** | **String**| keyword | [optional] |
| **topic** | **Boolean**| Limit search to repositories with keyword as topic | [optional] |
| **includeDesc** | **Boolean**| include search of keyword within repository description | [optional] |
| **uid** | **Long**| search only for repos that the user with the given id owns or contributes to | [optional] |
| **priorityOwnerId** | **Long**| repo owner to prioritize in the results | [optional] |
| **teamId** | **Long**| search only for repos that belong to the given team id | [optional] |
| **starredBy** | **Long**| search only for repos that the user with the given id has starred | [optional] |
| **_private** | **Boolean**| include private repositories this user has access to (defaults to true) | [optional] |
| **isPrivate** | **Boolean**| show only public, private or all repositories (defaults to all) | [optional] |
| **template** | **Boolean**| include template repositories this user has access to (defaults to true) | [optional] |
| **archived** | **Boolean**| show only archived, non-archived or all repositories (defaults to all) | [optional] |
| **mode** | **String**| type of repository to search for. Supported values are \&quot;fork\&quot;, \&quot;source\&quot;, \&quot;mirror\&quot; and \&quot;collaborative\&quot; | [optional] |
| **exclusive** | **Boolean**| if &#x60;uid&#x60; is given, search only for repos that the user owns | [optional] |
| **sort** | **String**| sort repos by attribute. Supported values are \&quot;alpha\&quot;, \&quot;created\&quot;, \&quot;updated\&quot;, \&quot;size\&quot;, \&quot;git_size\&quot;, \&quot;lfs_size\&quot;, \&quot;stars\&quot;, \&quot;forks\&quot; and \&quot;id\&quot;. Default is \&quot;alpha\&quot; | [optional] [enum: alpha, created, updated, size, git_size, lfs_size, id, stars, forks] |
| **order** | **String**| sort order, either \&quot;asc\&quot; (ascending) or \&quot;desc\&quot; (descending). Default is \&quot;asc\&quot;, ignored if \&quot;sort\&quot; is not specified. | [optional] [enum: asc, desc] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**SearchResults**](SearchResults.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SearchResults |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoSearchRunJobs"></a>
# **repoSearchRunJobs**
> List&lt;ActionRunJob&gt; repoSearchRunJobs(owner, repo, labels)

Search for repository&#39;s action jobs according filter conditions

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String labels = "labels_example"; // String | a comma separated list of run job labels to search for
    try {
      List<ActionRunJob> result = apiInstance.repoSearchRunJobs(owner, repo, labels);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoSearchRunJobs");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **labels** | **String**| a comma separated list of run job labels to search for | [optional] |

### Return type

[**List&lt;ActionRunJob&gt;**](ActionRunJob.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | RunJobList is a list of action run jobs |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="repoSetNote"></a>
# **repoSetNote**
> Note repoSetNote(owner, repo, sha, body)

Set a note corresponding to a single commit from a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String sha = "sha_example"; // String | a git ref or commit sha
    NoteOptions body = new NoteOptions(); // NoteOptions | 
    try {
      Note result = apiInstance.repoSetNote(owner, repo, sha, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoSetNote");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **sha** | **String**| a git ref or commit sha | |
| **body** | [**NoteOptions**](NoteOptions.md)|  | [optional] |

### Return type

[**Note**](Note.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Note |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoSigningKey"></a>
# **repoSigningKey**
> String repoSigningKey(owner, repo)

Get signing-key.gpg for given repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      String result = apiInstance.repoSigningKey(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoSigningKey");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

**String**

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GPG armored public key |  -  |

<a id="repoSubmitPullReview"></a>
# **repoSubmitPullReview**
> PullReview repoSubmitPullReview(owner, repo, index, id, body)

Submit a pending review to an pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    Long id = 56L; // Long | id of the review
    SubmitPullReviewOptions body = new SubmitPullReviewOptions(); // SubmitPullReviewOptions | 
    try {
      PullReview result = apiInstance.repoSubmitPullReview(owner, repo, index, id, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoSubmitPullReview");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **id** | **Long**| id of the review | |
| **body** | [**SubmitPullReviewOptions**](SubmitPullReviewOptions.md)|  | |

### Return type

[**PullReview**](PullReview.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullReview |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoSyncForkBranch"></a>
# **repoSyncForkBranch**
> repoSyncForkBranch(owner, repo, branch)

Syncs a fork branch with the base branch

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String branch = "branch_example"; // String | The branch
    try {
      apiInstance.repoSyncForkBranch(owner, repo, branch);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoSyncForkBranch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **branch** | **String**| The branch | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoSyncForkBranchInfo"></a>
# **repoSyncForkBranchInfo**
> SyncForkInfo repoSyncForkBranchInfo(owner, repo, branch)

Gets information about syncing a fork branch with the base branch

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String branch = "branch_example"; // String | The branch
    try {
      SyncForkInfo result = apiInstance.repoSyncForkBranchInfo(owner, repo, branch);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoSyncForkBranchInfo");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **branch** | **String**| The branch | |

### Return type

[**SyncForkInfo**](SyncForkInfo.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SyncForkInfo |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoSyncForkDefault"></a>
# **repoSyncForkDefault**
> repoSyncForkDefault(owner, repo)

Syncs the default branch of a fork with the base branch

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      apiInstance.repoSyncForkDefault(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoSyncForkDefault");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoSyncForkDefaultInfo"></a>
# **repoSyncForkDefaultInfo**
> SyncForkInfo repoSyncForkDefaultInfo(owner, repo)

Gets information about syncing the fork default branch with the base branch

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      SyncForkInfo result = apiInstance.repoSyncForkDefaultInfo(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoSyncForkDefaultInfo");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**SyncForkInfo**](SyncForkInfo.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SyncForkInfo |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoTestHook"></a>
# **repoTestHook**
> repoTestHook(owner, repo, id, ref)

Test a push webhook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long id = 56L; // Long | id of the hook to test
    String ref = "ref_example"; // String | The name of the commit/branch/tag, indicates which commit will be loaded to the webhook payload.
    try {
      apiInstance.repoTestHook(owner, repo, id, ref);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoTestHook");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **id** | **Long**| id of the hook to test | |
| **ref** | **String**| The name of the commit/branch/tag, indicates which commit will be loaded to the webhook payload. | [optional] |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoTrackedTimes"></a>
# **repoTrackedTimes**
> List&lt;TrackedTime&gt; repoTrackedTimes(owner, repo, user, since, before, page, limit)

List a repo&#39;s tracked times

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String user = "user_example"; // String | optional filter by user (available for issue managers)
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | Only show times updated after the given time. This is a timestamp in RFC 3339 format
    OffsetDateTime before = OffsetDateTime.now(); // OffsetDateTime | Only show times updated before the given time. This is a timestamp in RFC 3339 format
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<TrackedTime> result = apiInstance.repoTrackedTimes(owner, repo, user, since, before, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoTrackedTimes");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **user** | **String**| optional filter by user (available for issue managers) | [optional] |
| **since** | **OffsetDateTime**| Only show times updated after the given time. This is a timestamp in RFC 3339 format | [optional] |
| **before** | **OffsetDateTime**| Only show times updated before the given time. This is a timestamp in RFC 3339 format | [optional] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;TrackedTime&gt;**](TrackedTime.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | TrackedTimeList |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoTransfer"></a>
# **repoTransfer**
> Repository repoTransfer(owner, repo, body)

Transfer a repo ownership

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo to transfer
    String repo = "repo_example"; // String | name of the repo to transfer
    TransferRepoOption body = new TransferRepoOption(); // TransferRepoOption | Transfer Options
    try {
      Repository result = apiInstance.repoTransfer(owner, repo, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoTransfer");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo to transfer | |
| **repo** | **String**| name of the repo to transfer | |
| **body** | [**TransferRepoOption**](TransferRepoOption.md)| Transfer Options | |

### Return type

[**Repository**](Repository.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **202** | Repository |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoUnDismissPullReview"></a>
# **repoUnDismissPullReview**
> PullReview repoUnDismissPullReview(owner, repo, index, id)

Cancel to dismiss a review for a pull request

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request
    Long id = 56L; // Long | id of the review
    try {
      PullReview result = apiInstance.repoUnDismissPullReview(owner, repo, index, id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoUnDismissPullReview");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request | |
| **id** | **Long**| id of the review | |

### Return type

[**PullReview**](PullReview.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PullReview |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoUpdateAvatar"></a>
# **repoUpdateAvatar**
> repoUpdateAvatar(owner, repo, body)

Update a repository&#39;s avatar

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    UpdateRepoAvatarOption body = new UpdateRepoAvatarOption(); // UpdateRepoAvatarOption | 
    try {
      apiInstance.repoUpdateAvatar(owner, repo, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoUpdateAvatar");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**UpdateRepoAvatarOption**](UpdateRepoAvatarOption.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="repoUpdateBranch"></a>
# **repoUpdateBranch**
> repoUpdateBranch(owner, repo, branch, body)

Update a branch

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String branch = "branch_example"; // String | name of the branch
    UpdateBranchRepoOption body = new UpdateBranchRepoOption(); // UpdateBranchRepoOption | 
    try {
      apiInstance.repoUpdateBranch(owner, repo, branch, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoUpdateBranch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **branch** | **String**| name of the branch | |
| **body** | [**UpdateBranchRepoOption**](UpdateBranchRepoOption.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoUpdateFile"></a>
# **repoUpdateFile**
> FileResponse repoUpdateFile(owner, repo, filepath, body)

Update a file in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String filepath = "filepath_example"; // String | path of the file to update
    UpdateFileOptions body = new UpdateFileOptions(); // UpdateFileOptions | 
    try {
      FileResponse result = apiInstance.repoUpdateFile(owner, repo, filepath, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoUpdateFile");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **filepath** | **String**| path of the file to update | |
| **body** | [**UpdateFileOptions**](UpdateFileOptions.md)|  | |

### Return type

[**FileResponse**](FileResponse.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | FileResponse |  -  |
| **403** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | APIConflict is a conflict empty response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **422** | APIError is error format response |  -  |
| **423** | APIRepoArchivedError is an error that is raised when an archived repo should be modified |  -  |

<a id="repoUpdatePullRequest"></a>
# **repoUpdatePullRequest**
> repoUpdatePullRequest(owner, repo, index, style)

Merge PR&#39;s baseBranch into headBranch

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    Long index = 56L; // Long | index of the pull request to get
    String style = "merge"; // String | how to update pull request
    try {
      apiInstance.repoUpdatePullRequest(owner, repo, index, style);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoUpdatePullRequest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **index** | **Long**| index of the pull request to get | |
| **style** | **String**| how to update pull request | [optional] [enum: merge, rebase] |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | APIEmpty is an empty response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | APIError is error format response |  -  |
| **413** | QuotaExceeded |  * user_id -  <br>  * message -  <br>  * username -  <br>  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="repoUpdateTopics"></a>
# **repoUpdateTopics**
> repoUpdateTopics(owner, repo, body)

Replace list of topics for a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    RepoTopicOptions body = new RepoTopicOptions(); // RepoTopicOptions | 
    try {
      apiInstance.repoUpdateTopics(owner, repo, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoUpdateTopics");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **body** | [**RepoTopicOptions**](RepoTopicOptions.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIInvalidTopicsError is error format response to invalid topics |  -  |

<a id="repoValidateIssueConfig"></a>
# **repoValidateIssueConfig**
> IssueConfigValidation repoValidateIssueConfig(owner, repo)

Returns the validation information for a issue config

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      IssueConfigValidation result = apiInstance.repoValidateIssueConfig(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#repoValidateIssueConfig");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**IssueConfigValidation**](IssueConfigValidation.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | RepoIssueConfigValidation |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="topicSearch"></a>
# **topicSearch**
> TopicSearchResults topicSearch(q, page, limit)

Search for topics by keyword

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String q = "q_example"; // String | keyword to search for
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      TopicSearchResults result = apiInstance.topicSearch(q, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#topicSearch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **q** | **String**| keyword to search for | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**TopicSearchResults**](TopicSearchResults.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SearchResults of a successful search |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="updateRepoSecret"></a>
# **updateRepoSecret**
> updateRepoSecret(owner, repo, secretname, body)

Create or Update a secret value in a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repository
    String repo = "repo_example"; // String | name of the repository
    String secretname = "secretname_example"; // String | name of the secret
    CreateOrUpdateSecretOption body = new CreateOrUpdateSecretOption(); // CreateOrUpdateSecretOption | 
    try {
      apiInstance.updateRepoSecret(owner, repo, secretname, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#updateRepoSecret");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repository | |
| **repo** | **String**| name of the repository | |
| **secretname** | **String**| name of the secret | |
| **body** | [**CreateOrUpdateSecretOption**](CreateOrUpdateSecretOption.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | response when creating a secret |  -  |
| **204** | response when updating a secret |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="updateRepoVariable"></a>
# **updateRepoVariable**
> updateRepoVariable(owner, repo, variablename, body)

Update a repo-level variable

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | name of the owner
    String repo = "repo_example"; // String | name of the repository
    String variablename = "variablename_example"; // String | name of the variable
    UpdateVariableOption body = new UpdateVariableOption(); // UpdateVariableOption | 
    try {
      apiInstance.updateRepoVariable(owner, repo, variablename, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#updateRepoVariable");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| name of the owner | |
| **repo** | **String**| name of the repository | |
| **variablename** | **String**| name of the variable | |
| **body** | [**UpdateVariableOption**](UpdateVariableOption.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | response when updating a repo-level variable |  -  |
| **204** | response when updating a repo-level variable |  -  |
| **400** | APIError is error format response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentCheckSubscription"></a>
# **userCurrentCheckSubscription**
> WatchInfo userCurrentCheckSubscription(owner, repo)

Check if the current user is watching a repo

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      WatchInfo result = apiInstance.userCurrentCheckSubscription(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#userCurrentCheckSubscription");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**WatchInfo**](WatchInfo.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | WatchInfo |  -  |
| **404** | User is not watching this repo or repo do not exist |  -  |

<a id="userCurrentDeleteSubscription"></a>
# **userCurrentDeleteSubscription**
> userCurrentDeleteSubscription(owner, repo)

Unwatch a repo

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      apiInstance.userCurrentDeleteSubscription(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#userCurrentDeleteSubscription");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

null (empty response body)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentPutSubscription"></a>
# **userCurrentPutSubscription**
> WatchInfo userCurrentPutSubscription(owner, repo)

Watch a repo

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      WatchInfo result = apiInstance.userCurrentPutSubscription(owner, repo);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#userCurrentPutSubscription");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |

### Return type

[**WatchInfo**](WatchInfo.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | WatchInfo |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userTrackedTimes"></a>
# **userTrackedTimes**
> List&lt;TrackedTime&gt; userTrackedTimes(owner, repo, user)

List a user&#39;s tracked times in a repo

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.RepositoryApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    RepositoryApi apiInstance = new RepositoryApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    String user = "user_example"; // String | username of user
    try {
      List<TrackedTime> result = apiInstance.userTrackedTimes(owner, repo, user);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RepositoryApi#userTrackedTimes");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| owner of the repo | |
| **repo** | **String**| name of the repo | |
| **user** | **String**| username of user | |

### Return type

[**List&lt;TrackedTime&gt;**](TrackedTime.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | TrackedTimeList |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

