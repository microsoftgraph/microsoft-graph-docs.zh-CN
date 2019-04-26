---
title: resourceReference 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: accd2b0b12f8068ea990fbd611b46053f66d6de4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339984"
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
