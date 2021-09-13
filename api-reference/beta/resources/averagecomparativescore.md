---
title: " averageComparativeScore 资源类型"
description: 此资源包含根据不同范围（例如 (按行业垂直、按公司席位大小等计算的平均分数）和控件类别) 和控制类别 (Identity、数据、设备、应用、基础结构) 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 4c563d8754ba5afb1c4fe89d237f978d886f9eab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064607"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore 资源类型

命名空间：microsoft.graph

此资源包含根据不同范围（例如 (按行业垂直、按公司席位大小等计算的平均分数）和控件类别) 和控制类别 (Identity、数据、设备、应用、基础结构) 。

|属性 |类型 |描述 |
|:--|:--|:--|
|   basis   |   String  |   范围类型 (AllTenants、TotalSeats、IndustryTypes) 。  |
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


