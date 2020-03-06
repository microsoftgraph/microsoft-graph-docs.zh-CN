---
title: convertIdResult 资源类型
description: 由 translateExchangeIds 函数执行的 ID 格式转换的结果。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 6eb66033ef1b0e345c3929982b9f08d6e4ce2573
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531745"
---
# <a name="convertidresult-resource-type"></a>convertIdResult 资源类型

命名空间：microsoft.graph

由[translateExchangeIds](../api/user-translateexchangeids.md)函数执行的 ID 格式转换的结果。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| sourceId | 字符串 | 已转换的标识符。 此值是未转换的原始标识符。 |
| targetId | 字符串 | 转换后的标识符。 如果转换失败，则不会出现此值。 |
| errorDetails | [genericError](genericerror.md) | 一个指示转换失败原因的 error 对象。 如果转换成功，则不会出现此值。 |

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
