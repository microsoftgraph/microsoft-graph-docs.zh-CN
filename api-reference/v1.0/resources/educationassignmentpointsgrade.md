---
title: educationAssignmentPointsGrade 资源类型
description: 当作业设置为分数类型时，每个提交都将具有与此对象关联的 **submission.grade** 属性。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b624bd0e82336e4e416641240e072c8b4ac6392d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912310"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>educationAssignmentPointsGrade 资源类型

命名空间：microsoft.graph

当作业设置为分数类型时，每个提交都将具有与此对象关联的 **submission.grade** 属性。 这将从 [educationAssignmentGrade](educationassignmentgrade.md)创建一个子类，它将向此属性添加 who 数据。 最大点数存储在 **assignments.assignments** 属性中。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|points|单一|教师提供此提交对象的点数。|

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
  "points": "Double"
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
  "suppressions": []
}
-->


