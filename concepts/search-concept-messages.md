---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索邮件
description: 您可以使用 Microsoft 搜索 API 搜索电子邮件中的信息，返回按相关性排序的邮件，并呈现专用搜索体验。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 1b47155e761a28ccaf3e93719bd9967b9f9eff67
ms.sourcegitcommit: 093d89c7583bb6880c8395e9498a1f33cdd938b4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44568768"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-messages"></a><span data-ttu-id="b393a-103">在 Microsoft Graph 中使用 Microsoft Search API 搜索邮件</span><span class="sxs-lookup"><span data-stu-id="b393a-103">Use the Microsoft Search API in Microsoft Graph to search messages</span></span>

<span data-ttu-id="b393a-104">您可以使用 Microsoft 搜索 API 搜索电子邮件中的信息，返回按相关性排序的邮件，并呈现专用搜索体验。</span><span class="sxs-lookup"><span data-stu-id="b393a-104">You can use the Microsoft Search API to search for information in email messages, return messages ranked by relevance, and render a dedicated search experience.</span></span> <span data-ttu-id="b393a-105">搜索适用于用户自己的邮箱中邮件的正文和附件。</span><span class="sxs-lookup"><span data-stu-id="b393a-105">The search applies to the body and attachments of messages in the user's own mailbox.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="b393a-106">搜索查询可以包含最终用户在 Outlook 的 "**搜索**" 文本框中输入的[筛选器](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da)。</span><span class="sxs-lookup"><span data-stu-id="b393a-106">A search query can include [filters](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) that end users enter in the **Search** text box in Outlook.</span></span>

<span data-ttu-id="b393a-107">邮件搜索结果按**receivedDateTime**降序排列。</span><span class="sxs-lookup"><span data-stu-id="b393a-107">Message search results are sorted by **receivedDateTime** in descending order.</span></span>

<span data-ttu-id="b393a-108">邮件搜索适用于工作或学校帐户。</span><span class="sxs-lookup"><span data-stu-id="b393a-108">Message search applies to work or school accounts.</span></span> <span data-ttu-id="b393a-109">用户可以搜索其自己的邮箱，但不能搜索委派的邮箱。</span><span class="sxs-lookup"><span data-stu-id="b393a-109">Users can search their own mailbox, but can't search delegated mailboxes.</span></span> <span data-ttu-id="b393a-110">有关详细信息，请参阅[已知限制](#known-limitations)。</span><span class="sxs-lookup"><span data-stu-id="b393a-110">For details, see [known limitations](#known-limitations).</span></span>

<span data-ttu-id="b393a-111">邮件搜索还会查找附件。</span><span class="sxs-lookup"><span data-stu-id="b393a-111">Message search also looks for attachments.</span></span> <span data-ttu-id="b393a-112">邮件附件搜索支持的文件类型与 SharePoint Online 搜索所[支持的文件类型](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types)相同。</span><span class="sxs-lookup"><span data-stu-id="b393a-112">The [supported file types](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) for message attachment search are the same as those for SharePoint Online search.</span></span>

## <a name="examples"></a><span data-ttu-id="b393a-113">示例</span><span class="sxs-lookup"><span data-stu-id="b393a-113">Examples</span></span>

### <a name="example-1-search-messages-in-a-users-mailbox"></a><span data-ttu-id="b393a-114">示例1：搜索用户邮箱中的邮件</span><span class="sxs-lookup"><span data-stu-id="b393a-114">Example 1: Search messages in a user's mailbox</span></span>

<span data-ttu-id="b393a-115">下面的示例查询登录用户邮箱中的邮件，其中包含邮件的任何部分（发件人姓名、主题、邮件正文或任何附件）中的字符串 "contoso"。</span><span class="sxs-lookup"><span data-stu-id="b393a-115">The following example queries messages in the signed-in user's mailbox that contain the string "contoso" in any part of the message (the sender name, subject, message body, or any attachments).</span></span> <span data-ttu-id="b393a-116">查询返回前25个结果。</span><span class="sxs-lookup"><span data-stu-id="b393a-116">The query returns the first 25 results.</span></span> <span data-ttu-id="b393a-117">搜索结果按**日期/** 降序进行排序。</span><span class="sxs-lookup"><span data-stu-id="b393a-117">The search results are ordered by **DateTime** descending.</span></span>

#### <a name="request"></a><span data-ttu-id="b393a-118">请求</span><span class="sxs-lookup"><span data-stu-id="b393a-118">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="b393a-119">响应</span><span class="sxs-lookup"><span data-stu-id="b393a-119">Response</span></span>

<span data-ttu-id="b393a-120">下面是一个响应示例，其中包含一个与搜索条件相匹配的邮件。</span><span class="sxs-lookup"><span data-stu-id="b393a-120">The following is an example of the response, which contains one message that matches the search criterion.</span></span> 

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
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
              "_id": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
              "_score": 1,
              "_sortField": "DateTime",
              "_summary": "Here is a summary of your messages from last week",
              "_source": {
                "@odata.type": "#microsoft.graph.message",
                "createdDateTime": "2019-10-07T10:00:08Z",
                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                "receivedDateTime": "2019-10-07T10:00:09Z",
                "sentDateTime": "2019-10-07T09:59:52Z",
                "hasAttachments": false,
                "subject": "Weekly digest: Office 365 changes",
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

### <a name="example-2-search-top-results-messages"></a><span data-ttu-id="b393a-121">示例2：搜索排名靠前的结果邮件</span><span class="sxs-lookup"><span data-stu-id="b393a-121">Example 2: Search top results messages</span></span>

<span data-ttu-id="b393a-122">下面的示例使用示例1中所示的搜索查询，并按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="b393a-122">The following example uses the search query shown in Example 1, and sorts the results by relevance.</span></span> 

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="b393a-123">请求</span><span class="sxs-lookup"><span data-stu-id="b393a-123">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 15,
      "enableTopResults": true
    }
  ]
}
```

## <a name="known-limitations"></a><span data-ttu-id="b393a-124">已知限制</span><span class="sxs-lookup"><span data-stu-id="b393a-124">Known limitations</span></span>

- <span data-ttu-id="b393a-125">您只能访问用户自己的邮箱。</span><span class="sxs-lookup"><span data-stu-id="b393a-125">You can only access a user’s own mailbox.</span></span> <span data-ttu-id="b393a-126">不支持搜索委派的邮箱。</span><span class="sxs-lookup"><span data-stu-id="b393a-126">Searching delegated mailboxes is not supported.</span></span>
- <span data-ttu-id="b393a-127">对于邮件， [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta)类型的**total**属性包含页面上的结果数，而不是匹配结果的总数。</span><span class="sxs-lookup"><span data-stu-id="b393a-127">For messages, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) type contains the number of results on the page, not the total number of matching results.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b393a-128">后续步骤</span><span class="sxs-lookup"><span data-stu-id="b393a-128">Next steps</span></span>

- [<span data-ttu-id="b393a-129">使用 Microsoft 搜索 API</span><span class="sxs-lookup"><span data-stu-id="b393a-129">Use the Microsoft Search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
