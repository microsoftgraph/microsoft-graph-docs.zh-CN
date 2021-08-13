---
title: resourceReference 资源类型
description: 包含属性的复杂Insights。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7ade1e86fc601d1f00a16136a8610634934d0b4faf7b377a85ff55cf65fab671
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152619"
---
# <a name="resourcereference-resource-type"></a>resourceReference 资源类型

命名空间：microsoft.graph

包含 [officeGraphInsights 属性的复杂类型](officegraphinsights.md)。

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
| id            | String    | 项的唯一标识符。           |
| type          | String    | 可用于对项目进行分类的字符串值，例如"microsoft.graph.driveItem" |

