---
title: printPageRange 资源类型
description: 指定要打印的页面范围。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: a8bd855bc4b7d561d9157923d7ce3ace8323b899
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176884"
---
# <a name="printpagerange-resource-type"></a>printPageRange 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定要打印的页面范围。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|startPage|Int32|范围的起始页 (非独占) 。 只读。|
|endPage|Int32|结束页 (区域的非独占) 。 只读。|

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
  "startPage": "Int32",
  "endPage": "Int32"
}
```


