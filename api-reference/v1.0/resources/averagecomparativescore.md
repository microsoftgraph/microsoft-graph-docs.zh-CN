---
title: averageComparativeScore 资源类型
description: 包含基于不同范围的各种不同分数。
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eb78b045105725d8151d229525396fd205cd427f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089849"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore 资源类型

命名空间：microsoft.graph

包含基于不同范围的不同的分数 (例如，按行业垂直的平均值、按公司席位大小等的平均值) 和控制类别 (Identity、Data、Device、Apps、Infrastructure) 。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|basis|String|范围类型。 可能的值包括 `AllTenants`、`TotalSeats`、`IndustryTypes`。|
|averageScore|双精度|指定范围内的平均分数。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

