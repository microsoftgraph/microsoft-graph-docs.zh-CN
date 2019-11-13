---
title: 搜索邮件
description: Microsoft Search API 允许应用搜索电子邮件中的信息，返回相关性排名的邮件，并呈现专用搜索体验。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 985da47e5a7b96cead416e8e5cda32dae0357adb
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38303130"
---
# <a name="search-messages"></a><span data-ttu-id="f6992-103">搜索邮件</span><span class="sxs-lookup"><span data-stu-id="f6992-103">Search messages</span></span>

<span data-ttu-id="f6992-104">Microsoft Search API 允许应用搜索电子邮件中的信息，返回相关性排名的邮件，并呈现专用搜索体验。</span><span class="sxs-lookup"><span data-stu-id="f6992-104">The Microsoft Search API lets apps search for information in email messages, return messages ranked by relevance, and render a dedicated search experience.</span></span> <span data-ttu-id="f6992-105">搜索适用于用户自己的邮箱中邮件的正文和附件。</span><span class="sxs-lookup"><span data-stu-id="f6992-105">The search applies to the body and attachments of messages in the user's own mailbox.</span></span>

<span data-ttu-id="f6992-106">搜索查询可以包含最终用户在 Outlook 的 "**搜索**" 文本框中输入的[筛选器](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da)。</span><span class="sxs-lookup"><span data-stu-id="f6992-106">A search query can include [filters](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) that end users enter in the **Search** text box in Outlook.</span></span>

<span data-ttu-id="f6992-107">邮件搜索结果按**receivedDateTime**降序排列。</span><span class="sxs-lookup"><span data-stu-id="f6992-107">Message search results are sorted by **receivedDateTime** in descending order.</span></span>

<span data-ttu-id="f6992-108">邮件搜索适用于工作或学校帐户。</span><span class="sxs-lookup"><span data-stu-id="f6992-108">Message search applies to work or school accounts.</span></span> <span data-ttu-id="f6992-109">用户可以搜索其自己的邮箱，但不能搜索委派邮箱中的邮箱。</span><span class="sxs-lookup"><span data-stu-id="f6992-109">Users can search their own mailbox, but not in delegated mailboxes.</span></span> <span data-ttu-id="f6992-110">请参阅下面的[已知限制](#known-limitations)。</span><span class="sxs-lookup"><span data-stu-id="f6992-110">See further [known limitations](#known-limitations) below.</span></span>

<span data-ttu-id="f6992-111">邮件搜索还会查找附件。</span><span class="sxs-lookup"><span data-stu-id="f6992-111">Message search also looks for attachments.</span></span> <span data-ttu-id="f6992-112">[附件支持的文件类型](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types)与 SharePoint Online 中的文件类型相同。</span><span class="sxs-lookup"><span data-stu-id="f6992-112">The [file types supported for attachments](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) is the same as that for SharePoint Online.</span></span>

## <a name="examples"></a><span data-ttu-id="f6992-113">示例</span><span class="sxs-lookup"><span data-stu-id="f6992-113">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="f6992-114">示例 1</span><span class="sxs-lookup"><span data-stu-id="f6992-114">Example 1</span></span>

<span data-ttu-id="f6992-115">下面的示例查询登录用户邮箱中的邮件，其中包含邮件的任何部分（发件人姓名、主题、邮件正文或任何附件）中的字符串 "contoso"。</span><span class="sxs-lookup"><span data-stu-id="f6992-115">The following example queries messages in the signed-in user's mailbox that contain the string "contoso" in any part of the message (the sender name, subject, message body, or any attachments).</span></span> <span data-ttu-id="f6992-116">查询返回前25个结果。</span><span class="sxs-lookup"><span data-stu-id="f6992-116">The query returns the first 25 results.</span></span> <span data-ttu-id="f6992-117">搜索结果按日期/降序进行排序。</span><span class="sxs-lookup"><span data-stu-id="f6992-117">The search results are ordered by Datetime descending.</span></span>

#### <a name="request"></a><span data-ttu-id="f6992-118">请求</span><span class="sxs-lookup"><span data-stu-id="f6992-118">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f6992-119">响应</span><span class="sxs-lookup"><span data-stu-id="f6992-119">Response</span></span> 

<span data-ttu-id="f6992-120">以下是包含一条与搜索条件相匹配的邮件的响应示例。</span><span class="sxs-lookup"><span data-stu-id="f6992-120">The following is an example of the response which contains one message that matches the search criterion.</span></span> 

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

### <a name="example-2-search-top-results-messages"></a><span data-ttu-id="f6992-121">示例2搜索热门结果邮件</span><span class="sxs-lookup"><span data-stu-id="f6992-121">Example 2 Search top results messages</span></span>
<span data-ttu-id="f6992-122">下面的示例使用与[示例 1](#example-1)相同的搜索查询，并按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="f6992-122">The following example uses the same search query as [example 1](#example-1), and sorts the results by relevance.</span></span> 

#### <a name="request"></a><span data-ttu-id="f6992-123">请求</span><span class="sxs-lookup"><span data-stu-id="f6992-123">Request</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="f6992-124">已知限制</span><span class="sxs-lookup"><span data-stu-id="f6992-124">Known limitations</span></span>

- <span data-ttu-id="f6992-125">您只能访问用户自己的邮箱。</span><span class="sxs-lookup"><span data-stu-id="f6992-125">You can only access a user’s own mailbox.</span></span> <span data-ttu-id="f6992-126">不支持搜索委派的邮箱</span><span class="sxs-lookup"><span data-stu-id="f6992-126">Searching delegated mailbox is not supported</span></span> 

- <span data-ttu-id="f6992-127">对于邮件， [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta)类型的**total**属性包含页面上的结果数，而不是匹配结果的总数。</span><span class="sxs-lookup"><span data-stu-id="f6992-127">For messages, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) type contains the number of results on the page, not the total number of matching results.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f6992-128">后续步骤</span><span class="sxs-lookup"><span data-stu-id="f6992-128">Next steps</span></span>

<span data-ttu-id="f6992-129">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="f6992-129">Find out more about:</span></span>

- [<span data-ttu-id="f6992-130">使用搜索 API</span><span class="sxs-lookup"><span data-stu-id="f6992-130">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
