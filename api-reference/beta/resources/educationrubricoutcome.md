---
title: educationRubricOutcome 资源类型
description: 提供分级的 rubric 的 educationOutcome
ms.localizationpriority: medium
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c46a79cf9f6bd0620a519c059a382a7afa59d83b
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684716"
---
# <a name="educationrubricoutcome-resource-type"></a>educationRubricOutcome 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供分级标准的 [educationOutcome](educationoutcome.md) 。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [更新 educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | 更新 educationOutcome 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|educationRubricOutcome 的唯一标识符。|
|lastModifiedBy|[identitySet](identityset.md)|最后一个修改资源的用户。|
|lastModifiedDateTime|DateTimeOffset|上次修改资源的时间。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|publishedRubricQualityFeedback|[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) 集合|在将成绩发布到学生时创建的 rubricQualityFeedback 属性的副本。|
|publishedRubricQualitySelectedLevels|[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) 集合|在成绩发布给学生时创建的 rubricQualitySelectedLevels 属性的副本。|
|rubricQualityFeedback|[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) 集合|此标准的每个质量的特定反馈集合。|
|rubricQualitySelectedLevels|[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) 集合|教师在评分此作业时为每个质量选择的级别。|

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
  "id": "String (identifier)",
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

