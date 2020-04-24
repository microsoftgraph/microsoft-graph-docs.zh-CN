---
title: externalItemContent 资源类型
description: 通过 Microsoft Search 连接编制索引的项目的内容。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: db0276307e824faa0c5606a8fb1212a0ad25e654
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805659"
---
# <a name="externalitemcontent-resource-type"></a>externalItemContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过 Microsoft Search[连接](externalconnection.md)编制索引的[externalItem](externalitem.md)的内容。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>属性

| 属性 | 类型   | 说明                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| 值    | String | ExternalItem 的内容。 此为必需属性。                                                 |
| type     | 字符串 | Value 属性中的内容类型。 可能的值为 `text` 和 `html`。 必需。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItemContent",
  "baseType": ""
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
