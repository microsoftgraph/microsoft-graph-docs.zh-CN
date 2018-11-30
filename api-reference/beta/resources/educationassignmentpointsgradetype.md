---
title: educationAssignmentPointsGradeType 资源类型
description: '**Assignments.grading**属性一起使用。 这是 educationAssignmentGradeType 的一个子类。'
ms.openlocfilehash: 5c170540e99003a78df0550d4d6542c07df8f1ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048485"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>educationAssignmentPointsGradeType 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**Assignments.grading**属性一起使用。 这是[educationAssignmentGradeType](educationassignmentgradetype.md)的一个子类。

这表示工作分配的分级范围，并将每个学生可以获得的点的最大数目存储在此工作项。 当此设置工作分配上时，每个提交将获取与之关联的每个学生的点的存储[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)属性。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|maxPoints|Single| 最大点可能的此工作分配。  |

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->