---
title: 自定义 Microsoft Graph SDK 服务客户端
description: 提供有关如何更改 Microsoft Graph SDK 服务客户端的默认行为的说明。
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 67e0fbc00d1c2760d1d6f226213447fe88a70670
ms.sourcegitcommit: df2c52f84aae5d4fed641d7411ba547371f0eaad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2020
ms.locfileid: "44052525"
---
# <a name="customize-the-microsoft-graph-sdk-service-client"></a><span data-ttu-id="f3c8c-103">自定义 Microsoft Graph SDK 服务客户端</span><span class="sxs-lookup"><span data-stu-id="f3c8c-103">Customize the Microsoft Graph SDK service client</span></span>

<span data-ttu-id="f3c8c-104">Microsoft Graph SDK 客户端配置一组默认中间件，以允许 SDK 与 Microsoft Graph 终结点进行通信。</span><span class="sxs-lookup"><span data-stu-id="f3c8c-104">The Microsoft Graph SDK client configures a default set of middleware that allows the SDK to communicate with the Microsoft Graph endpoints.</span></span> <span data-ttu-id="f3c8c-105">此默认集是可自定义的，允许您更改客户端的行为。</span><span class="sxs-lookup"><span data-stu-id="f3c8c-105">This default set is customizable, allowing you to change the behavior of the client.</span></span> <span data-ttu-id="f3c8c-106">例如，可以插入自定义日志记录，也可以添加测试处理程序以模拟特定方案。</span><span class="sxs-lookup"><span data-stu-id="f3c8c-106">For example, you can insert customized logging, or add a test handler to simulate specific scenarios.</span></span> <span data-ttu-id="f3c8c-107">您可以添加和删除中间件组件。</span><span class="sxs-lookup"><span data-stu-id="f3c8c-107">You can add and remove middleware components.</span></span> <span data-ttu-id="f3c8c-108">需要注意的是，中间件组件运行的顺序非常重要。</span><span class="sxs-lookup"><span data-stu-id="f3c8c-108">It is important to note that the order in which middleware components run is significant.</span></span>

## <a name="c"></a>[<span data-ttu-id="f3c8c-109">C#</span><span class="sxs-lookup"><span data-stu-id="f3c8c-109">C#</span></span>](#tab/csharp)

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

## <a name="typescript"></a>[<span data-ttu-id="f3c8c-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="f3c8c-110">TypeScript</span></span>](#tab/typeScript)

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

### <a name="simpleauthproviderts"></a><span data-ttu-id="f3c8c-111">SimpleAuthProvider</span><span class="sxs-lookup"><span data-stu-id="f3c8c-111">SimpleAuthProvider.ts</span></span>

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

### <a name="customlogginghandlerts"></a><span data-ttu-id="f3c8c-112">CustomLoggingHandler</span><span class="sxs-lookup"><span data-stu-id="f3c8c-112">CustomLoggingHandler.ts</span></span>

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

---
