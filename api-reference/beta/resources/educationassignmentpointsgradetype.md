---
title: educationAssignmentPointsGradeType 资源类型
description: 与**工作分配. 评分**属性一起使用。 这是 educationAssignmentGradeType 的子类。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 61e6e425730685d4447875cdb074526e7ebc0a17
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334428"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>educationAssignmentPointsGradeType 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与**工作分配. 评分**属性一起使用。 这是[educationAssignmentGradeType](educationassignmentgradetype.md)的子类。

这表示将对工作分配进行评分, 并存储每个学生可在此工作项上实现的最大分数数。 在工作分配上设置此设置后, 每个提交都将获取一个[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)属性, 该属性与每个学生的点数相关联。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|maxPoints|单精度| 此工作分配可能的最大分数。  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
