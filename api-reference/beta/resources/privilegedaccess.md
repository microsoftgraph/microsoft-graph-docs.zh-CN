---
title: privilegedAccess 资源类型
description: " 例如，`privilegedAccess/azureResources`代表 PIM 管理特权 Azure 资源的访问。"
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512925"
---
# <a name="privilegedaccess-resource-type"></a>privilegedAccess 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表一组特权标识管理 (PIM) 服务提供的功能。 不同实例`privilegedAccess`表示不同的提供程序托管的 PIM;例如，`privilegedAccess/azureResources`代表 PIM 管理特权 Azure 资源的访问。


`privilegedAccess`现在是只读的。 不`POST`， `PUT`， `PATCH`，或`DELETE`支持操作`privilegedAccess`实体集。

## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----------|:----------|:----------|
|id         |String     |由 PIM 管理提供程序的 id。|
|displayName|String     |由 PIM 管理提供程序的显示名称。|


## <a name="relationships"></a>关系
| 关系   | 类型                                         |说明|
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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
