---
title: averageComparativeScore 资源类型
description: 包含基于不同范围的各种不同分数。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 88444bfab00622a6ac8cc89a3af287650ad1af7e
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899972"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore 资源类型

命名空间：microsoft.graph

包含基于不同范围的各种不同分数 (例如，按行业垂直平均值、按公司席位大小平均值等) 和控制类别 (标识、数据、设备、应用、基础结构) 。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|基础|String|范围类型。 可能的值包括 `AllTenants`、`TotalSeats`、`IndustryTypes`。|
|averageScore|双精度|指定基础内的平均分数。|

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

