---
title: 更新 calendarpermission
description: 更新 calendarpermission 对象的属性。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e69a1b4cdc66e9c591d060bed6600c4383e14a63
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936788"
---
# <a name="update-calendarpermission"></a>更新 calendarPermission

更新 calendarPermission 对象的属性。

## <a name="permissions"></a>权限

根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。 要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。

| 日历 | 委派（工作或学校帐户） | 委派（个人 Microsoft 帐户） | 应用程序 |
|:-----|:-----|:-----|:-----|
| 用户日历 | Calendars.ReadWrite | Calendars.ReadWrite | Calendars.ReadWrite |
| 组日历 | Group.ReadWrite.All | 不支持。 | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
PATCH /groups/{id}/calendar/calendarPermissions/{id}
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|allowedRoles|string 集合| 日历的允许共享权限级别列表。 可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。|
|emailAddress|[emailAddress](../resources/email.md)| 代表有权访问日历的 sharee。 对于 "My Organization" sharee， **address**属性为 null。 |
|id|字符串| 共享日历的用户（sharee）的唯一标识符。 只读。|
|isInsideOrganization|Boolean| 如此如果上下文中的用户（sharee）与日历所有者在同一个组织中。|
|isRemovable|Boolean| `True`如果可以从指定日历的 sharees 列表中删除用户， `false`否则为。 "我的组织" 用户决定了贵组织内的其他人对给定日历的权限。 您无法将 "我的组织" 作为 sharee 删除到日历中。|
|role|calendarRoleType| 日历 sharee 的当前权限级别。 可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。|

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[calendarPermission](../resources/calendarpermission.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendarpermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->