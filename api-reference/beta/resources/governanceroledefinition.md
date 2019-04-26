---
title: governanceRoleDefinition 资源类型
description: 表示角色定义。 对于 azure 资源, 它可以表示 azure RBAC 角色, 如所有者、读者、参与者等。
localization_priority: Normal
ms.openlocfilehash: 27b4b144f834f3b5eb4270a2875da5add10efb9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333748"
---
# <a name="governanceroledefinition-resource-type"></a>governanceRoleDefinition 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


表示角色定义。 对于 azure 资源, 它可以表示 azure RBAC 角色, 如所有者、读者、参与者等。


## <a name="methods"></a>方法

| 方法          | 返回类型 |说明|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md)集合 |列出资源上的角色定义的集合。|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |读取由 id 指定的角色定义实体的属性和关系。|
目前`POST`, `PUT`entity `PATCH`set `DELETE`上`roleDefinitions`不支持,,,。
## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----|:----------|:----------|:----------|
|id         |字符串     |角色定义的 id。 |
|resourceId |String     |必需。 与角色定义关联的资源的 id。 |
|externalId   |String     |角色定义的外部 id。|
|displayName|字符串     |角色定义的显示名称。|
|templateId | String | |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|资源|[governanceResource](../resources/governanceresource.md)|只读。 角色定义的关联资源。|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|角色定义的关联角色设置。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "templateId":"String"
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
  "suppressions": []
}
-->
