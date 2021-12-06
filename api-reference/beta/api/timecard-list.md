---
title: 列出 timeCard
description: 检索计划中的 timeCard 条目列表。
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4f6d99e8c4ac38b5238365f8cd49896a924f43e8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989153"
---
# <a name="list-timecard"></a>列出 timeCard

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索计划 [中的 timeCard](../resources/timecard.md) 条目 [列表](../resources/schedule.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Schedule.Read.All、Schedule.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Schedule.Read.All *、Schedule.ReadWrite.All* |

>\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timecards
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$filter` 、 `$orderBy` 、 、 OData 查询 `$top` `$skipToken` 参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| MS-APP-ACTS-AS | 应用代表其操作的用户的 ID。 使用应用程序权限范围时是必需的。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [timeCard](../resources/timeCard.md) 对象列表。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面展示了示例请求。 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-list"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards?$top=2&$filter=state eq 'clockedOut'

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timecard-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timecard-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/timecard-list-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "@odata.etag": "\"3400c313-0000-0d00-0000-60afe1940000\"",
            "id": "TCK_d1e0f245-9996-4125-b128-d3eb5c4b0164",
            "createdDateTime": "2020-09-21T18:01:29.302Z",
            "lastModifiedDateTime": "2021-05-27T18:14:44.503Z",
            "userId": "66b4f2a4-425d-4dec-8172-7e889950885e",
            "state": "clockedOut",
            "confirmedBy": "none",
            "notes": null,
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
                    "displayName": "Jing Jing GuTwo"
                }
            },
            "clockInEvent": {
                "dateTime": "2020-09-21T18:01:29.302Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "ClockIn-OBO Shorbani"
                }
            },
            "clockOutEvent": {
                "dateTime": "2021-05-27T18:14:44.503Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "clock out notes"
                }
            },
            "breaks": [],
            "originalEntry": {
                "clockInEvent": {
                    "dateTime": "2020-09-21T18:01:29.302Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "ClockIn-OBO Shorbani"
                    }
                },
                "clockOutEvent": {
                    "dateTime": "2021-05-27T18:14:44.503Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "clock out notes"
                    }
                },
                "breaks": []
            },
            "createdBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "66b4f2a4-425d-4dec-8172-7e889950885e",
                    "displayName": "Janani Varadharajan"
                }
            }
        },
        {
            "@odata.etag": "\"3400d914-0000-0d00-0000-60afe1ee0000\"",
            "id": "TCK_aa73c610-dd75-4021-bb5c-6b071c7aa835",
            "createdDateTime": "2020-09-21T18:02:48.688Z",
            "lastModifiedDateTime": "2021-05-27T18:16:14.766Z",
            "userId": "3041ccde-7544-4ae0-b44f-3618b08ba1ce",
            "state": "clockedOut",
            "confirmedBy": "none",
            "notes": null,
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
                    "displayName": "Jing Jing GuTwo"
                }
            },
            "clockInEvent": {
                "dateTime": "2020-09-21T18:02:48.688Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "ClockIn-OBO Shorbani"
                }
            },
            "clockOutEvent": {
                "dateTime": "2021-05-27T18:16:14.766Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "clock out notes"
                }
            },
            "breaks": [],
            "originalEntry": {
                "clockInEvent": {
                    "dateTime": "2020-09-21T18:02:48.688Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "ClockIn-OBO Shorbani"
                    }
                },
                "clockOutEvent": {
                    "dateTime": "2021-05-27T18:16:14.766Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "clock out notes"
                    }
                },
                "breaks": []
            },
            "createdBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "66b4f2a4-425d-4dec-8172-7e889950885e",
                    "displayName": "Janani Varadharajan"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a list of timeCard entries in the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
