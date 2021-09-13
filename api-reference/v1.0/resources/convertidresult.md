---
title: convertIdResult 资源类型
description: translateExchangeIds 函数执行的 ID 格式转换的结果。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: e2bb28e7ee4d889fec24152de27e37399e8acfa1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59053152"
---
# <a name="convertidresult-resource-type"></a>convertIdResult 资源类型

命名空间：microsoft.graph

[translateExchangeIds](../api/user-translateexchangeids.md)函数执行的 ID 格式转换的结果。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| sourceId | String | 已转换的标识符。 此值为未转换的原始标识符。 |
| targetId | String | 转换后的标识符。 如果转换失败，则此值不存在。 |
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

