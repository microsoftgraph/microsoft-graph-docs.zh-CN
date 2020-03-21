---
title: printSettings 资源类型
description: 表示通用打印服务的租户范围的设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 08d8409113c9c2f480200999c47ca18c300f245f
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895622"
---
# <a name="printsettings-resource-type"></a>printSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通用打印服务的租户范围的设置。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|documentConversionEnabled|布尔|指定是否为租户启用文档转换。 如果启用了文档转换，则通用打印服务会在需要时自动将文档转换为与打印机兼容的格式（xps 到 pdf）。|

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
