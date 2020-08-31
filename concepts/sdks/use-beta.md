---
title: 将 Microsoft Graph Sdk 与 beta API 结合使用
description: 介绍如何将 Microsoft Graph Sdk 与 API 的 beta 版本一起使用。
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: a384384b4172a835160cf12b8e1fb0c06edc7fe7
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312193"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>将 Microsoft Graph Sdk 与 beta API 结合使用

默认情况下，Microsoft Graph Sdk 使用 [1.0](/graph/api/overview?view=graph-rest-1.0) 版 microsoft Graph 终结点。 Sdk 可用于非生产应用程序的 [beta](/graph/api/overview?view=graph-rest-beta) 终结点。 访问 beta 终结点的方法取决于所使用的 SDK。

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[C#](#tab/CS)

若要调用 beta API，您必须安装 " [Microsoft. Graph](https://www.nuget.org/packages/Microsoft.Graph.Beta) " 程序包。 用法与 `Microsoft.Graph` 包相同。

```csharp
using Microsoft.Graph.Beta;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

## <a name="typescript"></a>[TypeScript](#tab/typeScript)

[Microsoft Graph JavaScript 客户端库](https://github.com/microsoftgraph/msgraph-sdk-javascript)可以通过以下两种方式之一调用 beta API。

- 您可以在创建版本时对 `MicrosoftGraph.Client` 其进行设置。 客户端发出的所有请求都将转到指定的版本。

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- 您可以通过使用对象上的函数来设置特定请求的版本 `version` `GraphRequest` 。

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[Java](#tab/Java)

为了调用 beta API，您必须安装 [Microsoft Graph Beta JAVA SDK](https://github.com/microsoftgraph/msgraph-beta-sdk-java)。 使用与非 beta SDK 相同。

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

[Microsoft GRAPH SDK For ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc)要求您构建指向要调用的 API 的 URL 字符串。 它 `MSGraphBaseURL` 为1.0 终结点提供常量。 若要使用 beta，只需将其替换为 `https://graph.microsoft.com/beta` 。

但是， [Microsoft Graph 模型 SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) 中的模型是从 v1.0 API 中的对象生成的，因此它们可能不会与 beta 对象一起使用。

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

---
