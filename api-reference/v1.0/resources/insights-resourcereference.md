---
title: resourceReference 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c75eab84dea4e0f9134185fd9679770369073bf4
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844355"
---
# <a name="resourcereference-resource-type"></a>resourceReference 资源类型

包含[officeGraphInsights](officegraphinsights.md)的属性的复杂类型。

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
| webUrl        | String    | 指向引用项的 URL。 |
| id            | String    | 项目的唯一标识符。           |
| type          | String    | 一个可用于对项目进行分类的字符串值，例如 "driveItem" |
