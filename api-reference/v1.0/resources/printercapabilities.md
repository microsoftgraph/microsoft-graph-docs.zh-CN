---
title: printerCapabilities 复杂类型
description: 表示打印机报告的功能。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: bda913275aff692df2f66472f61436665cbc3dd7
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944224"
---
# <a name="printercapabilities-resource-type"></a>printerCapabilities 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示 printer/printerShare 报告的功能。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|contentTypes|字符串集合|受支持内容列表 (打印机) 类型的 MIME。 不保证通用打印服务支持打印所有这些 MIME 类型。|
|isColorPrintingSupported|布尔|如此 如果打印机支持彩色打印;否则为 false。 只读。|
|feedOrientations|printerFeedOrientation 集合|打印机支持的送纸方向列表。|
|isPageRangeSupported|布尔|如此 如果打印机支持按页范围打印;否则为 false。|
|一些|[printQuality](enums.md#printquality-values) 集合|打印机支持的打印质量。|
|dpis|Int32 集合|打印机支持的以 DPI 表示的打印分辨率列表。|
|duplexModes|[printDuplexMode](enums.md#printduplexmode-values) 集合|打印机支持的双面模式列表。 下表介绍了有效值。|
|queueBufferSizeInBytes|Int32|打印机可以存储的最大打印作业队列大小。|
|copiesPerJob|[integerRange](integerrange.md)|打印机支持每个作业的副本范围。|
|finishings|[printFinishing](enums.md#printfinishing-values) 集合|打印机对打印文档支持的完成过程。|
|mediaColors|字符串集合|媒体 (即纸张) 打印机支持的颜色。|
|mediaTypes|字符串集合|打印机支持的媒体类型。|
|mediaSizes|字符串集合|打印机支持的媒体大小。 支持 ISO 和 ANSI 媒体大小的标准大小名称。 有效值如下表 [所示](#mediasizes-values)。|
|pagesPerSheet|Int32 集合|支持对单个展示施加的输入页面数。|
|orientations|[printOrientation](enums.md#printorientation-values) 集合|打印机支持的打印方向。 下表介绍了有效值。|
|inputBins|字符串集合|打印机支持的输入箱。|
|outputBins|字符串集合|打印机支持的输出箱 (纸盒) 。|
|supportsFitPdfToPage|布尔|如此 如果打印机支持缩放 PDF 页面以匹配打印媒体大小;否则为 false。|
|multipageLayouts|[printMultipageLayout](enums.md#printmultipagelayout-values) 集合|打印机支持的演示文稿方向。 下表介绍了支持的值。|
|colorModes|[printColorMode](enums.md#printcolormode-values) 集合|打印机支持的颜色模式。 下表介绍了有效值。|
|topMargins|Int32 集合|打印机支持的上边距 (以) 表示。|
|bottomMargins|Int32 集合|支持的底部边距列表 (打印机) 以百分之位表示。|
|rightMargins|Int32 集合|打印机支持的右边距 (以) 表示。|
|leftMargins|Int32 集合|支持的左边距列表 (打印机) 的边距。|
|collation|布尔|如此 如果打印机支持逐份打印多页文档的副本;否则为 false。|
|scalings|[printScaling](enums.md#printscaling-values) 集合|支持的打印缩放。|

### <a name="mediasizes-values"></a>mediaSizes 值

|值|
|:---|
|A3|
|A4|
|A5|
|A6|
|JIS B4|
|JIS B5|
|JPN Hag一|
|北美 5x7in|
|北美管理人员|
|北美 Goverment 信函|
|北美索引 3x5in|
|北美索引 4x8in|
|北美索引 5x8in|
|北美发票|
|北美分类帐|
|北美法律|
|北美字母|
|Photo l 3.5x5in|
|名片|
|Photo|

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

