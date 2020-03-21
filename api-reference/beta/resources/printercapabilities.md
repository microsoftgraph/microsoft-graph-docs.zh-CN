---
title: printerCapabilities 复杂类型
description: 代表打印机报告的功能。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 42ae340e349b282d5480520ed118d049c77cf8bc
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895627"
---
# <a name="printercapabilities-complex-type"></a>printerCapabilities 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表打印机报告的功能。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|isColorPrintingSupported|布尔|如果打印机支持彩色打印，则为 True;否则为 false。 只读。|
|supportsFitPdfToPage|布尔|如此如果打印机支持缩放 PDF 页面以匹配打印介质大小;否则为 false。|
|supportedCopiesPerJob|[integerRange](integerrange.md)|打印机支持的每个作业的副本的范围。|
|supportedDocumentMimeTypes|String collection|打印机支持的文档 mime 类型。|
|supportedFinishings|printFinishing 集合|打印机支持的 finishings。|
|supportedMediaColors|String collection|打印机支持的媒体（即纸张）颜色。|
|supportedMediaTypes|printMediaType 集合|打印机支持的媒体类型。 有效值如下表所述。|
|supportedDuplexConfigurations|printDuplexConfiguration 集合|打印机支持的双工配置。 有效值如下表所述。|
|supportedMediaSizes|String collection|打印机支持的媒体大小。 支持 ISO 和 ANSI 媒体大小的标准大小名称，以及关联打印机支持的任何自定义大小。|
|supportedPagesPerSheet|[integerRange](integerrange.md)|打印机支持的 pagesPerSheet 值。|
|supportedOrientations|printOrientation 集合|打印机支持的打印方向。 有效值如下表所述。|
|supportedOutputBins|String collection|打印机支持的输出箱（送纸器）。|
|supportedPresentationDirections|printPresentationDirection 集合|打印机支持的演示文稿说明。 下表介绍了受支持的值。|
|supportedColorConfigurations|printColorConfiguration 集合|打印机支持的颜色模式。 有效值如下表所述。|
|supportedPrintQualities|printQuality 集合|打印机支持的打印质量。|

### <a name="printpresentationdirection-values"></a>printPresentationDirection 值

|成员|值|说明|
|:---|:---|:---|
|clockwiseFromTopLeft|0|从左上角开始沿顺时针方向的网格排列页面。|
|counterClockwiseFromTopLeft|1|在从左上角开始的逆时针网格中排列页面。|
|counterClockwiseFromTopRight|双面|从右上部开始以逆时针网格线排列页面。|
|clockwiseFromTopRight|第三章|从右上部开始沿顺时针网格排列页面。|
|counterClockwiseFromBottomLeft|4 |从左下角开始以逆时针网格线排列页面。|
|clockwiseFromBottomLeft|5 |从左下角开始沿顺时针方向的网格排列页面。|
|counterClockwiseFromBottomRight|6 |从右下角开始以逆时针网格线排列页面。|
|clockwiseFromBottomRight|7 |从右下角开始沿顺时针方向的网格排列页面。|

### <a name="printmediatype-values"></a>printMediaType 值

|成员|值|说明|
|:---|:---|:---|
|设计|0|一张标准纸张。|
|透明度|1|与投影机投影仪配合使用的透明胶片。|
|信封|双面|信封。|
|envelopePlain|第三章|纯信封。|
|保持|4 |连续一卷纸。|
|闪屏|5 |数字屏幕。|
|screenPaged|6 |支持分页的数字屏幕。|
|continuousLong|7 |较长的连续纸张。|
|continuousShort|8 |简短的连续纸。|
|envelopeWindow|9 |带有透明窗口裁剪的信封。|
|multiPartForm|10 |多部分 perforated 窗体。|
|层|11x17|多层中型。|
|标题|12 |带有标签切出的工作表。|

### <a name="printfinishing-values"></a>printFinishing 值

|成员|值|说明|
|:---|:---|:---|
|无|第三章|无 finishings。 包括此值等效于提供空的 finishings 集合。|
|侧|4 |使用打印机的默认装订配置对文档进行装订。|
|穿透|5 |打孔使用打印机的默认打孔配置来打孔文档。|
|包装盒|6 |将封面应用于文档。|
|绑定|7 |使用打印机的默认绑定配置绑定文档。|
|saddleStitch|8 |骑马-使用打印机的默认装订配置 stich 文档。|
|edgeStitch|9 |使用打印机的默认装订配置对文档进行边缘装订。|
|stapleTopLeft|20|将文档装订在左上角。|
|stapleBottomLeft|不足|在左下角对文档进行装订。|
|stapleTopRight|22|在右上角将文档装订在一起。|
|stapleBottomRight|上午|在右下角将文档装订在一起。|
|edgeStitchLeft|24|沿左边缘对文档进行边缘装订。|
|edgeStitchTop|word|沿上边缘对文档进行边缘装订。|
|edgeStitchRight|26|将文档沿右边缘装订。|
|edgeStitchBottom|27|对文档沿下边缘进行边缘装订。|
|stapleDualLeft|28|将文档沿左边缘两次装订。|
|stapleDualTop|29|将文档沿上边缘两次装订。|
|stapleDualRight|30|将文档沿右边缘两次装订。|
|stapleDualBottom|31|将文档沿下边缘两次装订。|

### <a name="printduplexconfiguration-values"></a>printDuplexConfiguration 值

|成员|值|说明|
|:---|:---|:---|
|twoSidedLongEdge|0|打印机将双面打印，并且将沿长边翻转文档。|
|twoSidedShortEdge|1|打印机将双面打印，并且将沿短边翻转文档。|
|oneSided|双面|打印机将单面打印。|

## <a name="printorientation-values"></a>printOrientation 值

|成员|值|说明|
|:---|:---|:---|
|纵|第三章|打印机将在 "纵向" 方向上打印为印记。|
|现状|4 |打印机将在 "横向" 方向上打印为印记。|
|reverseLandscape|5 |打印机将在 "翻转横向" 方向上打印为印记。|
|reversePortrait|6 |打印机将在 "反转纵向" 方向上打印为印记。|

### <a name="printcolorconfiguration-values"></a>printColorConfiguration 值

|成员|值|说明|
|:---|:---|:---|
|blackAndWhite|0|黑色和白色（仅使用黑色标记材料。）|
|灰度|1|灰度（可能使用某些颜色标记材料。）|
|color|双面|颜色（使用标记材料的任意组合来创建颜色印象）。|
|自动|第三章|让打印机决定要使用哪种颜色模式。|

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
  "isColorPrintingSupported": true,
  "supportsFitPdfToPage": true,
  "supportedCopiesPerJob": {"@odata.type": "microsoft.graph.integerRange"},
  "supportedDocumentMimeTypes": ["String"],
  "supportedFinishings": ["String"],
  "supportedMediaColors": ["String"],
  "supportedMediaTypes": ["String"],
  "supportedDuplexConfigurations": ["String"],
  "supportedMediaSizes": ["String"],
  "supportedPagesPerSheet": {"@odata.type": "microsoft.graph.integerRange"},
  "supportedOrientations": ["String"],
  "supportedOutputBins": ["String"],
  "supportedPresentationDirections": ["String"],
  "supportedColorConfigurations": ["String"],
  "supportedPrintQualities": ["String"]
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