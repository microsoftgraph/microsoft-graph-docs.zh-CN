---
title: 创建 Microsoft Graph 客户端
description: 说明如何创建客户端，以使用客户端呼叫 Microsoft Graph。 包含如何设置身份验证和选择主权云。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 0256ad20b3078c081102221189a12e27432df058
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971358"
---
# <a name="create-a-microsoft-graph-client"></a><span data-ttu-id="1ed52-104">创建 Microsoft Graph 客户端</span><span class="sxs-lookup"><span data-stu-id="1ed52-104">Create a Microsoft Graph client</span></span>

<span data-ttu-id="1ed52-105">Microsoft Graph 客户端用于简化呼叫 Microsoft Graph 的操作。</span><span class="sxs-lookup"><span data-stu-id="1ed52-105">The Microsoft Graph client is designed to make it simple to make calls to Microsoft Graph.</span></span> <span data-ttu-id="1ed52-106">应用程序的生命周期内，仅需使用一个客户端实例。</span><span class="sxs-lookup"><span data-stu-id="1ed52-106">You can use a single client instance for the lifetime of the application.</span></span> <span data-ttu-id="1ed52-107">有关如何添加和安装 Microsoft Graph 客户端程序包到项目中的信息，请参阅 [安装 SDK](sdk-installation.md)。</span><span class="sxs-lookup"><span data-stu-id="1ed52-107">For information about how to add and install the Microsoft Graph client package into your project, see  [Install the SDK](sdk-installation.md).</span></span>

<span data-ttu-id="1ed52-108">以下代码示例说明了如何通过身份验证认证器以支持语言创建 Microsoft Graph 客户端示例。</span><span class="sxs-lookup"><span data-stu-id="1ed52-108">The following code examples show how to create an instance of a Microsoft Graph client with an authentication provider in the supported languages.</span></span> <span data-ttu-id="1ed52-109">身份验证认证器将负责获取应用程序的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="1ed52-109">The authentication provider will handle acquiring access tokens for the application.</span></span> <span data-ttu-id="1ed52-110">每种语言和平台都有多个不同的身份验证认证器可用。</span><span class="sxs-lookup"><span data-stu-id="1ed52-110">Many different authentication providers are available for each language and platform.</span></span> <span data-ttu-id="1ed52-111">不同的身份验证认证器支持不同的客户端场景。</span><span class="sxs-lookup"><span data-stu-id="1ed52-111">The different application providers support different client scenarios.</span></span> <span data-ttu-id="1ed52-112">有关认证器和选项适用场景的详细信息，请参阅 [选择身份验证认证器](choose-authentication-providers.md)。</span><span class="sxs-lookup"><span data-stu-id="1ed52-112">For details about which provider and options are appropriate for your scenario, see [Choose an Authentication Provider](choose-authentication-providers.md).</span></span>

# <a name="c"></a>[<span data-ttu-id="1ed52-113">C#</span><span class="sxs-lookup"><span data-stu-id="1ed52-113">C#</span></span>](#tab/CS)

```csharp
// Build a client application.
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create("INSERT-CLIENT-APP-ID")
            .Build();
// Create an authentication provider by passing in a client application and graph scopes.
DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, graphScopes);
// Create a new instance of GraphServiceClient with the authentication provider.
GraphServiceClient graphClient = new GraphServiceClient(authProvider);
```

# <a name="javascript"></a>[<span data-ttu-id="1ed52-114">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ed52-114">Javascript</span></span>](#tab/Javascript)

```javascript
const clientId = "INSERT-CLIENT-APP-ID"; // Client Id of the registered application

/**
* Create an authProvider to authenticate againt the Microsoft Graph API.
* You can use the TokenCredentialAuthenticationProvider instance with @azure/identity library or
* you can authentication using any MSAL auth library with a custom authentication provider.
*/
const credential = new ClientSecretCredential(tenantId, clientId, clientSecret);
const authProvider = new TokenCredentialAuthenticationProvider(credential, { scopes: [scopes] });
const client = Client.initWithMiddleware({
    debugLogging: true,
    authProvider,
});
```

# <a name="java"></a>[<span data-ttu-id="1ed52-115">Java</span><span class="sxs-lookup"><span data-stu-id="1ed52-115">Java</span></span>](#tab/Java)

```java
final ClientSecretCredential clientSecretCredential = new ClientSecretCredentialBuilder()
        .clientId(CLIENT_ID)
        .clientSecret(CLIENT_SECRET)
        .tenantId(TENANT_GUID)
        .build();

final TokenCredentialAuthProvider tokenCredAuthProvider = new TokenCredentialAuthProvider(SCOPES, clientSecretCredential);

final GraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(tokenCredAuthProvider)
                .buildClient();
```

# <a name="android"></a>[<span data-ttu-id="1ed52-116">Android</span><span class="sxs-lookup"><span data-stu-id="1ed52-116">Android</span></span>](#tab/Android)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(CLIENT_ID)
                .redirectUrl("http://localhost:8765")
                .build();

final TokenCredentialAuthProvider tokenCredAuthProvider = new TokenCredentialAuthProvider(SCOPES, interactiveBrowserCredential);

GraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(tokenCredAuthProvider)
                .buildClient();
```

# <a name="objective-c"></a>[<span data-ttu-id="1ed52-117">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ed52-117">Objective-C</span></span>](#tab/Objective-C)

```objc
// Create the authenticationProvider.
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];
MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];
 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];

// Create the client with the authenticationProvider and create a request to the /me resource.
MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me"]]];

// Create the task to send the request and handle the response.
MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest
    completionHandler:^(NSData *data, NSURLResponse *response, NSError *error) {

    //Do something

    }];

[meDataTask execute];
```

# <a name="php"></a>[<span data-ttu-id="1ed52-118">PHP</span><span class="sxs-lookup"><span data-stu-id="1ed52-118">PHP</span></span>](#tab/PHP)

```php
// PHP client currently doesn't have an authentication provider. You will need to handle
// getting an access token. The following example demonstrates the client credential
// OAuth flow and assumes that an administrator has consented to the application.
$guzzle = new \GuzzleHttp\Client();
$url = 'https://login.microsoftonline.com/' . $tenantId . '/oauth2/token?api-version=1.0';
$token = json_decode($guzzle->post($url, [
    'form_params' => [
        'client_id' => $clientId,
        'client_secret' => $clientSecret,
        'resource' => 'https://graph.microsoft.com/',
        'grant_type' => 'client_credentials',
    ],
])->getBody()->getContents());
$accessToken = $token->access_token;

// Create a new Graph client.
$graph = new Graph();
$graph->setAccessToken($accessToken);

// Make a call to /me Graph resource.
$user = $graph->createRequest("GET", "/me")
                ->setReturnType(Model\User::class)
                ->execute();
```
---
