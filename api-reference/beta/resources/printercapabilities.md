---
title: printerCapabilities 复杂类型
description: 表示打印机报告的功能。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 37e011eedfe00d905f4bf862327e948787207270
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944140"
---
# <a name="printercapabilities-complex-type"></a>printerCapabilities 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印机报告的功能。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|contentTypes|字符串集合|受支持内容列表 (打印机) 类型的 MIME。 不保证通用打印服务支持打印所有这些 MIME 类型。|
|isColorPrintingSupported|布尔|如此 如果打印机支持彩色打印;否则为 false。 只读。|
|feedOrientations|printerFeedOrientation 集合|打印机支持的送纸方向列表。|
|isPageRangeSupported|布尔|如此 如果打印机支持按页范围打印;否则为 false。|
|一些|printQuality 集合|打印机支持的打印质量。|
|dpis|Int32 集合|打印机支持的以 DPI 表示的打印分辨率列表。|
|duplexModes|printDuplexMode 集合|打印机支持的双面模式列表。 下表介绍了有效值。|
|queueBufferSizeInBytes|Int32|打印机可以存储的最大打印作业队列大小。|
|copiesPerJob|[integerRange](integerrange.md)|打印机支持每个作业的副本范围。|
|finishings|printFinishing 集合|打印机对打印文档支持的完成过程。|
|mediaColors|字符串集合|媒体 (即纸张) 打印机支持的颜色。|
|mediaTypes|字符串集合|打印机支持的媒体类型。|
|mediaSizes|字符串集合|打印机支持的媒体大小。 支持 ISO 和 ANSI 媒体大小的标准大小名称。 有效值如下表 [所示](#mediasizes-values)。|
|pagesPerSheet|Int32 集合|支持对单个展示施加的输入页面数。|
|orientations|printOrientation 集合|打印机支持的打印方向。 下表介绍了有效值。|
|inputBins|字符串集合|打印机支持的输入箱。|
|outputBins|字符串集合|打印机支持的输出箱 (纸盒) 。|
|supportsFitPdfToPage|布尔|如此 如果打印机支持缩放 PDF 页面以匹配打印媒体大小;否则为 false。|
|multipageLayouts|printMultipageLayout 集合|打印机支持的演示文稿方向。 下表介绍了支持的值。|
|colorModes|printColorMode 集合|打印机支持的颜色模式。 下表介绍了有效值。|
|topMargins|Int32 集合|打印机支持的上边距 (以) 表示。|
|bottomMargins|Int32 集合|支持的底部边距列表 (打印机) 以百分之位表示。|
|rightMargins|Int32 集合|打印机支持的右边距 (以) 表示。|
|leftMargins|Int32 集合|支持的左边距列表 (打印机) 的边距。|
|collation|布尔|如此 如果打印机支持逐份打印多页文档的副本;否则为 false。|
|scalings|printScaling 集合|支持的打印缩放。|

## <a name="printerfeedorientation-values"></a>printerFeedOrientation 值

|成员|值|说明|
|:---|:---|
|longEdgeFirst|0|打印机将在"横向"方向使用活动纸盒中的纸张，首先使用纸张的长边缘。|
|shortEdgeFirst|1|打印机将在"纵向"方向使用活动纸盒中的纸张，首先使用纸张的短边缘。|
|unknownFutureValue|2|可发展枚举 sentinel 值。 请勿使用。|

### <a name="printquality-values"></a>printQuality 值

|成员|值|说明|
|:---|:---|
|low|0|打印机使用通常称为"草稿 ("低质量打印) 作业。|
|中等|1|打印机使用 medim 打印作业 (通常称为"正常") 质量。|
|high|2|打印机会使用通常称为"最好"或 (质量"的高性能打印) 作业。|
|unknownFutureValue|3|可发展枚举 sentinel 值。 请勿使用。|

### <a name="printduplexmode-values"></a>printDuplexMode 值

|成员|值|说明|
|:---|:---|:---|
|flipOnLongEdge|0|打印机将进行双面打印，并沿长边翻转文档。|
|flipOnShortEdge|1|打印机将进行双面打印，并沿短边翻转文档。|
|oneSided|2|打印机将单面打印。|

### <a name="printfinishing-values"></a>printFinishing 值

|成员|值|说明|
|:---|:---|:---|
|无|3|没有完成。 包括此值等效于提供一个空的完成集合。|
|装订|4 |使用打印机的默认装订配置装订文档。|
|一个|5 |使用打印机的默认内径配置将文档内径。|
|cover|6 |将封面应用于文档。|
|bind|7 |使用打印机的默认绑定配置绑定文档。|
|一些|8 |使用打印机的默认连接配置来安装文档。|
|一些|9 |使用打印机的默认连接配置边缘连接文档。|
|stapleTopLeft|20|将文档装订在左上角。|
|装订BottomLeft| 21|将文档装订在左下角。|
|stapleTopRight|22|将文档装订在右上角。|
|装订BottomRight|23|将文档装订在右下角。|
|将leftEdge|24|将文档沿左边缘进行边缘装订。|
|将topEdge|25|将文档沿上边缘进行边缘装订。|
|将rightEdge|26|将文档沿右边缘进行边缘装订。|
|将bottomEdge|27|将文档沿下边缘进行边缘装订。|
|stapleDualLeft|28|沿左边缘装订文档两次。|
|stapleDualTop|29|沿上边缘装订文档两次。|
|stapleDualRight|30|沿右边缘装订文档两次。|
|stapleDualBottom|31|沿下边缘装订文档两次。|
|unknownFutureValue|32|可发展枚举 sentinel 值。 请勿使用。|

## <a name="printorientation-values"></a>printOrientation 值

|成员|值|说明|
|:---|:---|:---|
|纵向|3|打印机将打印"纵向"方向的展示。|
|横向|4 |打印机将打印"横向"方向的打印展示。|
|reverseLandscape|5 |打印机将打印"反向横向"方向的打印展示。|
|reversePortrait|6 |打印机将打印"反向纵向"方向的展示。|

### <a name="printmultipagelayout-values"></a>printMultipageLayout 值

|成员|值|说明|
|:---|:---|:---|
|顺时针FromTopLeft|0|从左上开始按顺时针网格排列页面。|
|counterclockwiseFromTopLeft|1|从左上开始按逆时针网格排列页面。|
|counterclockwiseFromTopRight|2|从右上方开始按逆时针网格排列页面。|
|clockwiseFromTopRight|3|从右上开始按顺时针网格排列页面。|
|counterclockwiseFromBottomLeft|4 |从左下角开始按逆时针网格排列页面。|
|顺时针FromBottomLeft|5 |从左下角开始按顺时针网格排列页面。|
|counterclockwiseFromBottomRight|6 |从右下角开始按逆时针网格排列页面。|
|clockwiseFromBottomRight|7 |从右下角开始按顺时针网格排列页面。|

### <a name="printcolormode-values"></a>printColorMode 值

|成员|值|说明|
|:---|:---|:---|
|blackAndWhite|0|黑白标记 (使用黑色标记材料。) |
|灰度|1|灰度 (可能会使用一些颜色标记材料。) |
|颜色|2|颜色 (使用标记材料的任意组合来创建颜色展示) 。|
|自动|3|让打印机决定使用哪种颜色模式。|

### <a name="printscaling-values"></a>printScaling 值

|成员|值|说明|
|:---|:---|:---|
|自动|0|如果文档大于所请求的媒体并且页边距不为零，则打印机会像调整 printScaling 一样缩放文档。 否则，打印机会使用填充 printScaling 缩放文档。 如果文档小于请求的媒体，则使用"none"printScaling。|
|shrinkToFit|1|如果文档大于请求的媒体，打印机会像调整 printScaling 一样缩放文档。 否则，打印机会像无 printScaling 一样缩放文档。|
|fill|2|打印机缩放文档以填充请求的媒体大小，保持其纵横比，但可能会裁剪文档部分。|
|fit|3|打印机缩放文档以适应所请求的媒体大小的可打印区域，从而保留文档数据的纵横比，而不裁剪文档。|
|无|4 |打印机不缩放文档以适合请求的媒体大小。 如果文档大于请求的媒体，则打印机将设置其中心并剪辑生成的输出。 如果文档小于请求的媒体，打印机将生成的输出作为中心。|
|unknownFutureValue|5 |可发展枚举 sentinel 值。 请勿使用。|

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

