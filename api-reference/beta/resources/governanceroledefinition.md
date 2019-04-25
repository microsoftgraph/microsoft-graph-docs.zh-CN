---
title: governanceRoleDefinition 资源类型
description: 表示角色定义。 对于 azure 资源, 它可以表示 azure RBAC 角色, 如所有者、读者、参与者等。
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547438"
---
# <a name="governanceroledefinition-resource-type"></a>governanceRoleDefinition 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


表示角色定义。 对于 azure 资源, 它可以表示 azure RBAC 角色, 如所有者、读者、参与者等。


## <a name="methods"></a>方法

| 方法          | 返回类型 |说明|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md)集合 |列出资源上的角色定义的集合。|
|[获取](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |读取由 id 指定的角色定义实体的属性和关系。|
目前`POST`, `PUT`entity `PATCH`set `DELETE`上`roleDefinitions`不支持,,,。
## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----|:----------|:----------|:----------|
|id         |String     |角色定义的 id。 |
|resourceId |String     |必需。 与角色定义关联的资源的 id。 |
|externalId   |String     |角色定义的外部 id。|
|displayName|字符串     |角色定义的显示名称。|
|subjectCount|Int32     |可选。 分配给角色的主题数量。 它表示请求者对资源的访问状态。 若要获取属性, 请明确在`$select=subjectCount`查询中使用。|
|eligibleAssignmentCount|Int32|可选。 与角色定义关联的符合条件的角色分配数。 若要获取属性, 请明确在`$select=eligibleAssignmentCount`查询中使用。|
|activeAssignmentCount|Int32    |可选。 与角色定义关联的活动角色分配的数量。  若要获取属性, 请明确在`$select=activeAssignmentCount`查询中使用。|


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|资源|[governanceResource](../resources/governanceresource.md)|只读。 角色定义的关联资源。|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|角色定义的关联角色设置。|

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroledefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
