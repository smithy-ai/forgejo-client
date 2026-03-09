

# ActionRun

ActionRun represents an action run

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**scheduleID** | **Long** | the cron id for the schedule trigger |  [optional] |
|**approvedBy** | **Long** | who approved this action run |  [optional] |
|**commitSha** | **String** | the commit sha the action run ran on |  [optional] |
|**created** | **OffsetDateTime** | when the action run was created |  [optional] |
|**duration** | **Long** | A Duration represents the elapsed time between two instants as an int64 nanosecond count. The representation limits the largest representable duration to approximately 290 years. |  [optional] |
|**event** | **String** | the webhook event that causes the workflow to run |  [optional] |
|**eventPayload** | **String** | the payload of the webhook event that causes the workflow to run |  [optional] |
|**htmlUrl** | **String** | the url of this action run |  [optional] |
|**id** | **Long** | the action run id |  [optional] |
|**indexInRepo** | **Long** | a unique number for each run of a repository |  [optional] |
|**isForkPullRequest** | **Boolean** | If this is triggered by a PR from a forked repository or an untrusted user, we need to check if it is approved and limit permissions when running the workflow. |  [optional] |
|**isRefDeleted** | **Boolean** | has the commit/tag/… the action run ran on been deleted |  [optional] |
|**needApproval** | **Boolean** | may need approval if it&#39;s a fork pull request |  [optional] |
|**prettyref** | **String** | the commit/tag/… the action run ran on |  [optional] |
|**repository** | [**Repository**](Repository.md) |  |  [optional] |
|**started** | **OffsetDateTime** | when the action run was started |  [optional] |
|**status** | **String** | the current status of this run |  [optional] |
|**stopped** | **OffsetDateTime** | when the action run was stopped |  [optional] |
|**title** | **String** | the action run&#39;s title |  [optional] |
|**triggerEvent** | **String** | the trigger event defined in the &#x60;on&#x60; configuration of the triggered workflow |  [optional] |
|**triggerUser** | [**User**](User.md) |  |  [optional] |
|**updated** | **OffsetDateTime** | when the action run was last updated |  [optional] |
|**workflowId** | **String** | the name of workflow file |  [optional] |



