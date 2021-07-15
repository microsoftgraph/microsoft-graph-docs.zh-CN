---
title: '使用 Microsoft Microsoft 搜索 中的 Graph API 搜索预览 (人员) '
description: 可以使用 Microsoft 搜索 API 搜索与自己相关的人员。
author: acsehi
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 0540ee40c672af4305a396b7348d7d87276c0ce7
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443114"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-people-preview"></a><span data-ttu-id="59e3a-103">使用 Microsoft Microsoft 搜索 中的 Graph API 搜索预览 (人员) </span><span class="sxs-lookup"><span data-stu-id="59e3a-103">Use the Microsoft Search API in Microsoft Graph to search people (preview)</span></span>

<span data-ttu-id="59e3a-104">Microsoft Graph应用程序可以使用 Microsoft 搜索 API 检索与用户最相关的人员。</span><span class="sxs-lookup"><span data-stu-id="59e3a-104">Microsoft Graph applications can use the Microsoft Search API to retrieve the people who are most relevant to a user.</span></span> <span data-ttu-id="59e3a-105">相关性由用户的通信和协作模式及业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="59e3a-105">Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="59e3a-106">人员可以是本地联系人，也可以来自组织目录，也可以来自最近通信的人。</span><span class="sxs-lookup"><span data-stu-id="59e3a-106">People can be local contacts or from an organization’s directory, and people from recent communications.</span></span> <span data-ttu-id="59e3a-107">除了生成此见解外，搜索还提供模糊匹配搜索支持以及检索与登录用户组织中其他用户相关的用户列表的能力。</span><span class="sxs-lookup"><span data-stu-id="59e3a-107">Along with generating this insight, search also provides fuzzy matching search support and the ability to retrieve the list of users relevant to another user in the signed in user's organization.</span></span>

## <a name="example-search-person-by-name"></a><span data-ttu-id="59e3a-108">示例：按姓名搜索人员</span><span class="sxs-lookup"><span data-stu-id="59e3a-108">Example: Search person by name</span></span>

<span data-ttu-id="59e3a-109">以下请求根据通信和协作模式以及业务关系，获取与登录用户最相关的人员。</span><span class="sxs-lookup"><span data-stu-id="59e3a-109">The following request gets the people most relevant to the signed-in user, based on communication and collaboration patterns and business relationships.</span></span>

### <a name="request"></a><span data-ttu-id="59e3a-110">请求</span><span class="sxs-lookup"><span data-stu-id="59e3a-110">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "person"
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

### <a name="response"></a><span data-ttu-id="59e3a-111">响应</span><span class="sxs-lookup"><span data-stu-id="59e3a-111">Response</span></span>

<span data-ttu-id="59e3a-112">下面是一个响应示例，其中包含一条匹配搜索条件的邮件。</span><span class="sxs-lookup"><span data-stu-id="59e3a-112">The following is an example of the response, which contains one message that matches the search criterion.</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://canary.graph.microsoft.com/testprodbetapersoninsearch/$metadata#microsoft.graph.searchResponse",
    "value": [
        {
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "hitId": "fc138b85-18ac-48e0-80a4-633ae4b594e0@41f988bf-86f1-53af-91ab-2d7cd034db47",
                            "rank": 1,
                            "summary": "",
                            "resource": {
                                "@odata.type": "#microsoft.graph.person",
                                "displayName": "Example User",
                                "givenName": "User",
                                "surname": "User",
                                "department": "Finance",
                                "officeLocation": "London",
                                "userPrincipalName": "example.user@contoso.com",
                                "emailAddresses": [
                                    {
                                        "address": "example.user@contoso.com",
                                        "rank": 1
                                    }
                                ],
                                "phones": [
                                    {
                                        "type": "business",
                                        "number": "+44 (20) 12345678"
                                    }
                                ]
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="next-steps"></a><span data-ttu-id="59e3a-113">后续步骤</span><span class="sxs-lookup"><span data-stu-id="59e3a-113">Next steps</span></span>

- [<span data-ttu-id="59e3a-114">使用 Microsoft 搜索 API</span><span class="sxs-lookup"><span data-stu-id="59e3a-114">Use the Microsoft Search API</span></span>](/graph/api/resources/search-api-overview)
