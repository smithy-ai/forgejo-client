# AdminApi

All URIs are relative to */api/v1*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**adminAddRuleToQuotaGroup**](AdminApi.md#adminAddRuleToQuotaGroup) | **PUT** /admin/quota/groups/{quotagroup}/rules/{quotarule} | Adds a rule to a quota group |
| [**adminAddUserToQuotaGroup**](AdminApi.md#adminAddUserToQuotaGroup) | **PUT** /admin/quota/groups/{quotagroup}/users/{username} | Add a user to a quota group |
| [**adminAdoptRepository**](AdminApi.md#adminAdoptRepository) | **POST** /admin/unadopted/{owner}/{repo} | Adopt unadopted files as a repository |
| [**adminCreateHook**](AdminApi.md#adminCreateHook) | **POST** /admin/hooks | Create a hook |
| [**adminCreateOrg**](AdminApi.md#adminCreateOrg) | **POST** /admin/users/{username}/orgs | Create an organization |
| [**adminCreatePublicKey**](AdminApi.md#adminCreatePublicKey) | **POST** /admin/users/{username}/keys | Add an SSH public key to user&#39;s account |
| [**adminCreateQuotaGroup**](AdminApi.md#adminCreateQuotaGroup) | **POST** /admin/quota/groups | Create a new quota group |
| [**adminCreateQuotaRule**](AdminApi.md#adminCreateQuotaRule) | **POST** /admin/quota/rules | Create a new quota rule |
| [**adminCreateRepo**](AdminApi.md#adminCreateRepo) | **POST** /admin/users/{username}/repos | Create a repository on behalf of a user |
| [**adminCreateUser**](AdminApi.md#adminCreateUser) | **POST** /admin/users | Create a user account |
| [**adminCronList**](AdminApi.md#adminCronList) | **GET** /admin/cron | List cron tasks |
| [**adminCronRun**](AdminApi.md#adminCronRun) | **POST** /admin/cron/{task} | Run cron task |
| [**adminDeleteHook**](AdminApi.md#adminDeleteHook) | **DELETE** /admin/hooks/{id} | Delete a hook |
| [**adminDeleteQuotaGroup**](AdminApi.md#adminDeleteQuotaGroup) | **DELETE** /admin/quota/groups/{quotagroup} | Delete a quota group |
| [**adminDeleteQuotaRule**](AdminApi.md#adminDeleteQuotaRule) | **DELETE** /admin/quota/rules/{quotarule} | Deletes a quota rule |
| [**adminDeleteUnadoptedRepository**](AdminApi.md#adminDeleteUnadoptedRepository) | **DELETE** /admin/unadopted/{owner}/{repo} | Delete unadopted files |
| [**adminDeleteUser**](AdminApi.md#adminDeleteUser) | **DELETE** /admin/users/{username} | Delete user account |
| [**adminDeleteUserEmails**](AdminApi.md#adminDeleteUserEmails) | **DELETE** /admin/users/{username}/emails | Delete email addresses from a user&#39;s account |
| [**adminDeleteUserPublicKey**](AdminApi.md#adminDeleteUserPublicKey) | **DELETE** /admin/users/{username}/keys/{id} | Remove a public key from user&#39;s account |
| [**adminEditHook**](AdminApi.md#adminEditHook) | **PATCH** /admin/hooks/{id} | Update a hook |
| [**adminEditQuotaRule**](AdminApi.md#adminEditQuotaRule) | **PATCH** /admin/quota/rules/{quotarule} | Change an existing quota rule |
| [**adminEditUser**](AdminApi.md#adminEditUser) | **PATCH** /admin/users/{username} | Edit an existing user |
| [**adminGetAllEmails**](AdminApi.md#adminGetAllEmails) | **GET** /admin/emails | List all users&#39; email addresses |
| [**adminGetAllOrgs**](AdminApi.md#adminGetAllOrgs) | **GET** /admin/orgs | List all organizations |
| [**adminGetHook**](AdminApi.md#adminGetHook) | **GET** /admin/hooks/{id} | Get a hook |
| [**adminGetQuotaGroup**](AdminApi.md#adminGetQuotaGroup) | **GET** /admin/quota/groups/{quotagroup} | Get information about the quota group |
| [**adminGetQuotaRule**](AdminApi.md#adminGetQuotaRule) | **GET** /admin/quota/rules/{quotarule} | Get information about a quota rule |
| [**adminGetRunnerRegistrationToken**](AdminApi.md#adminGetRunnerRegistrationToken) | **GET** /admin/runners/registration-token | Get an global actions runner registration token |
| [**adminGetUserQuota**](AdminApi.md#adminGetUserQuota) | **GET** /admin/users/{username}/quota | Get the user&#39;s quota info |
| [**adminListHooks**](AdminApi.md#adminListHooks) | **GET** /admin/hooks | List global (system) webhooks |
| [**adminListQuotaGroups**](AdminApi.md#adminListQuotaGroups) | **GET** /admin/quota/groups | List the available quota groups |
| [**adminListQuotaRules**](AdminApi.md#adminListQuotaRules) | **GET** /admin/quota/rules | List the available quota rules |
| [**adminListUserEmails**](AdminApi.md#adminListUserEmails) | **GET** /admin/users/{username}/emails | List all email addresses for a user |
| [**adminListUsersInQuotaGroup**](AdminApi.md#adminListUsersInQuotaGroup) | **GET** /admin/quota/groups/{quotagroup}/users | List users in a quota group |
| [**adminRemoveRuleFromQuotaGroup**](AdminApi.md#adminRemoveRuleFromQuotaGroup) | **DELETE** /admin/quota/groups/{quotagroup}/rules/{quotarule} | Removes a rule from a quota group |
| [**adminRemoveUserFromQuotaGroup**](AdminApi.md#adminRemoveUserFromQuotaGroup) | **DELETE** /admin/quota/groups/{quotagroup}/users/{username} | Remove a user from a quota group |
| [**adminRenameUser**](AdminApi.md#adminRenameUser) | **POST** /admin/users/{username}/rename | Rename a user |
| [**adminSearchEmails**](AdminApi.md#adminSearchEmails) | **GET** /admin/emails/search | Search users&#39; email addresses |
| [**adminSearchRunJobs**](AdminApi.md#adminSearchRunJobs) | **GET** /admin/runners/jobs | Search action jobs according filter conditions |
| [**adminSearchUsers**](AdminApi.md#adminSearchUsers) | **GET** /admin/users | Search users according filter conditions |
| [**adminSetUserQuotaGroups**](AdminApi.md#adminSetUserQuotaGroups) | **POST** /admin/users/{username}/quota/groups | Set the user&#39;s quota groups to a given list. |
| [**adminUnadoptedList**](AdminApi.md#adminUnadoptedList) | **GET** /admin/unadopted | List unadopted repositories |


<a id="adminAddRuleToQuotaGroup"></a>
# **adminAddRuleToQuotaGroup**
> adminAddRuleToQuotaGroup(quotagroup, quotarule)

Adds a rule to a quota group

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String quotagroup = "quotagroup_example"; // String | quota group to add a rule to
    String quotarule = "quotarule_example"; // String | the name of the quota rule to add to the group
    try {
      apiInstance.adminAddRuleToQuotaGroup(quotagroup, quotarule);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminAddRuleToQuotaGroup");
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
| **quotagroup** | **String**| quota group to add a rule to | |
| **quotarule** | **String**| the name of the quota rule to add to the group | |

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
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | APIError is error format response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminAddUserToQuotaGroup"></a>
# **adminAddUserToQuotaGroup**
> adminAddUserToQuotaGroup(quotagroup, username)

Add a user to a quota group

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String quotagroup = "quotagroup_example"; // String | quota group to add the user to
    String username = "username_example"; // String | username of the user to add to the quota group
    try {
      apiInstance.adminAddUserToQuotaGroup(quotagroup, username);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminAddUserToQuotaGroup");
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
| **quotagroup** | **String**| quota group to add the user to | |
| **username** | **String**| username of the user to add to the quota group | |

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
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | APIError is error format response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminAdoptRepository"></a>
# **adminAdoptRepository**
> adminAdoptRepository(owner, repo)

Adopt unadopted files as a repository

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      apiInstance.adminAdoptRepository(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminAdoptRepository");
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

<a id="adminCreateHook"></a>
# **adminCreateHook**
> Hook adminCreateHook(body)

Create a hook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    CreateHookOption body = new CreateHookOption(); // CreateHookOption | 
    try {
      Hook result = apiInstance.adminCreateHook(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminCreateHook");
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

<a id="adminCreateOrg"></a>
# **adminCreateOrg**
> Organization adminCreateOrg(username, organization)

Create an organization

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String username = "username_example"; // String | username of the user that will own the created organization
    CreateOrgOption organization = new CreateOrgOption(); // CreateOrgOption | 
    try {
      Organization result = apiInstance.adminCreateOrg(username, organization);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminCreateOrg");
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
| **username** | **String**| username of the user that will own the created organization | |
| **organization** | [**CreateOrgOption**](CreateOrgOption.md)|  | |

### Return type

[**Organization**](Organization.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Organization |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminCreatePublicKey"></a>
# **adminCreatePublicKey**
> PublicKey adminCreatePublicKey(username, key)

Add an SSH public key to user&#39;s account

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String username = "username_example"; // String | username of the user
    CreateKeyOption key = new CreateKeyOption(); // CreateKeyOption | 
    try {
      PublicKey result = apiInstance.adminCreatePublicKey(username, key);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminCreatePublicKey");
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
| **key** | [**CreateKeyOption**](CreateKeyOption.md)|  | [optional] |

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
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminCreateQuotaGroup"></a>
# **adminCreateQuotaGroup**
> QuotaGroup adminCreateQuotaGroup(group)

Create a new quota group

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    CreateQuotaGroupOptions group = new CreateQuotaGroupOptions(); // CreateQuotaGroupOptions | Definition of the quota group
    try {
      QuotaGroup result = apiInstance.adminCreateQuotaGroup(group);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminCreateQuotaGroup");
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
| **group** | [**CreateQuotaGroupOptions**](CreateQuotaGroupOptions.md)| Definition of the quota group | |

### Return type

[**QuotaGroup**](QuotaGroup.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | QuotaGroup |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **409** | APIError is error format response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminCreateQuotaRule"></a>
# **adminCreateQuotaRule**
> QuotaRuleInfo adminCreateQuotaRule(rule)

Create a new quota rule

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    CreateQuotaRuleOptions rule = new CreateQuotaRuleOptions(); // CreateQuotaRuleOptions | Definition of the quota rule
    try {
      QuotaRuleInfo result = apiInstance.adminCreateQuotaRule(rule);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminCreateQuotaRule");
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
| **rule** | [**CreateQuotaRuleOptions**](CreateQuotaRuleOptions.md)| Definition of the quota rule | |

### Return type

[**QuotaRuleInfo**](QuotaRuleInfo.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | QuotaRuleInfo |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **409** | APIError is error format response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminCreateRepo"></a>
# **adminCreateRepo**
> Repository adminCreateRepo(username, repository)

Create a repository on behalf of a user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String username = "username_example"; // String | username of the user. This user will own the created repository
    CreateRepoOption repository = new CreateRepoOption(); // CreateRepoOption | 
    try {
      Repository result = apiInstance.adminCreateRepo(username, repository);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminCreateRepo");
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
| **username** | **String**| username of the user. This user will own the created repository | |
| **repository** | [**CreateRepoOption**](CreateRepoOption.md)|  | |

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
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **409** | APIError is error format response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminCreateUser"></a>
# **adminCreateUser**
> User adminCreateUser(body)

Create a user account

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    CreateUserOption body = new CreateUserOption(); // CreateUserOption | 
    try {
      User result = apiInstance.adminCreateUser(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminCreateUser");
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
| **body** | [**CreateUserOption**](CreateUserOption.md)|  | [optional] |

### Return type

[**User**](User.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | User |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminCronList"></a>
# **adminCronList**
> List&lt;Cron&gt; adminCronList(page, limit)

List cron tasks

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Cron> result = apiInstance.adminCronList(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminCronList");
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

[**List&lt;Cron&gt;**](Cron.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | CronList |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="adminCronRun"></a>
# **adminCronRun**
> adminCronRun(task)

Run cron task

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String task = "task_example"; // String | task to run
    try {
      apiInstance.adminCronRun(task);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminCronRun");
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
| **task** | **String**| task to run | |

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

<a id="adminDeleteHook"></a>
# **adminDeleteHook**
> adminDeleteHook(id)

Delete a hook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    Long id = 56L; // Long | id of the hook to delete
    try {
      apiInstance.adminDeleteHook(id);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminDeleteHook");
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
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | APIEmpty is an empty response |  -  |

<a id="adminDeleteQuotaGroup"></a>
# **adminDeleteQuotaGroup**
> adminDeleteQuotaGroup(quotagroup)

Delete a quota group

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String quotagroup = "quotagroup_example"; // String | quota group to delete
    try {
      apiInstance.adminDeleteQuotaGroup(quotagroup);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminDeleteQuotaGroup");
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
| **quotagroup** | **String**| quota group to delete | |

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
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="adminDeleteQuotaRule"></a>
# **adminDeleteQuotaRule**
> adminDeleteQuotaRule(quotarule)

Deletes a quota rule

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String quotarule = "quotarule_example"; // String | quota rule to delete
    try {
      apiInstance.adminDeleteQuotaRule(quotarule);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminDeleteQuotaRule");
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
| **quotarule** | **String**| quota rule to delete | |

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
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="adminDeleteUnadoptedRepository"></a>
# **adminDeleteUnadoptedRepository**
> adminDeleteUnadoptedRepository(owner, repo)

Delete unadopted files

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String owner = "owner_example"; // String | owner of the repo
    String repo = "repo_example"; // String | name of the repo
    try {
      apiInstance.adminDeleteUnadoptedRepository(owner, repo);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminDeleteUnadoptedRepository");
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

<a id="adminDeleteUser"></a>
# **adminDeleteUser**
> adminDeleteUser(username, purge)

Delete user account

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String username = "username_example"; // String | username of user to delete
    Boolean purge = true; // Boolean | purge the user from the system completely
    try {
      apiInstance.adminDeleteUser(username, purge);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminDeleteUser");
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
| **username** | **String**| username of user to delete | |
| **purge** | **Boolean**| purge the user from the system completely | [optional] |

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
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminDeleteUserEmails"></a>
# **adminDeleteUserEmails**
> adminDeleteUserEmails(username, body)

Delete email addresses from a user&#39;s account

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String username = "username_example"; // String | username of user to delete email addresses from
    DeleteEmailOption body = new DeleteEmailOption(); // DeleteEmailOption | 
    try {
      apiInstance.adminDeleteUserEmails(username, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminDeleteUserEmails");
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
| **username** | **String**| username of user to delete email addresses from | |
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
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminDeleteUserPublicKey"></a>
# **adminDeleteUserPublicKey**
> adminDeleteUserPublicKey(username, id)

Remove a public key from user&#39;s account

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String username = "username_example"; // String | username of user
    Long id = 56L; // Long | id of the key to delete
    try {
      apiInstance.adminDeleteUserPublicKey(username, id);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminDeleteUserPublicKey");
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
| **id** | **Long**| id of the key to delete | |

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

<a id="adminEditHook"></a>
# **adminEditHook**
> Hook adminEditHook(id, body)

Update a hook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    Long id = 56L; // Long | id of the hook to update
    EditHookOption body = new EditHookOption(); // EditHookOption | 
    try {
      Hook result = apiInstance.adminEditHook(id, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminEditHook");
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

<a id="adminEditQuotaRule"></a>
# **adminEditQuotaRule**
> QuotaRuleInfo adminEditQuotaRule(quotarule, rule)

Change an existing quota rule

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String quotarule = "quotarule_example"; // String | Quota rule to change
    EditQuotaRuleOptions rule = new EditQuotaRuleOptions(); // EditQuotaRuleOptions | 
    try {
      QuotaRuleInfo result = apiInstance.adminEditQuotaRule(quotarule, rule);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminEditQuotaRule");
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
| **quotarule** | **String**| Quota rule to change | |
| **rule** | [**EditQuotaRuleOptions**](EditQuotaRuleOptions.md)|  | |

### Return type

[**QuotaRuleInfo**](QuotaRuleInfo.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | QuotaRuleInfo |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminEditUser"></a>
# **adminEditUser**
> User adminEditUser(username, body)

Edit an existing user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String username = "username_example"; // String | username of user to edit
    EditUserOption body = new EditUserOption(); // EditUserOption | 
    try {
      User result = apiInstance.adminEditUser(username, body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminEditUser");
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
| **username** | **String**| username of user to edit | |
| **body** | [**EditUserOption**](EditUserOption.md)|  | [optional] |

### Return type

[**User**](User.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminGetAllEmails"></a>
# **adminGetAllEmails**
> List&lt;Email&gt; adminGetAllEmails(page, limit)

List all users&#39; email addresses

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Email> result = apiInstance.adminGetAllEmails(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminGetAllEmails");
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
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="adminGetAllOrgs"></a>
# **adminGetAllOrgs**
> List&lt;Organization&gt; adminGetAllOrgs(page, limit)

List all organizations

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Organization> result = apiInstance.adminGetAllOrgs(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminGetAllOrgs");
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

[**List&lt;Organization&gt;**](Organization.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OrganizationList |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="adminGetHook"></a>
# **adminGetHook**
> Hook adminGetHook(id)

Get a hook

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    Long id = 56L; // Long | id of the hook to get
    try {
      Hook result = apiInstance.adminGetHook(id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminGetHook");
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

<a id="adminGetQuotaGroup"></a>
# **adminGetQuotaGroup**
> QuotaGroup adminGetQuotaGroup(quotagroup)

Get information about the quota group

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String quotagroup = "quotagroup_example"; // String | quota group to query
    try {
      QuotaGroup result = apiInstance.adminGetQuotaGroup(quotagroup);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminGetQuotaGroup");
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
| **quotagroup** | **String**| quota group to query | |

### Return type

[**QuotaGroup**](QuotaGroup.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | QuotaGroup |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="adminGetQuotaRule"></a>
# **adminGetQuotaRule**
> QuotaRuleInfo adminGetQuotaRule(quotarule)

Get information about a quota rule

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String quotarule = "quotarule_example"; // String | quota rule to query
    try {
      QuotaRuleInfo result = apiInstance.adminGetQuotaRule(quotarule);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminGetQuotaRule");
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
| **quotarule** | **String**| quota rule to query | |

### Return type

[**QuotaRuleInfo**](QuotaRuleInfo.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | QuotaRuleInfo |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="adminGetRunnerRegistrationToken"></a>
# **adminGetRunnerRegistrationToken**
> RegistrationToken adminGetRunnerRegistrationToken()

Get an global actions runner registration token

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    try {
      RegistrationToken result = apiInstance.adminGetRunnerRegistrationToken();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminGetRunnerRegistrationToken");
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

<a id="adminGetUserQuota"></a>
# **adminGetUserQuota**
> QuotaInfo adminGetUserQuota(username)

Get the user&#39;s quota info

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String username = "username_example"; // String | username of user to query
    try {
      QuotaInfo result = apiInstance.adminGetUserQuota(username);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminGetUserQuota");
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
| **username** | **String**| username of user to query | |

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
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminListHooks"></a>
# **adminListHooks**
> List&lt;Hook&gt; adminListHooks(page, limit)

List global (system) webhooks

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Hook> result = apiInstance.adminListHooks(page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminListHooks");
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

<a id="adminListQuotaGroups"></a>
# **adminListQuotaGroups**
> List&lt;QuotaGroup&gt; adminListQuotaGroups()

List the available quota groups

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    try {
      List<QuotaGroup> result = apiInstance.adminListQuotaGroups();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminListQuotaGroups");
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

[**List&lt;QuotaGroup&gt;**](QuotaGroup.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | QuotaGroupList |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="adminListQuotaRules"></a>
# **adminListQuotaRules**
> List&lt;QuotaRuleInfo&gt; adminListQuotaRules()

List the available quota rules

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    try {
      List<QuotaRuleInfo> result = apiInstance.adminListQuotaRules();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminListQuotaRules");
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

[**List&lt;QuotaRuleInfo&gt;**](QuotaRuleInfo.md)

### Authorization

[TOTPHeader](../README.md#TOTPHeader), [AuthorizationHeaderToken](../README.md#AuthorizationHeaderToken), [SudoHeader](../README.md#SudoHeader), [BasicAuth](../README.md#BasicAuth), [AccessToken](../README.md#AccessToken), [SudoParam](../README.md#SudoParam), [Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | QuotaRuleInfoList |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="adminListUserEmails"></a>
# **adminListUserEmails**
> List&lt;Email&gt; adminListUserEmails(username)

List all email addresses for a user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String username = "username_example"; // String | username of user to get email addresses of
    try {
      List<Email> result = apiInstance.adminListUserEmails(username);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminListUserEmails");
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
| **username** | **String**| username of user to get email addresses of | |

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
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="adminListUsersInQuotaGroup"></a>
# **adminListUsersInQuotaGroup**
> List&lt;User&gt; adminListUsersInQuotaGroup(quotagroup)

List users in a quota group

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String quotagroup = "quotagroup_example"; // String | quota group to list members of
    try {
      List<User> result = apiInstance.adminListUsersInQuotaGroup(quotagroup);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminListUsersInQuotaGroup");
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
| **quotagroup** | **String**| quota group to list members of | |

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
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="adminRemoveRuleFromQuotaGroup"></a>
# **adminRemoveRuleFromQuotaGroup**
> adminRemoveRuleFromQuotaGroup(quotagroup, quotarule)

Removes a rule from a quota group

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String quotagroup = "quotagroup_example"; // String | quota group to remove a rule from
    String quotarule = "quotarule_example"; // String | the name of the quota rule to remove from the group
    try {
      apiInstance.adminRemoveRuleFromQuotaGroup(quotagroup, quotarule);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminRemoveRuleFromQuotaGroup");
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
| **quotagroup** | **String**| quota group to remove a rule from | |
| **quotarule** | **String**| the name of the quota rule to remove from the group | |

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
| **201** | APIEmpty is an empty response |  -  |
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="adminRemoveUserFromQuotaGroup"></a>
# **adminRemoveUserFromQuotaGroup**
> adminRemoveUserFromQuotaGroup(quotagroup, username)

Remove a user from a quota group

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String quotagroup = "quotagroup_example"; // String | quota group to remove a user from
    String username = "username_example"; // String | username of the user to remove from the quota group
    try {
      apiInstance.adminRemoveUserFromQuotaGroup(quotagroup, username);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminRemoveUserFromQuotaGroup");
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
| **quotagroup** | **String**| quota group to remove a user from | |
| **username** | **String**| username of the user to remove from the quota group | |

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
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |

<a id="adminRenameUser"></a>
# **adminRenameUser**
> adminRenameUser(username, body)

Rename a user

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String username = "username_example"; // String | existing username of user
    RenameUserOption body = new RenameUserOption(); // RenameUserOption | 
    try {
      apiInstance.adminRenameUser(username, body);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminRenameUser");
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
| **username** | **String**| existing username of user | |
| **body** | [**RenameUserOption**](RenameUserOption.md)|  | |

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
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminSearchEmails"></a>
# **adminSearchEmails**
> List&lt;Email&gt; adminSearchEmails(q, page, limit)

Search users&#39; email addresses

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String q = "q_example"; // String | keyword
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<Email> result = apiInstance.adminSearchEmails(q, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminSearchEmails");
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
| **page** | **Integer**| page number of results to return (1-based) | [optional] |
| **limit** | **Integer**| page size of results | [optional] |

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
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="adminSearchRunJobs"></a>
# **adminSearchRunJobs**
> List&lt;ActionRunJob&gt; adminSearchRunJobs(labels)

Search action jobs according filter conditions

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String labels = "labels_example"; // String | a comma separated list of run job labels to search for
    try {
      List<ActionRunJob> result = apiInstance.adminSearchRunJobs(labels);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminSearchRunJobs");
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
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="adminSearchUsers"></a>
# **adminSearchUsers**
> List&lt;User&gt; adminSearchUsers(sourceId, loginName, sort, page, limit)

Search users according filter conditions

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    Long sourceId = 56L; // Long | ID of the user's login source to search for
    String loginName = "loginName_example"; // String | user's login name to search for
    String sort = "oldest"; // String | sort order of results
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    try {
      List<User> result = apiInstance.adminSearchUsers(sourceId, loginName, sort, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminSearchUsers");
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
| **sourceId** | **Long**| ID of the user&#39;s login source to search for | [optional] |
| **loginName** | **String**| user&#39;s login name to search for | [optional] |
| **sort** | **String**| sort order of results | [optional] [enum: oldest, newest, alphabetically, reversealphabetically, recentupdate, leastupdate] |
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
| **403** | APIForbiddenError is a forbidden error response |  -  |

<a id="adminSetUserQuotaGroups"></a>
# **adminSetUserQuotaGroups**
> adminSetUserQuotaGroups(username, groups)

Set the user&#39;s quota groups to a given list.

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    String username = "username_example"; // String | username of the user to modify the quota groups from
    SetUserQuotaGroupsOptions groups = new SetUserQuotaGroupsOptions(); // SetUserQuotaGroupsOptions | list of groups that the user should be a member of
    try {
      apiInstance.adminSetUserQuotaGroups(username, groups);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminSetUserQuotaGroups");
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
| **username** | **String**| username of the user to modify the quota groups from | |
| **groups** | [**SetUserQuotaGroupsOptions**](SetUserQuotaGroupsOptions.md)| list of groups that the user should be a member of | |

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
| **400** | APIError is error format response |  -  |
| **403** | APIForbiddenError is a forbidden error response |  -  |
| **404** | APINotFound is a not found error response |  -  |
| **422** | APIValidationError is error format response related to input validation |  -  |

<a id="adminUnadoptedList"></a>
# **adminUnadoptedList**
> List&lt;String&gt; adminUnadoptedList(page, limit, pattern)

List unadopted repositories

### Example
```java
// Import classes:
import dev.smithyai.forgejoclient.ApiClient;
import dev.smithyai.forgejoclient.ApiException;
import dev.smithyai.forgejoclient.Configuration;
import dev.smithyai.forgejoclient.auth.*;
import dev.smithyai.forgejoclient.models.*;
import dev.smithyai.forgejoclient.api.AdminApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("/api/v1");
    
    // Configure API key authorization: TOTPHeader
    ApiKeyAuth TOTPHeader = (ApiKeyAuth) defaultClient.getAuthentication("TOTPHeader");
    TOTPHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //TOTPHeader.setApiKeyPrefix("Token");

    // Configure API key authorization: AuthorizationHeaderToken
    ApiKeyAuth AuthorizationHeaderToken = (ApiKeyAuth) defaultClient.getAuthentication("AuthorizationHeaderToken");
    AuthorizationHeaderToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AuthorizationHeaderToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoHeader
    ApiKeyAuth SudoHeader = (ApiKeyAuth) defaultClient.getAuthentication("SudoHeader");
    SudoHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoHeader.setApiKeyPrefix("Token");

    // Configure HTTP basic authorization: BasicAuth
    HttpBasicAuth BasicAuth = (HttpBasicAuth) defaultClient.getAuthentication("BasicAuth");
    BasicAuth.setUsername("YOUR USERNAME");
    BasicAuth.setPassword("YOUR PASSWORD");

    // Configure API key authorization: AccessToken
    ApiKeyAuth AccessToken = (ApiKeyAuth) defaultClient.getAuthentication("AccessToken");
    AccessToken.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //AccessToken.setApiKeyPrefix("Token");

    // Configure API key authorization: SudoParam
    ApiKeyAuth SudoParam = (ApiKeyAuth) defaultClient.getAuthentication("SudoParam");
    SudoParam.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //SudoParam.setApiKeyPrefix("Token");

    // Configure API key authorization: Token
    ApiKeyAuth Token = (ApiKeyAuth) defaultClient.getAuthentication("Token");
    Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Token.setApiKeyPrefix("Token");

    AdminApi apiInstance = new AdminApi(defaultClient);
    Integer page = 56; // Integer | page number of results to return (1-based)
    Integer limit = 56; // Integer | page size of results
    String pattern = "pattern_example"; // String | pattern of repositories to search for
    try {
      List<String> result = apiInstance.adminUnadoptedList(page, limit, pattern);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminApi#adminUnadoptedList");
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
| **pattern** | **String**| pattern of repositories to search for | [optional] |

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

