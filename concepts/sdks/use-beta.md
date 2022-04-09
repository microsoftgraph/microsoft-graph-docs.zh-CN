---
title: 将 Microsoft Graph SDK 与 beta API 配合使用
description: 介绍如何将 Microsoft Graph SDK 与 aPI 的 beta 版本配合使用。
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: aee313a4f4e5eb9efd68c9fd0877dcc96722633c
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733190"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>将 Microsoft Graph SDK 与 beta API 配合使用

默认情况下，许多 Microsoft Graph SDK 使用 [v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) Microsoft Graph终结点。 SDK 可用于非生产应用程序的 [beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true) 终结点。 访问 beta 终结点的方法取决于使用的 SDK。

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD025 -->
# <a name="c"></a>[C#](#tab/CS)

若要调用 beta API，必须安装 [Microsoft.Graph。Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) 包。 使用情况与包相同 `Microsoft.Graph` 。

```csharp
using Microsoft.Graph;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[TypeScript](#tab/typeScript)

[Microsoft Graph JavaScript 客户端库](https://github.com/microsoftgraph/msgraph-sdk-javascript)可以通过两种方式之一调用 beta API。

- 可以在创建版本 `MicrosoftGraph.Client` 时对其进行设置。 客户端发出的所有请求都将转到指定的版本。

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- 可以使用 `version` 对象上的函数在特定请求上 `GraphRequest` 设置版本。

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[Java](#tab/Java)

若要调用 beta API，必须安装 [Microsoft Graph Beta Java SDK](https://github.com/microsoftgraph/msgraph-beta-sdk-java)。 使用情况与非 beta SDK 相同。

```Java
GraphServiceClient graphClient = GraphServiceClient
    .builder()
    .authenticationProvider(authProvider)
    .buildClient();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

[Microsoft Graph SDK for ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) 要求你生成要调用的 API 的 URL 字符串。 它为 v1.0 终结点提供常 `MSGraphBaseURL` 量。 若要使用 beta，只需将其替换为 `https://graph.microsoft.com/beta`。

但是，[Microsoft Graph Models SDK 中的模型](https://github.com/microsoftgraph/msgraph-sdk-objc-models)是从 v1.0 API 中的对象生成的，因此它们可能不适用于 beta 对象。

```objectivec
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[PHP](#tab/PHP)

[Microsoft Graph SDK for PHP](https://github.com/microsoftgraph/msgraph-sdk-php) 支持 beta 终结点和模型。 使用该方法设置 beta 终结点 `setApiVersion` 。 需要通过提供别名来消除 v1.0 和 beta 模型的歧义。

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

# <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

若要调用 beta API，必须安装 [Microsoft Graph Beta SDK for Go](https://github.com/microsoftgraph/msgraph-beta-sdk-go) 包。

```go
import (
    msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
    a "github.com/microsoft/kiota-authentication-azure-go"
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(...)

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)
```

---
