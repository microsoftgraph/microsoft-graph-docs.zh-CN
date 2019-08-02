---
title: averageComparativeScore 资源类型
description: 包含基于不同范围的各种不同分数。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f128fd22562889a5a537f3815a4003aec9bfc8a9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030014"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore 资源类型

包含基于不同范围的各种不同分数 (例如, 按行业垂直、按公司座位大小的平均值等) 和控制类别 (标识、数据、设备、应用程序、基础结构)。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|基本|String|范围类型。 可能的值包括 `AllTenants`、`TotalSeats`、`IndustryTypes`。|
|averageScore|双精度|指定基准中的平均分数。|

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
