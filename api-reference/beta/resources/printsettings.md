---
title: printSettings 资源类型
description: 表示通用打印服务的租户范围的设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c9af888d85256b88d4212cc84ba74d8dcdd5b590
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973818"
---
# <a name="printsettings-resource-type"></a>printSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通用打印服务的租户范围的设置。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|documentConversionEnabled|Boolean|指定是否为租户启用文档转换。 如果启用了文档转换，则通用打印服务会在需要时自动将文档转换为与打印机 (xps) 兼容的格式。|

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


