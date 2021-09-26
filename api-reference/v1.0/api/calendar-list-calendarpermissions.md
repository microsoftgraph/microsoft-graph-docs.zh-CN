---
title: 列出 calendarPermissions
description: '获取 calendarPermission 资源的集合，这些资源描述已共享或委派指定日历的用户的身份和角色。 '
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 515859c6bd4fe55277985e46253b63905636d6ab
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507612"
---
# <a name="list-calendarpermissions"></a>列出 calendarPermissions

命名空间：microsoft.graph

获取 [calendarPermission](../resources/calendarpermission.md) 资源的集合，这些资源描述已共享或委派指定日历的用户的身份和角色。 此处，日历可以是用户日历或组日历。

## <a name="permissions"></a>权限

根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。 要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。

| 日历 | 委派（工作或学校帐户） | 委派（个人 Microsoft 帐户） | 应用程序 |
|:-----|:-----|:-----|:-----|
| 用户日历 | Calendars.Read、Calendars.ReadWrite | Calendars.Read、Calendars.ReadWrite | Calendars.Read、Calendars.ReadWrite |
| 组日历 | Group.Read.All、Group.ReadWrite.All | 不支持。 | 不支持。 |

## <a name="http-request"></a>HTTP 请求

列出用户的主日历的指定权限：
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions
```

列出组日历的指定权限：
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions
```

列出包含已标识事件的用户日历的指定权限：
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **calendarPermission** 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions
```
### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('458d4c95-124e-49da-ba9d-1dd0387e682e')/calendar/calendarPermissions",
    "value": [
        {
            "id": "RXhjaGFuZ2VQdWJsaXNoZWRVc2VyLmFkbWluQE0zNjVCODc3NzE5Lm9ubWljcm9zb2Z0LmNvbQ==",
            "isRemovable": true,
            "isInsideOrganization": false,
            "role": "read",
            "allowedRoles": [
                "freeBusyRead",
                "limitedRead",
                "read"
            ],
            "emailAddress": {
                "name": "admin@M365B877719.onmicrosoft.com",
                "address": "admin@M365B877719.onmicrosoft.com"
            }
        },
        {
            "id": "RGVmYXVsdA==",
            "isRemovable": false,
            "isInsideOrganization": true,
            "role": "freeBusyRead",
            "allowedRoles": [
                "none",
                "freeBusyRead",
                "limitedRead",
                "read",
                "write"
            ],
            "emailAddress": {
                "name": "My Organization"
            }
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
