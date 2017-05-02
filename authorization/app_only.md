# <a name="call-microsoft-graph-in-a-service-or-daemon-app"></a>在服务或守护程序应用中调用 Microsoft Graph

本文介绍了连接单租户服务或守护程序应用与 Office 365，以及调用 Microsoft Graph API 之前至少需要完成的任务。

> **注意：**本主题介绍了将 Azure Active Directory 用作应用的验证提供程序。若要了解如何使用 Azure AD v2.0 终结点实现服务或守护程序应用，请参阅 <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-client-creds/" target="_newtab">v2.0 协议 - OAuth 2.0 客户端凭据流</a>。

## <a name="register-the-application-in-azure-active-directory"></a>在 Azure Active Directory 中注册应用程序

需要先在 [Azure 门户](https://portal.azure.com) 注册应用程序，然后才能开始使用 Office 365。请记住下列具体事项：

- 注册应用程序后，配置服务或守护程序应用需要的应用程序权限。
- 请记下 Azure 应用程序注册过程中的下列值。需要使用这些值在服务或守护程序应用中配置 OAuth 流：
    * 应用程序 ID（应用程序专用）
    * 应用密钥或机密（应用程序专用）
    * 应用 OAuth 2.0 令牌终结点
      * 在应用页面中，单击 Azure 管理门户底部的“*查看终结点*”，找到此值。终结点看起来像 `https://login.microsoftonline.com/{tenantId}/oauth2/token`。

## <a name="request-an-access-token-from-the-token-issuing-endpoint"></a>从令牌颁发终结点请求获取访问令牌

与客户端应用不同，服务或守护程序应用不具有用户登录功能，也无法授权您的应用程序。相反，应用程序必须实现允许其使用它自己的凭据、客户端 ID 和应用程序键的 OAuth 2.0 客户端凭据授予流，以便在调用 Microsoft Graph 时进行身份验证（而不是模拟用户）。有关身份验证流的详细信息，请参阅 [使用客户端凭据的服务到服务调用](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service)。

对令牌颁发终结点提出包含以下参数的 HTTP POST 请求（用您应用的客户端 ID 和应用程序键分别替换 `<clientId>` 和 `<clientSecret>`）。

```http
POST https://login.microsoftonline.com/{tenantId}/oauth2/token HTTP/1.1
Content-Type: application/x-www-form-urlencoded

grant_type=client_credentials
&client_id=<clientId>
&client_secret=<clientSecret>
&resource=https://graph.microsoft.com
```

响应将包含访问令牌和过期信息。

```json
{ 
  "token_type": "Bearer",
  "expires_in": "3599",
  "scope": "User.Read",
  "expires_on": "1449685363",
  "not_before": "1449681463",
  "resource": "https://graph.microsoft.com",
  "access_token": "<token>"
}
```

## <a name="use-the-access-token-in-a-request-to-the-microsoft-graph-api"></a>在对 Microsoft Graph API 提出的请求中使用访问令牌

使用访问令牌，您的应用可以对 Microsoft Graph API 提出身份验证请求。您的应用必须将访问令牌附加到各个请求的**授权**头中。

例如，如果你在 Azure 管理门户中为服务或守护程序应用选取了“*读取所有用户的完整配置文件*”权限，则服务或守护程序应用可以检索租户中的所有用户。 

```http
GET https://graph.microsoft.com/v1.0/users
Authorization: Bearer <token>
```
