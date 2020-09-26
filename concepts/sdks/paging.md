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
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a><span data-ttu-id="1dfc8-103">使用 Microsoft Graph Sdk 逐页浏览集合</span><span class="sxs-lookup"><span data-stu-id="1dfc8-103">Page through a collection using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="1dfc8-104">出于性能原因，实体的集合通常会拆分为多个页面，并且每个页面都将使用下一页的 URL 进行返回。</span><span class="sxs-lookup"><span data-stu-id="1dfc8-104">For performance reasons, collections of entities are often split into pages and each page is returned with a URL to the next page.</span></span> <span data-ttu-id="1dfc8-105">**PageIterator**类简化了分页集合的使用。</span><span class="sxs-lookup"><span data-stu-id="1dfc8-105">The **PageIterator** class simplifies consuming of paged collections.</span></span> <span data-ttu-id="1dfc8-106">**PageIterator** 句柄枚举当前页面并自动请求后续页面。</span><span class="sxs-lookup"><span data-stu-id="1dfc8-106">**PageIterator** handles enumerating the current page and requesting subsequent pages automatically.</span></span>

## <a name="iterate-over-all-the-messages"></a><span data-ttu-id="1dfc8-107">循环访问所有邮件</span><span class="sxs-lookup"><span data-stu-id="1dfc8-107">Iterate over all the messages</span></span>

<span data-ttu-id="1dfc8-108">下面的示例演示如何对用户邮箱中的所有邮件进行迭代。</span><span class="sxs-lookup"><span data-stu-id="1dfc8-108">The following example shows iterating over all the messages in a user's mailbox.</span></span>

> [!TIP]
> <span data-ttu-id="1dfc8-109">本示例将使用参数设置较小的页面大小 `top` 以用于演示目的。</span><span class="sxs-lookup"><span data-stu-id="1dfc8-109">This example sets a small page size using the `top` parameter for demonstration purposes.</span></span> <span data-ttu-id="1dfc8-110">最多可以将页面大小设置为999，以最大限度地减少所需的请求数。</span><span class="sxs-lookup"><span data-stu-id="1dfc8-110">You can set the page size up to 999 to minimize the number of requests that are necessary.</span></span>

### <a name="c"></a>[<span data-ttu-id="1dfc8-111">C#</span><span class="sxs-lookup"><span data-stu-id="1dfc8-111">C#</span></span>](#tab/csharp)

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

### <a name="typescript"></a>[<span data-ttu-id="1dfc8-112">TypeScript</span><span class="sxs-lookup"><span data-stu-id="1dfc8-112">TypeScript</span></span>](#tab/typeScript)

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

### <a name="java"></a>[<span data-ttu-id="1dfc8-113">Java</span><span class="sxs-lookup"><span data-stu-id="1dfc8-113">Java</span></span>](#tab/java)

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

## <a name="stopping-and-resuming-the-iteration"></a><span data-ttu-id="1dfc8-114">停止和恢复迭代</span><span class="sxs-lookup"><span data-stu-id="1dfc8-114">Stopping and resuming the iteration</span></span>

<span data-ttu-id="1dfc8-115">在某些情况下，需要停止迭代过程才能执行其他操作。</span><span class="sxs-lookup"><span data-stu-id="1dfc8-115">Some scenarios require stopping the iteration process in order to perform other actions.</span></span> <span data-ttu-id="1dfc8-116">可以通过 `false` 从迭代回调中返回来暂停迭代。</span><span class="sxs-lookup"><span data-stu-id="1dfc8-116">It is possible to pause the iteration by returning `false` from the iteration callback.</span></span> <span data-ttu-id="1dfc8-117">可以通过对 PageIterator 调用方法来恢复迭代 `resume` 。 **PageIterator**</span><span class="sxs-lookup"><span data-stu-id="1dfc8-117">Iteration can be resumed by calling the `resume` method on the **PageIterator**.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[<span data-ttu-id="1dfc8-118">C#</span><span class="sxs-lookup"><span data-stu-id="1dfc8-118">C#</span></span>](#tab/csharp)

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

### <a name="typescript"></a>[<span data-ttu-id="1dfc8-119">TypeScript</span><span class="sxs-lookup"><span data-stu-id="1dfc8-119">TypeScript</span></span>](#tab/typeScript)

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

### <a name="java"></a>[<span data-ttu-id="1dfc8-120">Java</span><span class="sxs-lookup"><span data-stu-id="1dfc8-120">Java</span></span>](#tab/java)

```java
// not supported in java SDK
```

---
<!-- markdownlint-enable MD024 -->
