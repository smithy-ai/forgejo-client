

# PullRequest

PullRequest represents a pull request

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**additions** | **Long** |  |  [optional] |
|**allowMaintainerEdit** | **Boolean** |  |  [optional] |
|**assignee** | [**User**](User.md) |  |  [optional] |
|**assignees** | [**List&lt;User&gt;**](User.md) |  |  [optional] |
|**base** | [**PRBranchInfo**](PRBranchInfo.md) |  |  [optional] |
|**body** | **String** |  |  [optional] |
|**changedFiles** | **Long** |  |  [optional] |
|**closedAt** | **OffsetDateTime** |  |  [optional] |
|**comments** | **Long** |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**deletions** | **Long** |  |  [optional] |
|**diffUrl** | **String** |  |  [optional] |
|**draft** | **Boolean** |  |  [optional] |
|**dueDate** | **OffsetDateTime** |  |  [optional] |
|**flow** | **Long** |  |  [optional] |
|**head** | [**PRBranchInfo**](PRBranchInfo.md) |  |  [optional] |
|**htmlUrl** | **String** |  |  [optional] |
|**id** | **Long** |  |  [optional] |
|**isLocked** | **Boolean** |  |  [optional] |
|**labels** | [**List&lt;Label&gt;**](Label.md) |  |  [optional] |
|**mergeBase** | **String** |  |  [optional] |
|**mergeCommitSha** | **String** |  |  [optional] |
|**mergeable** | **Boolean** |  |  [optional] |
|**merged** | **Boolean** |  |  [optional] |
|**mergedAt** | **OffsetDateTime** |  |  [optional] |
|**mergedBy** | [**User**](User.md) |  |  [optional] |
|**milestone** | [**Milestone**](Milestone.md) |  |  [optional] |
|**number** | **Long** |  |  [optional] |
|**patchUrl** | **String** |  |  [optional] |
|**pinOrder** | **Long** |  |  [optional] |
|**requestedReviewers** | [**List&lt;User&gt;**](User.md) |  |  [optional] |
|**requestedReviewersTeams** | [**List&lt;Team&gt;**](Team.md) |  |  [optional] |
|**reviewComments** | **Long** | number of review comments made on the diff of a PR review (not including comments on commits or issues in a PR) |  [optional] |
|**state** | **String** | StateType issue state type |  [optional] |
|**title** | **String** |  |  [optional] |
|**updatedAt** | **OffsetDateTime** |  |  [optional] |
|**url** | **String** |  |  [optional] |
|**user** | [**User**](User.md) |  |  [optional] |



