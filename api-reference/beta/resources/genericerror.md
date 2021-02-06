---
title: genericError 资源类型
description: 通用错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 611671cc6e35fa9376bff2761719c58f0255f19d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129448"
---
# <a name="genericerror-resource-type"></a>genericError 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通用错误。

## <a name="properties"></a>属性

| 属性 | 类型 | 描述 |
|:---------|:-----|:------------|
| message | String | 错误消息。 |
| code | 字符串 | 错误代码。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```


