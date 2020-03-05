---
title: educationPointsOutcome 资源类型
description: 提供数字等级的 educationOutcome
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 51f57683e06f90e877b4cd72e62d0898d0ef8013
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501428"
---
# <a name="educationpointsoutcome-resource-type"></a>educationPointsOutcome 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供数字等级的[educationOutcome](educationoutcome.md) 。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [更新 educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | 更新 educationOutcome 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|points|[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)|教师为此工作分配提供了学生的数字等级。|
|publishedPoints|[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)|在向学生释放评分时所进行的 points 属性的副本。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "points": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"},
  "publishedPoints": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationPointsOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->