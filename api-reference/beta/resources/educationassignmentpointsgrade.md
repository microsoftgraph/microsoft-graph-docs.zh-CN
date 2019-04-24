---
title: educationAssignmentPointsGrade 资源类型
description: 当工作分配设置为 "点" 评分类型时, 每个提交都将具有与 "**提交. 年级**" 属性相关联的此对象。 这将从 educationAssignmentGrade 中创建一个子类,
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5d2a5cf6f6f886185179c6f1a61c1bb1d9d1ecfc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507334"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>educationAssignmentPointsGrade 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

当工作分配设置为 "点" 评分类型时, 每个提交都将具有与 "**提交. 年级**" 属性相关联的此对象。 这将从[educationAssignmentGrade](educationassignmentgrade.md)创建一个子类, 该子类将向此属性添加数据。 最大分数存储在**工作分配. 评分**属性中。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|points|单倍行距|教师向此提交对象提供的积分数。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
