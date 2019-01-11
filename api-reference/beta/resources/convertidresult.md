---
title: convertIdResult 资源类型
description: 执行由 translateExchangeIds 函数 ID 格式转换的结果。
localization_priority: Normal
ms.openlocfilehash: 7e1878de3d3b7ddee36d799c928d6a130b578200
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821453"
---
# <a name="convertidresult-resource-type"></a>convertIdResult 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

执行由[translateExchangeIds](../api/user-translateexchangeids.md)函数 ID 格式转换的结果。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:---------|:-----|:------------|
| sourceId | 字符串 | 已转换的标识符。 此值是原始、 未转换标识符。 |
| targetId | 字符串 | 转换后的标识符。 此值不存在，如果转换失败。 |
| errorDetails | [genericError](genericerror.md) | Error 对象指示转换失败的原因。 此值不存在，如果转换成功。 |

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
