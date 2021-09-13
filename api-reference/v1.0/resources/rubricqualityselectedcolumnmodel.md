---
title: rubricQualitySelectedColumnModel 资源类型
description: 指示教师在对 educationRubric 进行评分时选择的评分标准。
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 53a3369e4332fd0dfddbca3be1eeb6da21aaf228
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117737"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a>rubricQualitySelectedColumnModel 资源类型

命名空间：microsoft.graph

指示教师 [在评分](rubriclevel.md) [educationRubric](educationrubric.md)时选择的评分标准。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|columnId|String|此质量的选定级别的 ID。|
|qualityId|String|关联质量的 ID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel",
  "baseType": null
}-->

```json
{
  "columnId": "String",
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualitySelectedColumnModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

