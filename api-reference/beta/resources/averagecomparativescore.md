---
title: " averageComparativeScore 资源类型"
description: 此资源包含基于按不同的作用域 （例如，平均通过行业垂直，平均按公司座位大小等） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 的各种不同分数。
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834592"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore 资源类型

此资源包含基于按不同的作用域 （例如，平均通过行业垂直，平均按公司座位大小等） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 的各种不同分数。

|属性 |类型 |Description |
|:--|:--|:--|
|   基础   |   字符串  |   范围类型 (通过 AllTenants，TotalSeats，IndustryTypes)。  |
|   averageScore    |   Double  | 指定基础内的平均得分。 |
|   deviceScore |   Double  | 指定基础内的平均得分。 |
|   dataScore   |   Double  | 指定基础内的平均得分。 |
|   identityScore   |   Double  | 指定基础内的平均得分。 |

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
