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
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>将 Microsoft Graph SDK 与 beta API 一同使用

默认情况下，许多 Microsoft Graph SDK 使用 [v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) Microsoft Graph 终结点。 SDK 可用于非生产应用程序的 [beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true) 终结点。 用于访问 beta 终结点的方法取决于您使用的 SDK。

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[C#](#tab/CS)

若要调用 beta API，必须安装 [Microsoft.Graph.Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) 程序包。 用法与程序包 `Microsoft.Graph` 相同。

```csharp
using Microsoft.Graph;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[TypeScript](#tab/typeScript)

[Microsoft Graph JavaScript 客户端库](https://github.com/microsoftgraph/msgraph-sdk-javascript)可以通过以下两种方法之一调用 beta API。

- 可以在 创建版本 `MicrosoftGraph.Client` 时在 上设置版本。 客户端提出的所有请求都将转到指定的版本。

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- 可以通过使用 对象上的 函数来设置特定 `version` 请求 `GraphRequest` 的版本。

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[Java](#tab/Java)

若要调用 beta API，必须安装 Microsoft [Graph Beta Java SDK。](https://github.com/microsoftgraph/msgraph-beta-sdk-java) 用法与非 beta SDK 相同。

```Java
GraphServiceClient graphClient = GraphServiceClient
    .builder()
    .authenticationProvider(authProvider)
    .buildClient();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

适用于 [ObjC 的 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-objc) 需要你生成要调用的 API 的 URL 字符串。 它为 `MSGraphBaseURL` v1.0 终结点提供一个常量。 若要使用 beta 版本，只需将其替换为 `https://graph.microsoft.com/beta` 。

但是 [，Microsoft Graph 模型 SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) 中的模型是通过 v1.0 API 中的对象生成的，因此它们可能无法使用 beta 对象。

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[PHP](#tab/PHP)

适用于 [PHP 的 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-php) 支持 beta 终结点和模型。 使用 方法设置 beta `setApiVersion` 终结点。 你需要通过提供别名来对 v1.0 和 beta 模型进行分色。

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
