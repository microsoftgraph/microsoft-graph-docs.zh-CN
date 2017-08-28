# <a name="get-started-with-microsoft-graph-and-rest"></a>开始使用 Microsoft Graph 和 REST

本文介绍了从 Azure AD v2.0 终结点获取访问令牌和使用 REST 调用来调用 Microsoft Graph 所需的任务。本文介绍了应用在进行身份验证和检索电子邮件时使用的请求和响应的顺序。

首先，需要使用 Azure Active Directory (Azure AD) 注册应用。 

## <a name="register-the-application"></a>注册应用程序

目前存在两种使用 Azure AD 注册应用的选项：

  - 注册应用以使用同时适用于个人 (Microsoft) 身份和工作/学校 (Azure AD) 帐户的 Azure AD v2.0 终结点。
  - 注册应用以使用仅支持工作和学校帐户的 Azure AD 终结点。

本文假定使用 v2.0 注册，因此需要在 [应用程序注册门户](https://apps.dev.microsoft.com/) 上注册应用。请按照 [使用 Azure AD v2.0 终结点注册 Microsoft Graph 应用程序](../concepts/auth_register_app_v2.md) 中的说明注册应用。有关使用 Azure AD 终结点的详细信息，请参阅 [使用 Azure AD 进行身份验证](../concepts/auth_v2_user.md)。

> 使用 v2.0 终结点时存在一些限制。若要判断是否适合你使用，请参阅 [是否应使用 v2.0 终结点？](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)

## <a name="authenticate-the-user-and-get-an-access-token"></a>对用户进行身份验证并获取一个访问令牌

本文所述的应用会实现 [授权代码授予流](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/)，以便从遵循标准 [OAuth 2.0 协议](http://tools.ietf.org/html/rfc6749) 的 Azure AD v2.0 终结点获取访问令牌。有关 Azure AD v2.0 终结点中支持的流的完整指南，请参阅 [v2.0 终结点类型](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/)。

要使用授权代码授予流，首先要获取授权代码，然后使用此代码交换访问令牌。

### <a name="getting-an-authorization-code"></a>获取授权代码

授权代码授予流的第一步是获取授权代码。用户登录并同意授予应用请求的权限后，授权服务器则会将此代码返回至应用。

然后通过向 Azure AD v2.0 终结点发送 GET 请求来请求授权代码。必须在浏览器中打开此 URL，这样用户才能登录并给予同意。

#### <a name="construct-the-request"></a>构建请求

1- 以基 URL开始：

```
https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
```

路径中的 *tenant* 段控制可以登录应用程序的人员。允许的值为 *common*、*organizations*、*consumers* 和租户标识符。有关详细信息，请参阅 [协议终结点](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints)。

2- 向基 URL 追加查询参数。这些参数用于标识应用、请求的权限和其他身份验证请求信息。下表介绍了一些通用参数。

| 参数 | 说明 |
|:------|:------|
| client_id | 注册应用生成的应用程序 ID。以便 Azure AD 知道哪个应用正在请求登录。 |
| redirect_uri | 在用户已向应用授予同意后，Azure 会重定向到的位置。此值必须对应于注册应用时所使用的**重定向 URI** 值。 |
| response_type | 应用预期的响应类型。此值是用于授权代码授予流的 `code`。 |
| scope | 应用请求的 [Microsoft Graph 权限范围](./permissions_reference.md) 的列表（用空格分隔）。还可以指定 [单一登录](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/) 的 [OpenId Connect 范围](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes)。  |
| state | 请求中包含的值，也将在令牌响应中返回，用于进行验证。 |

例如，需要获取邮件读取访问权限的应用程序的请求 URL 可能如下所示。

```
GET https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=<app ID>&redirect_uri=http%3A%2F%2Flocalhost/myapp%2F&response_type=code&state=1234&scope=mail.read
```

3- 将用户重定向到登录 URL。用户会看到登录屏幕（其中显示应用名称）。登录后，用户会看到应用需要获取的权限列表，还会提示用户确认是允许还是拒绝。如果用户允许，则浏览器将通过查询字符串中的授权代码和状态重定向至重定向 URL，如以下示例所示。

```
http://localhost/myapp/?code=AwABAAAA...cZZ6IgAA&state=1234
```

下一步是交换返回的授权代码，以获得访问令牌。

### <a name="getting-an-access-token"></a>获取访问令牌

为了获取访问令牌，应用会使用以下参数将表单编码参数发布到令牌请求 URL（例如，`https://login.microsoftonline.com/common/oauth2/v2.0/token`）中。

| 参数 | 说明 |
|:------|:------|
| client_id | 注册应用生成的应用程序 ID。 |
| client_secret | 注册应用后生成的应用程序机密。 |
| code | 在上一步中获得的授权代码。 |
| redirect_uri | 此值必须与授权代码请求中使用的值相同。 |
| grant_type | 应用正在使用的授予类型。此值是用于授权代码授予流的 `code`。 |
| scope | 应用请求的 [Microsoft Graph 权限范围](./permissions_reference.md) 的列表（用空格分隔）。 |

我们应用程序的请求 URL（使用上一步中的代码）如下所示。

```
POST https://login.microsoftonline.com/common/oauth2/v2.0/token
Content-Type: application/x-www-form-urlencoded

{
  grant_type=authorization_code
  &code=AwABAAAA...cZZ6IgAA
  &redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
  &resource=https%3A%2F%2Fgraph.microsoft.com%2F
  &scope=mail.read
  &client\_id=<app ID>
  &client\_secret=<app SECRET>
}
```

服务器响应的是包括访问令牌的 JSON 有效负载。

```
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

{
  "token_type":"Bearer",
  "expires_in":"3600",
  "access_token":"eyJ0eXAi...b66LoPVA",
  "scope":"https://graph.microsoft.com/mail.read",
  ...
}
```

访问令牌位于 JSON 有效负载的 `access_token` 字段中。在对 API 执行 REST 调用时，应用使用此值来设置授权标头。

## <a name="call-microsoft-graph"></a>调用 Microsoft Graph

在获得访问令牌后，应用便可以调用 Microsoft Graph。由于此示例应用是要检索邮件，因此它会对 `https://graph.microsoft.com/v1.0/me/messages` 终结点使用 HTTP GET 请求。

### <a name="refine-the-request"></a>优化请求

应用可以使用 OData 查询参数来控制 GET 请求的行为。建议应用使用这些参数来限制返回的结果数，以及针对每一项返回的字段。 

该示例应用会在表格中显示邮件，此表会显示主题、发件人以及邮件接收日期和时间。此表最多显示 25 行，并进行排序，将最近收到的邮件置顶。该应用使用以下查询参数来获得这些结果。

- `$select` - 仅指定 `subject`、`sender` 和 `dateTimeReceived` 字段。
- `$top` - 最多指定 25 个项。
- `$orderby` - 按 `dateTimeReceived` 字段对结果进行排序。

这会生成以下请求。

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

既然你已经了解如何调用 Microsoft Graph，现在就可以使用 API 参考来构造应用需要执行的其他任何种类调用。不过，请注意，应用需要获得应用注册时配置的适当权限，才能执行调用。

## <a name="next-steps"></a>后续步骤
- 使用 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer) 试用更多 REST API。

## <a name="see-also"></a>另请参阅
- [Azure AD v2.0 协议](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0 令牌](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
