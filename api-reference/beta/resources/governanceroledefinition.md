---
title: governanceRoleDefinition 资源类型
description: 表示角色定义。 有关 Azure 资源，它可以表示 Azure RBAC 角色，如所有者、 读者、 参与者、 等。
localization_priority: Normal
ms.openlocfilehash: 3f94dd1a741545760951875fbc064307823a65dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842447"
---
# <a name="governanceroledefinition-resource-type"></a>governanceRoleDefinition 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。 


表示角色定义。 有关 Azure 资源，它可以表示 Azure RBAC 角色，如所有者、 读者、 参与者、 等。


## <a name="methods"></a>方法

| 方法          | 返回类型 |说明|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md)集合 |列出对资源的角色定义的集合。|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |读取的属性并由 id 指定的角色定义实体的关系。|
不`POST`， `PUT`， `PATCH`，`DELETE`支持`roleDefinitions`现在实体集。
## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----|:----------|:----------|:----------|
|id         |字符串     |角色定义的 id。 |
|resourceId |String     |必需。 与角色定义关联的资源的 id。 |
|externalId   |String     |外部角色定义的 id。|
|displayName|字符串     |角色定义的显示名称。|
|subjectCount|Int32     |可选。 分配给角色的主题数。 它表示对资源的请求者的访问状态。 若要获取的属性，请是明确使用`$select=subjectCount`查询中。|
|eligibleAssignmentCount|Int32|可选。 合格的角色分配相关联的角色定义数。 若要获取的属性，请是明确使用`$select=eligibleAssignmentCount`查询中。|
|activeAssignmentCount|Int32    |可选。 活动的角色分配相关联的角色定义数。  若要获取的属性，请是明确使用`$select=activeAssignmentCount`查询中。|


## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|资源|[governanceResource](../resources/governanceresource.md)|此为只读属性。 相关联的角色定义的资源。|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|角色定义关联的角色设置。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
