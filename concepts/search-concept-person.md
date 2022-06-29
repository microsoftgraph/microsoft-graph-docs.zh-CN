---
title: 使用 Microsoft 搜索 API 搜索人员
description: 使用 Microsoft Graph 中的 Microsoft 搜索 API 搜索与由用户的通信模式和业务关系决定的用户相关的人员。
author: acsehi
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 3b1165a0bcac91ef7a74078b2d88fb268d0f40c6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436195"
---
# <a name="use-the-microsoft-search-api-to-search-people"></a>使用 Microsoft 搜索 API 搜索人员

Microsoft Graph 应用程序可以使用 Microsoft 搜索 API 检索与用户关系最相关的人员。 相关性由用户的通信和协作模式及业务关系决定。 人员可以是本地联系人，也可以是组织目录中的人员，也可以是最近通信中的人员。

除了生成此见解，搜索还提供模糊匹配的搜索支持，并能够检索与登录用户组织中其他用户相关的用户列表。

## <a name="example-search-person-by-name"></a>示例：按姓名搜索人员

以下请求基于通信和协作模式以及业务关系，获取与已登录用户最相关的人员。

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

下面是响应的示例，其中包含一条与搜索条件匹配的消息。

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

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview)
