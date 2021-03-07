---
title: printerCapabilities 复杂类型
description: 表示打印机报告的功能。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5416cf43e266bab65254ac5aaee1a79c9c3e17be
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516948"
---
# <a name="printercapabilities-resource-type"></a>printerCapabilities 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示打印机/打印机共享报告的功能。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|contentTypes|String collection|打印机支持的 MIME (类型) 支持的内容列表。 不保证通用打印服务支持打印所有这些 MIME 类型。|
|isColorPrintingSupported|Boolean|如此 如果打印机支持彩色打印;否则为 false。 只读。|
|feedOrientations|printerFeedOrientation 集合|打印机支持的送纸方向列表。|
|isPageRangeSupported|Boolean|如此 如果打印机支持按页范围打印;否则为 false。|
|质量|[printQuality](enums.md#printquality-values) 集合|打印机支持的打印质量。|
|dpis|Int32 集合|打印机支持的以 DPI 表示的打印分辨率列表。|
|duplexModes|[printDuplexMode](enums.md#printduplexmode-values) 集合|打印机支持的双面模式列表。 下表介绍了有效值。|
|queueBufferSizeInBytes|Int32|打印机可存储的最大打印作业队列大小。|
|copiesPerJob|[integerRange](integerrange.md)|打印机支持每个作业的副本范围。|
|finishings|[printFinishing](enums.md#printfinishing-values) 集合|打印机支持打印文档的完成过程。|
|mediaColors|String collection|媒体 (，即纸张) 打印机支持的颜色。|
|mediaTypes|String collection|打印机支持的媒体类型。 下表介绍了有效值。|
|mediaSizes|String collection|打印机支持的媒体大小。 支持 ISO 和 ANSI 媒体大小的标准大小名称，以及关联的打印机支持的任何自定义大小。|
|pagesPerSheet|Int32 集合|支持对单个展示施加的输入页面数。|
|orientations|[printOrientation](enums.md#printorientation-values) 集合|打印机支持的打印方向。 下表介绍了有效值。|
|inputBins|String collection|打印机支持的输入箱。|
|outputBins|String collection|打印机支持的输出箱 (纸盒) 。|
|supportsFitPdfToPage|Boolean|如此 如果打印机支持缩放 PDF 页面以匹配打印媒体大小;否则为 false。|
|multipageLayouts|[printMultipageLayout](enums.md#printmultipagelayout-values) 集合|打印机支持的演示方向。 下表介绍了受支持的值。|
|colorModes|[printColorMode](enums.md#printcolormode-values) 集合|打印机支持的颜色模式。 下表介绍了有效值。|
|topMargins|Int32 集合|支持的上边距列表 (打印机) 以密) 。|
|bottomMargins|Int32 集合|支持的底部边距列表 (打印机) 以密) 。|
|rightMargins|Int32 集合|支持的右边距列表 (以) 以小数表示。|
|leftMargins|Int32 集合|打印机支持的左边距 (以) 以密分表示。|
|collation|Boolean|如此 如果打印多页文档的副本时打印机支持整理;否则为 false。|
|scalings|[printScaling](enums.md#printscaling-values) 集合|支持的打印缩放。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerCapabilities"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCapabilities",
  "contentTypes": [
    "String"
  ],
  "isColorPrintingSupported": "Boolean",
  "feedOrientations": [
    "String"
  ],
  "isPageRangeSupported": "Boolean",
  "qualities": [
    "String"
  ],
  "dpis": [
    "Integer"
  ],
  "duplexModes": [
    "String"
  ],
  "copiesPerJob": {
    "@odata.type": "microsoft.graph.integerRange"
  },
  "finishings": [
    "String"
  ],
  "mediaColors": [
    "String"
  ],
  "mediaTypes": [
    "String"
  ],
  "mediaSizes": [
    "String"
  ],
  "pagesPerSheet": [
    "Integer"
  ],
  "orientations": [
    "String"
  ],
  "outputBins": [
    "String"
  ],
  "supportsFitPdfToPage": "Boolean",
  "multipageLayouts": [
    "String"
  ],
  "colorModes": [
    "String"
  ],
  "inputBins": [
    "String"
  ],
  "topMargins": [
    "Integer"
  ],
  "bottomMargins": [
    "Integer"
  ],
  "rightMargins": [
    "Integer"
  ],
  "leftMargins": [
    "Integer"
  ],
  "collation": "Boolean",
  "scalings": [
    "String"
  ]
}
```

