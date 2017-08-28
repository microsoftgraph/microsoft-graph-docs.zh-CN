# <a name="get-started-with-microsoft-graph-and-rest"></a><span data-ttu-id="82937-101">开始使用 Microsoft Graph 和 REST</span><span class="sxs-lookup"><span data-stu-id="82937-101">Get started with Microsoft Graph and REST</span></span>

<span data-ttu-id="82937-p101">本文介绍了从 Azure AD v2.0 终结点获取访问令牌和使用 REST 调用来调用 Microsoft Graph 所需的任务。本文介绍了应用在进行身份验证和检索电子邮件时使用的请求和响应的顺序。</span><span class="sxs-lookup"><span data-stu-id="82937-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph using REST calls. It describes the sequence of requests and responses that an app uses to authenticate and retrieve email messages.</span></span>

<span data-ttu-id="82937-104">首先，需要使用 Azure Active Directory (Azure AD) 注册应用。</span><span class="sxs-lookup"><span data-stu-id="82937-104">First, you need register your app with Azure Active Directory (Azure AD).</span></span> 

## <a name="register-the-application"></a><span data-ttu-id="82937-105">注册应用程序</span><span class="sxs-lookup"><span data-stu-id="82937-105">Register the application</span></span>

<span data-ttu-id="82937-106">目前存在两种使用 Azure AD 注册应用的选项：</span><span class="sxs-lookup"><span data-stu-id="82937-106">There are currently two options to register your app with Azure AD.</span></span>

  - <span data-ttu-id="82937-107">注册应用以使用同时适用于个人 (Microsoft) 身份和工作/学校 (Azure AD) 帐户的 Azure AD v2.0 终结点。</span><span class="sxs-lookup"><span data-stu-id="82937-107">Register an app to use the Azure AD v2.0 endpoint that works for both personal (Microsoft) identities and work and school (Azure AD) accounts.</span></span>
  - <span data-ttu-id="82937-108">注册应用以使用仅支持工作和学校帐户的 Azure AD 终结点。</span><span class="sxs-lookup"><span data-stu-id="82937-108">Register an app to use the Azure AD endpoint that supports work and school accounts only.</span></span>

<span data-ttu-id="82937-p102">本文假定使用 v2.0 注册，因此需要在 [应用程序注册门户](https://apps.dev.microsoft.com/) 上注册应用。请按照 [使用 Azure AD v2.0 终结点注册 Microsoft Graph 应用程序](../concepts/auth_register_app_v2.md) 中的说明注册应用。有关使用 Azure AD 终结点的详细信息，请参阅 [使用 Azure AD 进行身份验证](../concepts/auth_v2_user.md)。</span><span class="sxs-lookup"><span data-stu-id="82937-p102">This article assumes a v2.0 registration, so you'll register your app on the [Application Registration Portal](https://apps.dev.microsoft.com/). Follow the instructions in [Register your Microsoft Graph application with the Azure AD v2.0 endpoint](../concepts/auth_register_app_v2.md) to register your app. For information about using the Azure AD endpoint, see [Authenticate using Azure AD](../concepts/auth_v2_user.md).</span></span>

> <span data-ttu-id="82937-p103">使用 v2.0 终结点时存在一些限制。若要判断是否适合你使用，请参阅 [是否应使用 v2.0 终结点？](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)</span><span class="sxs-lookup"><span data-stu-id="82937-p103">Some limitations apply when using the v2.0 endpoint. To decide if it's right for you, see [Should I use the v2.0 endpoint?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)</span></span>

## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="82937-114">对用户进行身份验证并获取一个访问令牌</span><span class="sxs-lookup"><span data-stu-id="82937-114">Authenticate the user and get an access token</span></span>

<span data-ttu-id="82937-p104">本文所述的应用会实现 [授权代码授予流](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/)，以便从遵循标准 [OAuth 2.0 协议](http://tools.ietf.org/html/rfc6749) 的 Azure AD v2.0 终结点获取访问令牌。有关 Azure AD v2.0 终结点中支持的流的完整指南，请参阅 [v2.0 终结点类型](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/)。</span><span class="sxs-lookup"><span data-stu-id="82937-p104">The app described in this article implements the [Authorization Code Grant flow](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/) to get access tokens from the Azure AD v2.0 endpoint, following standard [OAuth 2.0 protocols](http://tools.ietf.org/html/rfc6749). For a complete guide to the flows supported in the Azure AD v2.0 endpoint see [Types of the v2.0 endpoint](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/).</span></span>

<span data-ttu-id="82937-117">要使用授权代码授予流，首先要获取授权代码，然后使用此代码交换访问令牌。</span><span class="sxs-lookup"><span data-stu-id="82937-117">With the Authorization Code Grant flow, first you get an authorization code and then you exchange the code for an access token.</span></span>

### <a name="getting-an-authorization-code"></a><span data-ttu-id="82937-118">获取授权代码</span><span class="sxs-lookup"><span data-stu-id="82937-118">Getting an authorization code</span></span>

<span data-ttu-id="82937-p105">授权代码授予流的第一步是获取授权代码。用户登录并同意授予应用请求的权限后，授权服务器则会将此代码返回至应用。</span><span class="sxs-lookup"><span data-stu-id="82937-p105">The first step in the Authorization Code Grant flow is to get an authorization code. The code is returned to the app by the authorization server when the user signs in and consents to the permissions requested by the app.</span></span>

<span data-ttu-id="82937-p106">然后通过向 Azure AD v2.0 终结点发送 GET 请求来请求授权代码。必须在浏览器中打开此 URL，这样用户才能登录并给予同意。</span><span class="sxs-lookup"><span data-stu-id="82937-p106">You request an authorization code by sending a GET request to the Azure AD v2.0 endpoint. This URL must be opened in a browser so that the user can sign in and provide consent.</span></span>

#### <a name="construct-the-request"></a><span data-ttu-id="82937-123">构建请求</span><span class="sxs-lookup"><span data-stu-id="82937-123">Construct the request</span></span>

<span data-ttu-id="82937-124">1- 以基 URL开始：</span><span class="sxs-lookup"><span data-stu-id="82937-124">1- Start with the base URL:</span></span>

```
https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
```

<span data-ttu-id="82937-p107">路径中的 *tenant* 段控制可以登录应用程序的人员。允许的值为 *common*、*organizations*、*consumers* 和租户标识符。有关详细信息，请参阅 [协议终结点](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints)。</span><span class="sxs-lookup"><span data-stu-id="82937-p107">The *tenant* segment in the path controls who can sign into the application. Allowed values are *common*, *organizations*, *consumers*, and tenant identifiers. For more information, see [Protocol endpoints](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints).</span></span>

<span data-ttu-id="82937-p108">2- 向基 URL 追加查询参数。这些参数用于标识应用、请求的权限和其他身份验证请求信息。下表介绍了一些通用参数。</span><span class="sxs-lookup"><span data-stu-id="82937-p108">2- Append query parameters to the base URL. These are used to identify the app, the requested permissions, and other auth request information. The following table describes some common parameters.</span></span>

| <span data-ttu-id="82937-131">参数</span><span class="sxs-lookup"><span data-stu-id="82937-131">Parameter</span></span> | <span data-ttu-id="82937-132">说明</span><span class="sxs-lookup"><span data-stu-id="82937-132">Descriptions</span></span> |
|:------|:------|
| <span data-ttu-id="82937-133">client_id</span><span class="sxs-lookup"><span data-stu-id="82937-133">client_id</span></span> | <span data-ttu-id="82937-p109">注册应用生成的应用程序 ID。以便 Azure AD 知道哪个应用正在请求登录。</span><span class="sxs-lookup"><span data-stu-id="82937-p109">The app ID generated by registering the app. This lets Azure AD know which app is requesting the logon.</span></span> |
| <span data-ttu-id="82937-136">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="82937-136">redirect_uri</span></span> | <span data-ttu-id="82937-p110">在用户已向应用授予同意后，Azure 会重定向到的位置。此值必须对应于注册应用时所使用的**重定向 URI** 值。</span><span class="sxs-lookup"><span data-stu-id="82937-p110">The location that Azure will redirect to after the user has granted consent to the app. This value must correspond to the value of **Redirect URI** used when registering the app.</span></span> |
| <span data-ttu-id="82937-139">response_type</span><span class="sxs-lookup"><span data-stu-id="82937-139">response_type</span></span> | <span data-ttu-id="82937-p111">应用预期的响应类型。此值是用于授权代码授予流的 `code`。</span><span class="sxs-lookup"><span data-stu-id="82937-p111">The type of response the app is expecting. This value is `code` for the Authorization Code Grant flow.</span></span> |
| <span data-ttu-id="82937-142">scope</span><span class="sxs-lookup"><span data-stu-id="82937-142">scope</span></span> | <span data-ttu-id="82937-p112">应用请求的 [Microsoft Graph 权限范围](./permissions_reference.md) 的列表（用空格分隔）。还可以指定 [单一登录](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/) 的 [OpenId Connect 范围](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes)。</span><span class="sxs-lookup"><span data-stu-id="82937-p112">A space-separated list of [Microsoft Graph permission scopes](./permissions_reference.md) that the app is requesting. You can also specify [OpenId Connect scopes](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes) for [single sign-on](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/).</span></span>  |
| <span data-ttu-id="82937-145">state</span><span class="sxs-lookup"><span data-stu-id="82937-145">state</span></span> | <span data-ttu-id="82937-146">请求中包含的值，也将在令牌响应中返回，用于进行验证。</span><span class="sxs-lookup"><span data-stu-id="82937-146">A value included in the request that will also be returned in the token response, used for validation.</span></span> |

<span data-ttu-id="82937-147">例如，需要获取邮件读取访问权限的应用程序的请求 URL 可能如下所示。</span><span class="sxs-lookup"><span data-stu-id="82937-147">For example, the request URL for an application that requires read access to mail might look like the following.</span></span>

```
GET https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=<app ID>&redirect_uri=http%3A%2F%2Flocalhost/myapp%2F&response_type=code&state=1234&scope=mail.read
```

<span data-ttu-id="82937-p113">3- 将用户重定向到登录 URL。用户会看到登录屏幕（其中显示应用名称）。登录后，用户会看到应用需要获取的权限列表，还会提示用户确认是允许还是拒绝。如果用户允许，则浏览器将通过查询字符串中的授权代码和状态重定向至重定向 URL，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="82937-p113">3- Redirect the user to the logon URL. The user is presented with a sign in screen that displays the name of the app. After signing in, the user is presented with the list of the permissions the app requires and prompted to allow or deny. If the user consents, the browser redirects to the redirect URI with the authorization code and state in the query string, as shown in the following example.</span></span>

```
http://localhost/myapp/?code=AwABAAAA...cZZ6IgAA&state=1234
```

<span data-ttu-id="82937-152">下一步是交换返回的授权代码，以获得访问令牌。</span><span class="sxs-lookup"><span data-stu-id="82937-152">The next step is to exchange the authorization code returned for an access token.</span></span>

### <a name="getting-an-access-token"></a><span data-ttu-id="82937-153">获取访问令牌</span><span class="sxs-lookup"><span data-stu-id="82937-153">Getting an access token</span></span>

<span data-ttu-id="82937-154">为了获取访问令牌，应用会使用以下参数将表单编码参数发布到令牌请求 URL（例如，`https://login.microsoftonline.com/common/oauth2/v2.0/token`）中。</span><span class="sxs-lookup"><span data-stu-id="82937-154">To get an access token, the app posts form-encoded parameters to the token request URL (for example, `https://login.microsoftonline.com/common/oauth2/v2.0/token`) with the following parameters.</span></span>

| <span data-ttu-id="82937-155">参数</span><span class="sxs-lookup"><span data-stu-id="82937-155">Parameter</span></span> | <span data-ttu-id="82937-156">说明</span><span class="sxs-lookup"><span data-stu-id="82937-156">Descriptions</span></span> |
|:------|:------|
| <span data-ttu-id="82937-157">client_id</span><span class="sxs-lookup"><span data-stu-id="82937-157">client_id</span></span> | <span data-ttu-id="82937-158">注册应用生成的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="82937-158">The app ID generated by registering the app.</span></span> |
| <span data-ttu-id="82937-159">client_secret</span><span class="sxs-lookup"><span data-stu-id="82937-159">client_secret</span></span> | <span data-ttu-id="82937-160">注册应用后生成的应用程序机密。</span><span class="sxs-lookup"><span data-stu-id="82937-160">The app secret generated when registering the app.</span></span> |
| <span data-ttu-id="82937-161">code</span><span class="sxs-lookup"><span data-stu-id="82937-161">code</span></span> | <span data-ttu-id="82937-162">在上一步中获得的授权代码。</span><span class="sxs-lookup"><span data-stu-id="82937-162">The authorization code obtained in the prior step.</span></span> |
| <span data-ttu-id="82937-163">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="82937-163">redirect_uri</span></span> | <span data-ttu-id="82937-164">此值必须与授权代码请求中使用的值相同。</span><span class="sxs-lookup"><span data-stu-id="82937-164">This value must be the same as the value used in the authorization code request.</span></span> |
| <span data-ttu-id="82937-165">grant_type</span><span class="sxs-lookup"><span data-stu-id="82937-165">grant_type</span></span> | <span data-ttu-id="82937-p114">应用正在使用的授予类型。此值是用于授权代码授予流的 `code`。</span><span class="sxs-lookup"><span data-stu-id="82937-p114">The type of grant the app is using. This value is `code` for the Authorization Code Grant flow.</span></span> |
| <span data-ttu-id="82937-168">scope</span><span class="sxs-lookup"><span data-stu-id="82937-168">scope</span></span> | <span data-ttu-id="82937-169">应用请求的 [Microsoft Graph 权限范围](./permissions_reference.md) 的列表（用空格分隔）。</span><span class="sxs-lookup"><span data-stu-id="82937-169">A space-separated list of [Microsoft Graph permission scopes](./permissions_reference.md) that the app is requesting.</span></span> |

<span data-ttu-id="82937-170">我们应用程序的请求 URL（使用上一步中的代码）如下所示。</span><span class="sxs-lookup"><span data-stu-id="82937-170">The request URL for our application, using the code from the previous step, looks like the following.</span></span>

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

<span data-ttu-id="82937-171">服务器响应的是包括访问令牌的 JSON 有效负载。</span><span class="sxs-lookup"><span data-stu-id="82937-171">The server responds with a JSON payload which includes the access token.</span></span>

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

<span data-ttu-id="82937-p115">访问令牌位于 JSON 有效负载的 `access_token` 字段中。在对 API 执行 REST 调用时，应用使用此值来设置授权标头。</span><span class="sxs-lookup"><span data-stu-id="82937-p115">The access token is found in the `access_token` field of the JSON payload. The app uses this value to set the Authorization header when making REST calls to the API.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="82937-174">调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="82937-174">Call Microsoft Graph</span></span>

<span data-ttu-id="82937-p116">在获得访问令牌后，应用便可以调用 Microsoft Graph。由于此示例应用是要检索邮件，因此它会对 `https://graph.microsoft.com/v1.0/me/messages` 终结点使用 HTTP GET 请求。</span><span class="sxs-lookup"><span data-stu-id="82937-p116">After the app has an access token, it's ready to call Microsoft Graph. Because this sample app is retrieving messages, it will use an HTTP GET request to the `https://graph.microsoft.com/v1.0/me/messages` endpoint.</span></span>

### <a name="refine-the-request"></a><span data-ttu-id="82937-177">优化请求</span><span class="sxs-lookup"><span data-stu-id="82937-177">Refine the request</span></span>

<span data-ttu-id="82937-p117">应用可以使用 OData 查询参数来控制 GET 请求的行为。建议应用使用这些参数来限制返回的结果数，以及针对每一项返回的字段。</span><span class="sxs-lookup"><span data-stu-id="82937-p117">Apps can control the behavior of GET requests by using OData query parameters. We recommend that apps use these parameters to limit the number of results that are returned and to limit the fields that are returned for each item.</span></span> 

<span data-ttu-id="82937-p118">该示例应用会在表格中显示邮件，此表会显示主题、发件人以及邮件接收日期和时间。此表最多显示 25 行，并进行排序，将最近收到的邮件置顶。该应用使用以下查询参数来获得这些结果。</span><span class="sxs-lookup"><span data-stu-id="82937-p118">This sample app will display messages in a table that shows the subject, sender, and the date and time the message was received. The table displays a maximum of 25 rows and is sorted so that the most recently received message is at the top. The app uses the following query parameters to get these results.</span></span>

- <span data-ttu-id="82937-183">`$select` - 仅指定 `subject`、`sender` 和 `dateTimeReceived` 字段。</span><span class="sxs-lookup"><span data-stu-id="82937-183">`$select` - Specifies only the `subject`, `sender`, and `dateTimeReceived` fields.</span></span>
- <span data-ttu-id="82937-184">`$top` - 最多指定 25 个项。</span><span class="sxs-lookup"><span data-stu-id="82937-184">`$top` - Specifies a maximum of 25 items.</span></span>
- <span data-ttu-id="82937-185">`$orderby` - 按 `dateTimeReceived` 字段对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="82937-185">`$orderby` - Sorts the results by the `dateTimeReceived` field.</span></span>

<span data-ttu-id="82937-186">这会生成以下请求。</span><span class="sxs-lookup"><span data-stu-id="82937-186">This results in the following request.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

<span data-ttu-id="82937-p119">既然你已经了解如何调用 Microsoft Graph，现在就可以使用 API 参考来构造应用需要执行的其他任何种类调用。不过，请注意，应用需要获得应用注册时配置的适当权限，才能执行调用。</span><span class="sxs-lookup"><span data-stu-id="82937-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="82937-189">后续步骤</span><span class="sxs-lookup"><span data-stu-id="82937-189">Next steps</span></span>
- <span data-ttu-id="82937-190">使用 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer) 试用更多 REST API。</span><span class="sxs-lookup"><span data-stu-id="82937-190">Try out more of the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="82937-191">另请参阅</span><span class="sxs-lookup"><span data-stu-id="82937-191">See also</span></span>
- [<span data-ttu-id="82937-192">Azure AD v2.0 协议</span><span class="sxs-lookup"><span data-stu-id="82937-192">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="82937-193">Azure AD v2.0 令牌</span><span class="sxs-lookup"><span data-stu-id="82937-193">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
