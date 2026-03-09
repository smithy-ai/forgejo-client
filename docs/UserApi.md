# UserApi

All URIs are relative to */api/v1*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCurrentUserRepo**](UserApi.md#createCurrentUserRepo) | **POST** /user/repos | Create a repository |
| [**createUserVariable**](UserApi.md#createUserVariable) | **POST** /user/actions/variables/{variablename} | Create a user-level variable |
| [**deleteUserSecret**](UserApi.md#deleteUserSecret) | **DELETE** /user/actions/secrets/{secretname} | Delete a secret in a user scope |
| [**deleteUserVariable**](UserApi.md#deleteUserVariable) | **DELETE** /user/actions/variables/{variablename} | Delete a user-level variable which is created by current doer |
| [**getUserSettings**](UserApi.md#getUserSettings) | **GET** /user/settings | Get current user&#39;s account settings |
| [**getUserVariable**](UserApi.md#getUserVariable) | **GET** /user/actions/variables/{variablename} | Get a user-level variable which is created by current doer |
| [**getUserVariablesList**](UserApi.md#getUserVariablesList) | **GET** /user/actions/variables | Get the user-level list of variables which is created by current doer |
| [**getVerificationToken**](UserApi.md#getVerificationToken) | **GET** /user/gpg_key_token | Get a Token to verify |
| [**updateUserSecret**](UserApi.md#updateUserSecret) | **PUT** /user/actions/secrets/{secretname} | Create or Update a secret value in a user scope |
| [**updateUserSettings**](UserApi.md#updateUserSettings) | **PATCH** /user/settings | Update settings in current user&#39;s account |
| [**updateUserVariable**](UserApi.md#updateUserVariable) | **PUT** /user/actions/variables/{variablename} | Update a user-level variable which is created by current doer |
| [**userAddEmail**](UserApi.md#userAddEmail) | **POST** /user/emails | Add an email addresses to the current user&#39;s account |
| [**userBlockUser**](UserApi.md#userBlockUser) | **PUT** /user/block/{username} | Blocks a user from the doer |
| [**userCheckFollowing**](UserApi.md#userCheckFollowing) | **GET** /users/{username}/following/{target} | Check if one user is following another user |
| [**userCheckQuota**](UserApi.md#userCheckQuota) | **GET** /user/quota/check | Check if the authenticated user is over quota for a given subject |
| [**userCreateHook**](UserApi.md#userCreateHook) | **POST** /user/hooks | Create a hook |
| [**userCreateOAuth2Application**](UserApi.md#userCreateOAuth2Application) | **POST** /user/applications/oauth2 | Creates a new OAuth2 application |
| [**userCreateToken**](UserApi.md#userCreateToken) | **POST** /users/{username}/tokens | Generate an access token for the specified user |
| [**userCurrentCheckFollowing**](UserApi.md#userCurrentCheckFollowing) | **GET** /user/following/{username} | Check whether a user is followed by the authenticated user |
| [**userCurrentCheckStarring**](UserApi.md#userCurrentCheckStarring) | **GET** /user/starred/{owner}/{repo} | Whether the authenticated is starring the repo |
| [**userCurrentDeleteFollow**](UserApi.md#userCurrentDeleteFollow) | **DELETE** /user/following/{username} | Unfollow a user |
| [**userCurrentDeleteGPGKey**](UserApi.md#userCurrentDeleteGPGKey) | **DELETE** /user/gpg_keys/{id} | Remove a GPG public key from current user&#39;s account |
| [**userCurrentDeleteKey**](UserApi.md#userCurrentDeleteKey) | **DELETE** /user/keys/{id} | Delete a public key |
| [**userCurrentDeleteStar**](UserApi.md#userCurrentDeleteStar) | **DELETE** /user/starred/{owner}/{repo} | Unstar the given repo |
| [**userCurrentGetGPGKey**](UserApi.md#userCurrentGetGPGKey) | **GET** /user/gpg_keys/{id} | Get a GPG key |
| [**userCurrentGetKey**](UserApi.md#userCurrentGetKey) | **GET** /user/keys/{id} | Get a public key |
| [**userCurrentListFollowers**](UserApi.md#userCurrentListFollowers) | **GET** /user/followers | List the authenticated user&#39;s followers |
| [**userCurrentListFollowing**](UserApi.md#userCurrentListFollowing) | **GET** /user/following | List the users that the authenticated user is following |
| [**userCurrentListGPGKeys**](UserApi.md#userCurrentListGPGKeys) | **GET** /user/gpg_keys | List the authenticated user&#39;s GPG keys |
| [**userCurrentListKeys**](UserApi.md#userCurrentListKeys) | **GET** /user/keys | List the authenticated user&#39;s public keys |
| [**userCurrentListRepos**](UserApi.md#userCurrentListRepos) | **GET** /user/repos | List the repos that the authenticated user owns |
| [**userCurrentListStarred**](UserApi.md#userCurrentListStarred) | **GET** /user/starred | The repos that the authenticated user has starred |
| [**userCurrentListSubscriptions**](UserApi.md#userCurrentListSubscriptions) | **GET** /user/subscriptions | List repositories watched by the authenticated user |
| [**userCurrentPostGPGKey**](UserApi.md#userCurrentPostGPGKey) | **POST** /user/gpg_keys | Add a GPG public key to current user&#39;s account |
| [**userCurrentPostKey**](UserApi.md#userCurrentPostKey) | **POST** /user/keys | Create a public key |
| [**userCurrentPutFollow**](UserApi.md#userCurrentPutFollow) | **PUT** /user/following/{username} | Follow a user |
| [**userCurrentPutStar**](UserApi.md#userCurrentPutStar) | **PUT** /user/starred/{owner}/{repo} | Star the given repo |
| [**userCurrentTrackedTimes**](UserApi.md#userCurrentTrackedTimes) | **GET** /user/times | List the current user&#39;s tracked times |
| [**userDeleteAccessToken**](UserApi.md#userDeleteAccessToken) | **DELETE** /users/{username}/tokens/{token} | Delete an access token from the specified user&#39;s account |
| [**userDeleteAvatar**](UserApi.md#userDeleteAvatar) | **DELETE** /user/avatar | Delete avatar of the current user. It will be replaced by a default one |
| [**userDeleteEmail**](UserApi.md#userDeleteEmail) | **DELETE** /user/emails | Delete email addresses from the current user&#39;s account |
| [**userDeleteHook**](UserApi.md#userDeleteHook) | **DELETE** /user/hooks/{id} | Delete a hook |
| [**userDeleteOAuth2Application**](UserApi.md#userDeleteOAuth2Application) | **DELETE** /user/applications/oauth2/{id} | Delete an OAuth2 application |
| [**userEditHook**](UserApi.md#userEditHook) | **PATCH** /user/hooks/{id} | Update a hook |
| [**userGet**](UserApi.md#userGet) | **GET** /users/{username} | Get a user |
| [**userGetCurrent**](UserApi.md#userGetCurrent) | **GET** /user | Get the authenticated user |
| [**userGetHeatmapData**](UserApi.md#userGetHeatmapData) | **GET** /users/{username}/heatmap | Get a user&#39;s heatmap |
| [**userGetHook**](UserApi.md#userGetHook) | **GET** /user/hooks/{id} | Get a hook |
| [**userGetOAuth2Application**](UserApi.md#userGetOAuth2Application) | **GET** /user/applications/oauth2/{id} | Get an OAuth2 application |
| [**userGetOAuth2Applications**](UserApi.md#userGetOAuth2Applications) | **GET** /user/applications/oauth2 | List the authenticated user&#39;s oauth2 applications |
| [**userGetQuota**](UserApi.md#userGetQuota) | **GET** /user/quota | Get quota information for the authenticated user |
| [**userGetRunnerRegistrationToken**](UserApi.md#userGetRunnerRegistrationToken) | **GET** /user/actions/runners/registration-token | Get an user&#39;s actions runner registration token |
| [**userGetStopWatches**](UserApi.md#userGetStopWatches) | **GET** /user/stopwatches | Get list of all existing stopwatches |
| [**userGetTokens**](UserApi.md#userGetTokens) | **GET** /users/{username}/tokens | List the specified user&#39;s access tokens |
| [**userListActivityFeeds**](UserApi.md#userListActivityFeeds) | **GET** /users/{username}/activities/feeds | List a user&#39;s activity feeds |
| [**userListBlockedUsers**](UserApi.md#userListBlockedUsers) | **GET** /user/list_blocked | List the authenticated user&#39;s blocked users |
| [**userListEmails**](UserApi.md#userListEmails) | **GET** /user/emails | List all email addresses of the current user |
| [**userListFollowers**](UserApi.md#userListFollowers) | **GET** /users/{username}/followers | List the given user&#39;s followers |
| [**userListFollowing**](UserApi.md#userListFollowing) | **GET** /users/{username}/following | List the users that the given user is following |
| [**userListGPGKeys**](UserApi.md#userListGPGKeys) | **GET** /users/{username}/gpg_keys | List the given user&#39;s GPG keys |
| [**userListHooks**](UserApi.md#userListHooks) | **GET** /user/hooks | List the authenticated user&#39;s webhooks |
| [**userListKeys**](UserApi.md#userListKeys) | **GET** /users/{username}/keys | List the given user&#39;s public keys |
| [**userListQuotaArtifacts**](UserApi.md#userListQuotaArtifacts) | **GET** /user/quota/artifacts | List the artifacts affecting the authenticated user&#39;s quota |
| [**userListQuotaAttachments**](UserApi.md#userListQuotaAttachments) | **GET** /user/quota/attachments | List the attachments affecting the authenticated user&#39;s quota |
| [**userListQuotaPackages**](UserApi.md#userListQuotaPackages) | **GET** /user/quota/packages | List the packages affecting the authenticated user&#39;s quota |
| [**userListRepos**](UserApi.md#userListRepos) | **GET** /users/{username}/repos | List the repos owned by the given user |
| [**userListStarred**](UserApi.md#userListStarred) | **GET** /users/{username}/starred | The repos that the given user has starred |
| [**userListSubscriptions**](UserApi.md#userListSubscriptions) | **GET** /users/{username}/subscriptions | List the repositories watched by a user |
| [**userListTeams**](UserApi.md#userListTeams) | **GET** /user/teams | List all the teams a user belongs to |
| [**userSearch**](UserApi.md#userSearch) | **GET** /users/search | Search for users |
| [**userSearchRunJobs**](UserApi.md#userSearchRunJobs) | **GET** /user/actions/runners/jobs | Search for user&#39;s action jobs according filter conditions |
| [**userUnblockUser**](UserApi.md#userUnblockUser) | **PUT** /user/unblock/{username} | Unblocks a user from the doer |
| [**userUpdateAvatar**](UserApi.md#userUpdateAvatar) | **POST** /user/avatar | Update avatar of the current user |
| [**userUpdateOAuth2Application**](UserApi.md#userUpdateOAuth2Application) | **PATCH** /user/applications/oauth2/{id} | Update an OAuth2 application, this includes regenerating the client secret |
| [**userVerifyGPGKey**](UserApi.md#userVerifyGPGKey) | **POST** /user/gpg_key_verify | Verify a GPG key |


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
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    CreateRepoOption body = new CreateRepoOption(); // CreateRepoOption | 
    try {
      Repository result = apiInstance.createCurrentUserRepo(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#createCurrentUserRepo");
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

<a id="createUserVariable"></a>
# **createUserVariable**
> createUserVariable(variablename, body)

Create a user-level variable

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String variablename = "variablename_example"; // String | name of the variable
    CreateVariableOption body = new CreateVariableOption(); // CreateVariableOption | 
    try {
      apiInstance.createUserVariable(variablename, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#createUserVariable");
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
| **variablename** | **String**| name of the variable | |
| **body** | [**CreateVariableOption**](CreateVariableOption.md)|  | [optional] |

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
| **201** | response when creating a variable |  -  |
| **204** | response when creating a variable |  -  |
| **400** | APIError is error format response |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="deleteUserSecret"></a>
# **deleteUserSecret**
> deleteUserSecret(secretname)

Delete a secret in a user scope

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String secretname = "secretname_example"; // String | name of the secret
    try {
      apiInstance.deleteUserSecret(secretname);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#deleteUserSecret");
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
| **204** | delete one secret of the user |  -  |
| **400** | APIError is error format response |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="deleteUserVariable"></a>
# **deleteUserVariable**
> deleteUserVariable(variablename)

Delete a user-level variable which is created by current doer

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String variablename = "variablename_example"; // String | name of the variable
    try {
      apiInstance.deleteUserVariable(variablename);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#deleteUserVariable");
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
| **201** | response when deleting a variable |  -  |
| **204** | response when deleting a variable |  -  |
| **400** | APIError is error format response |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="getUserSettings"></a>
# **getUserSettings**
> UserSettings getUserSettings()

Get current user&#39;s account settings

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    try {
      UserSettings result = apiInstance.getUserSettings();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#getUserSettings");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserSettings**](UserSettings.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | UserSettings |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="getUserVariable"></a>
# **getUserVariable**
> ActionVariable getUserVariable(variablename)

Get a user-level variable which is created by current doer

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String variablename = "variablename_example"; // String | name of the variable
    try {
      ActionVariable result = apiInstance.getUserVariable(variablename);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#getUserVariable");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="getUserVariablesList"></a>
# **getUserVariablesList**
> List&lt;ActionVariable&gt; getUserVariablesList(page, limit)

Get the user-level list of variables which is created by current doer

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<ActionVariable> result = apiInstance.getUserVariablesList(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#getUserVariablesList");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="getVerificationToken"></a>
# **getVerificationToken**
> String getVerificationToken()

Get a Token to verify

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    try {
      String result = apiInstance.getVerificationToken();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#getVerificationToken");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="updateUserSecret"></a>
# **updateUserSecret**
> updateUserSecret(secretname, body)

Create or Update a secret value in a user scope

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String secretname = "secretname_example"; // String | name of the secret
    CreateOrUpdateSecretOption body = new CreateOrUpdateSecretOption(); // CreateOrUpdateSecretOption | 
    try {
      apiInstance.updateUserSecret(secretname, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#updateUserSecret");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="updateUserSettings"></a>
# **updateUserSettings**
> UserSettings updateUserSettings(body)

Update settings in current user&#39;s account

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    UserSettingsOptions body = new UserSettingsOptions(); // UserSettingsOptions | 
    try {
      UserSettings result = apiInstance.updateUserSettings(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#updateUserSettings");
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
| **body** | [**UserSettingsOptions**](UserSettingsOptions.md)|  | [optional] |

### Return type

[**UserSettings**](UserSettings.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | UserSettings |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="updateUserVariable"></a>
# **updateUserVariable**
> updateUserVariable(variablename, body)

Update a user-level variable which is created by current doer

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String variablename = "variablename_example"; // String | name of the variable
    UpdateVariableOption body = new UpdateVariableOption(); // UpdateVariableOption | 
    try {
      apiInstance.updateUserVariable(variablename, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#updateUserVariable");
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
| **variablename** | **String**| name of the variable | |
| **body** | [**UpdateVariableOption**](UpdateVariableOption.md)|  | [optional] |

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
| **201** | response when updating a variable |  -  |
| **204** | response when updating a variable |  -  |
| **400** | APIError is error format response |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userAddEmail"></a>
# **userAddEmail**
> List&lt;Email&gt; userAddEmail(body)

Add an email addresses to the current user&#39;s account

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    CreateEmailOption body = new CreateEmailOption(); // CreateEmailOption | 
    try {
      List<Email> result = apiInstance.userAddEmail(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userAddEmail");
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
| **body** | [**CreateEmailOption**](CreateEmailOption.md)|  | [optional] |

### Return type

[**List&lt;Email&gt;**](Email.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | EmailList |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="userBlockUser"></a>
# **userBlockUser**
> userBlockUser(username)

Blocks a user from the doer

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of the user
    try {
      apiInstance.userBlockUser(username);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userBlockUser");
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
| **username** | **String**| username of the user | |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="userCheckFollowing"></a>
# **userCheckFollowing**
> userCheckFollowing(username, target)

Check if one user is following another user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of following user
    String target = "target_example"; // String | username of followed user
    try {
      apiInstance.userCheckFollowing(username, target);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCheckFollowing");
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
| **username** | **String**| username of following user | |
| **target** | **String**| username of followed user | |

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

<a id="userCheckQuota"></a>
# **userCheckQuota**
> Boolean userCheckQuota(subject)

Check if the authenticated user is over quota for a given subject

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String subject = "subject_example"; // String | subject of the quota
    try {
      Boolean result = apiInstance.userCheckQuota(subject);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCheckQuota");
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
| **subject** | **String**| subject of the quota | |

### Return type

**Boolean**

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Returns true if the action is accepted. |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="userCreateHook"></a>
# **userCreateHook**
> Hook userCreateHook(body)

Create a hook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    CreateHookOption body = new CreateHookOption(); // CreateHookOption | 
    try {
      Hook result = apiInstance.userCreateHook(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCreateHook");
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
| **body** | [**CreateHookOption**](CreateHookOption.md)|  | |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userCreateOAuth2Application"></a>
# **userCreateOAuth2Application**
> OAuth2Application userCreateOAuth2Application(body)

Creates a new OAuth2 application

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    CreateOAuth2ApplicationOptions body = new CreateOAuth2ApplicationOptions(); // CreateOAuth2ApplicationOptions | 
    try {
      OAuth2Application result = apiInstance.userCreateOAuth2Application(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCreateOAuth2Application");
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
| **body** | [**CreateOAuth2ApplicationOptions**](CreateOAuth2ApplicationOptions.md)|  | |

### Return type

[**OAuth2Application**](OAuth2Application.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | OAuth2Application |  -  |
| **400** | APIError is error format response |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userCreateToken"></a>
# **userCreateToken**
> AccessToken userCreateToken(username, body)

Generate an access token for the specified user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user
    CreateAccessTokenOption body = new CreateAccessTokenOption(); // CreateAccessTokenOption | 
    try {
      AccessToken result = apiInstance.userCreateToken(username, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCreateToken");
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
| **username** | **String**| username of user | |
| **body** | [**CreateAccessTokenOption**](CreateAccessTokenOption.md)|  | [optional] |

### Return type

[**AccessToken**](AccessToken.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | AccessToken represents an API access token. |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentCheckFollowing"></a>
# **userCurrentCheckFollowing**
> userCurrentCheckFollowing(username)

Check whether a user is followed by the authenticated user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of followed user
    try {
      apiInstance.userCurrentCheckFollowing(username);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentCheckFollowing");
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
| **username** | **String**| username of followed user | |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentCheckStarring"></a>
# **userCurrentCheckStarring**
> userCurrentCheckStarring(owner, repo)

Whether the authenticated is starring the repo

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      apiInstance.userCurrentCheckStarring(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentCheckStarring");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentDeleteFollow"></a>
# **userCurrentDeleteFollow**
> userCurrentDeleteFollow(username)

Unfollow a user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user to unfollow
    try {
      apiInstance.userCurrentDeleteFollow(username);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentDeleteFollow");
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
| **username** | **String**| username of user to unfollow | |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentDeleteGPGKey"></a>
# **userCurrentDeleteGPGKey**
> userCurrentDeleteGPGKey(id)

Remove a GPG public key from current user&#39;s account

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Long id = 56L; // Long | id of key to delete
    try {
      apiInstance.userCurrentDeleteGPGKey(id);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentDeleteGPGKey");
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
| **id** | **Long**| id of key to delete | |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentDeleteKey"></a>
# **userCurrentDeleteKey**
> userCurrentDeleteKey(id)

Delete a public key

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Long id = 56L; // Long | id of key to delete
    try {
      apiInstance.userCurrentDeleteKey(id);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentDeleteKey");
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
| **id** | **Long**| id of key to delete | |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentDeleteStar"></a>
# **userCurrentDeleteStar**
> userCurrentDeleteStar(owner, repo)

Unstar the given repo

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo to unstar
    String repo = "repo_example"; // String | name of the repo to unstar
    try {
      apiInstance.userCurrentDeleteStar(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentDeleteStar");
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
| **owner** | **String**| owner of the repo to unstar | |
| **repo** | **String**| name of the repo to unstar | |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentGetGPGKey"></a>
# **userCurrentGetGPGKey**
> GPGKey userCurrentGetGPGKey(id)

Get a GPG key

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Long id = 56L; // Long | id of key to get
    try {
      GPGKey result = apiInstance.userCurrentGetGPGKey(id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentGetGPGKey");
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
| **id** | **Long**| id of key to get | |

### Return type

[**GPGKey**](GPGKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GPGKey |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentGetKey"></a>
# **userCurrentGetKey**
> PublicKey userCurrentGetKey(id)

Get a public key

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Long id = 56L; // Long | id of key to get
    try {
      PublicKey result = apiInstance.userCurrentGetKey(id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentGetKey");
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
| **id** | **Long**| id of key to get | |

### Return type

[**PublicKey**](PublicKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PublicKey |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentListFollowers"></a>
# **userCurrentListFollowers**
> List&lt;User&gt; userCurrentListFollowers(page, limit)

List the authenticated user&#39;s followers

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<User> result = apiInstance.userCurrentListFollowers(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentListFollowers");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userCurrentListFollowing"></a>
# **userCurrentListFollowing**
> List&lt;User&gt; userCurrentListFollowing(page, limit)

List the users that the authenticated user is following

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<User> result = apiInstance.userCurrentListFollowing(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentListFollowing");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userCurrentListGPGKeys"></a>
# **userCurrentListGPGKeys**
> List&lt;GPGKey&gt; userCurrentListGPGKeys(page, limit)

List the authenticated user&#39;s GPG keys

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<GPGKey> result = apiInstance.userCurrentListGPGKeys(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentListGPGKeys");
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
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;GPGKey&gt;**](GPGKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GPGKeyList |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userCurrentListKeys"></a>
# **userCurrentListKeys**
> List&lt;PublicKey&gt; userCurrentListKeys(fingerprint, page, limit)

List the authenticated user&#39;s public keys

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String fingerprint = "fingerprint_example"; // String | fingerprint of the key
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<PublicKey> result = apiInstance.userCurrentListKeys(fingerprint, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentListKeys");
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
| **fingerprint** | **String**| fingerprint of the key | [optional] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;PublicKey&gt;**](PublicKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PublicKeyList |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userCurrentListRepos"></a>
# **userCurrentListRepos**
> List&lt;Repository&gt; userCurrentListRepos(page, limit, orderBy)

List the repos that the authenticated user owns

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    String orderBy = "name"; // String | order the repositories
    try {
      List<Repository> result = apiInstance.userCurrentListRepos(page, limit, orderBy);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentListRepos");
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
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |
| **orderBy** | **String**| order the repositories | [optional] [enum: name, id, newest, oldest, recentupdate, leastupdate, reversealphabetically, alphabetically, reversesize, size, reversegitsize, gitsize, reverselfssize, lfssize, moststars, feweststars, mostforks, fewestforks] |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="userCurrentListStarred"></a>
# **userCurrentListStarred**
> List&lt;Repository&gt; userCurrentListStarred(page, limit)

The repos that the authenticated user has starred

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Repository> result = apiInstance.userCurrentListStarred(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentListStarred");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userCurrentListSubscriptions"></a>
# **userCurrentListSubscriptions**
> List&lt;Repository&gt; userCurrentListSubscriptions(page, limit)

List repositories watched by the authenticated user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Repository> result = apiInstance.userCurrentListSubscriptions(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentListSubscriptions");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userCurrentPostGPGKey"></a>
# **userCurrentPostGPGKey**
> GPGKey userCurrentPostGPGKey(form)

Add a GPG public key to current user&#39;s account

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    CreateGPGKeyOption form = new CreateGPGKeyOption(); // CreateGPGKeyOption | 
    try {
      GPGKey result = apiInstance.userCurrentPostGPGKey(form);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentPostGPGKey");
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
| **form** | [**CreateGPGKeyOption**](CreateGPGKeyOption.md)|  | [optional] |

### Return type

[**GPGKey**](GPGKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | GPGKey |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="userCurrentPostKey"></a>
# **userCurrentPostKey**
> PublicKey userCurrentPostKey(body)

Create a public key

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    CreateKeyOption body = new CreateKeyOption(); // CreateKeyOption | 
    try {
      PublicKey result = apiInstance.userCurrentPostKey(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentPostKey");
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
| **body** | [**CreateKeyOption**](CreateKeyOption.md)|  | [optional] |

### Return type

[**PublicKey**](PublicKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | PublicKey |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="userCurrentPutFollow"></a>
# **userCurrentPutFollow**
> userCurrentPutFollow(username)

Follow a user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user to follow
    try {
      apiInstance.userCurrentPutFollow(username);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentPutFollow");
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
| **username** | **String**| username of user to follow | |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentPutStar"></a>
# **userCurrentPutStar**
> userCurrentPutStar(owner, repo)

Star the given repo

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo to star
    String repo = "repo_example"; // String | name of the repo to star
    try {
      apiInstance.userCurrentPutStar(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentPutStar");
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
| **owner** | **String**| owner of the repo to star | |
| **repo** | **String**| name of the repo to star | |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userCurrentTrackedTimes"></a>
# **userCurrentTrackedTimes**
> List&lt;TrackedTime&gt; userCurrentTrackedTimes(page, limit, since, before)

List the current user&#39;s tracked times

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | Only show times updated after the given time. This is a timestamp in RFC 3339 format
    OffsetDateTime before = OffsetDateTime.now(); // OffsetDateTime | Only show times updated before the given time. This is a timestamp in RFC 3339 format
    try {
      List<TrackedTime> result = apiInstance.userCurrentTrackedTimes(page, limit, since, before);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userCurrentTrackedTimes");
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
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |
| **since** | **OffsetDateTime**| Only show times updated after the given time. This is a timestamp in RFC 3339 format | [optional] |
| **before** | **OffsetDateTime**| Only show times updated before the given time. This is a timestamp in RFC 3339 format | [optional] |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userDeleteAccessToken"></a>
# **userDeleteAccessToken**
> userDeleteAccessToken(username, token)

Delete an access token from the specified user&#39;s account

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user
    String token = "token_example"; // String | token to be deleted, identified by ID and if not available by name
    try {
      apiInstance.userDeleteAccessToken(username, token);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userDeleteAccessToken");
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
| **username** | **String**| username of user | |
| **token** | **String**| token to be deleted, identified by ID and if not available by name | |

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
| **422** | APIError is error format response |  -  |

<a id="userDeleteAvatar"></a>
# **userDeleteAvatar**
> userDeleteAvatar()

Delete avatar of the current user. It will be replaced by a default one

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    try {
      apiInstance.userDeleteAvatar();
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userDeleteAvatar");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userDeleteEmail"></a>
# **userDeleteEmail**
> userDeleteEmail(body)

Delete email addresses from the current user&#39;s account

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    DeleteEmailOption body = new DeleteEmailOption(); // DeleteEmailOption | 
    try {
      apiInstance.userDeleteEmail(body);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userDeleteEmail");
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
| **body** | [**DeleteEmailOption**](DeleteEmailOption.md)|  | [optional] |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userDeleteHook"></a>
# **userDeleteHook**
> userDeleteHook(id)

Delete a hook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Long id = 56L; // Long | id of the hook to delete
    try {
      apiInstance.userDeleteHook(id);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userDeleteHook");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userDeleteOAuth2Application"></a>
# **userDeleteOAuth2Application**
> userDeleteOAuth2Application(id)

Delete an OAuth2 application

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Long id = 56L; // Long | token to be deleted
    try {
      apiInstance.userDeleteOAuth2Application(id);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userDeleteOAuth2Application");
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
| **id** | **Long**| token to be deleted | |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userEditHook"></a>
# **userEditHook**
> Hook userEditHook(id, body)

Update a hook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Long id = 56L; // Long | id of the hook to update
    EditHookOption body = new EditHookOption(); // EditHookOption | 
    try {
      Hook result = apiInstance.userEditHook(id, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userEditHook");
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
| **id** | **Long**| id of the hook to update | |
| **body** | [**EditHookOption**](EditHookOption.md)|  | [optional] |

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
| **200** | Hook |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userGet"></a>
# **userGet**
> User userGet(username)

Get a user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user to get
    try {
      User result = apiInstance.userGet(username);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userGet");
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
| **username** | **String**| username of user to get | |

### Return type

[**User**](User.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userGetCurrent"></a>
# **userGetCurrent**
> User userGetCurrent()

Get the authenticated user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    try {
      User result = apiInstance.userGetCurrent();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userGetCurrent");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**User**](User.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userGetHeatmapData"></a>
# **userGetHeatmapData**
> List&lt;UserHeatmapData&gt; userGetHeatmapData(username)

Get a user&#39;s heatmap

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user to get
    try {
      List<UserHeatmapData> result = apiInstance.userGetHeatmapData(username);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userGetHeatmapData");
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
| **username** | **String**| username of user to get | |

### Return type

[**List&lt;UserHeatmapData&gt;**](UserHeatmapData.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | UserHeatmapData |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userGetHook"></a>
# **userGetHook**
> Hook userGetHook(id)

Get a hook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Long id = 56L; // Long | id of the hook to get
    try {
      Hook result = apiInstance.userGetHook(id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userGetHook");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userGetOAuth2Application"></a>
# **userGetOAuth2Application**
> OAuth2Application userGetOAuth2Application(id)

Get an OAuth2 application

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Long id = 56L; // Long | Application ID to be found
    try {
      OAuth2Application result = apiInstance.userGetOAuth2Application(id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userGetOAuth2Application");
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
| **id** | **Long**| Application ID to be found | |

### Return type

[**OAuth2Application**](OAuth2Application.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OAuth2Application |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userGetOAuth2Applications"></a>
# **userGetOAuth2Applications**
> List&lt;OAuth2Application&gt; userGetOAuth2Applications(page, limit)

List the authenticated user&#39;s oauth2 applications

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<OAuth2Application> result = apiInstance.userGetOAuth2Applications(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userGetOAuth2Applications");
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
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;OAuth2Application&gt;**](OAuth2Application.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OAuth2ApplicationList represents a list of OAuth2 applications. |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userGetQuota"></a>
# **userGetQuota**
> QuotaInfo userGetQuota()

Get quota information for the authenticated user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    try {
      QuotaInfo result = apiInstance.userGetQuota();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userGetQuota");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**QuotaInfo**](QuotaInfo.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | QuotaInfo |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userGetRunnerRegistrationToken"></a>
# **userGetRunnerRegistrationToken**
> RegistrationToken userGetRunnerRegistrationToken()

Get an user&#39;s actions runner registration token

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    try {
      RegistrationToken result = apiInstance.userGetRunnerRegistrationToken();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userGetRunnerRegistrationToken");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userGetStopWatches"></a>
# **userGetStopWatches**
> List&lt;StopWatch&gt; userGetStopWatches(page, limit)

Get list of all existing stopwatches

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<StopWatch> result = apiInstance.userGetStopWatches(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userGetStopWatches");
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
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;StopWatch&gt;**](StopWatch.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | StopWatchList |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userGetTokens"></a>
# **userGetTokens**
> List&lt;AccessToken&gt; userGetTokens(username, page, limit)

List the specified user&#39;s access tokens

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<AccessToken> result = apiInstance.userGetTokens(username, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userGetTokens");
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
| **username** | **String**| username of user | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;AccessToken&gt;**](AccessToken.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | AccessTokenList represents a list of API access token. |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userListActivityFeeds"></a>
# **userListActivityFeeds**
> List&lt;Activity&gt; userListActivityFeeds(username, onlyPerformedBy, date, page, limit)

List a user&#39;s activity feeds

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user
    Boolean onlyPerformedBy = true; // Boolean | if true, only show actions performed by the requested user
    LocalDate date = LocalDate.now(); // LocalDate | the date of the activities to be found
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Activity> result = apiInstance.userListActivityFeeds(username, onlyPerformedBy, date, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListActivityFeeds");
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
| **username** | **String**| username of user | |
| **onlyPerformedBy** | **Boolean**| if true, only show actions performed by the requested user | [optional] |
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

<a id="userListBlockedUsers"></a>
# **userListBlockedUsers**
> List&lt;BlockedUser&gt; userListBlockedUsers(page, limit)

List the authenticated user&#39;s blocked users

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<BlockedUser> result = apiInstance.userListBlockedUsers(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListBlockedUsers");
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
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;BlockedUser&gt;**](BlockedUser.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | BlockedUserList |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userListEmails"></a>
# **userListEmails**
> List&lt;Email&gt; userListEmails()

List all email addresses of the current user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    try {
      List<Email> result = apiInstance.userListEmails();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListEmails");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List&lt;Email&gt;**](Email.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | EmailList |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userListFollowers"></a>
# **userListFollowers**
> List&lt;User&gt; userListFollowers(username, page, limit)

List the given user&#39;s followers

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<User> result = apiInstance.userListFollowers(username, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListFollowers");
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
| **username** | **String**| username of user | |
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

<a id="userListFollowing"></a>
# **userListFollowing**
> List&lt;User&gt; userListFollowing(username, page, limit)

List the users that the given user is following

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<User> result = apiInstance.userListFollowing(username, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListFollowing");
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
| **username** | **String**| username of user | |
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

<a id="userListGPGKeys"></a>
# **userListGPGKeys**
> List&lt;GPGKey&gt; userListGPGKeys(username, page, limit)

List the given user&#39;s GPG keys

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<GPGKey> result = apiInstance.userListGPGKeys(username, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListGPGKeys");
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
| **username** | **String**| username of user | |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;GPGKey&gt;**](GPGKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | GPGKeyList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userListHooks"></a>
# **userListHooks**
> List&lt;Hook&gt; userListHooks(page, limit)

List the authenticated user&#39;s webhooks

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Hook> result = apiInstance.userListHooks(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListHooks");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userListKeys"></a>
# **userListKeys**
> List&lt;PublicKey&gt; userListKeys(username, fingerprint, page, limit)

List the given user&#39;s public keys

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user
    String fingerprint = "fingerprint_example"; // String | fingerprint of the key
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<PublicKey> result = apiInstance.userListKeys(username, fingerprint, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListKeys");
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
| **username** | **String**| username of user | |
| **fingerprint** | **String**| fingerprint of the key | [optional] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;PublicKey&gt;**](PublicKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | PublicKeyList |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userListQuotaArtifacts"></a>
# **userListQuotaArtifacts**
> List&lt;QuotaUsedArtifact&gt; userListQuotaArtifacts(page, limit)

List the artifacts affecting the authenticated user&#39;s quota

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<QuotaUsedArtifact> result = apiInstance.userListQuotaArtifacts(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListQuotaArtifacts");
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
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;QuotaUsedArtifact&gt;**](QuotaUsedArtifact.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | QuotaUsedArtifactList |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userListQuotaAttachments"></a>
# **userListQuotaAttachments**
> List&lt;QuotaUsedAttachment&gt; userListQuotaAttachments(page, limit)

List the attachments affecting the authenticated user&#39;s quota

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<QuotaUsedAttachment> result = apiInstance.userListQuotaAttachments(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListQuotaAttachments");
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
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;QuotaUsedAttachment&gt;**](QuotaUsedAttachment.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | QuotaUsedAttachmentList |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userListQuotaPackages"></a>
# **userListQuotaPackages**
> List&lt;QuotaUsedPackage&gt; userListQuotaPackages(page, limit)

List the packages affecting the authenticated user&#39;s quota

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<QuotaUsedPackage> result = apiInstance.userListQuotaPackages(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListQuotaPackages");
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
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**List&lt;QuotaUsedPackage&gt;**](QuotaUsedPackage.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | QuotaUsedPackageList |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userListRepos"></a>
# **userListRepos**
> List&lt;Repository&gt; userListRepos(username, page, limit)

List the repos owned by the given user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Repository> result = apiInstance.userListRepos(username, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListRepos");
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
| **username** | **String**| username of user | |
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

<a id="userListStarred"></a>
# **userListStarred**
> List&lt;Repository&gt; userListStarred(username, page, limit)

The repos that the given user has starred

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of user
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Repository> result = apiInstance.userListStarred(username, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListStarred");
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
| **username** | **String**| username of user | |
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

<a id="userListSubscriptions"></a>
# **userListSubscriptions**
> List&lt;Repository&gt; userListSubscriptions(username, page, limit)

List the repositories watched by a user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of the user
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Repository> result = apiInstance.userListSubscriptions(username, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListSubscriptions");
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
| **username** | **String**| username of the user | |
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

<a id="userListTeams"></a>
# **userListTeams**
> List&lt;Team&gt; userListTeams(page, limit)

List all the teams a user belongs to

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Team> result = apiInstance.userListTeams(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userListTeams");
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
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userSearch"></a>
# **userSearch**
> UserSearchResults userSearch(q, uid, sort, page, limit)

Search for users

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String q = "q_example"; // String | keyword
    Long uid = 56L; // Long | ID of the user to search for
    String sort = "oldest"; // String | sort order of results
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      UserSearchResults result = apiInstance.userSearch(q, uid, sort, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userSearch");
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
| **uid** | **Long**| ID of the user to search for | [optional] |
| **sort** | **String**| sort order of results | [optional] [enum: oldest, newest, alphabetically, reversealphabetically, recentupdate, leastupdate] |
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

### Return type

[**UserSearchResults**](UserSearchResults.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SearchResults of a successful search |  -  |

<a id="userSearchRunJobs"></a>
# **userSearchRunJobs**
> List&lt;ActionRunJob&gt; userSearchRunJobs(labels)

Search for user&#39;s action jobs according filter conditions

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String labels = "labels_example"; // String | a comma separated list of run job labels to search for
    try {
      List<ActionRunJob> result = apiInstance.userSearchRunJobs(labels);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userSearchRunJobs");
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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userUnblockUser"></a>
# **userUnblockUser**
> userUnblockUser(username)

Unblocks a user from the doer

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    String username = "username_example"; // String | username of the user
    try {
      apiInstance.userUnblockUser(username);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userUnblockUser");
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
| **username** | **String**| username of the user | |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="userUpdateAvatar"></a>
# **userUpdateAvatar**
> userUpdateAvatar(body)

Update avatar of the current user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    UpdateUserAvatarOption body = new UpdateUserAvatarOption(); // UpdateUserAvatarOption | 
    try {
      apiInstance.userUpdateAvatar(body);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userUpdateAvatar");
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
| **body** | [**UpdateUserAvatarOption**](UpdateUserAvatarOption.md)|  | [optional] |

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
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="userUpdateOAuth2Application"></a>
# **userUpdateOAuth2Application**
> OAuth2Application userUpdateOAuth2Application(id, body)

Update an OAuth2 application, this includes regenerating the client secret

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    Long id = 56L; // Long | application to be updated
    CreateOAuth2ApplicationOptions body = new CreateOAuth2ApplicationOptions(); // CreateOAuth2ApplicationOptions | 
    try {
      OAuth2Application result = apiInstance.userUpdateOAuth2Application(id, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userUpdateOAuth2Application");
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
| **id** | **Long**| application to be updated | |
| **body** | [**CreateOAuth2ApplicationOptions**](CreateOAuth2ApplicationOptions.md)|  | |

### Return type

[**OAuth2Application**](OAuth2Application.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OAuth2Application |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="userVerifyGPGKey"></a>
# **userVerifyGPGKey**
> GPGKey userVerifyGPGKey(body)

Verify a GPG key

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.UserApi;

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

    UserApi apiInstance = new UserApi(defaultClient);
    VerifyGPGKeyOption body = new VerifyGPGKeyOption(); // VerifyGPGKeyOption | 
    try {
      GPGKey result = apiInstance.userVerifyGPGKey(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserApi#userVerifyGPGKey");
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
| **body** | [**VerifyGPGKeyOption**](VerifyGPGKeyOption.md)|  | [optional] |

### Return type

[**GPGKey**](GPGKey.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | GPGKey |  -  |
| **401** | APIUnauthorizedError is a unauthorized error response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

