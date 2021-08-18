---
title: calendarPermission 资源类型
description: 与日历共享的用户的权限。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4f0f7f54fd7f2dc76a8511ab918e38d5c8ab64de18323a19669a86a29dee472e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164368"
---
# <a name="calendarpermission-resource-type"></a>calendarPermission 资源类型

命名空间：microsoft.graph

日历已在客户端中共享或委派的用户Outlook权限。

仅代表日历所有者支持获取、更新和删除日历权限。

代表共享者或代理人获取日历的日历权限将返回一个空的日历权限集合。

为日历设置共享者或代理人后，只能更新 **role** 属性以 [](../api/calendarpermission-update.md)更改共享者或代理人的权限。 不能更新 **allowedRoles** **、emailAddress** **、isInsideOrganization** 或 **isRemovable** 属性。 若要更改这些属性，您应 [删除](../api/calendarpermission-delete.md)相应的 **calendarPermission** 对象，并创建另一个共享者或Outlook客户端。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 calendarPermission](../api/calendarpermission-get.md) | [calendarPermission](calendarpermission.md) | 读取 calendarPermission 对象的属性和关系。 |
| [更新](../api/calendarpermission-update.md) | [calendarPermission](calendarpermission.md) | 更新 calendarPermission 对象。 |
| [Delete](../api/calendarpermission-delete.md) | 无 | 删除 calendarPermission 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|allowedRoles|[calendarRoleType](#calendarroletype-values) 集合| 日历允许的共享或委派权限级别列表。 可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。|
|emailAddress|[emailAddress](emailaddress.md)| 表示有权访问日历的共享者或代理人。 对于"我的组织"共享者 **，address** 属性为 null。 只读。 |
|id|String| 共享者或 (日历) 的用户的唯一标识符。 只读。|
|isInsideOrganization|布尔值| 如此 如果上下文中的用户共享 (委派) 日历所有者位于同一组织内部。|
|isRemovable|Boolean| `True` 如果用户可以从指定日历的共享者或代理人列表中删除，否则 `false` 为 。 "我的组织"用户确定组织中其他人对给定日历拥有的权限。 不能删除"我的组织"作为日历共享者。|
|role|[calendarRoleType](#calendarroletype-values)| 日历共享者或代理人的当前权限级别。 |

### <a name="calendarroletype-values"></a>calendarRoleType 值

| 成员        | 说明 |
|:--------------|:------------|
| 无 | 日历不与用户共享。 |
| freeBusyRead | 用户是共享者，可以查看日历上所有者的忙/闲状态。 |
| limitedRead | 用户是共享者，可以查看忙/闲状态以及日历上事件的标题和位置。 |
| 阅读 | 用户是一个共享者，可以查看日历上的所有事件详细信息，所有者的私人活动除外。 |
| 写入 | 用户是共享者，可以查看所有详细信息 (日历上的私人事件) 和编辑事件除外。 |
| delegateWithoutPrivateEventAccess | 用户是具有写入访问权限但无法查看日历上所有者私人活动信息的代理人。 |
| delegateWithPrivateEventAccess | 用户是具有写入访问权限的代理人，可以查看日历上所有者的私人活动的信息。 |
| custom | 用户对日历具有自定义权限。 |


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

