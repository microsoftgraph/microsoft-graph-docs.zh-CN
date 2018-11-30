---
title: privilegedRoleAssignment 资源类型
description: '表示特定用户特权的角色分配。 '
ms.openlocfilehash: 40cfe6487184171fc0d120f9a0e2cd98070f96f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043584"
---
# <a name="privilegedroleassignment-resource-type"></a>privilegedRoleAssignment 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示特定用户特权的角色分配。 


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 privilegedRoleAssignment 集合](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md)集合|获取 privilegedRoleAssignment 对象的集合。|
|[获取 privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |读取属性和 privilegedRoleAssignment 对象的关系。|
|[创建工作分配](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| 通过发布到 assignments 集合中创建新的工作分配。|
|[删除](../api/privilegedroleassignment-delete.md) | 无 |删除 privilegedRoleAssignment 对象。 |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|请为永久的角色分配。|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|请作为合格的角色分配。|
|[我](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](privilegedroleassignment.md)集合|获取当前用户的特权的角色分配。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|UTC DateTime 时将过期的临时特权的角色分配。 永久角色分配的值为 null。|
|id|string| 特权的角色分配的唯一标识符。 只读。 处于 userId_roleId，其中 userId 是 Azure AD 用户 id 的 GUID 字符串，roleId 是 Azure 管理员角色 id 的 GUID 字符串的格式。|
|isElevated|boolean|**true**如果激活该角色分配。 **false**如果停用的角色分配。|
|resultMessage|string|结果消息由服务设置。|
|roleId|string|角色标识符。 格式字符串 GUID。|
|userId|string|用户标识符。 格式字符串 GUID。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| 只读。 可为 Null。 相关联的角色的信息。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->