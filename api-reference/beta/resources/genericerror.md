---
title: genericError 资源类型
description: 常规用途错误。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: non-product-specific
author: abheek-das
ms.openlocfilehash: 24e54a0efb033347f9bf7479dc9592f97a5fc9e6
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899790"
---
# <a name="genericerror-resource-type"></a>genericError 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

常规用途错误。

## <a name="properties"></a>属性

| 属性 | 类型 | 描述 |
|:---------|:-----|:------------|
| message | String | 错误消息。 |
| code | String | 错误代码。 |

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


