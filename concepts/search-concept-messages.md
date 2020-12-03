---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索邮件
description: 您可以使用 Microsoft 搜索 API 搜索电子邮件中的信息，返回按相关性排序的邮件，并呈现专用搜索体验。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 0ee9950ff136b3f97e063da252ec22d166f05b74
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49521360"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a><span data-ttu-id="2dc85-103">使用 Microsoft 搜索 API 搜索 Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="2dc85-103">Use the Microsoft Search API to search Outlook messages</span></span>

<span data-ttu-id="2dc85-104">使用 Microsoft Search API 搜索电子邮件中的信息，返回相关性排名的邮件，并呈现专用搜索体验。</span><span class="sxs-lookup"><span data-stu-id="2dc85-104">Use the Microsoft Search API to search for information in email messages, return messages ranked by relevance, and render a dedicated search experience.</span></span> <span data-ttu-id="2dc85-105">搜索适用于登录用户自己的邮箱中的邮件的正文和附件。</span><span class="sxs-lookup"><span data-stu-id="2dc85-105">The search applies to the body and attachments of messages in the signed-in user's own mailbox.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="2dc85-106">搜索查询可以包含最终用户在 Outlook 的 "**搜索**" 文本框中输入的 [筛选器](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da)。</span><span class="sxs-lookup"><span data-stu-id="2dc85-106">A search query can include [filters](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) that end users enter in the **Search** text box in Outlook.</span></span>

<span data-ttu-id="2dc85-107">邮件搜索结果按 **receivedDateTime** 降序排列。</span><span class="sxs-lookup"><span data-stu-id="2dc85-107">Message search results are sorted by **receivedDateTime** in descending order.</span></span>

<span data-ttu-id="2dc85-108">邮件搜索适用于工作或学校帐户。</span><span class="sxs-lookup"><span data-stu-id="2dc85-108">Message search applies to work or school accounts.</span></span> <span data-ttu-id="2dc85-109">用户可以搜索其自己的邮箱，但不能搜索委派的邮箱。</span><span class="sxs-lookup"><span data-stu-id="2dc85-109">Users can search their own mailbox, but can't search delegated mailboxes.</span></span> <span data-ttu-id="2dc85-110">有关详细信息，请参阅 [已知限制](#known-limitations)。</span><span class="sxs-lookup"><span data-stu-id="2dc85-110">For details, see [known limitations](#known-limitations).</span></span>

<span data-ttu-id="2dc85-111">邮件搜索还会查找附件。</span><span class="sxs-lookup"><span data-stu-id="2dc85-111">Message search also looks for attachments.</span></span> <span data-ttu-id="2dc85-112">邮件附件搜索支持的文件类型与 SharePoint Online 搜索所 [支持的文件类型](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) 相同。</span><span class="sxs-lookup"><span data-stu-id="2dc85-112">The [supported file types](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) for message attachment search are the same as those for SharePoint Online search.</span></span>

## <a name="example-1-search-messages-in-a-users-mailbox"></a><span data-ttu-id="2dc85-113">示例1：搜索用户邮箱中的邮件</span><span class="sxs-lookup"><span data-stu-id="2dc85-113">Example 1: Search messages in a user's mailbox</span></span>

<span data-ttu-id="2dc85-114">下面的示例在登录用户的邮箱中查询邮件的任何部分中包含字符串 "contoso" 的邮件， (发件人姓名、主题、邮件正文或任何附件) 。</span><span class="sxs-lookup"><span data-stu-id="2dc85-114">The following example queries messages in the signed-in user's mailbox that contain the string "contoso" in any part of the message (the sender name, subject, message body, or any attachments).</span></span> <span data-ttu-id="2dc85-115">查询返回前25个结果。</span><span class="sxs-lookup"><span data-stu-id="2dc85-115">The query returns the first 25 results.</span></span> <span data-ttu-id="2dc85-116">搜索结果按 **日期/** 降序进行排序。</span><span class="sxs-lookup"><span data-stu-id="2dc85-116">The search results are ordered by **DateTime** descending.</span></span>

### <a name="request"></a><span data-ttu-id="2dc85-117">请求</span><span class="sxs-lookup"><span data-stu-id="2dc85-117">Request</span></span>

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="2dc85-118">响应</span><span class="sxs-lookup"><span data-stu-id="2dc85-118">Response</span></span>

<span data-ttu-id="2dc85-119">下面是一个响应示例，其中包含一个与搜索条件相匹配的邮件。</span><span class="sxs-lookup"><span data-stu-id="2dc85-119">The following is an example of the response, which contains one message that matches the search criterion.</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
              "rank": 1,
              "summary": "Here is a summary of your messages from last week",
              "resource": {
                "@odata.type": "#microsoft.graph.message",
                "createdDateTime": "2019-10-07T10:00:08Z",
                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                "receivedDateTime": "2019-10-07T10:00:09Z",
                "sentDateTime": "2019-10-07T09:59:52Z",
                "hasAttachments": false,
                "subject": "Weekly digest: Microsoft 365 changes",
                "bodyPreview": "Here is a summary of your messages from last week -   New Feature: Live captions in English-US a",
                "importance": "normal",
                "replyTo": [
                  {
                    "emailAddress": {
                      "name": "Goncalo Torres"
                    }
                  }
                ],
                "sender": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
                  }
                },
                "from": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
                  }
                }
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="example-2-search-top-results-messages"></a><span data-ttu-id="2dc85-120">示例2：搜索排名靠前的结果邮件</span><span class="sxs-lookup"><span data-stu-id="2dc85-120">Example 2: Search top results messages</span></span>

<span data-ttu-id="2dc85-121">下面的示例使用示例1中所示的搜索查询，并按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="2dc85-121">The following example uses the search query shown in Example 1, and sorts the results by relevance.</span></span> 

<!-- markdownlint-disable MD024 -->
### <a name="request"></a><span data-ttu-id="2dc85-122">请求</span><span class="sxs-lookup"><span data-stu-id="2dc85-122">Request</span></span>

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 15,
      "enableTopResults": true
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="2dc85-123">响应</span><span class="sxs-lookup"><span data-stu-id="2dc85-123">Response</span></span>
```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
              "rank": 1,
              "summary": "Here is a summary of your messages from last week",
              "resource": {
                "@odata.type": "#microsoft.graph.message",
                "createdDateTime": "2019-10-07T10:00:08Z",
                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                "receivedDateTime": "2019-10-07T10:00:09Z",
                "sentDateTime": "2019-10-07T09:59:52Z",
                "hasAttachments": false,
                "subject": "Weekly digest: Microsoft 365 changes",
                "bodyPreview": "Here is a summary of your messages from last week -   New Feature: Live captions in English-US a",
                "importance": "normal",
                "replyTo": [
                  {
                    "emailAddress": {
                      "name": "Goncalo Torres"
                    }
                  }
                ],
                "sender": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
                  }
                },
                "from": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
                  }
                }
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="known-limitations"></a><span data-ttu-id="2dc85-124">已知限制</span><span class="sxs-lookup"><span data-stu-id="2dc85-124">Known limitations</span></span>

- <span data-ttu-id="2dc85-125">您只能访问登录用户自己的邮箱。</span><span class="sxs-lookup"><span data-stu-id="2dc85-125">You can access only the signed-in user’s own mailbox.</span></span> <span data-ttu-id="2dc85-126">不支持搜索委派的邮箱。</span><span class="sxs-lookup"><span data-stu-id="2dc85-126">Searching delegated mailboxes is not supported.</span></span>
- <span data-ttu-id="2dc85-127">对于邮件， [searchHitsContainer](/graph/api/resources/searchhitscontainer)类型的 **total** 属性包含页面上的结果数，而不是匹配结果的总数。</span><span class="sxs-lookup"><span data-stu-id="2dc85-127">For messages, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer) type contains the number of results on the page, not the total number of matching results.</span></span>
- <span data-ttu-id="2dc85-128">事件不支持排序结果。</span><span class="sxs-lookup"><span data-stu-id="2dc85-128">Sorting results is not supported for events.</span></span> <span data-ttu-id="2dc85-129">请求中的 sort 子句将在响应中返回错误的请求错误代码。</span><span class="sxs-lookup"><span data-stu-id="2dc85-129">A sort clause in the request will return a Bad Request error code in the response.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2dc85-130">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2dc85-130">Next steps</span></span>

- [<span data-ttu-id="2dc85-131">使用 Microsoft 搜索 API</span><span class="sxs-lookup"><span data-stu-id="2dc85-131">Use the Microsoft Search API</span></span>](/graph/api/resources/search-api-overview)