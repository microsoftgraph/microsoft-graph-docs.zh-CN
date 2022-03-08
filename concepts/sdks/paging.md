---
title: 使用 Microsoft SDK 分页Graph集合
description: 提供有关使用 Microsoft Graph SDK 创建 Microsoft Graph API 请求的说明。
ms.localizationpriority: medium
author: DarrelMiller
ms.openlocfilehash: 515b24324309c8121ec231bca73f0878f5c227f7
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337409"
---
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a>使用 Microsoft SDK 分页Graph集合

出于性能原因，实体集合通常拆分为多个页面，并且每个页面返回一个指向下一页的 URL。 **PageIterator** 类简化了分页集合的使用。 **PageIterator** 自动枚举当前页面和请求后续页面。

## <a name="request-headers"></a>请求标头

如果在初始请求中发送任何其他请求头，则默认情况下这些标头不会包含在后续页面请求中。 如果需要在后续请求中发送这些标头，则必须显式设置它们。

## <a name="iterate-over-all-the-messages"></a>在所有邮件上进行 Iterate

下面的示例展示了如何对用户邮箱中所有邮件进行访问。

> [!TIP]
> 此示例使用 参数设置一个小页面 `top` 大小以用于演示。 可以将页面大小设置为最多 999，以最大限度地减少所需的请求数。

### <a name="c"></a>[C#](#tab/csharp)

```csharp
var messages = await graphClient.Me.Messages
    .Request()
    .Header("Prefer", "outlook.body-content-type=\"text\"")
    .Select(e => new {
        e.Sender,
        e.Subject,
        e.Body
    })
    .Top(10)
    .GetAsync();

var pageIterator = PageIterator<Message>
    .CreatePageIterator(
        graphClient,
        messages,
        // Callback executed for each item in
        // the collection
        (m) =>
        {
            Console.WriteLine(m.Subject);
            return true;
        },
        // Used to configure subsequent page
        // requests
        (req) =>
        {
            // Re-add the header to subsequent requests
            req.Header("Prefer", "outlook.body-content-type=\"text\"");
            return req;
        }
    );

await pageIterator.IterateAsync();
```

### <a name="typescript"></a>[TypeScript](#tab/typeScript)

```typescript
// Makes request to fetch mails list.
let response: PageCollection = await client
  .api("/me/messages?$top=10&$select=sender,subject,body")
  .header('Prefer', 'outlook.body-content-type="text"')
  .get();

// A callback function to be called for every item in the collection.
// This call back should return boolean indicating whether not to
// continue the iteration process.
let callback: PageIteratorCallback = (data) => {
  console.log(data.subject);
  return true;
};

// A set of request options to be applied to
// all subsequent page requests
let requestOptions: GraphRequestOptions = {
  // Re-add the header to subsequent requests
  headers: {
    'Prefer': 'outlook.body-content-type="text"'
  }
};

// Creating a new page iterator instance with client a graph client
// instance, page collection response from request and callback
let pageIterator = new PageIterator(client, response, callback, requestOptions);

// This iterates the collection until the nextLink is drained out.
await pageIterator.iterate();
```

### <a name="java"></a>[Java](#tab/java)

```java
MessageCollectionPage messagesPage = graphClient.me().messages()
    .buildRequest(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""))
    .select("Sender,Subject,Body")
    .top(10)
    .get();


while(messagesPage != null) {
  final List<Message> messages = messagesPage.getCurrentPage();
  final MessageCollectionRequestBuilder nextPage = messagesPage.getNextPage();
  if (nextPage == null) {
    break;
  } else {
    messagesPage = nextPage.buildRequest(
        // Re-add the header to subsequent requests
        new HeaderOption("Prefer", "outlook.body-content-type=\"text\"")
    ).get();
  }
}
```

### <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    msgraphcore "github.com/microsoftgraph/msgraph-sdk-go-core"
    "github.com/microsoftgraph/msgraph-sdk-go/me/messages"
    "github.com/microsoftgraph/msgraph-sdk-go/models/microsoft/graph"
)

query := messages.MessagesRequestBuilderGetQueryParameters{
    Select: []string{"body", "sender", "subject"},
}

options := messages.MessagesRequestBuilderGetOptions{
    H: map[string]string{
        "Prefer": "outlook.body-content-type=\"text\"",
    },
    Q: &query,
}

result, err := client.Me().Messages().Get(&options)

// Initialize iterator
pageIterator, err := msgraphcore.NewPageIterator(result, adapter.GraphRequestAdapterBase,
    func() serialization.Parsable {
        return messages.NewMessagesResponse()
    })

// Any custom headers sent in original request should also be added
// to the iterator
pageIterator.SetHeaders(options.H)

// Iterate over all pages
iterateErr := pageIterator.Iterate(func(pageItem interface{}) bool {
    message := pageItem.(graph.Message)
    fmt.Printf("%s\n", *message.GetSubject())
    // Return true to continue the iteration
    return true
})
```

---

## <a name="stopping-and-resuming-the-iteration"></a>停止和恢复迭代

在某些情况下，为了执行其他操作，需要停止迭代过程。 通过从迭代回调返回可以 `false` 暂停迭代。 可以通过在 **PageIterator** 上调用 `resume` 方法来恢复迭代。

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[C#](#tab/csharp)

```csharp
int count = 0;
int pauseAfter = 25;

var messages = await graphClient.Me.Messages
    .Request()
    .Select(e => new {
        e.Sender,
        e.Subject
    })
    .Top(10)
    .GetAsync();

var pageIterator = PageIterator<Message>
    .CreatePageIterator(
        graphClient,
        messages,
        (m) =>
        {
            Console.WriteLine(m.Subject);
            count++;
            // If we've iterated over the limit,
            // stop the iteration by returning false
            return count < pauseAfter;
        }
    );

await pageIterator.IterateAsync();

while (pageIterator.State != PagingState.Complete)
{
    Console.WriteLine("Iteration paused for 5 seconds...");
    await Task.Delay(5000);
    // Reset count
    count = 0;
    await pageIterator.ResumeAsync();
}
```

### <a name="typescript"></a>[TypeScript](#tab/typeScript)

```typescript
let count: number = 0;
let pauseAfter: number = 25;

let response: PageCollection = await client
  .api('/me/messages?$top=10&$select=sender,subject')
  .get();

let callback: PageIteratorCallback = (data) => {
  result = `${result}${data.subject}\n`;
  console.log(data.subject);
  count++;

  // If we've iterated over the limit,
  // stop the iteration by returning false
  return count < pauseAfter;
};

let pageIterator = new PageIterator(client, response, callback);
await pageIterator.iterate();

while (!pageIterator.isComplete()) {
  console.log('Iteration paused for 5 seconds...');
  await new Promise(resolve => setTimeout(resolve, 5000));

  // Reset count
  count = 0;
  await pageIterator.resume();
}
```

### <a name="java"></a>[Java](#tab/java)

```java
// not supported in java SDK
```

### <a name="go"></a>[转到](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    msgraphcore "github.com/microsoftgraph/msgraph-sdk-go-core"
    "github.com/microsoftgraph/msgraph-sdk-go/me/messages"
    "github.com/microsoftgraph/msgraph-sdk-go/models/microsoft/graph"
)

query := messages.MessagesRequestBuilderGetQueryParameters{
    Select: []string{"body", "sender", "subject"},
}

options := messages.MessagesRequestBuilderGetOptions{
    H: map[string]string{
        "Prefer": "outlook.body-content-type=\"text\"",
    },
    Q: &query,
}

result, err := client.Me().Messages().Get(&options)

// Initialize iterator
pageIterator, err := msgraphcore.NewPageIterator(result, adapter.GraphRequestAdapterBase,
    func() serialization.Parsable {
        return messages.NewMessagesResponse()
    })

// Any custom headers sent in original request should also be added
// to the iterator
pageIterator.SetHeaders(options.H)

// Pause iterating after 25
var count, pauseAfter = 0, 25

// Iterate over all pages
iterateErr := pageIterator.Iterate(func(pageItem interface{}) bool {
    message := pageItem.(graph.Message)
    count++
    fmt.Printf("%d: %s\n", count, *message.GetSubject())
    // Once count = 25, this returns false,
    // Which pauses the iteration
    return count < pauseAfter
})

// Pause 5 seconds
fmt.Printf("Iterated first %d messages, pausing for 5 seconds...\n", pauseAfter)
time.Sleep(5 * time.Second)
fmt.Printf("Resuming iteration...\n")

// Resume iteration
iterateErr = pageIterator.Iterate(func(pageItem interface{}) bool {
    message := pageItem.(graph.Message)
    count++
    fmt.Printf("%d: %s\n", count, *message.GetSubject())
    // Return true to continue the iteration
    return true
})
```

---
<!-- markdownlint-enable MD024 -->
