---
title: educationAssignmentResource 资源类型
description: 包装对象，用于存储与工作分配关联的资源。 包装添加**distributeForStudentWork**属性，指示该资源将
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 4d05cf5307e77dc6a7ac438c1bd4f4af4e73784e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529227"
---
# <a name="educationassignmentresource-resource-type"></a>educationAssignmentResource 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包装对象，用于存储与工作分配关联的资源。 包装添加**distributeForStudentWork**属性，指示该资源将被复制到学生提交。  如果没有复制对象，每个学生工作分配上将显示资源的链接。 学生不能以更新此资源。 这是与任何打开学生到从教师讲义。 如果资源分布，每个学生将收到其提交的资源列表中的此资源的副本。 每个学生都将能够修改其副本并将其提交的分级。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 educationAssignmentResource](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |读取属性和**educationAssignmentResource**对象的关系。|
|[Update](../api/educationassignmentresource-update.md) | [educationAssignmentResource](educationassignmentresource.md) |更新**educationAssignmentResource**对象。 |
|[删除](../api/educationassignmentresource-delete.md) | 无 |删除**educationAssignmentResource**对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|distributeForStudentWork|Boolean|指示是否应将此资源复制到每个学生提交修改和提交。|
|id|String| 此资源的 ID。 只读。|
|资源|[educationResource](educationresource.md)|已经与此工作分配的资源对象。|

## <a name="relationships"></a>关系
无。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
