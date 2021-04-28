---
title: 更改response 资源类型
description: 提供与更改响应中的拼写更正有关的信息。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e23b94b4e35776b2278c7818efc71f14edcc6cbb
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067996"
---
# <a name="alterationresponse-resource-type"></a>更改response 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供与更改响应中的拼写更正有关的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|originalQueryString|String| 定义原始用户查询字符串。|
|queryAlteration|[searchAlteration](searchalteration.md)| 定义拼写更正更改信息的详细信息。|
|queryAlterationType|searchAlterationType| 定义拼写更正的类型。 可能的值是 `suggestion` `modification` 、。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alterationResponse",
  "baseType": null
}-->

```json
{
  "originalQueryString": "String",
  "queryAlteration": "String",
  "queryAlterationType": "suggestion"
}
```
