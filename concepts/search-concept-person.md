---
title: '使用 Microsoft Microsoft 搜索 中的 Graph API 搜索预览 (人员) '
description: 可以使用 Microsoft 搜索 API 搜索与自己相关的人员。
author: acsehi
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: ac978f09477db841e8f71a630128ba58d4f19ec2567813704a326ba49b13b818
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235091"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-people-preview"></a>使用 Microsoft Microsoft 搜索 中的 Graph API 搜索预览 (人员) 

Microsoft Graph应用程序可以使用 Microsoft 搜索 API 检索与用户最相关的人员。 相关性由用户的通信和协作模式及业务关系决定。 人员可以是本地联系人，也可以来自组织目录，也可以来自最近通信的人。 除了生成此见解外，搜索还提供模糊匹配搜索支持以及检索与登录用户组织中其他用户相关的用户列表的能力。

## <a name="example-search-person-by-name"></a>示例：按姓名搜索人员

以下请求根据通信和协作模式以及业务关系，获取与登录用户最相关的人员。

### <a name="request"></a>请求

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

### <a name="response"></a>响应

下面是一个响应示例，其中包含一条匹配搜索条件的邮件。

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

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API](/graph/api/resources/search-api-overview)
