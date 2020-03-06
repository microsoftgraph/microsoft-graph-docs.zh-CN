---
title: averageComparativeScore 资源类型
description: 包含基于不同范围的各种不同分数。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1ed82e040121f49bdef29009f6ac387ed4c79cbc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532029"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore 资源类型

命名空间：microsoft.graph

包含基于不同范围的各种不同分数（例如，按行业垂直、按公司座位大小的平均值等）和控制类别（标识、数据、设备、应用程序、基础结构）。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|基本|字符串|范围类型。 可能的值包括 `AllTenants`、`TotalSeats`、`IndustryTypes`。|
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
