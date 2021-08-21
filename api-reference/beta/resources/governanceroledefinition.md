---
title: governanceRoleDefinition 资源类型
description: 表示角色定义。 对于 Azure 资源，它可以表示 Azure RBAC 角色，如所有者、读者、参与者等。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 4f0144f4d26c8440b4e2bdc0965e88310a4f9145
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453721"
---
# <a name="governanceroledefinition-resource-type"></a>governanceRoleDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


表示角色定义。 对于 Azure 资源，它可以表示 Azure RBAC 角色，如所有者、读者、参与者等。


## <a name="methods"></a>方法

| 方法          | 返回类型 |Description|
|:---------------|:--------|:--------|
|[List](../api/governanceroledefinition-list.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) 集合 |列出资源上的角色定义集合。|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |读取由 id 指定的角色定义实体的属性和关系。|

目前 `POST` `PUT` ， `PATCH` 实体 `DELETE` 集不支持 `roleDefinitions` 、 。

## <a name="properties"></a>属性
| 属性    | 类型   | 说明                                                           |
|:------------|:-------|:----------------------------------------------------------------------|
| id          | String | 角色定义的 ID。                                        |
| resourceId  | String | 必填。 与角色定义关联的资源的 ID。 |
| externalId  | String | 角色定义的外部 ID。                               |
| displayName | String | 角色显示名称的组。                              |
| templateId  | 字符串 |                                                                       |

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


