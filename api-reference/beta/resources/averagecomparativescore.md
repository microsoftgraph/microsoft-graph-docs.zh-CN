---
title: " averageComparativeScore 资源类型"
description: 此资源包含根据不同范围（例如 (按行业垂直、按公司席位大小等计算的平均分数）和控件类别) Identity、数据、设备、应用、基础结构等 (评分) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 7a09d3b2c6457063457eee4a4bfbe3d1f88823f8864f66ac4a1ea690e33c77e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54210146"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore 资源类型

命名空间：microsoft.graph

此资源包含根据不同范围（例如 (按行业垂直、按公司席位大小等计算的平均分数）和控件类别) Identity、数据、设备、应用、基础结构等 (评分) 。

|属性 |类型 |说明 |
|:--|:--|:--|
|   basis   |   字符串  |   范围类型 (AllTenants、TotalSeats、IndustryTypes) 。  |
|   averageScore    |   双精度  | 指定范围内的平均分数。 |
|   deviceScore |   双精度  | 指定范围内的平均分数。 |
|   dataScore   |   双精度  | 指定范围内的平均分数。 |
|   identityScore   |   双精度  | 指定范围内的平均分数。 |

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
  "averageScore": "Double",
  "deviceScore": "Double",
  "dataScore": "Double",
  "identityScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


