---
title: educationRubricOutcome 资源类型
description: 提供评分标准评分的 educationOutcome。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3fad9c8aa16653875060f1ec35a7abd09e875643aea77e40c665300878ba86b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229274"
---
# <a name="educationrubricoutcome-resource-type"></a>educationRubricOutcome 资源类型

命名空间：microsoft.graph

提供评分标准评分的[educationOutcome。](educationoutcome.md)

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [更新 educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | 更新 educationOutcome 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|lastModifiedBy|[identitySet](identityset.md)|最后一个修改资源的用户。|
|lastModifiedDateTime|DateTimeOffset|上次修改资源的时间。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|publishedRubricQualityFeedback|[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) 集合|评分发布给学生时所创建 rubricQualityFeedback 属性的副本。|
|publishedRubricQualitySelectedLevels|[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) 集合|评分发布给学生时所创建 rubricQualitySelectedLevels 属性的副本。|
|rubricQualityFeedback|[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) 集合|此标准的每个质量的特定反馈的集合。|
|rubricQualitySelectedLevels|[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) 集合|教师在为此作业评分时针对每个质量选择的级别。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
  "keyProperty": "id"
}-->

```json
{
  "publishedRubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "publishedRubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}],
  "rubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "rubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubricOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

