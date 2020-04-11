---
title: calendarPermission 资源类型
description: 共享日历的用户的权限。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 80c704dbb3e50d3f4d0ba586a40f06f74f032321
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229463"
---
# <a name="calendarpermission-resource-type"></a>calendarPermission 资源类型

在 Outlook 客户端中共享或委派了日历的用户的权限。

仅代表日历所有者支持获取、更新和删除日历权限。

代表 sharee 或代理人获取日历的日历权限时，将返回一个空的日历权限集合。

为日历设置了 sharee 或委派后，您可以仅[更新](../api/calendarpermission-update.md) **role**属性来更改 sharee 或委派的权限。 您不**update**能更新**allowedRoles**、 **emailAddress**、 **isInsideOrganization**或**isRemovable**属性。 若要更改这些属性，应[删除](../api/calendarpermission-delete.md)相应的**calendarPermission**对象，并在 Outlook 客户端中创建另一个 sharee 或委派。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 calendarPermission](../api/calendarpermission-get.md) | [calendarPermission](calendarpermission.md) | 读取 calendarPermission 对象的属性和关系。 |
| [更新](../api/calendarpermission-update.md) | [calendarPermission](calendarpermission.md) | 更新 calendarPermission 对象。 |
| [删除](../api/calendarpermission-delete.md) | 无 | 删除 calendarPermission 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|allowedRoles|[calendarRoleType](#calendarroletype-values)集合| 允许共享或委派日历权限级别的列表。 可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。|
|emailAddress|[emailAddress](emailaddress.md)| 代表有权访问日历的 sharee 或代理人。 对于 "My Organization" sharee， **address**属性为 null。 只读。 |
|id|String| 为其共享日历的用户（sharee 或代理人）的唯一标识符。 只读。|
|isInsideOrganization|布尔| 如此如果上下文中的用户（sharee 或代理人）与日历所有者在同一个组织中。|
|isRemovable|Boolean| `True`如果可以从指定日历的 sharees 或代理列表中删除用户， `false`否则为。 "我的组织" 用户决定了贵组织内的其他人对给定日历的权限。 您无法将 "我的组织" 作为 sharee 删除到日历中。|
|role|[calendarRoleType](#calendarroletype-values)| 日历 sharee 或代理人的当前权限级别。 |

### <a name="calendarroletype-values"></a>calendarRoleType 值

| 值        | 说明 |
|:--------------|:------------|
| 无 | 日历不与用户共享。 |
| freeBusyRead | 用户是可以查看日历上的所有者的忙/闲状态的 sharee。 |
| limitedRead | 用户是可以查看忙/闲状态以及日历上的事件的标题和位置的 sharee。 |
| 自述 | 用户是可以查看日历上的事件的所有详细信息的 sharee，所有者的私人活动除外。 |
| 销帐 | 用户是可以查看所有详细信息（私有事件除外）和编辑日历上的事件的 sharee。 |
| delegateWithoutPrivateEventAccess | 用户是具有写入权限的代理，但无法查看日历上所有者的私人活动的信息。 |
| delegateWithPrivateEventAccess | 用户是具有写访问权限的代理，可以在日历上查看所有者的私人活动的信息。 |
| 自 | 用户对日历具有自定义权限。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.calendarPermission",
  "keyProperty": "id"
}-->

```json
{
  "allowedRoles": ["string"],
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "id": "String (identifier)",
  "isInsideOrganization": "boolean",
  "isRemovable": "boolean",
  "role": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarPermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->