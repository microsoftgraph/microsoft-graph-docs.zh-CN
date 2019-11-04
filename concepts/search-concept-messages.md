---
title: 搜索邮件
description: Microsoft Search API 允许应用搜索电子邮件中的信息，返回相关性排名的邮件，并呈现专用搜索体验。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: f78ad8af81a7d2b72ab61914cc441db279913dc1
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939542"
---
# <a name="search-messages"></a><span data-ttu-id="91628-103">搜索邮件</span><span class="sxs-lookup"><span data-stu-id="91628-103">Search messages</span></span>

<span data-ttu-id="91628-104">Microsoft Search API 允许应用搜索电子邮件中的信息，返回相关性排名的邮件，并呈现专用搜索体验。</span><span class="sxs-lookup"><span data-stu-id="91628-104">The Microsoft Search API lets apps search for information in email messages, return messages ranked by relevance, and render a dedicated search experience.</span></span> <span data-ttu-id="91628-105">搜索适用于用户自己的邮箱中邮件的正文和附件。</span><span class="sxs-lookup"><span data-stu-id="91628-105">The search applies to the body and attachments of messages in the user's own mailbox.</span></span> 

<span data-ttu-id="91628-106">搜索查询可以包含最终用户在 Outlook 的 "**搜索**" 文本框中输入的[筛选器](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da)。</span><span class="sxs-lookup"><span data-stu-id="91628-106">A search query can include [filters](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) that end users enter in the **Search** text box in Outlook.</span></span>

<span data-ttu-id="91628-107">邮件搜索结果按**receivedDateTime**降序排列。</span><span class="sxs-lookup"><span data-stu-id="91628-107">Message search results are sorted by **receivedDateTime** in descending order.</span></span>

<span data-ttu-id="91628-108">目前，邮件搜索仅适用于用户自己的个人帐户，但不适用于工作或学校帐户，而不是委派的邮箱。</span><span class="sxs-lookup"><span data-stu-id="91628-108">Currently, message search applies to only users' own personal accounts, but not work or school accounts, and not in delegated mailboxes.</span></span> <span data-ttu-id="91628-109">请参阅下面的[已知限制](#known-limitations)。</span><span class="sxs-lookup"><span data-stu-id="91628-109">See further [known limitations](#known-limitations) below.</span></span>

## <a name="examples"></a><span data-ttu-id="91628-110">示例</span><span class="sxs-lookup"><span data-stu-id="91628-110">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="91628-111">示例 1</span><span class="sxs-lookup"><span data-stu-id="91628-111">Example 1</span></span>

<span data-ttu-id="91628-112">下面的示例查询登录用户邮箱中的邮件，其中包含邮件的任何部分（发件人姓名、主题、邮件正文或任何附件）中的字符串 "contoso"。</span><span class="sxs-lookup"><span data-stu-id="91628-112">The following example queries messages in the signed-in user's mailbox that contain the string "contoso" in any part of the message (the sender name, subject, message body, or any attachments).</span></span> <span data-ttu-id="91628-113">查询返回前25个结果。</span><span class="sxs-lookup"><span data-stu-id="91628-113">The query returns the first 25 results.</span></span> <span data-ttu-id="91628-114">搜索结果按日期/降序进行排序。</span><span class="sxs-lookup"><span data-stu-id="91628-114">The search results are ordered by Datetime descending.</span></span>

#### <a name="request"></a><span data-ttu-id="91628-115">请求</span><span class="sxs-lookup"><span data-stu-id="91628-115">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [{
      "entityTypes": ["microsoft.graph.message"],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="91628-116">响应</span><span class="sxs-lookup"><span data-stu-id="91628-116">Response</span></span> 

<span data-ttu-id="91628-117">以下是包含一条与搜索条件相匹配的邮件的响应示例。</span><span class="sxs-lookup"><span data-stu-id="91628-117">The following is an example of the response which contains one message that matches the search criterion.</span></span> 

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
    "value": [
        {
            "searchTerms": [
                "contoso"
            ],
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "_id": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
                            "_score": 1,
                            "_sortField": "DateTime",
                            "_summary": "Here is a summary of your messages from last week",
                            "_source": {
                                "@odata.type": "#microsoft.graph.message",
                                "createdDateTime": "2019-10-07T10:00:08Z",
                                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                                "receivedDateTime": "2019-10-07T10:00:09Z",
                                "sentDateTime": "2019-10-07T09:59:52Z",
                                "hasAttachments": false,
                                "subject": "Weekly digest: Office 365 changes",
                                "bodyPreview": "Here is a summary of your messages from last week -   New Feature: Live captions in English-US a",
                                "importance": "normal",
                                "replyTo": [
                                    {
                                        "emailAddress": {
                                            "name": "Goncalo Torres"
                                        }
                                    }
                                ],
                                "sender": {
                                    "emailAddress": {
                                        "name": "Office365 Message Center",
                                        "address": "gtorres@contoso.com"
                                    }
                                },
                                "from": {
                                    "emailAddress": {
                                        "name": "Office365 Message Center",
                                        "address": "gtorres@contoso.com",
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

### <a name="example-2-search-top-results-messages"></a><span data-ttu-id="91628-118">示例2搜索热门结果邮件</span><span class="sxs-lookup"><span data-stu-id="91628-118">Example 2 Search top results messages</span></span>
<span data-ttu-id="91628-119">下面的示例使用与[示例 1](#example-1)相同的搜索查询，并按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="91628-119">The following example uses the same search query as [example 1](#example-1), and sorts the results by relevance.</span></span> 

#### <a name="request"></a><span data-ttu-id="91628-120">请求</span><span class="sxs-lookup"><span data-stu-id="91628-120">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
    "requests": [{
        "entityTypes": ["microsoft.graph.message"],
        "query": {
            "query_string": {
                "query": "contoso"
            }
        },
        "from": 0,
        "size": 15,
        "enableTopResults": true
    }]
}
```

## <a name="known-limitations"></a><span data-ttu-id="91628-121">已知限制</span><span class="sxs-lookup"><span data-stu-id="91628-121">Known limitations</span></span>

- <span data-ttu-id="91628-122">您只能访问用户自己的邮箱。</span><span class="sxs-lookup"><span data-stu-id="91628-122">You can only access a user’s own mailbox.</span></span> <span data-ttu-id="91628-123">不支持搜索委派的邮箱</span><span class="sxs-lookup"><span data-stu-id="91628-123">Searching delegated mailbox is not supported</span></span> 

- <span data-ttu-id="91628-124">对于邮件， [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta)类型的**total**属性包含页面上的结果数，而不是匹配结果的总数。</span><span class="sxs-lookup"><span data-stu-id="91628-124">For messages, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) type contains the number of results on the page, not the total number of matching results.</span></span>

## <a name="next-steps"></a><span data-ttu-id="91628-125">后续步骤</span><span class="sxs-lookup"><span data-stu-id="91628-125">Next steps</span></span>

<span data-ttu-id="91628-126">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="91628-126">Find out more about:</span></span>

- [<span data-ttu-id="91628-127">使用搜索 API</span><span class="sxs-lookup"><span data-stu-id="91628-127">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
