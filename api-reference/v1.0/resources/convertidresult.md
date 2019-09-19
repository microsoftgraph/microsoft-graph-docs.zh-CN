---
title: convertIdResult 资源类型
description: 由 translateExchangeIds 函数执行的 ID 格式转换的结果。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 405d663e4f1f7fb040e79cdd10669bc824e3edef
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036443"
---
# <a name="convertidresult-resource-type"></a>convertIdResult 资源类型

由[translateExchangeIds](../api/user-translateexchangeids.md)函数执行的 ID 格式转换的结果。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| sourceId | String | 已转换的标识符。 此值是未转换的原始标识符。 |
| targetId | String | 转换后的标识符。 如果转换失败，则不会出现此值。 |
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
