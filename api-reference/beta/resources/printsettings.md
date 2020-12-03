---
title: printSettings 资源类型
description: 表示通用打印服务的租户范围的设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 01c98eb68031018e6f7a32837e49a2095c7880d2
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521234"
---
# <a name="printsettings-resource-type"></a>printSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通用打印服务的租户范围的设置。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|documentConversionEnabled|布尔值|指定是否为租户启用文档转换。 如果启用了文档转换，则通用打印服务会在需要时自动将文档转换为与打印机 (xps) 兼容的格式。|

## <a name="json-representation"></a>JSON 表示形式

以下是 printSettings 的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printSettings"
}-->

```json
{
  "documentConversionEnabled": true
}
```


