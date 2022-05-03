---
title: printerCapabilities 复杂类型
description: 表示打印机报告的功能。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 045fd0b29b1cf6c1baa0d70659556d2f49a3391c
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176365"
---
# <a name="printercapabilities-complex-type"></a>printerCapabilities 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印机报告的功能。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|contentTypes|String collection|支持的内容列表 (MIME) 打印机支持的类型。 不能保证通用打印服务支持打印所有这些 MIME 类型。|
|isColorPrintingSupported|Boolean|如此 如果打印机支持颜色打印;否则为 false。 只读。|
|feedOrientations|printerFeedOrientation 集合|打印机支持的源方向列表。|
|isPageRangeSupported|Boolean|如此 如果打印机支持按页范围打印;否则为 false。|
|素质|printQuality 集合|打印机支持的打印质量。|
|dpis|Int32 集合|打印机支持的 DPI 中的打印分辨率列表。|
|duplexModes|printDuplexMode 集合|打印机支持的双工模式列表。 下表描述了有效值。|
|queueBufferSizeInBytes|Int32|打印机可以存储的最大打印作业队列大小。|
|copiesPerJob|[integerRange](integerrange.md)|打印机支持的每个作业的副本范围。|
|finishings|printFinishing 集合|打印机支持打印文档的完成过程。|
|mediaColors|String collection|媒体 (，即打印机支持的纸张) 颜色。|
|mediaTypes|String collection|打印机支持的媒体类型。|
|mediaSizes|String collection|打印机支持的媒体大小。 支持 ISO 和 ANSI 媒体大小的标准大小名称。 有效值位于下 [表](#mediasizes-values)中。|
|pagesPerSheet|Int32 集合|支持对单个印象施加的输入页数。|
|取向|printOrientation 集合|打印机支持的打印方向。 下表描述了有效值。|
|inputBins|String collection|打印机支持的输入箱。|
|outputBins|String collection|打印机支持的输出箱 (托盘) 。|
|supportsFitPdfToPage|Boolean|如此 如果打印机支持缩放 PDF 页面以匹配打印媒体大小;否则为 false。|
|multipageLayouts|printMultipageLayout 集合|打印机支持的演示说明。 下表描述了支持的值。|
|colorModes|printColorMode 集合|打印机支持的颜色模式。 下表描述了有效值。|
|topMargins|Int32 集合|打印机) 中支持的顶级边距 (列表。|
|bottomMargins|Int32 集合|打印机) 中支持的底边距 (的列表。|
|rightMargins|Int32 集合|打印机) 中支持的右边距 (的列表。|
|leftMargins|Int32 集合|打印机的) 中支持的左侧边距 (列表。|
|collation|Boolean|如此 如果打印机支持在打印多页文档的粘合副本时进行排序;否则为 false。|
|scalings|printScaling 集合|支持的打印缩放。|

## <a name="printerfeedorientation-values"></a>printerFeedOrientation 值

|成员|值|Description|
|:---|:---|
|longEdgeFirst|0|打印机将在“横向”方向使用活动托盘中的工作表，其中首先使用工作表的长边缘。|
|shortEdgeFirst|1|打印机将以“纵向”方向使用活动托盘中的工作表，并首先使用工作表的短边缘。|
|unknownFutureValue|2|可变枚举 sentinel 值。 请勿使用。|

### <a name="printquality-values"></a>printQuality 值

|成员|值|Description|
|:---|:---|
|低|0|打印机将使用低 (通常称为“草稿”) 质量打印作业。|
|中等|1|打印机将使用 medim 打印作业 (通常称为“普通”) 质量。|
|高|2|打印机将使用高 (通常称为“最佳”或“精细”) 质量来打印作业。|
|unknownFutureValue|3|可变枚举 sentinel 值。 请勿使用。|

### <a name="printduplexmode-values"></a>printDuplexMode 值

|成员|值|Description|
|:---|:---|:---|
|flipOnLongEdge|0|打印机将双面打印，并将沿长边缘翻转文档。|
|flipOnShortEdge|1|打印机将双面打印，并将沿短边缘翻转文档。|
|oneSided|2|打印机将单面打印。|

### <a name="printfinishing-values"></a>printFinishing 值

|成员|值|Description|
|:---|:---|:---|
|无|3|无完成。 包含此值等效于提供空的完成集合。|
|短|4|使用打印机的默认装入配置对文档进行装订。|
|冲床|5|使用打印机的默认孔冲孔配置打孔文档。|
|覆盖|6 |将封面应用到文档。|
|绑定|7 |使用打印机的默认绑定配置绑定文档。|
|saddleStitch|8 |使用打印机的默认拼接配置对文档进行修补。|
|stitchEdge|9 |使用打印机的默认拼接配置对文档进行边缘缝合。|
|stapleTopLeft|20|在左上角键入文档。|
|stapleBottomLeft| 21|在左下角键入文档。|
|stapleTopRight|22|在右上角键入文档。|
|stapleBottomRight|23|将文档装订到右下角。|
|stitchLeftEdge|24|沿左边缘边缘缝合文档。|
|stitchTopEdge|25|沿上边缘边缘缝合文档。|
|stitchRightEdge|26|沿右边缘边缘缝合文档。|
|stitchBottomEdge|27|沿底部边缘边缘缝合文档。|
|stapleDualLeft|28|沿左边缘键入文档两次。|
|stapleDualTop|29|沿着上边缘对文档进行两次装订。|
|stapleDualRight|30|沿着右边缘对文档进行两次装订。|
|stapleDualBottom|31|沿着底部边缘对文档进行两次装订。|
|unknownFutureValue|32|可变枚举 sentinel 值。 请勿使用。|

## <a name="printorientation-values"></a>printOrientation 值

|成员|值|Description|
|:---|:---|:---|
|肖像|3|打印机将以“纵向”方向打印印象。|
|景观|4|打印机将以“横向”方向打印印象。|
|reverseLandscape|5|打印机将以“反向横向”方向打印印象。|
|reversePortrait|6 |打印机将以“反向纵向”方向打印印象。|

### <a name="printmultipagelayout-values"></a>printMultipageLayout 值

|成员|值|Description|
|:---|:---|:---|
|clockwiseFromTopLeft|0|从左上角开始，在顺时针网格中排列页面。|
|counterclockwiseFromTopLeft|1|从左上角开始，在逆时针网格中排列页面。|
|counterclockwiseFromTopRight|2|从右上角开始，在逆时针网格中排列页面。|
|clockwiseFromTopRight|3|从右上角开始，在顺时针网格中排列页面。|
|counterclockwiseFromBottomLeft|4|从左下角开始，在逆时针网格中排列页面。|
|clockwiseFromBottomLeft|5|从左下角开始，在顺时针网格中排列页面。|
|counterclockwiseFromBottomRight|6 |从右下角开始，在逆时针网格中排列页面。|
|clockwiseFromBottomRight|7 |从右下角开始，在顺时针网格中排列页面。|

### <a name="printcolormode-values"></a>printColorMode 值

|成员|值|Description|
|:---|:---|:---|
|blackAndWhite|0|黑白 (只使用黑色标记材料。) |
|灰度|1|灰度 (可能使用一些颜色标记材料。) |
|颜色|2|颜色 (使用标记材料的任何组合来创建颜色印象) 。|
|自动|3|让打印机决定要使用的颜色模式。|

### <a name="printscaling-values"></a>printScaling 值

|成员|值|Description|
|:---|:---|:---|
|自动|0|如果文档大于请求的媒体且边距为非零，则打印机会缩放文档，如 **拟合** printScaling。 否则，打印机将使用 **填充** printScaling 缩放文档。 如果文档小于请求的媒体，则使用“无”printScaling。|
|shrinkToFit|1|如果文档大于请求的媒体，打印机会缩放文档，如 **拟合** printScaling。 否则，打印机会缩放文档，就像 **无** 打印缩放一样。|
|fill|2|打印机缩放文档以填充请求的媒体大小，保留其纵横比，但可能会裁剪文档的部分。|
|适合|3|打印机缩放文档以适应所请求媒体大小的可打印区域，在不裁剪文档的情况下保留文档数据的纵横比。|
|无|4|打印机不缩放文档以适应所请求的媒体大小。 如果文档大于请求的媒体，打印机会居中并剪辑生成的输出。 如果文档小于请求的媒体，打印机将生成的输出居中。|
|unknownFutureValue|5|可变枚举 sentinel 值。 请勿使用。|

### <a name="mediasizes-values"></a>mediaSizes 值

|值|
|:---|
|A3|
|A4|
|A5|
|A6|
|JIS B4|
|JIS B5|
|JPN Hagaki|
|北美 5x7in|
|北美执行|
|北美文字母|
|北美索引 3x5in|
|北美索引 4x8in|
|北美索引 5x8in|
|北美发票|
|北美账本|
|北美法律|
|北美字母|
|照片 l 3.5x5in|
|名片|
|Photo|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerCapabilities"
}-->

```json
{
  "contentTypes": [""],
  "isColorPrintingSupported": true,
  "feedOrientations": [{"@odata.type": "microsoft.graph.printerFeedOrientation"}],
  "isPageRangeSupported": true,
  "qualities": [{"@odata.type": "microsoft.graph.printQuality"}],
  "dpis": [12345],
  "duplexModes": [{"@odata.type": "microsoft.graph.printDuplexMode"}],
  "queueBufferSizeInBytes": 12345,
  "copiesPerJob": {"@odata.type": "microsoft.graph.integerRange"},
  "finishings": [{"@odata.type": "microsoft.graph.printFinishing"}],
  "mediaColors": [""],
  "mediaTypes": [""],
  "mediaSizes": [""],
  "pagesPerSheet": [12345],
  "orientations": [{"@odata.type": "microsoft.graph.printOrientation"}],
  "inputBins": [""],
  "outputBins": [""],
  "supportsFitPdfToPage": true,
  "multipageLayouts": [{"@odata.type": "microsoft.graph.printMultipageLayout"}],
  "colorModes": [{"@odata.type": "microsoft.graph.printColorMode"}],
  "topMargins": [12345],
  "bottomMargins": [12345],
  "rightMargins": [12345],
  "leftMargins": [12345],
  "collation": true,
  "scalings": [{"@odata.type": "microsoft.graph.printScaling"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerCapabilities resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

