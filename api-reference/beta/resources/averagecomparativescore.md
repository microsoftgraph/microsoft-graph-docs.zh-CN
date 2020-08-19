---
title: " averageComparativeScore 资源类型"
description: 此资源包含基于不同范围的不同分数 (例如，按行业垂直、按公司座位大小的平均值等，) 和控制类别 (标识、数据、设备、应用程序、基础结构) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f2ac965d4dae0b038f3aad9fe13ed57a283a42bc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812553"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore 资源类型

命名空间：microsoft.graph

此资源包含基于不同范围的不同分数 (例如，按行业垂直、按公司座位大小的平均值等，) 和控制类别 (标识、数据、设备、应用程序、基础结构) 。

|属性 |类型 |说明 |
|:--|:--|:--|
|   基本   |   String  |   AllTenants、TotalSeats、IndustryTypes)  (的作用域类型。  |
|   averageScore    |   双精度  | 指定基准中的平均分数。 |
|   deviceScore |   双精度  | 指定基准中的平均分数。 |
|   dataScore   |   双精度  | 指定基准中的平均分数。 |
|   identityScore   |   双精度  | 指定基准中的平均分数。 |

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
