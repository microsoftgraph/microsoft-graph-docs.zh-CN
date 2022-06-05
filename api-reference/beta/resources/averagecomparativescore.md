---
title: " averageComparativeScore 资源类型"
description: 此资源包含基于不同范围的各种不同分数 (例如，按行业垂直平均、按公司席位大小平均等) 和控制类别 (标识、数据、设备、应用、基础结构) 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: b5cf6482b76180a64e2ec468648a48113377114d
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900210"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore 资源类型

命名空间：microsoft.graph

此资源包含基于不同范围的各种不同分数 (例如，按行业垂直平均、按公司席位大小平均等) 和控制类别 (标识、数据、设备、应用、基础结构) 。

|属性 |类型 |说明 |
|:--|:--|:--|
|   基础   |   字符串  |   按 AllTenants、TotalSeats、IndustryTypes)  (的范围类型。  |
|   averageScore    |   双精度  | 指定基础内的平均分数。 |
|   deviceScore |   双精度  | 指定基础内的平均分数。 |
|   dataScore   |   双精度  | 指定基础内的平均分数。 |
|   identityScore   |   双精度  | 指定基础内的平均分数。 |

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


