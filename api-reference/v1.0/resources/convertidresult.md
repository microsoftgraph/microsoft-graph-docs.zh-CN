---
title: convertIdResult 资源类型
description: translateExchangeIds 函数执行的 ID 格式转换的结果。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: ec94f586f0f8233f1b56965f4dea4640360b63eb43f9d1fae69988ae61d401e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155160"
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

