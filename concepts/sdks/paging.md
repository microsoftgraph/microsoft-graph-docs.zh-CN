---
title: 使用 Microsoft Graph Sdk 逐页浏览集合
description: 提供有关使用 Microsoft Graph Sdk 创建 Microsoft Graph API 请求的说明。
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: ef48af29a4cc0388c405e2a42894d98ce6c98010
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289483"
---
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a>使用 Microsoft Graph Sdk 逐页浏览集合

出于性能原因，实体的集合通常会拆分为多个页面，并且每个页面都将使用下一页的 URL 进行返回。 **PageIterator**类简化了分页集合的使用。 **PageIterator** 句柄枚举当前页面并自动请求后续页面。

## <a name="iterate-over-all-the-messages"></a>循环访问所有邮件

下面的示例演示如何对用户邮箱中的所有邮件进行迭代。

> [!TIP]
> 本示例将使用参数设置较小的页面大小 `top` 以用于演示目的。 最多可以将页面大小设置为999，以最大限度地减少所需的请求数。

### <a name="c"></a>[C#](#tab/csharp)

```csharp
var messages = await graphClient.Me.Messages
    .Request()
    .Select(e => new {
        e.Sender,
        e.Subject
    })
    .Top(10)
    .GetAsync();

var pageIterator = PageIterator<Message>
    .CreatePageIterator(graphClient, messages, (m) => {
        Console.WriteLine(m.Subject);
        return true;
    });

await pageIterator.IterateAsync();
```

### <a name="typescript"></a>[TypeScript](#tab/typeScript)

```typescript
// Makes request to fetch mails list.
let response: PageCollection = await client
  .api("/me/messages?$top=10&$select=sender,subject")
  .get();

// A callback function to be called for every item in the collection.
// This call back should return boolean indicating whether not to
// continue the iteration process.
let callback: PageIteratorCallback = (data) => {
  console.log(data.subject);
  return true;
};

// Creating a new page iterator instance with client a graph client
// instance, page collection response from request and callback
let pageIterator = new PageIterator(client, response, callback);

// This iterates the collection until the nextLink is drained out.
await pageIterator.iterate();
```

### <a name="java"></a>[Java](#tab/java)

```java
IMessageCollectionPage messagesPage = graphClient.me().messages()
    .buildRequest()
    .select("Sender,Subject")
    .top(10)
    .get();


while(messagesPage != null) {
  final List<Message> messages = messagesPage.GetCurrentPage();
  final IMessageCollectionRequestBuilder nextPage = messagesPage.GetNextPage();
  if(nextPage == null) {
    break;
  } else {
    messagePage = nextPage.buildRequest().get();
  }
}
```

---

## <a name="stopping-and-resuming-the-iteration"></a>停止和恢复迭代

在某些情况下，需要停止迭代过程才能执行其他操作。 可以通过 `false` 从迭代回调中返回来暂停迭代。 可以通过对 PageIterator 调用方法来恢复迭代 `resume` 。 **PageIterator**

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
    .CreatePageIterator(graphClient, messages, (m) => {
        Console.WriteLine(m.Subject);
        count++;
        // If we've iterated over the limit,
        // stop the iteration by returning false
        return count < pauseAfter;
    });

await pageIterator.IterateAsync();

while (pageIterator.State != PagingState.Complete)
{
    Console.WriteLine("Iteration paused for 5 seconds...");
    Thread.Sleep(5000);
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

---
<!-- markdownlint-enable MD024 -->
