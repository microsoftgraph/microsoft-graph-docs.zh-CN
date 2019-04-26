---
title: privilegedRoleAssignment 资源类型
description: '表示特定用户的特权角色分配。 '
localization_priority: Normal
ms.openlocfilehash: 1e58f144eb3dda19225a836aa966f9479d3a9350
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344218"
---
# <a name="privilegedroleassignment-resource-type"></a>privilegedRoleAssignment 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示特定用户的特权角色分配。 


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 privilegedRoleAssignment 集合](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md) 集合|获取 privilegedRoleAssignment 对象的集合。|
|[获取 privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |读取 privilegedRoleAssignment 对象的属性和关系。|
|[创建作业](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| 通过发布到工作分配集合来创建新的工作分配。|
|[删除](../api/privilegedroleassignment-delete.md) | 无 |删除 privilegedRoleAssignment 对象。 |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|将角色分配标记为永久。|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|使角色分配符合资格。|
|[My](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](privilegedroleassignment.md) 集合|获取当前用户的特权角色分配。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|临时权限角色分配将在何时过期时的 UTC 日期时间。 对于永久角色分配, 值为 null。|
|id|string| 特权角色分配的唯一标识符。 只读。 它的格式为 "userId_roleId", 其中 userId 是 azure AD 用户 id 的 guid 字符串, roleId 是 azure 管理员角色 id 的 guid 字符串。|
|isElevated|boolean|如果角色分配已激活,**则为 true** 。 **假**如果角色分配被停用。|
|resultMessage|string|由服务设置的结果消息。|
|roleId|string|角色标识符。 以 GUID 字符串格式。|
|userId|string|用户标识符。 以 GUID 字符串格式。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| 只读。 可为 Null。 相关联的角色信息。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
