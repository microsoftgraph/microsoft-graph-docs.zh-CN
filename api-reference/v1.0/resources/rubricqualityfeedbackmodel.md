---
title: rubricQualityFeedbackModel 资源类型
description: 与 educationRubric 的特定质量相关的反馈。
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0ca3a8877573751187f251b0a179498c44c0add8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117751"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a>rubricQualityFeedbackModel 资源类型

命名空间：microsoft.graph

与[educationRubric](educationrubric.md)的特定质量相关的反馈。 [](rubricquality.md)

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|反馈|[itemBody](itembody.md)|此标准中的一个质量的具体反馈。|
|qualityId|String|此反馈相关的 [rubricQuality](rubricquality.md) 的 ID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualityFeedbackModel",
  "baseType": null
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.itemBody"},
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualityFeedbackModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

