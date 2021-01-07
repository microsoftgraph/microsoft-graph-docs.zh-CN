---
title: externalItemContent 资源类型
description: 通过 Microsoft 搜索连接编制索引的项目的内容。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 66e3fccc8c072d06d2328301100d6bf3a0d50806
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777626"
---
# <a name="externalitemcontent-resource-type"></a>externalItemContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过 Microsoft 搜索连接编制索引的 [externalItem](externalitem.md) [的内容](externalconnection.md)。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>属性

| 属性 | 类型   | 说明                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| 值    | String | externalItem 的内容。 此为必需属性。                                                 |
| type     | String | 值属性中的内容类型。 可能的值为 `text` 和 `html`。 必填。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItemContent"
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


