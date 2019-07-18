---
title: 创建 Microsoft Graph 客户端
description: 介绍如何创建用于调用 Microsoft Graph 的客户端。 包含如何设置身份验证和选择 sovereign 云。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: cfff3b8f19b27e360977259d06df730abfd38bf3
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778731"
---
# <a name="create-a-microsoft-graph-client"></a><span data-ttu-id="31332-104">创建 Microsoft Graph 客户端</span><span class="sxs-lookup"><span data-stu-id="31332-104">Create a Microsoft Graph client</span></span>

<span data-ttu-id="31332-105">Microsoft Graph 客户端旨在使调用 Microsoft Graph 更加简单。</span><span class="sxs-lookup"><span data-stu-id="31332-105">The Microsoft Graph client is designed to make it simple to make calls to Microsoft Graph.</span></span> <span data-ttu-id="31332-106">您可以在应用程序的生存期中使用单个客户端实例。</span><span class="sxs-lookup"><span data-stu-id="31332-106">You can use a single client instance for the lifetime of the application.</span></span> <span data-ttu-id="31332-107">有关如何将 Microsoft Graph 客户端包添加并安装到项目中的信息, 请参阅[install THE SDK](sdk-installation.md)。</span><span class="sxs-lookup"><span data-stu-id="31332-107">For information about how to add and install the Microsoft Graph client package into your project, see  [Install the SDK](sdk-installation.md).</span></span>

<span data-ttu-id="31332-108">下面的代码示例演示如何使用支持的语言创建具有身份验证提供程序的 Microsoft Graph 客户端的实例。</span><span class="sxs-lookup"><span data-stu-id="31332-108">The following code examples show how to create an instance of a Microsoft Graph client with an authentication provider in the supported languages.</span></span> <span data-ttu-id="31332-109">身份验证提供程序将处理获取应用程序的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="31332-109">The authentication provider will handle acquiring access tokens for the application.</span></span> <span data-ttu-id="31332-110">每种语言和平台都提供了许多不同的身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="31332-110">Many different authentication providers are available for each language and platform.</span></span> <span data-ttu-id="31332-111">不同的应用程序提供程序支持不同的客户端方案。</span><span class="sxs-lookup"><span data-stu-id="31332-111">The different application providers support different client scenarios.</span></span> <span data-ttu-id="31332-112">有关适合您的方案的提供程序和选项的详细信息, 请参阅[选择身份验证提供程序](choose-authentication-providers.md)。</span><span class="sxs-lookup"><span data-stu-id="31332-112">For details about which provider and options are appropriate for your scenario, see [Choose an Authentication Provider](choose-authentication-providers.md).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="31332-113">C#</span><span class="sxs-lookup"><span data-stu-id="31332-113">C#</span></span>](#tab/CS)

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

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="31332-114">Javascript</span><span class="sxs-lookup"><span data-stu-id="31332-114">Javascript</span></span>](#tab/Javascript)

```javascript
const clientId = "INSERT-CLIENT-APP-ID"; // Client Id of the registered application
const callback = (errorDesc, token, error, tokenType) => {};
// An Optional options for initializing the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#configuration-options
const options = {
    redirectUri: "Your redirect URI",
};
const graphScopes = ["user.read", "mail.send"]; // An array of graph scopes

// Initialize the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#initialization-of-msal
const userAgentApplication = new UserAgentApplication(clientId, undefined, callback, options);
const authProvider = new MSALAuthenticationProvider(userAgentApplication, graphScopes );
```

# <a name="javatabjava"></a>[<span data-ttu-id="31332-115">Java</span><span class="sxs-lookup"><span data-stu-id="31332-115">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(CLIENT_ID, SCOPES, CLIENT_SECRET, TENANT_GUID, NATIONAL_CLOUD);

IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="31332-116">Android</span><span class="sxs-lookup"><span data-stu-id="31332-116">Android</span></span>](#tab/Android)

```java
PublicClientApplication publicClientApplication = new PublicClientApplication(getApplicationContext(), "INSERT-CLIENT-APP-ID");

MSALAuthenticationProvider msalAuthenticationProvider = new MSALAuthenticationProvider(
    getActivity(),
    getApplication(),
    publicClientApplication,
    scopes);

IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="31332-117">目标-C</span><span class="sxs-lookup"><span data-stu-id="31332-117">Objective-C</span></span>](#tab/Objective-C)

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

# <a name="phptabphp"></a>[<span data-ttu-id="31332-118">PHP</span><span class="sxs-lookup"><span data-stu-id="31332-118">PHP</span></span>](#tab/PHP)

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
