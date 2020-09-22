---
title: privilegedAccess 资源类型
description: " 例如， `privilegedAccess/azureResources` 表示用于管理对 Azure 资源的权限访问的 PIM。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: f815228157721f6100af79f53f84abf43763f632
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070630"
---
# <a name="privilegedaccess-resource-type"></a>privilegedAccess 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示由特权身份管理 (PIM) 服务提供的一组功能。 `privilegedAccess`表示由 PIM 管理的不同提供程序的不同实例; 例如， `privilegedAccess/azureResources` 表示用于管理对 Azure 资源的权限访问的 PIM。


`privilegedAccess` 目前为只读。 `POST` `PUT` `PATCH` `DELETE` 实体集上不支持、、或操作 `privilegedAccess` 。

## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----------|:----------|:----------|
|id         |String     |由 PIM 管理的提供程序的 id。|
|displayName|String     |由 PIM 管理的提供程序的显示名称。|


## <a name="relationships"></a>关系
| 关系   | 类型                                         |说明|
|:---------------|:---------------------------------------------|:----------|
|resources       |[governanceResource](../resources/governanceresource.md) 集合            |提供程序的资源集合。|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md) 集合|提供程序的角色分配的集合。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md) 集合|提供程序的角色 defintions 的集合。|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 集合|提供程序的角色分配请求的集合。|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md) 集合|提供程序的角色设置的集合。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedAccess"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


