---
title: 选择 Microsoft Graph 身份验证提供程序
description: 了解如何为您的应用程序选择特定于方案的身份验证提供程序。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 5061b38249f31a6eea959ecec94899337bf57326
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630193"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-oauth-flow"></a>根据 OAuth 流选择 Microsoft Graph 身份验证提供程序

身份验证提供程序通过抽象身份验证客户端库所需的参数简化了获取访问令牌的方法。 Microsoft Graph 身份验证提供程序通过为每个平台提供适配器简化了 Microsoft 身份验证库 (MSAL) 的使用。 这些适配器处理应用程序的令牌获取。 Microsoft Graph 身份验证提供程序映射到 OAuth 授予流。 您需要知道要用于应用程序的 OAuth 授予流, 以便为您的应用程序选择适当的身份验证提供程序。

## <a name="authorization-code-oauth-flow"></a>授权代码 OAuth 流

授权代码流使本机应用程序和 web 应用能够安全地获取用户名称中的令牌。 若要了解详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 授权代码流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow)。

# <a name="ctabcs"></a>[语言](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = AuthorizationCodeProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。 有关详细信息, 请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

不适用。

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/Objective-C)

不适用。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

尚不可用。 如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

---

## <a name="client-credential-oauth-flow"></a>客户端凭据 OAuth 流

客户端凭据流使服务应用程序可以在没有用户交互的情况下运行。 访问基于应用程序的标识。 有关详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 客户端凭据流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。

# <a name="ctabcs"></a>[语言](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = ClientCredentialProvider.CreateClientApplication(clientId, clientCredential);
ClientCredentialProvider authProvider = new ClientCredentialProvider(clientApplication);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。 有关详细信息, 请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

不适用。

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/Objective-C)

不适用。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

尚不可用。 如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

尚不可用。 如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

---

## <a name="on-behalf-of-oauth-flow"></a>代表 OAuth 流

当应用程序调用在其中打开 Microsoft Graph API 的服务/web API 时, 代表流是适用的。 若要了解详细信息, 请阅读[Microsoft identity platform 和 OAuth 2.0 代表流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="ctabcs"></a>[语言](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = OnBehalfOfProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
OnBehalfOfProvider authProvider = new OnBehalfOfProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。 有关详细信息, 请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。

# <a name="javatabjava"></a>[Java](#tab/Java)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

# <a name="androidtabandroid"></a>[Android](#tab/Android)

不适用。

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/Objective-C)

不适用。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

---

## <a name="implicit-grant-oauth-flow"></a>隐式授予 OAuth 流

隐式授予流在基于浏览器的应用程序中使用。 有关详细信息, 请参阅[Microsoft identity platform 和隐式授予流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)。

# <a name="ctabcs"></a>[语言](#tab/CS)

不适用。

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

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
const authProvider = new MicrosoftGraph.MSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

# <a name="javatabjava"></a>[Java](#tab/Java)

不适用。

# <a name="androidtabandroid"></a>[Android](#tab/Android)

不适用。

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/Objective-C)

不适用。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

不适用。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

不适用。

---

## <a name="device-code-oauth-flow"></a>设备代码 OAuth 流

设备代码流允许通过其他设备登录设备。 有关详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 设备代码流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code)。

# <a name="ctabcs"></a>[语言](#tab/CS)

```csharp
IPublicClientApplication clientApplication = DeviceCodeProvider.CreateClientApplication(clientId);
DeviceCodeProvider authProvider = new DeviceCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

# <a name="javatabjava"></a>[Java](#tab/Java)

尚不可用。 如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

# <a name="androidtabandroid"></a>[Android](#tab/Android)

不适用。

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/Objective-C)

不适用。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

---

## <a name="integrated-windows-flow"></a>集成的 Windows 流

集成的 Windows 流为 Windows 计算机提供了一种在加入域时无提示地获取访问令牌的方法。 有关详细信息, 请参阅[集成 Windows 身份验证](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)。

# <a name="ctabcs"></a>[语言](#tab/CS)

```csharp
IPublicClientApplication clientApplication = IntegratedWindowsAuthenticationProvider.CreateClientApplication(clientId);
IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

不适用。

# <a name="javatabjava"></a>[Java](#tab/Java)

不适用。

# <a name="androidtabandroid"></a>[Android](#tab/Android)

不适用。

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/Objective-C)

不适用。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

不适用。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

不适用。

---

## <a name="interactive-flow"></a>交互流

移动应用程序 (Xamarin 和 UWP) 和桌面应用程序使用交互流, 以在用户的名称中调用 Microsoft Graph。 有关详细信息, 请参阅[以交互方式获取令牌](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)。

# <a name="ctabcs"></a>[语言](#tab/CS)

```csharp
IPublicClientApplication clientApplication = InteractiveAuthenticationProvider.CreateClientApplication(clientId);
InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

# <a name="javatabjava"></a>[Java](#tab/Java)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

# <a name="androidtabandroid"></a>[Android](#tab/Android)

```java
PublicClientApplication publicClientApplication = new PublicClientApplication(getApplicationContext(), "CLIENT_ID_OF_YOUR_APPLICATION");
MSALAuthenticationProvider msalAuthenticationProvider = new MSALAuthenticationProvider(
    getActivity(),
    getApplication(),
    publicClientApplication,
    scopes);

IGraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(msalAuthenticationProvider)
    .buildClient();
```

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[PHP](#tab/PHP)

不适用。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

不适用。

---

## <a name="resource-owner-password-credential-grant-oauth-flow"></a>资源所有者密码凭据授予 OAuth 流

资源所有者密码凭据流允许应用程序使用用户名和密码登录用户。 仅当您不能使用任何其他 OAuth 流时, 才使用此流。 有关详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 资源所有者密码凭据](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)



# <a name="ctabcs"></a>[语言](#tab/CS)

```csharp
IPublicClientApplication clientApplication = UsernamePasswordProvider.CreateClientApplication(clientId);
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

不适用。

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/Objective-C)

不适用。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

尚不可用。 如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。

---

## <a name="next-steps"></a>后续步骤

* 身份验证提供程序需要客户端 ID。 设置身份验证提供程序后, 需要[注册应用程序](https://portal.azure.com/)。
* 如果[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)目前不支持所需的 OAuth 流, 请告知我们。