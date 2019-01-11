---
title: privilegedAccess 资源类型
description: " 例如，`privilegedAccess/azureResources`代表 PIM 管理特权 Azure 资源的访问。"
localization_priority: Normal
ms.openlocfilehash: f4166fb539d627730c68c7e039fd8d672ff4c785
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810050"
---
# <a name="privilegedaccess-resource-type"></a>privilegedAccess 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表一组特权标识管理 (PIM) 服务提供的功能。 不同实例`privilegedAccess`表示不同的提供程序托管的 PIM;例如，`privilegedAccess/azureResources`代表 PIM 管理特权 Azure 资源的访问。


`privilegedAccess`现在是只读的。 不`POST`， `PUT`， `PATCH`，或`DELETE`支持操作`privilegedAccess`实体集。

## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----------|:----------|:----------|
|id         |字符串     |由 PIM 管理提供程序的 id。|
|displayName|字符串     |由 PIM 管理提供程序的显示名称。|


## <a name="relationships"></a>Relationships
| 关系   | 类型                                         |Description|
|:---------------|:---------------------------------------------|:----------|
|resources       |[governanceResource](../resources/governanceresource.md)集合            |提供程序的资源的集合。|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md)集合|提供程序的角色分配的集合。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md)集合|提供程序的角色定义的集合。|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合|角色提供程序的工作分配请求的集合。|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md)集合|角色提供程序的设置的集合。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
