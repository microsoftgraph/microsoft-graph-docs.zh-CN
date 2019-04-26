---
title: privilegedAccess 资源类型
description: " 例如, `privilegedAccess/azureResources`表示用于管理对 Azure 资源的权限访问的 PIM。"
localization_priority: Normal
ms.openlocfilehash: 2dd131dd8f1ba5a2e7668949d2a03a9ab3321d1d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344257"
---
# <a name="privilegedaccess-resource-type"></a>privilegedAccess 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示由特权标识管理 (PIM) 服务提供的一组功能。 表示由 PIM `privilegedAccess`管理的不同提供程序的不同实例;例如, `privilegedAccess/azureResources`表示用于管理对 Azure 资源的权限访问的 PIM。


`privilegedAccess`目前为只读。 `privilegedAccess`实体`POST`集`PUT`上`PATCH`不支持`DELETE` 、、或操作。

## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----------|:----------|:----------|
|id         |String     |由 PIM 管理的提供程序的 id。|
|displayName|String     |由 PIM 管理的提供程序的显示名称。|


## <a name="relationships"></a>关系
| 关系   | 类型                                         |说明|
|:---------------|:---------------------------------------------|:----------|
|资源       |[governanceResource](../resources/governanceresource.md)集合            |提供程序的资源集合。|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md)集合|提供程序的角色分配的集合。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md)集合|提供程序的角色 defintions 的集合。|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合|提供程序的角色分配请求的集合。|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md)集合|提供程序的角色设置的集合。|


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
