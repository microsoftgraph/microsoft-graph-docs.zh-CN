---
title: 选择 Microsoft Graph身份验证提供程序
description: 了解如何为应用程序选择特定于方案的身份验证提供程序。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 0cdc407187ea0b5befc3704f877b1df11aeda545
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475533"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a>根据方案Graph Microsoft 身份验证提供程序

身份验证提供程序使用 MICROSOFT 身份验证库和 MSAL 身份验证库实现获取 (所需的) ;处理增量同意、密码过期和条件访问等情况下的一些潜在错误;，然后设置 HTTP 请求授权标头。 下表列出了一组与不同应用程序类型的方案匹配的 [提供程序](/azure/active-directory/develop/v2-app-types)。

|应用场景 | Flow/授予 | 受众 | 提供程序|
|--|--|--|--|
| [单页应用](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | 隐式 | 委派使用者/组织 |[隐式提供程序](#ImplicitProvider) |
| [调用 Web API 的 Web 应用](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | 授权代码 | 委派使用者/组织 | [授权代码提供程序](#AuthCodeProvider) |
| | 客户端凭据  | 仅限应用 | [客户端凭据提供程序](#ClientCredentialsProvider) |
| [调用 Web API 的 Web API](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | 代表 | 委派使用者/组织 | [代表提供商](#OnBehalfOfProvider) |
| | 客户端凭据  | 仅限应用 | [客户端凭据提供程序](#ClientCredentialsProvider) |
| [调用 Web API 的桌面应用](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | Interactive | 委派使用者/组织 | [交互式提供程序](#InteractiveProvider) |
| | 集成Windows | 委派组织 | [集成Windows提供程序](#IntegratedWindowsProvider) |
| | 资源所有者  | 委派组织 | [用户名/密码提供程序](#UsernamePasswordProvider) |
| | 设备代码  | 委派组织 | [设备代码提供程序](#DeviceCodeProvider) |
| [守护程序应用](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | 客户端凭据  | 仅限应用 | [客户端凭据提供程序](#ClientCredentialsProvider) |
| [调用 Web API 的移动应用](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | Interactive | 委派使用者/组织 | [交互式提供程序](#InteractiveProvider) |

> 注意Java和 android 开发人员需要添加 [azure-identity](/java/api/overview/azure/identity-readme?view=azure-java-stable) 库才能访问不同的凭据类型。

## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a>授权代码提供程序

授权代码流使本机和 Web 应用能够安全地获取用户名称中的令牌。 若要了解更多信息，请参阅[Microsoft 标识平台 和 OAuth 2.0 授权代码流](/azure/active-directory/develop/v2-oauth2-auth-code-flow)。

# <a name="c"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

授权代码、客户端凭据和代表 OAuth 流目前要求您实现自定义身份验证提供程序。 有关详细信息，请参阅 [使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。

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

尚不可用。 如果这对你很重要Graph支持或打开[Microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) Graph功能请求。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)请求（如果这对你很重要）。

---

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a>客户端凭据提供程序

客户端凭据流使服务应用程序无需用户交互即可运行。 访问基于应用程序的标识。 有关详细信息，请参阅 Microsoft 标识平台[和 OAuth 2.0 客户端凭据流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。

# <a name="c"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

授权代码、客户端凭据和代表 OAuth 流目前要求您实现自定义身份验证提供程序。 有关详细信息，请参阅 [使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。

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

尚不可用。 如果这对你很重要Graph支持或打开[Microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) Graph功能请求。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

尚不可用。 如果这对你很重要Graph支持或打开[Microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) Graph功能请求。

---

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a>代表提供程序

当应用程序调用服务/Web API 时，代表流适用，而服务/Web API 则调用 Microsoft Graph API。 有关详细信息，Microsoft 标识平台[OAuth 2.0 代表流](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="c"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

授权代码、客户端凭据和代表 OAuth 流目前要求您实现自定义身份验证提供程序。 有关详细信息 [，请参阅](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) 使用自定义验证提供程序。

# <a name="java"></a>[Java](#tab/Java)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)请求（如果这对你很重要）。

# <a name="android"></a>[Android](#tab/Android)

不适用。

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

不适用。

# <a name="php"></a>[PHP](#tab/PHP)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)请求（如果这对你很重要）。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)请求（如果这对你很重要）。

---

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a>隐式提供程序

隐式授予流用于基于浏览器的应用程序。 有关详细信息，请参阅Microsoft 标识平台[和隐式授予流](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)。

# <a name="c"></a>[C#](#tab/CS)

不适用。

# <a name="javascript"></a>[Javascript](#tab/Javascript)

```javascript
const clientId = "your_client_id"; // Client Id of the registered application
const callback = (errorDesc, token, error, tokenType) => {};
// An Optional options for initializing the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#configuration-options
const options = {
    redirectUri: "Your redirect URI",
};
const graphScopes = ["user.read", "mail.send"]; // An array of graph scopes

// Initialize the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#initialization-of-msal
const userAgentApplication = new Msal.UserAgentApplication(clientId, undefined, callback, options);
const authProvider = new MicrosoftGraph.ImplicitMSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

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

---

##  <a name="device-code-provider"></a><a name="DeviceCodeProvider"></a>设备代码提供程序

设备代码流允许通过另一台设备登录到设备。 有关详细信息，请参阅[Microsoft 标识平台 和 OAuth 2.0 设备代码流](/azure/active-directory/develop/v2-oauth2-device-code)。

# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)请求（如果这对你很重要）。

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

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)请求（如果这对你很重要）。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)请求（如果这对你很重要）。

---

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a>集成Windows提供程序

集成Windows流为计算机提供了一Windows加入域时以静默方式获取访问令牌的方法。 有关详细信息，请参阅集成Windows[身份验证](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)。

# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
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

---

##  <a name="interactive-provider"></a><a name="InteractiveProvider"></a>交互式提供程序

交互流由 Xamarin (UWP) 桌面应用程序使用，以用户Graph调用 Microsoft Graph。 有关详细信息，请参阅 [以交互方式获取令牌](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)。

# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)请求（如果这对你很重要）。

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

```objc
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

---

##  <a name="usernamepassword-provider"></a><a name="UsernamePasswordProvider"></a>用户名/密码提供程序

用户名/密码提供程序允许应用程序使用用户的用户名和密码登录。 只有在不能使用任何其他 OAuth 流时，才使用此流。 有关详细信息，请参阅 Microsoft 标识平台[和 OAuth 2.0 资源所有者密码凭据](/azure/active-directory/develop/v2-oauth-ropc)



# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

UsernamePasswordProvider authProvider = new UsernamePasswordProvider(publicClientApplication, scopes);

GraphServiceClient graphClient = new GraphServiceClient(authProvider);

User me = await graphClient.Me.Request()
                .WithUsernamePassword(email, password)
                .GetAsync();
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)请求（如果这对你很重要）。

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

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)请求（如果这对你很重要）。

# <a name="ruby"></a>[Ruby](#tab/Ruby)

尚不可用。 请投票支持或打开[Microsoft Graph功能](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)请求（如果这对你很重要）。

---

## <a name="next-steps"></a>后续步骤

* 有关显示如何使用 Microsoft 标识平台 保护不同应用程序类型的代码示例，请参阅 Microsoft 标识平台[v2.0 终结点 (代码) 。 ](/azure/active-directory/develop/sample-v2-code)
* 身份验证提供程序需要客户端 ID。 设置身份验证 [提供程序后](https://portal.azure.com/) ，需要注册应用程序。
* 通过投票或打开 Microsoft Graph请求，请告诉我们所需的 OAuth[流当前是否受支持](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)。
