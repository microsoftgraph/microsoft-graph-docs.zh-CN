---
title: convertIdResult 资源类型
description: translateExchangeIds 函数执行的 ID 格式转换的结果。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: eafc37f017c7f074c971d12b3b8e16d8da24b850
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136771"
---
# <a name="convertidresult-resource-type"></a>convertIdResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[translateExchangeIds](../api/user-translateexchangeids.md)函数执行的 ID 格式转换的结果。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| sourceId | 字符串 | 已转换的标识符。 此值为原始的未转换标识符。 |
| targetId | 字符串 | 转换后的标识符。 如果转换失败，则此值不存在。 |
| errorDetails | [genericError](genericerror.md) | 指示转换失败原因的错误对象。 如果转换成功，则此值不存在。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```


