---
title: educationOutcome 资源类型
description: 对工作分配进行评分的结果
ms.localizationpriority: medium
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 327ab957b3c78a9b6c848a6b29c1108fee6928c4
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767403"
---
# <a name="educationoutcome-resource-type"></a>educationOutcome 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对工作分配进行评分的结果。 这是一个基类;派生的类型是 [educationFeedbackOutcome](educationfeedbackoutcome.md) [、educationPointsOutcome](educationpointsoutcome.md)和 [educationRubricOutcome](educationrubricoutcome.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [更新 educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | 更新 educationOutcome 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String|只读。|
|lastModifiedBy|[identitySet](identityset.md)|更新资源的人。|
|lastModifiedDateTime|DateTimeOffset|上次修改资源的时间。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2021 年 1 月 1 日午夜 UTC 为 `2021-01-01T00:00:00Z` 。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOutcome",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

