---
title: resourceReference 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 06a8d99ba01a8a3fd3d171b800345f81b0819de0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005721"
---
# <a name="resourcereference-resource-type"></a>resourceReference 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含[见解](officegraphinsights.md)的属性的复杂类型。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a>属性

| 属性      | 类型      | 说明  |
| ------------- |-----------| -------------|
| WebUrl        | String    | 指向引用项的 URL。 |
| id            | String    | 项目的唯一标识符。           |
| type          | String    | 一个可用于对项目进行分类的字符串值, 例如 "driveItem" |
