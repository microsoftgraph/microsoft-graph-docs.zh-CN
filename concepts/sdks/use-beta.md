---
title: 将 Microsoft Graph SDK 与 beta API 一同使用
description: 介绍如何将 Microsoft Graph SDK 与 API 的 beta 版本一同使用。
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 4d984cd9c236b1fb2785cd998dd69fb998cd137e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941356"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a><span data-ttu-id="74ad8-103">将 Microsoft Graph SDK 与 beta API 一同使用</span><span class="sxs-lookup"><span data-stu-id="74ad8-103">Use the Microsoft Graph SDKs with the beta API</span></span>

<span data-ttu-id="74ad8-104">默认情况下，许多 Microsoft Graph SDK 使用 [v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) Microsoft Graph 终结点。</span><span class="sxs-lookup"><span data-stu-id="74ad8-104">Many of the Microsoft Graph SDKs use the [v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) Microsoft Graph endpoint by default.</span></span> <span data-ttu-id="74ad8-105">SDK 可用于非生产应用程序的 [beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true) 终结点。</span><span class="sxs-lookup"><span data-stu-id="74ad8-105">The SDKs can be used with the [beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true) endpoint for non-production applications.</span></span> <span data-ttu-id="74ad8-106">用于访问 beta 终结点的方法取决于您使用的 SDK。</span><span class="sxs-lookup"><span data-stu-id="74ad8-106">The method for accessing the beta endpoint depends on which SDK you are using.</span></span>

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[<span data-ttu-id="74ad8-107">C#</span><span class="sxs-lookup"><span data-stu-id="74ad8-107">C#</span></span>](#tab/CS)

<span data-ttu-id="74ad8-108">若要调用 beta API，必须安装 [Microsoft.Graph.Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) 程序包。</span><span class="sxs-lookup"><span data-stu-id="74ad8-108">In order to call the beta API, you must install the [Microsoft.Graph.Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) package.</span></span> <span data-ttu-id="74ad8-109">用法与程序包 `Microsoft.Graph` 相同。</span><span class="sxs-lookup"><span data-stu-id="74ad8-109">Usage is the same as the `Microsoft.Graph` package.</span></span>

```csharp
using Microsoft.Graph;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[<span data-ttu-id="74ad8-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="74ad8-110">TypeScript</span></span>](#tab/typeScript)

<span data-ttu-id="74ad8-111">[Microsoft Graph JavaScript 客户端库](https://github.com/microsoftgraph/msgraph-sdk-javascript)可以通过以下两种方法之一调用 beta API。</span><span class="sxs-lookup"><span data-stu-id="74ad8-111">The [Microsoft Graph JavaScript Client Library](https://github.com/microsoftgraph/msgraph-sdk-javascript) can call the beta API in one of two ways.</span></span>

- <span data-ttu-id="74ad8-112">可以在 创建版本 `MicrosoftGraph.Client` 时在 上设置版本。</span><span class="sxs-lookup"><span data-stu-id="74ad8-112">You can set the version on the `MicrosoftGraph.Client` when you create it.</span></span> <span data-ttu-id="74ad8-113">客户端提出的所有请求都将转到指定的版本。</span><span class="sxs-lookup"><span data-stu-id="74ad8-113">All requests made by the client will go to the specified version.</span></span>

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- <span data-ttu-id="74ad8-114">可以通过使用 对象上的 函数来设置特定 `version` 请求 `GraphRequest` 的版本。</span><span class="sxs-lookup"><span data-stu-id="74ad8-114">You can set the version on a specific request by using the `version` function on the `GraphRequest` object.</span></span>

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[<span data-ttu-id="74ad8-115">Java</span><span class="sxs-lookup"><span data-stu-id="74ad8-115">Java</span></span>](#tab/Java)

<span data-ttu-id="74ad8-116">若要调用 beta API，必须安装 Microsoft [Graph Beta Java SDK。](https://github.com/microsoftgraph/msgraph-beta-sdk-java)</span><span class="sxs-lookup"><span data-stu-id="74ad8-116">In order to call the beta API, you must install the [Microsoft Graph Beta Java SDK](https://github.com/microsoftgraph/msgraph-beta-sdk-java).</span></span> <span data-ttu-id="74ad8-117">用法与非 beta SDK 相同。</span><span class="sxs-lookup"><span data-stu-id="74ad8-117">Usage is the same as the non-beta SDK.</span></span>

```Java
GraphServiceClient graphClient = GraphServiceClient
    .builder()
    .authenticationProvider(authProvider)
    .buildClient();
```

# <a name="objective-c"></a>[<span data-ttu-id="74ad8-118">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74ad8-118">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="74ad8-119">适用于 [ObjC 的 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-objc) 需要你生成要调用的 API 的 URL 字符串。</span><span class="sxs-lookup"><span data-stu-id="74ad8-119">The [Microsoft Graph SDK for ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) requires you to build a URL string to the API you want to call.</span></span> <span data-ttu-id="74ad8-120">它为 `MSGraphBaseURL` v1.0 终结点提供一个常量。</span><span class="sxs-lookup"><span data-stu-id="74ad8-120">It provides a constant `MSGraphBaseURL` for the v1.0 endpoint.</span></span> <span data-ttu-id="74ad8-121">若要使用 beta 版本，只需将其替换为 `https://graph.microsoft.com/beta` 。</span><span class="sxs-lookup"><span data-stu-id="74ad8-121">To use beta, you simply replace that with `https://graph.microsoft.com/beta`.</span></span>

<span data-ttu-id="74ad8-122">但是 [，Microsoft Graph 模型 SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) 中的模型是通过 v1.0 API 中的对象生成的，因此它们可能无法使用 beta 对象。</span><span class="sxs-lookup"><span data-stu-id="74ad8-122">However, the models in the [Microsoft Graph Models SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) are generated from objects in the v1.0 API, so they may not work with beta objects.</span></span>

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[<span data-ttu-id="74ad8-123">PHP</span><span class="sxs-lookup"><span data-stu-id="74ad8-123">PHP</span></span>](#tab/PHP)

<span data-ttu-id="74ad8-124">适用于 [PHP 的 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-php) 支持 beta 终结点和模型。</span><span class="sxs-lookup"><span data-stu-id="74ad8-124">The [Microsoft Graph SDK for PHP](https://github.com/microsoftgraph/msgraph-sdk-php) supports the beta endpoint and models.</span></span> <span data-ttu-id="74ad8-125">使用 方法设置 beta `setApiVersion` 终结点。</span><span class="sxs-lookup"><span data-stu-id="74ad8-125">You set the beta endpoint with the `setApiVersion` method.</span></span> <span data-ttu-id="74ad8-126">你需要通过提供别名来对 v1.0 和 beta 模型进行分色。</span><span class="sxs-lookup"><span data-stu-id="74ad8-126">You will need to disambiguate the v1.0 and beta models by providing an alias.</span></span>

```php
use Microsoft\Graph\Graph;
use Beta\Microsoft\Graph\Model as BetaModel;

class UseBeta
{
    public function run()
    {
        $accessToken = 'xxx';

        $graph = new Graph();
        $graph->setAccessToken($accessToken);

        $user = $graph->setApiVersion("beta")
                      ->createRequest("GET", "/me")
                      ->setReturnType(BetaModel\User::class)
                      ->execute();

        echo "Hello, I am $user->getGivenName() ";
    }
}
```

---
