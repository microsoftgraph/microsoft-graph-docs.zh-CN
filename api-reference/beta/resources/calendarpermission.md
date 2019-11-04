---
title: calendarPermission 资源类型
description: 共享日历的用户的权限。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5d19a1738d3369f2d910dd590062016acf3047ab
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950449"
---
# <a name="calendarpermission-resource-type"></a>calendarPermission 资源类型

共享日历的用户的权限。 

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 calendarPermission](../api/calendarpermission-get.md) | [calendarPermission](calendarpermission.md) | 读取 calendarPermission 对象的属性和关系。 |
| [Update](../api/calendarpermission-update.md) | [calendarPermission](calendarpermission.md) | 更新 calendarPermission 对象。 |
| [删除](../api/calendarpermission-delete.md) | 无 | 删除 calendarPermission 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|allowedRoles|string 集合| 日历的允许共享权限级别列表。 可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。|
|emailAddress|[emailAddress](emailaddress.md)| 代表有权访问日历的 sharee。 对于 "My Organization" sharee， **address**属性为 null。 |
|id|String| 共享日历的用户（sharee）的唯一标识符。 只读。|
|isInsideOrganization|Boolean| 如此如果上下文中的用户（sharee）与日历所有者在同一个组织中。|
|isRemovable|Boolean| `True`如果可以从指定日历的 sharees 列表中删除用户， `false`否则为。 "我的组织" 用户决定了贵组织内的其他人对给定日历的权限。 您无法将 "我的组织" 作为 sharee 删除到日历中。|
|role|calendarRoleType| 日历 sharee 的当前权限级别。 可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。|

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