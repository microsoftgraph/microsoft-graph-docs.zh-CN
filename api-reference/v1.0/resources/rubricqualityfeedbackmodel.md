---
title: rubricQualityFeedbackModel 资源类型
description: 与 educationRubric 的特定质量相关的反馈。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d5874873a9d1f4f2d12a998fa9ebd7b113489b7a46ae0bbf49585bc0ec227336
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141348"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a>rubricQualityFeedbackModel 资源类型

命名空间：microsoft.graph

与[educationRubric](educationrubric.md)的特定[质量](rubricquality.md)相关的反馈。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|反馈|[itemBody](itembody.md)|有关此标准一个质量的具体反馈。|
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

