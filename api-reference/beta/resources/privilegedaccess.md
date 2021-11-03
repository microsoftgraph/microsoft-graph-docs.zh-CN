---
title: privilegedAccess 资源类型
description: " 例如， `privilegedAccess/azureResources` 表示管理 Azure 资源的特权访问的 PIM。"
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 9f7bf8f06ae75bd082664b5efad3e5ca9c46b70e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696950"
---
# <a name="privilegedaccess-resource-type"></a>privilegedAccess 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 PIM 服务Privileged Identity Management (一) 组功能。 的不同实例表示由 PIM 管理的不同提供程序;例如，表示管理 Azure 资源的特权访问 `privilegedAccess` `privilegedAccess/azureResources` 的 PIM。


`privilegedAccess` 目前为只读。 实体集不支持任何 、、 `POST` `PUT` 或 `PATCH` `DELETE` `privilegedAccess` 操作。

## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----------|:----------|:----------|
|id         |String     |由 PIM 管理的提供程序的 ID。|
|displayName|String     |PIM 显示名称提供程序的名称。|


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


