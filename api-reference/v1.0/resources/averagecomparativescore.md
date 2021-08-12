---
title: averageComparativeScore 资源类型
description: 包含基于不同范围的各种不同分数。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2041a366fcf37ff8a850fb8d6fd41e9c3fd6002a17916d41718588674a30a3e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54147019"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore 资源类型

命名空间：microsoft.graph

包含基于不同范围的不同分数 (例如，按行业垂直平均、按公司席位大小等进行平均分数) 控制类别 (标识、数据、设备、应用、基础结构) 。

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

