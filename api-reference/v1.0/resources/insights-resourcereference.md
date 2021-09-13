---
title: resourceReference 资源类型
description: 包含属性的复杂Insights。
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c7694aa2c9a487a3e07ce99d9850445de26c3acb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123361"
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

