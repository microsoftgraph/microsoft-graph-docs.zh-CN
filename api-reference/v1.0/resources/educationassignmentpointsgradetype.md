---
title: educationAssignmentPointsGradeType 资源类型
description: 与 **assignments.assignments** 属性一同使用的资源类型。 这是 educationAssignmentGradeType 的子类。
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5c2a59a9f34d2be02415021ece777021dacb34bb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036744"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>educationAssignmentPointsGradeType 资源类型

命名空间：microsoft.graph

与 **assignments.assignments** 属性一同使用的资源类型。 这是 [educationAssignmentGradeType 的子类](educationassignmentgradetype.md)。

这表示作业已评分，并存储每个学生可在此工作项上实现的最大分数数。 在作业中设置此选项时，每个提交都将获得一个 [与其关联的 educationAssignmentPointsGrade](educationassignmentpointsgrade.md) 属性，用于存储每个学生的分数。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|maxPoints|单一| 此工作分配可能的最大点数。  |

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
  "maxPoints": "Double"
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


