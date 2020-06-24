---
title: printerCapabilities 复杂类型
description: 代表打印机报告的功能。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fd739df6b8b294a52d2a17c34649557e6a2dbff0
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862470"
---
# <a name="printercapabilities-complex-type"></a>printerCapabilities 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表打印机报告的功能。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|contentTypes|String collection|打印机支持的受支持的内容（MIME）类型的列表。 不能保证通用打印服务支持打印所有这些 MIME 类型。|
|isColorPrintingSupported|Boolean|如果打印机支持彩色打印，则为 True;否则为 false。 只读。|
|feedDirections|printerFeedDirection 集合|打印机支持的送纸方向列表。|
|isPageRangeSupported|Boolean|如果打印机支持按页面范围打印，则为 True; 否则为 false。否则为 false。|
|特质|printQuality 集合|打印机支持的打印质量。|
|dpis|Int32 集合|打印机支持的打印分辨率（以 DPI 为单位）的列表。|
|duplexModes|printDuplexMode 集合|打印机支持的双工模式的列表。 有效值如下表所述。|
|queueBufferSizeInBytes|Int32|打印机可以存储的最大打印作业队列大小。|
|copiesPerJob|[integerRange](integerrange.md)|打印机支持的每个作业的副本的范围。|
|finishings|printFinishing 集合|完成打印文档的打印机支持的过程。|
|mediaColors|String collection|打印机支持的媒体（即纸张）颜色。|
|mediaTypes|String collection|打印机支持的媒体类型。 有效值如下表所述。|
|mediaSizes|String collection|打印机支持的媒体大小。 支持 ISO 和 ANSI 媒体大小的标准大小名称，以及关联打印机支持的任何自定义大小。|
|pagesPerSheet|Int32 集合|对单个印象施加支持的输入页面数量。|
|方向|printOrientation 集合|打印机支持的打印方向。 有效值如下表所述。|
|inputBins|String collection|打印机支持的输入纸盒。|
|outputBins|String collection|打印机支持的输出箱（送纸器）。|
|supportsFitPdfToPage|Boolean|如此如果打印机支持缩放 PDF 页面以匹配打印介质大小;否则为 false。|
|multipageLayouts|printMultipageLayout 集合|打印机支持的演示文稿说明。 下表介绍了受支持的值。|
|colorModes|printColorMode 集合|打印机支持的颜色模式。 有效值如下表所述。|
|topMargins|Int32 集合|打印机的受支持的上边距列表（在 microns 中）。|
|bottomMargins|Int32 集合|打印机受支持的下边距（以 microns 为单位）的列表。|
|rightMargins|Int32 集合|打印机的受支持的右边距（以 microns 为单位）的列表。|
|leftMargins|Int32 集合|打印机的受支持的左边距（以 microns 为单位）的列表。|
|排序|Boolean|如此如果打印机支持在打印多页文档的 muliple 副本时进行排序;否则为 false。|
|scalings|printScaling 集合|支持的打印 scalings。|

## <a name="printerfeeddirection-values"></a>printerFeedDirection 值

|成员|值|说明|
|:---|:---|
|longEdgeFirst|0|打印机将使用 "横向" 方向的活动栏中的工作表，并在工作表的长边先进行处理。|
|shortEdgeFirst|1 |打印机将使用 "纵向" 方向的活动托盘中的工作表，并在工作表中先短边。|
|向 unknownfuturevalue|双面|Evolvable 枚举 sentinel 值。 请勿使用。|

### <a name="printquality-values"></a>printQuality 值

|成员|值|Description|
|:---|:---|
|降低|0|打印机将使用低（通常称为 "草稿"）质量打印作业。|
|中等|1 |打印机将使用 medim （通常称为 "普通"）质量打印作业。|
|高效|双面|打印机将使用 "高" （通常称为 "最佳" 或 "精细"）质量打印作业。|
|向 unknownfuturevalue|第三章|Evolvable 枚举 sentinel 值。 请勿使用。|

### <a name="printduplexmode-values"></a>printDuplexMode 值

|成员|值|Description|
|:---|:---|:---|
|flipOnLongEdge|0|打印机将双面打印，并且将沿长边翻转文档。|
|flipOnShortEdge|1 |打印机将双面打印，并且将沿短边翻转文档。|
|oneSided|双面|打印机将单面打印。|

### <a name="printfinishing-values"></a>printFinishing 值

|成员|值|Description|
|:---|:---|:---|
|无|第三章|无 finishings。 包括此值等效于提供空的 finishings 集合。|
|侧|4 |使用打印机的默认装订配置对文档进行装订。|
|穿透|5 |打孔使用打印机的默认打孔配置来打孔文档。|
|包装盒|6 |将封面应用于文档。|
|绑定|7 |使用打印机的默认绑定配置绑定文档。|
|saddleStitch|8 |骑马-使用打印机的默认装订配置 stich 文档。|
|stitchEdge|9 |使用打印机的默认装订配置对文档进行边缘装订。|
|stapleTopLeft|20|将文档装订在左上角。|
|stapleBottomLeft| 21|在左下角对文档进行装订。|
|stapleTopRight|22|在右上角将文档装订在一起。|
|stapleBottomRight|上午|在右下角将文档装订在一起。|
|stitchLeftEdge|24|沿左边缘对文档进行边缘装订。|
|stitchTopEdge|word|沿上边缘对文档进行边缘装订。|
|stitchRightEdge|26|将文档沿右边缘装订。|
|stitchBottomEdge|27|对文档沿下边缘进行边缘装订。|
|stapleDualLeft|28|将文档沿左边缘两次装订。|
|stapleDualTop|29|将文档沿上边缘两次装订。|
|stapleDualRight|30|将文档沿右边缘两次装订。|
|stapleDualBottom|31|将文档沿下边缘两次装订。|

## <a name="printorientation-values"></a>printOrientation 值

|成员|值|Description|
|:---|:---|:---|
|纵|第三章|打印机将在 "纵向" 方向上打印为印记。|
|现状|4 |打印机将在 "横向" 方向上打印为印记。|
|reverseLandscape|5 |打印机将在 "翻转横向" 方向上打印为印记。|
|reversePortrait|6 |打印机将在 "反转纵向" 方向上打印为印记。|

### <a name="printmultipagelayout-values"></a>printMultipageLayout 值

|成员|值|Description|
|:---|:---|:---|
|clockwiseFromTopLeft|0|从左上角开始沿顺时针方向的网格排列页面。|
|counterclockwiseFromTopLeft|1 |在从左上角开始的逆时针网格中排列页面。|
|counterclockwiseFromTopRight|双面|从右上部开始以逆时针网格线排列页面。|
|clockwiseFromTopRight|第三章|从右上部开始沿顺时针网格排列页面。|
|counterclockwiseFromBottomLeft|4 |从左下角开始以逆时针网格线排列页面。|
|clockwiseFromBottomLeft|5 |从左下角开始沿顺时针方向的网格排列页面。|
|counterclockwiseFromBottomRight|6 |从右下角开始以逆时针网格线排列页面。|
|clockwiseFromBottomRight|7 |从右下角开始沿顺时针方向的网格排列页面。|

### <a name="printcolormode-values"></a>printColorMode 值

|成员|值|Description|
|:---|:---|:---|
|blackAndWhite|0|黑色和白色（仅使用黑色标记材料。）|
|灰度|1 |灰度（可能使用某些颜色标记材料。）|
|颜色|双面|颜色（使用标记材料的任意组合来创建颜色印象）。|
|自动|第三章|让打印机决定要使用哪种颜色模式。|

### <a name="printscaling-values"></a>printScaling 值

|成员|值|Description|
|:---|:---|:---|
|自动|0|如果文档大于所请求的媒体，且边距不为零，则打印机会缩放**文档，如 printScaling。** 否则，打印机将使用**填充**printScaling 对文档进行缩放。 如果文档小于请求的媒体，则使用 "无" printScaling。|
|shrinkToFit|1 |如果文档比请求的媒体大，则打印机会缩放文档，**如 printScaling。** 否则，打印机会缩放文档，如**none** printScaling。|
|fill|双面|打印机缩放文档以填充请求的媒体大小，并保留其纵横比，但可能会裁剪文档的某些部分。|
|尺寸|第三章|打印机缩放文档以匹配请求媒体大小的可打印区域，并保留文档数据的纵横比而不裁剪文档。|
|无|4 |打印机不会缩放文档以适应请求的媒体大小。 如果文档大于请求的媒体，打印机会居中并剪辑生成的输出。 如果文档小于请求的媒体，则打印机会将结果输出居中。|
|向 unknownfuturevalue|5 |Evolvable 枚举 sentinel 值。 请勿使用。|

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
  "feedDirections": [{"@odata.type": "microsoft.graph.printerFeedDirection"}],
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