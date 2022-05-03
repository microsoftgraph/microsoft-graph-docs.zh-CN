---
title: printSettings 资源类型
description: 表示通用打印服务的租户范围设置。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0339843083695904080104882ba9385a840b4c9e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176650"
---
# <a name="printsettings-resource-type"></a>printSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通用打印服务的租户范围设置。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|documentConversionEnabled|Boolean|指定是否为租户启用文档转换。 如果启用文档转换，则通用打印服务会根据需要自动将文档转换为与打印机兼容的格式 (xps 转换为 pdf) 。|

## <a name="json-representation"></a>JSON 表示形式

下面是 printSettings 的 JSON 表示形式。
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


