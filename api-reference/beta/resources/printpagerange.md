---
title: printPageRange 资源类型
description: 指定要打印的页面范围。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a8bbf452c337cb5c2ade7302eb29cff4bdb73d23
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052536"
---
# <a name="printpagerange-resource-type"></a>printPageRange 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定要打印的页面范围。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|startPage|Int32|范围 (包含) 的起始页。 只读。|
|endPage|Int32|区域 (包含) 的最后一页。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printPageRange"
}-->

```json
{
  "startPage": 123456,
  "endPage": 123456
}
```


