---
title: printerDefaults 资源类型
description: 表示打印机的默认设置。 检查打印机的功能以查看它支持的所有值。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fbee453d42fbcb056ce3dce3ff7311e4d976b7dc
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516949"
---
# <a name="printerdefaults-resource-type"></a>printerDefaults 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示打印机的默认设置。 检查打印机 [的功能以查看](printercapabilities.md) 它支持的所有值。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|copiesPerJob|Int32|每个作业打印的默认副本数。|
|contentType|String|处理文档 (MIME) 类型。|
|finishings|[printFinishing](enums.md#printfinishing-values) 集合|要应用于打印作业的默认完成项集。 下表介绍了有效值。|
|mediaColor|String|默认媒体 (打印文档) 纸张颜色等。
|mediaType|String|默认媒体 (类型，例如) 打印文档的纸张类型。 下表介绍了有效值。|
|mediaSize|String|使用的默认媒体大小。 支持 ISO 和 ANSI 媒体大小的标准大小名称，以及关联的打印机支持的任何自定义大小。
|pagesPerSheet|Int32|要在每个工作表上打印的默认文档页数。
|orientation|[printOrientation](enums.md#printorientation-values)|打印文档时使用的默认方向。 下表介绍了有效值。|
|outputBin|String|要放置已完成打印的默认输出箱。 有关受支持的 [输出箱](printercapabilities.md) 的列表，请参阅打印机的功能。|
|fitPdfToPage|Boolean|默认的 fitPdfToPage 设置。 True 表示 PDF 文档的每一页都适合媒体的物理工作表;false，让打印机决定如何设置展示次数。|
|multipageLayout|[printMultipageLayout](enums.md#printmultipagelayout-values)|当每张工作表打印多个页面时，页面布局的默认方向。 下表介绍了有效值。|
|colorMode|[printColorMode](enums.md#printcolormode-values)|打印文档时使用的默认颜色模式。 下表介绍了有效值。|
|quality|[printQuality](enums.md#printquality-values)|打印文档时使用的默认质量。 下表介绍了有效值。|
|duplexMode|[printDuplexMode](enums.md#printduplexmode-values)|默认双面 (双面) 打印文档时使用的配置。 下表介绍了有效值。|
|dpi|Int32|打印作业时使用的默认分辨率（DPI）。|
|scaling|[printScaling](enums.md#printscaling-values)|指定打印机如何缩放文档数据以适应请求的媒体。 下表介绍了有效值。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerDefaults"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerDefaults",
  "copiesPerJob": "Integer",
  "contentType": "String",
  "finishings": [
    "String"
  ],
  "mediaColor": "String",
  "mediaType": "String",
  "mediaSize": "String",
  "pagesPerSheet": "Integer",
  "orientation": "String",
  "outputBin": "String",
  "inputBin": "String",
  "fitPdfToPage": "Boolean",
  "multipageLayout": "String",
  "colorMode": "String",
  "quality": "String",
  "duplexMode": "String",
  "dpi": "Integer",
  "scaling": "String"
}
```

