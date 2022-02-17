---
title: 更改response 资源类型
description: 提供与更改响应中的拼写更正有关的信息。
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b26b3aee1db86018b8a32f5e2a4bb1b245ee7c5a
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62879265"
---
# <a name="alterationresponse-resource-type"></a>更改response 资源类型

命名空间：microsoft.graph

提供与更改响应中的拼写更正有关的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|originalQueryString|String| 定义原始用户查询字符串。|
|queryAlteration|[searchAlteration](searchalteration.md)| 定义拼写更正更改信息的详细信息。|
|queryAlterationType|searchAlterationType| 定义拼写更正的类型。 可取值为：`suggestion`、`modification`。|

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
  "queryAlterationType": "String"
}
```
