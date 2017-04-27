
# <a name="microsoft-graph-app-authentication-using-azure-ad"></a>使用 Azure AD 进行 Microsoft Graph 应用身份验证

本文详细介绍了 Microsoft Graph 应用的示例身份验证和授权流。该示例将 Azure Active Directory (Azure AD) 用作身份验证提供程序，并将<a href="https://msdn.microsoft.com/en-us/library/azure/dn645542.aspx" target="_newtab">授权代码授予流</a>用作身份验证流。该示例将演示如何使用 Microsoft Graph 应用中的 Azure AD 对用户进行身份验证、获取访问令牌及如何使用刷新令牌续订访问令牌。

对于代码授予流，身份验证流程可以分成两个基本步骤：

1. 请求获取授权代码
2. 使用授权代码请求访问令牌和刷新令牌。 

如果当前访问令牌过期，则可以使用刷新令牌获取新的访问令牌。
 
##<a name="authenticate-a-user-and-get-app-authorized"></a>对用户进行身份验证并让应用获得授权

若要让应用获得授权，则必须让用户先进行身份验证。可以通过将用户以及应用信息一起重定向至 Azure Active Directory (Azure AD) 授权终结点，然后登录其工作或学校帐户来执行此操作。用户登录并同意应用请求的权限（如果用户尚未执行此操作）后，应用将会收到获取 OAuth 访问令牌所需的授权代码。

> **注意**：你可以通过在 [Azure AD Authentication Library (ADAL)](https://msdn.microsoft.com/en-us/library/azure/jj573266.aspx) 上调用方法来执行此操作。有关授权流程的详细信息，请参阅[授权代码授予流程](https://msdn.microsoft.com/en-us/library/azure/dn645542.aspx)。

授权应用首先要使用下面的 URL 提交 HTTPS GET 请求：
 
```GET https://login.microsoftonline.com/common/oauth2/authorize?response_type=code&redirect_uri=<uri>&client_id=<id>```

**所需的查询字符串参数**

| 参数名  | 值  | 说明                                                                                            |
|:----------------|:-------|:-------------------------------------------------------------------------------------------------------|
| *client_id*     | string | 为你的应用创建的客户端 ID。这是应用在 Azure 租户应用程序注册表设置的**客户端 ID** 值。                                                                  |
| *response_type* | string | 指定请求的响应类型。在授权代码的授权请求中，该值必须是代码。 |
| *redirect_uri*  | string | 身份验证完成时浏览器发送到的重定向 URL。此值必须匹配应用预配置的**回复 URL** 值                        |
 


以下显示正在运行的应用程序中实现此类请求的示例：


```GET https://login.microsoftonline.com/common/oauth2/authorize?response_type=code&redirect_uri=http%3a%2f%2flocalhost:1339/auth/azureoauth/callback&client_id=8b8539cd-7b75-427f-bef1-4a6264fd4940``` 

此请求将返回 `200 OK` 响应并显示 Azure AD 帐户登录页。 

用户使用有效的凭据登录并同意对该应用授予的权限后，登录页会向 Azure 发送 `POST` 请求。如果上述请求成功，Azure 会响应 `302 Found` 消息，将调用转发到应用的重定向 URI，以便应用接收所需的访问令牌。响应的 `Location` 标头中指定的转发 URI 对应于应用的回复 URL，附加两个查询参数 `code=...` 和 `session_state=...`。下面的示例演示此类响应的摘要： 

```no-highlight 
HTTP/1.1 302 Found
Cache-Control: no-cache, no-store
Pragma: no-cache
Content-Type: text/html; charset=utf-8
Expires: -1
Location: http://localhost:1339/auth/azureoauth/callback?code=AAABAAAAvPM...&session_state=a9556cd3-cae6-4bc9-bf51-672f7b79b7c6
Server: Microsoft-IIS/8.5
P3P: CP="DSP CUR OTPi IND OTRi ONL FIN"

..... 
```

在此示例中，应用的回复 URL 是 `http://localhost:1339/auth/azureoauth/callback`。处理此响应时，你必须提取 `code` 参数值，并使用它来获取初始的 OAuth 2.0 访问令牌和刷新令牌（请参阅下一节）。

> **注意：**如果你已针对 `https://login.windows.net/{tenantId}/oauth2/authorize?...` URL 启动登录流程，则上面的 `302 Found` 响应不同于将获得的 `302 Found` 响应。对于后者，`302 Found` 响应会将请求转发到 `login.microsoftonline.com`。
 
<!---<a name="msg_get_app_authenticated"> </a> -->

##<a name="acquire-an-access-token"></a>获取访问令牌
若要访问 Microsoft Graph 资源，应用必须在每个 HTTP 请求中包含有效的 OAuth 2.0 访问令牌。可以使用下面的 POST 请求获取访问令牌：

```no-highlight 
POST https://login.microsoftonline.com/common/oauth2/token HTTP/1.1
content-type : application/x-www-form-urlencoded
content-length : 144
```
 
该请求需要以下格式的 URL 编码有效负载：
 
```no-highlight 
grant_type=authorization_code
&redirect_uri=<uri>
&client_id=<id>
&client_secret=<secret_key>
&code=<code>
&resource=https%3A%2F%2Fgraph.microsoft.com%2F
```

**所需的查询字符串参数**

| 参数名  | 值  | 说明                                                                                            |
|:----------------|:-------|:-------------------------------------------------------------------------------------------------------|
| *client_id*     | string | 为应用创建的客户端 ID。  |
| *client_secret*  | string | 为你的应用创建的密钥。此值与 Azure 管理门户上应用配置页面**密钥**一节中的值相同。|
| *redirect_uri*  | string | 身份验证完成时浏览器发送到的重定向 URL。  |
| *code*  | string | 授权代码。从对授权请求的响应中返回的 `code` 查询参数值。 |
| *resource*   | string | 您要访问的资源。若要调用 Microsoft Graph API，请将此参数值设置为 https://graph.microsoft.com/。|

下面的代码段举例说明用来获取初始 OAuth 2.0 访问令牌的请求有效负载。

```no-highlight  
grant_type=authorization_code&
redirect_uri=http%3A%2F%2Flocalhost%3A1339%2Fauth%2Fazureoauth%2Fcallback&
client_id=8b8539cd-7b75-427f-bef1-4a6264fd4940&client_secret=PJW3dznGfyNSm3rM9aHeXWGKsTMepKXT1Eqy45XXdU4%3D&
code=AAABAAAAvPM1KaPlrEqdFSBzjqfTGBLRVQc6BtQmJ_9DQZUg8Tb7TJgTmbTE7AHM93qB5EKc4Bf-bOgzt3mebAywK-09X1uBHwOluuqSWfd9LU2HHgZtxcZFIYI5UL7L1UEvhrJRvX2iHhfz9ZSRMZMVL55n_K79gCOxtSATeCUw52zPk5ZaQ87Y42SCLsRZN4Y_zddhD3mMpkObiHVT8HzfhBUiT0oX0e-Q439vkbZoKiq1HaqMR3IPHiCXDbPPH5u7a4NTe5xAhh-o2MUIe6s4Xqql86sv1-IwyroOJJMueGUarkfbgwqmYL9Tm-jWab8o-BAK_plVsN73GU8cXO8ts30wa2YmNR5ZxSkw8oiB4mSZwGzGQlch55DRnucDs0SZBgj5etGi3SeXv5jhKlDU2S0bAPnGxF3QAH0N_zBpfakETVlcsHKi714u-tn9da6aTPQsE0IYKTAYgxjTMei6zfRFvCZi-tKdFR6X9TvvmF2iPdGQGWKeLw8CMWUzU8VmOhiHc0aBKG6RaXAOTM067J_9WKYPxMopcytD2z8HVkL1QhggAA&
resource=https%3A%2F%2Fgraph.microsoft.com%2F
```

如果此请求成功，将返回 `200 OK` 响应。一个示例如下所示：

```no-highlight  
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8
Expires: -1
Content-Length: 2978
Access-Control-Allow-Origin: *

{
    "token_type":"Bearer",
    "expires_in":"3599",
    "expires_on":"1426551729",
    "not_before":"1426547829",
    "resource":"https://graph.microsoft.com/",
    "access_token":"eyJ0eXAiOiJKV1QiLCJhb...",
    "refresh_token":"AAABAAAAvPM1KaPlrEqd...",
    "scope": "Calendar.ReadWrite Directory.Read.All Files.ReadWrite Group.ReadWrite.All Mail.ReadWrite Mail.Send User.ReadBasic.All",
    "id_token":"eyJ0eXAiOiJKV1QiLCJhbGci..."
}
```

 
响应正文是包含访问令牌 (`access_token`) 的 JSON 格式的字符串。需要为任何后续的 HTTP 请求提供此令牌，以便访问 Microsoft Graph 资源。 

`scope` 属性值应与应用注册过程中为应用授予的权限匹配。

访问令牌从发放时起，在指定的时间间隔（上述示例中的 `3599`）秒数（或 1 小时）内保持有效，如 `expires_in` 属性中所指定。结果还包含必须用于续订即将过期或已过期访问令牌的刷新令牌 (`refresh_token`)。 

在任意生产代码中，你的应用需要关注这些令牌的有效期并在刷新令牌到期之前续订即将过期的访问令牌。 
-->

<!---<a name="msg_renew_access_token using refresh token"> </a> -->

##<a name="renew-expiring-access-token-using-refresh-token"></a>使用刷新令牌续订即将过期的访问令牌
若要刷新过期的访问令牌，请使用类似以下示例的 POST 请求（前提是刷新令牌没有过期）：

```no-highlight  
POST https://login.microsoftonline.com/common/oauth2/token HTTP/1.1
Host: login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded
Content-Length: 897


grant_type=refresh_token
&redirect_uri=http%3A%2F%2Flocalhost%3A1339%2Fauth%2Fazureoauth%2Fcallback
&client_id=8b8539cd-7b75-427f-bef1-4a6264fd4940
&client_secret=PJW3dznGfyNSm3rM9aHeXWGKsTMepKXT1Eqy45XXdU4%3D
&refresh_token=AAABAAAAvPM1KaPlrEqdFSBzjqfTGM74--...
&resource=https%3A%2F%2Fgraph.microsoft.com%2F
```

**所需的查询字符串参数**

| 参数名  | 值  | 说明                                                                                                                                         |
|:----------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| *client_id*     | string | 为应用程序创建的客户端 ID。  |
| *redirect_uri*  | string | 身份验证完成时浏览器发送到的重定向 URL。这应与第一个请求中使用的 *redirect_uri* 值匹配。 |
| *client_secret* | string | 为应用程序创建的其中一个密钥值。                                                                                                     |
| *refresh_token* | string | 以前收到的刷新令牌。    |
| *resource*      | string | 您要访问的资源。|

注意，此请求几乎等同于初始令牌获取请求。请求有效负载存在两个差异，即，`grant_type` 参数现在具有 `refresh_token` 值（而不是 `code`）。
 
成功的响应将返回类似于以下输出的 JSON 字符串的有效负载：

```no-highlight 
{
    "token_type":"Bearer",
    "expires_in":"3600",
    "expires_on":"1426561346",
    "not_before":"1426557446",
    "resource":"https://graph.microsoft.com/",
    "access_token":"eyJ0eXAiOiJKV1QiLCJhbGciOi...", 
    "refresh_token":"AAABAAAAvPM1KaPlrEqdFSBzj...",
   "scope":"Graph.Read",
    "pwd_exp":"6553342",
    "pwd_url":"https://portal.microsoftonline.com/ChangePassword.aspx"
}
```
 
除了缺少 `id_token` 属性外，该响应正文与初始令牌获取响应具有相同的语法和语义。新返回的 `access_token` 和 `refresh_token` 值的有效期已延长。访问令牌的新到期时间是 `expires_in` 值中指定的秒数，从令牌刷新请求成功提交之时算起。 
 
当刷新令牌到期时，无法使用上述 POST 请求续订任何过期的访问令牌。相反，你必须重新启动应用授权和身份验证过程。



