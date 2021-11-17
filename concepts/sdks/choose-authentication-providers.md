---
title: 选择 Microsoft Graph身份验证提供程序
description: 了解如何为应用程序选择特定于方案的身份验证提供程序。
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: e5375225aa8d9ab01b82f99fee1930e952767718
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020030"
---
<!-- markdownlint-disable MD001 MD024 MD025 -->

# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a>根据方案选择 Microsoft Graph 身份验证提供程序

身份验证提供程序使用 MICROSOFT 身份验证库和 MSAL 身份验证库实现 (所需的) ;处理增量同意、密码过期和条件访问等情况下的一些潜在错误;，然后设置 HTTP 请求授权标头。 下表列出了一组与不同应用程序类型的方案匹配的 [提供程序](/azure/active-directory/develop/v2-app-types)。

| 应用场景                                                                                               | Flow/授予         | 受众               | 提供程序 |
|--------------------------------------------------------------------------------------------------------|--------------------|------------------------|-----|
| [单页应用](/azure/active-directory/develop/scenario-spa-acquire-token)                          | PKCE 授权代码 | 委派使用者/组织 | [授权代码提供程序](#authorization-code-provider) |
| [调用 Web API 的 Web 应用](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) |                    |                        |     |
|                                                                                                        | 授权代码 | 委派使用者/组织 | [授权代码提供程序](#authorization-code-provider) |
|                                                                                                        | 客户端凭据 | 仅限应用               | [客户端凭据提供程序](#client-credentials-provider) |
| [调用 Web API 的 Web API](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) |                    |                        |     |
|                                                                                                        | 代表       | 委派使用者/组织 | [代表提供程序](#on-behalf-of-provider) |
|                                                                                                        | 客户端凭据 | 仅限应用               | [客户端凭据提供程序](#client-credentials-provider) |
| [调用 Web API 的桌面应用](/azure/active-directory/develop/scenario-desktop-acquire-token)      |                    |                        |     |
|                                                                                                        | Interactive        | 委派使用者/组织 | [交互式提供程序](#interactive-provider) |
|                                                                                                        | 集成Windows | 委派组织          | [集成Windows提供程序](#integrated-windows-provider) |
|                                                                                                        | 资源所有者     | 委派组织          | [用户名/密码提供程序](#usernamepassword-provider) |
|                                                                                                        | 设备代码        | 委派组织          | [设备代码提供程序](#device-code-provider) |
| [守护程序应用](/azure/active-directory/develop/scenario-daemon-acquire-token)                            |                    |                        |     |
|                                                                                                        | 客户端凭据 | 仅限应用               | [客户端凭据提供程序](#client-credentials-provider) |
| [调用 Web API 的移动应用](/azure/active-directory/develop/scenario-mobile-acquire-token)        |                    |                        |     |
|                                                                                                        | Interactive        | 委派使用者/组织 | [交互式提供程序](#interactive-provider) |

> [!NOTE]
> 以下代码段是使用其各自 SDK 的最新版本编写的。 如果你遇到这些代码段的编译器错误，请确保你拥有最新版本。 使用的身份验证提供程序由以下 Azure 标识库提供：
>
> - .NET 开发人员需要添加 [Azure.Identity](/dotnet/api/azure.identity) 包。
> - JavaScript 开发人员需要添加 [@azure/标识](/javascript/api/@azure/identity) 库。
> - Java和 Android 开发人员需要添加 azure [标识](/java/api/overview/azure/identity-readme) 库。

## <a name="authorization-code-provider"></a>授权代码提供程序

授权代码流使本机和 Web 应用能够安全地获取用户名称中的令牌。 若要了解更多信息，请参阅[Microsoft 标识平台 和 OAuth 2.0 授权代码流](/azure/active-directory/develop/v2-oauth2-auth-code-flow)。

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

// For authorization code flow, the user signs into the Microsoft
// identity platform, and the browser is redirected back to your app
// with an authorization code in the query parameters
var authorizationCode = "AUTH_CODE_FROM_REDIRECT";

// using Azure.Identity;
var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// https://docs.microsoft.com/dotnet/api/azure.identity.authorizationcodecredential
var authCodeCredential = new AuthorizationCodeCredential(
    tenantId, clientId, clientSecret, authorizationCode, options);

var graphClient = new GraphServiceClient(authCodeCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

### <a name="using-azuremsal-browser-for--browser-applications"></a>将 @azure/msal-browser 用于浏览器应用程序

```javascript

const {
    PublicClientApplication,
    InteractionType,
    AccountInfo
} = require("@azure/msal-browser");

const {
    AuthCodeMSALBrowserAuthenticationProvider,
    AuthCodeMSALBrowserAuthenticationProviderOptions
} = require("@microsoft/microsoft-graph-client/authProviders/authCodeMsalBrowser");

const options: AuthCodeMSALBrowserAuthenticationProviderOptions: {
    account: account, // the AccountInfo instance to acquire the token for.
    interactionType: InteractionType.PopUp, // msal-browser InteractionType
    scopes: ["user.read", "mail.send"] // example of the scopes to be passed
}

// Pass the PublicClientApplication instance from step 2 to create AuthCodeMSALBrowserAuthenticationProvider instance
const authProvider: new AuthCodeMSALBrowserAuthenticationProvider(publicClientApplication, options),
```

### <a name="using-azureidentity-for-server-side-applications"></a>对@azure应用程序使用 @azure/标识

```javascript
const {
    Client
} = require("@microsoft/microsoft-graph-client");
const {
    TokenCredentialAuthenticationProvider
} = require("@microsoft/microsoft-graph-client/authProviders/azureTokenCredentials");
const {
    AuthorizationCodeCredential
} = require("@azure/identity");

const credential = new AuthorizationCodeCredential(
    "<YOUR_TENANT_ID>",
    "<YOUR_CLIENT_ID>",
    "<AUTH_CODE_FROM_QUERY_PARAMETERS>",
    "<REDIRECT_URL>"
);
const authProvider = new TokenCredentialAuthenticationProvider(credential, {
    scopes: [scopes]
});

```

# <a name="java"></a>[Java](#tab/Java)

```java
final AuthorizationCodeCredential authCodeCredential = new AuthorizationCodeCredentialBuilder()
        .clientId(clientId)
        .clientSecret(clientSecret) //required for web apps, do not set for native apps
        .authorizationCode(authorizationCode)
        .redirectUrl(redirectUri)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, authCodeCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

不适用。

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

不适用。

# <a name="php"></a>[PHP](#tab/PHP)

尚不可用。 如果这对你很重要Graph支持或打开[Microsoft](https://aka.ms/graphrequests) Graph功能请求。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://aka.ms/graphrequests)请求（如果这对你很重要）。

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota/authentication/go/azure"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewAuthorizationCodeCredential(
    "TENANT_ID",
    "CLIENT_ID",
    "AUTH_CODE",
    "REDIRECT_URL",
    &azidentity.AuthorizationCodeCredentialOptions {
        ClientSecret: "CLIENT_SECRET",
    },
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="client-credentials-provider"></a>客户端凭据提供程序

客户端凭据流使服务应用程序无需用户交互即可运行。 访问基于应用程序的标识。 有关详细信息，请参阅 Microsoft 标识平台[和 OAuth 2.0 客户端凭据流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。

# <a name="c"></a>[C#](#tab/CS)

### <a name="using-a-client-secret"></a>使用客户端密码

```csharp
// The client credentials flow requires that you request the
// /.default scope, and preconfigure your permissions on the
// app registration in Azure. An administrator must grant consent
// to those permissions beforehand.
var scopes = new[] { "https://graph.microsoft.com/.default" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

// using Azure.Identity;
var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// https://docs.microsoft.com/dotnet/api/azure.identity.clientsecretcredential
var clientSecretCredential = new ClientSecretCredential(
    tenantId, clientId, clientSecret, options);

var graphClient = new GraphServiceClient(clientSecretCredential, scopes);
```

### <a name="using-a-client-certificate"></a>使用客户端证书

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientCertificate = new X509Certificate2("MyCertificate.pfx");

// using Azure.Identity;
var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// https://docs.microsoft.com/dotnet/api/azure.identity.clientcertificatecredential
var clientCertCredential = new ClientCertificateCredential(
    tenantId, clientId, clientCertificate, options);

var graphClient = new GraphServiceClient(clientCertCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

```javascript
const {
    Client
} = require("@microsoft/microsoft-graph-client");
const {
    TokenCredentialAuthenticationProvider
} = require("@microsoft/microsoft-graph-client/authProviders/azureTokenCredentials");
const {
    ClientSecretCredential
} = require("@azure/identity");

const credential = new ClientSecretCredential(tenantId, clientId, clientSecret);
const authProvider = new TokenCredentialAuthenticationProvider(credential, {
    scopes: [scopes]
});

const client = Client.initWithMiddleware({
    debugLogging: true,
    authProvider
    // Use the authProvider object to create the class.
});
```

# <a name="java"></a>[Java](#tab/Java)

```java
final ClientSecretCredential clientSecretCredential = new ClientSecretCredentialBuilder()
        .clientId(clientId)
        .clientSecret(clientSecret)
        .tenantId(tenant)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, clientSecretCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

不适用。

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

不适用。

# <a name="php"></a>[PHP](#tab/PHP)

尚不可用。 如果这对你很重要Graph支持或打开[Microsoft](https://aka.ms/graphrequests) Graph功能请求。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

尚不可用。 如果这对你很重要Graph支持或打开[Microsoft](https://aka.ms/graphrequests) Graph功能请求。

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota/authentication/go/azure"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewClientSecretCredential(
    "TENANT_ID",
    "CLIENT_ID",
    "CLIENT_SECRET",
    nil,
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="on-behalf-of-provider"></a>代表提供程序

当应用程序调用服务/Web API 时，代表流适用，而服务/Web API 则调用 Microsoft Graph API。 通过阅读 Microsoft 标识平台 和[OAuth 2.0 代表流了解更多信息](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="c"></a>[C#](#tab/CS)

`Azure.Identity`自版本 1.4.0 起，程序包不支持代表流。 而是使用 MSAL 创建自定义身份验证提供程序。

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

// using Azure.Identity;
var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// This is the incoming token to exchange using on-behalf-of flow
var oboToken = "JWT_TOKEN_TO_EXCHANGE";

var cca = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantId)
    .WithClientSecret(clientSecret)
    .Build();

// DelegateAuthenticationProvider is a simple auth provider implementation
// that allows you to define an async function to retrieve a token
// Alternatively, you can create a class that implements IAuthenticationProvider
// for more complex scenarios
var authProvider = new DelegateAuthenticationProvider(async (request) => {
    // Use Microsoft.Identity.Client to retrieve token
    var assertion = new UserAssertion(oboToken);
    var result = await cca.AcquireTokenOnBehalfOf(scopes, assertion).ExecuteAsync();

    request.Headers.Authorization =
        new System.Net.Http.Headers.AuthenticationHeaderValue("Bearer", result.AccessToken);
});

var graphClient = new GraphServiceClient(authProvider);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

代表 OAuth 流目前要求您实现自定义身份验证提供程序。 有关详细信息 [，请参阅](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) 使用自定义验证提供程序。

# <a name="java"></a>[Java](#tab/Java)

```java
final OnBehalfOfCredential onBehalfOfCredential = new OnBehalfOfCredentialBuilder()
        .clientId(clientID)
        .pfxCertificate(pfxCertificatePath) // or .pemCertificate(certificatePath) or .clientSecret("ClientSecret")
        .clientCertificatePassword(pfxCertificatePassword) // remove if using pemCertificate or clientSecret
        .tokenCachePersistenceOptions(tokenCachePersistenceOptions) //Optional: enables the persistent token cache which is disabled by default
        .userAssertion(userAssertion)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, onBehalfOfCredential);

final GraphServiceClient graphClient = GraphServiceClient
        .builder()
        .authenticationProvider(tokenCredentialAuthProvider)
        .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

不适用。

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

不适用。

# <a name="php"></a>[PHP](#tab/PHP)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://aka.ms/graphrequests)请求（如果这对你很重要）。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://aka.ms/graphrequests)请求（如果这对你很重要）。

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://aka.ms/graphrequests)请求（如果这对你很重要）。

---

## <a name="implicit-provider"></a>隐式提供程序

由于存在隐式身份验证流的缺点， [因此不建议使用隐式身份验证流](https://datatracker.ietf.org/doc/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6)。 公共客户端（如本机应用和 JavaScript 应用）现在应该改为将授权代码流与 PKCE 扩展一同使用。 [参考](https://oauth.net/2/grant-types/implicit/)。

## <a name="device-code-provider"></a>设备代码提供程序

设备代码流允许通过其他设备登录设备。 有关详细信息，请参阅[Microsoft 标识平台 和 OAuth 2.0 设备代码流](/azure/active-directory/develop/v2-oauth2-device-code)。

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

// using Azure.Identity;
var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// Callback function that receives the user prompt
// Prompt contains the generated device code that use must
// enter during the auth process in the browser
Func<DeviceCodeInfo, CancellationToken, Task> callback = (code, cancellation) => {
    Console.WriteLine(code.Message);
    return Task.FromResult(0);
};

// https://docs.microsoft.com/dotnet/api/azure.identity.devicecodecredential
var deviceCodeCredential = new DeviceCodeCredential(
    callback, tenantId, clientId, options);

var graphClient = new GraphServiceClient(deviceCodeCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

```javascript
const {
    Client
} = require("@microsoft/microsoft-graph-client");
const {
    TokenCredentialAuthenticationProvider
} = require("@microsoft/microsoft-graph-client/authProviders/azureTokenCredentials");
const {
    DeviceCodeCredential
} = require("@azure/identity");

const credential = new DeviceCodeCredential(tenantId, clientId, clientSecret);
const authProvider = new TokenCredentialAuthenticationProvider(credential, {
    scopes: [scopes]
});

const client = Client.initWithMiddleware({
    debugLogging: true,
    authProvider
    // Use the authProvider object to create the class.
});
```

# <a name="java"></a>[Java](#tab/Java)

```java
final DeviceCodeCredential deviceCodeCredential = new DeviceCodeCredentialBuilder()
                    .clientId(clientId)
                    .challengeConsumer(challenge -> {
                        // lets user know of the challenge
                        System.out.println(challenge.getMessage());
                    })
                    .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, deviceCodeCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

不适用。

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

不适用。

# <a name="php"></a>[PHP](#tab/PHP)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://aka.ms/graphrequests)请求（如果这对你很重要）。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://aka.ms/graphrequests)请求（如果这对你很重要）。

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota/authentication/go/azure"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewDeviceCodeCredential(&azidentity.DeviceCodeCredentialOptions{
    ClientID: "CLIENT_ID",
    UserPrompt: func(ctx context.Context, message azidentity.DeviceCodeMessage) error {
        fmt.Println(message.Message)
        return nil
    },
})

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="integrated-windows-provider"></a>集成Windows提供程序

集成Windows流为计算机提供了一Windows加入域时以静默方式获取访问令牌的方法。 有关详细信息，请参阅集成Windows[身份验证](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)。

# <a name="c"></a>[C#](#tab/CS)

`Azure.Identity`程序包当前不支持Windows身份验证。 而是使用 MSAL 创建自定义身份验证提供程序。

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

var pca = PublicClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantId)
    .Build();

// DelegateAuthenticationProvider is a simple auth provider implementation
// that allows you to define an async function to retrieve a token
// Alternatively, you can create a class that implements IAuthenticationProvider
// for more complex scenarios
var authProvider = new DelegateAuthenticationProvider(async (request) => {
    // Use Microsoft.Identity.Client to retrieve token
    var result = await pca.AcquireTokenByIntegratedWindowsAuth(scopes).ExecuteAsync();

    request.Headers.Authorization =
        new System.Net.Http.Headers.AuthenticationHeaderValue("Bearer", result.AccessToken);
});

var graphClient = new GraphServiceClient(authProvider);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

不适用。

# <a name="java"></a>[Java](#tab/Java)

不适用。

# <a name="android"></a>[Android](#tab/Android)

不适用。

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

不适用。

# <a name="php"></a>[PHP](#tab/PHP)

不适用。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

不适用。

# <a name="go"></a>[转到](#tab/Go)

不适用。

---

## <a name="interactive-provider"></a>交互式提供程序

交互流由 Xamarin (UWP) 桌面应用程序使用，以用户Graph调用 Microsoft Graph。 有关详细信息，请参阅 [以交互方式获取令牌](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)。

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

// using Azure.Identity;
var options = new InteractiveBrowserCredentialOptions
{
    TenantId = tenantId,
    ClientId = clientId,
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud,
    // MUST be http://localhost or http://localhost:PORT
    // See https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/System-Browser-on-.Net-Core
    RedirectUri = new Uri("http://localhost"),
};

// https://docs.microsoft.com/dotnet/api/azure.identity.interactivebrowsercredential
var interactiveCredential = new InteractiveBrowserCredential(options);

var graphClient = new GraphServiceClient(interactiveCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://aka.ms/graphrequests)请求（如果这对你很重要）。

# <a name="java"></a>[Java](#tab/Java)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(clientId)
                .redirectUrl("http://localhost:8765")
                .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, interactiveBrowserCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(clientId)
                .redirectUrl("http://localhost:8765")
                .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, interactiveBrowserCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

```objectivec
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[PHP](#tab/PHP)

不适用。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

不适用。

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota/authentication/go/azure"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewInteractiveBrowserCredential(&azidentity.InteractiveBrowserCredentialOptions {
    TenantID: "TENANT_ID",
    ClientID: "CLIENT_ID",
    RedirectURL: "REDIRECT_URL",
})

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="usernamepassword-provider"></a>用户名/密码提供程序

用户名/密码提供程序允许应用程序使用用户的用户名和密码登录。 只有在不能使用任何其他 OAuth 流时，才使用此流。 有关详细信息，请参阅 Microsoft 标识平台[和 OAuth 2.0 资源所有者密码凭据](/azure/active-directory/develop/v2-oauth-ropc)

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

// using Azure.Identity;
var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

var userName = "adelev@contoso.com";
var password = "P@ssword1!";

// https://docs.microsoft.com/dotnet/api/azure.identity.usernamepasswordcredential
var userNamePasswordCredential = new UsernamePasswordCredential(
    userName, password, tenantId, clientId, options);

var graphClient = new GraphServiceClient(userNamePasswordCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://aka.ms/graphrequests)请求（如果这对你很重要）。

# <a name="java"></a>[Java](#tab/Java)

```java
final UsernamePasswordCredential usernamePasswordCredential = new UsernamePasswordCredentialBuilder()
        .clientId(clientId)
        .username(username)
        .password(password)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, usernamePasswordCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

不适用。

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

不适用。

# <a name="php"></a>[PHP](#tab/PHP)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://aka.ms/graphrequests)请求（如果这对你很重要）。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://aka.ms/graphrequests)请求（如果这对你很重要）。

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota/authentication/go/azure"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewUsernamePasswordCredential(
    "TENANT_ID",
    "CLIENT_ID",
    "USER_NAME",
    "PASSWORD",
    nil,
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="next-steps"></a>后续步骤

- 有关显示如何使用 Microsoft 标识平台 保护不同应用程序类型的代码示例，请参阅 Microsoft 标识平台[v2.0](/azure/active-directory/develop/sample-v2-code)终结点 (代码) 。
- 身份验证提供程序需要客户端 ID。 设置身份验证 [提供程序后](https://portal.azure.com/) ，需要注册应用程序。
- 通过投票或打开 Microsoft Graph请求，请告诉我们所需的 OAuth[流当前是否受支持](https://aka.ms/graphrequests)。
