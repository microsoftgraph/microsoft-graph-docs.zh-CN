---
title: externalItemContent 资源类型
description: 通过连接建立索引的项目Microsoft 搜索内容。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d895d0056da71ea065dbc62d08c9deda054a6f29
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467664"
---
# <a name="externalitemcontent-resource-type"></a>externalItemContent 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过连接[建立索引的 externalItem](externalconnectors-externalitem.md) Microsoft 搜索[内容](externalconnectors-externalconnection.md)。

## <a name="properties"></a>属性

| 属性 | 类型   | 说明                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| 值    | String | externalItem 的内容。 此为必需属性。                                                 |
| type     | String | value 属性中的内容类型。 可能的值为 `text` 和 `html`。 必填。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
}-->

```json
{
  "value": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItemContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->