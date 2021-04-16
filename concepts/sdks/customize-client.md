---
title: 自定义 Microsoft Graph SDK 服务客户端
description: 提供有关如何更改 Microsoft Graph SDK 服务客户端的默认行为的说明。
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: e666a9e976455f640d29edf2d460523935e53d97
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836855"
---
# <a name="customize-the-microsoft-graph-sdk-service-client"></a><span data-ttu-id="1f474-103">自定义 Microsoft Graph SDK 服务客户端</span><span class="sxs-lookup"><span data-stu-id="1f474-103">Customize the Microsoft Graph SDK service client</span></span>

<span data-ttu-id="1f474-104">Microsoft Graph SDK 客户端配置了一组默认的中间件，允许 SDK 与 Microsoft Graph 终结点进行通信。</span><span class="sxs-lookup"><span data-stu-id="1f474-104">The Microsoft Graph SDK client configures a default set of middleware that allows the SDK to communicate with the Microsoft Graph endpoints.</span></span> <span data-ttu-id="1f474-105">此默认集是可自定义的，允许您更改客户端的行为。</span><span class="sxs-lookup"><span data-stu-id="1f474-105">This default set is customizable, allowing you to change the behavior of the client.</span></span> <span data-ttu-id="1f474-106">例如，可以插入自定义日志记录，或添加测试处理程序以模拟特定方案。</span><span class="sxs-lookup"><span data-stu-id="1f474-106">For example, you can insert customized logging, or add a test handler to simulate specific scenarios.</span></span> <span data-ttu-id="1f474-107">可以添加和删除中间件组件。</span><span class="sxs-lookup"><span data-stu-id="1f474-107">You can add and remove middleware components.</span></span> <span data-ttu-id="1f474-108">需要注意的是，中间件组件的运行顺序非常重要。</span><span class="sxs-lookup"><span data-stu-id="1f474-108">It is important to note that the order in which middleware components run is significant.</span></span>

## <a name="c"></a>[<span data-ttu-id="1f474-109">C#</span><span class="sxs-lookup"><span data-stu-id="1f474-109">C#</span></span>](#tab/csharp)

```csharp
var handlers = GraphClientFactory.CreateDefaultHandlers(authProvider);

// Remove a default handler
var compressionHandler =
    handlers.Where(h => h is CompressionHandler).FirstOrDefault();
handlers.Remove(compressionHandler);

// Add a new one
// ChaosHandler simulates random server failures
handlers.Add(new ChaosHandler());

var httpClient = GraphClientFactory.Create(handlers);

var customGraphClient = new GraphServiceClient(httpClient);

var messages = await customGraphClient.Me.Messages.Request()
    .Top(100)
    .Select(m => m.Subject)
    .GetAsync();
```

## <a name="typescript"></a>[<span data-ttu-id="1f474-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="1f474-110">TypeScript</span></span>](#tab/typeScript)

```typescript
// Create a custom auth provider
let authProvider = new SimpleAuthProvider(accessToken);
// Create an authentication handler that uses custom auth provider
let authHandler = new MicrosoftGraph.AuthenticationHandler(authProvider);

// Create a custom logging handler
let loggingHandler = new CustomLoggingHandler();

// Create a standard HTTP message handler
let httpHandler = new MicrosoftGraph.HTTPMessageHandler();

// Use setNext to chain handlers together
// auth -> logging -> http
authHandler.setNext(loggingHandler);
loggingHandler.setNext(httpHandler);

// Pass the first middleware in the chain in the middleWare property
const client = MicrosoftGraph.Client.initWithMiddleware({
  defaultVersion: 'v1.0',
  debugLogging: true,
  middleware: authHandler,
});

let response: PageCollection = await client
  .api('/me/messages?$top=10&$select=sender,subject')
  .get();
```

### <a name="simpleauthproviderts"></a><span data-ttu-id="1f474-111">SimpleAuthProvider.ts</span><span class="sxs-lookup"><span data-stu-id="1f474-111">SimpleAuthProvider.ts</span></span>

```typescript
import { AuthenticationProvider } from "@microsoft/microsoft-graph-client";

export default class SimpleAuthProvider implements AuthenticationProvider {
  private accessToken: string;

  constructor(accessToken: string) {
    this.accessToken = accessToken;
  }

  getAccessToken = async (): Promise<string> => {
    return this.accessToken;
  }
}
```

### <a name="customlogginghandlerts"></a><span data-ttu-id="1f474-112">CustomLoggingHandler.ts</span><span class="sxs-lookup"><span data-stu-id="1f474-112">CustomLoggingHandler.ts</span></span>

```typescript
import { Context, Middleware } from "@microsoft/microsoft-graph-client";

export default class CustomLoggingHandler implements Middleware {
  private nextMiddleware: any = null;

  execute = async (context: Context): Promise<void> => {
    console.log(`Logging request: ${context.request.toString()}`);
    return await this.nextMiddleware.execute(context);
  }
  setNext = (middleware: Middleware): void => {
    this.nextMiddleware = middleware;
  }
}
```

## <a name="java"></a>[<span data-ttu-id="1f474-113">Java</span><span class="sxs-lookup"><span data-stu-id="1f474-113">Java</span></span>](#tab/java)

```java
// you can configure any OkHttpClient option and add interceptors
// Note: com.microsoft.graph:microsoft-graph:3.0 or above is required
// for a complete description of available configuration options https://square.github.io/okhttp/4.x/okhttp/okhttp3/-ok-http-client/-builder/
final OkHttpClient httpClient = HttpClients.createDefault(authenticationProvider)
                                .newBuilder()
                                .followSslRedirects(false) // sample configuration to apply to client
                                .build();

final GraphServiceClient graphServiceClient = GraphServiceClient
                .builder()
                .httpClient(httpClient)
                .buildClient();
```

---
