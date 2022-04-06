---
title: privilegedAccess 资源类型
description: " 例如，表示 `privilegedAccess/azureResources` 管理 Azure 资源的特权访问的 PIM。"
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: f90b76ca24a4bded8c2206a4a5f45ebcfde4d825
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509551"
---
# <a name="privilegedaccess-resource-type"></a>privilegedAccess 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 PIM 服务Privileged Identity Management (提供的) 组功能。 的不同实例表示 `privilegedAccess` 由 PIM 管理的不同提供程序; `privilegedAccess/azureResources` 例如，表示管理 Azure 资源的特权访问的 PIM。


`privilegedAccess` 目前为只读。 实体`POST`集`PATCH`不支持`DELETE`任何 、、 或 `privilegedAccess` 操作。 `PUT`

## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----------|:----------|:----------|
|id         |字符串     |由 PIM 管理的提供程序的 ID。|
|displayName|String     |由 PIM 显示名称提供程序的提供程序的名称。|


## <a name="relationships"></a>关系
| 关系   | 类型                                         |说明|
|:---------------|:---------------------------------------------|:----------|
|resources       |[governanceResource](../resources/governanceresource.md) 集合            |提供程序的资源集合。|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md) 集合|提供程序的角色分配集合。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md) 集合|提供程序的角色定义的集合。|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 集合|提供程序角色分配请求的集合。|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md) 集合|提供程序的角色设置集合。|


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


