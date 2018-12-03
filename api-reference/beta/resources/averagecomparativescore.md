---
title: " averageComparativeScore 资源类型"
description: 此资源包含基于按不同的作用域 （例如，平均通过行业垂直，平均按公司座位大小等） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 的各种不同分数。
ms.openlocfilehash: 08e4ec60788b21476d8f1491ab5548c7a4ca2e01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042774"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore 资源类型

此资源包含基于按不同的作用域 （例如，平均通过行业垂直，平均按公司座位大小等） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 的各种不同分数。

|属性 |类型 |Description |
|:--|:--|:--|
|   基础   |   字符串  |   范围类型 (通过 AllTenants，TotalSeats，IndustryTypes)。  |
|   averageScore    |   双精度数  | 指定基础内的平均得分。 |
|   deviceScore |   双精度数  | 指定基础内的平均得分。 |
|   dataScore   |   双精度数  | 指定基础内的平均得分。 |
|   identityScore   |   双精度数  | 指定基础内的平均得分。 |

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
