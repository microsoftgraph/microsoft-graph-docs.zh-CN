---
title: printerDocumentConfiguration 资源类型
description: 打印机打印文档时应使用的一组设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 3bd0235b7b0dd1cebe5298a1f2357cd4a9f1fd81
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081352"
---
# <a name="printerdocumentconfiguration-resource-type"></a>printerDocumentConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

打印机打印文档时应使用的一组设置。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|pageRanges|[integerRange](integerrange.md)集合|要打印的页面范围。 只读。|
|品质|printQuality|打印作业时使用的打印质量。 有效值如下表所示。 只读。|
|dpi|Int32|打印作业时要使用的分辨率，以每英寸点数（DPI）表示。 只读。|
|feedDirection|printerFeedDirection|将媒体送进打印机时使用的方向。 有效值如下表所述。 只读。|
|orientation|printOrientation|打印机打印作业时应使用的方向设置。 有效值如下表所述。|
|duplexMode|printDuplexMode|打印作业时打印机应使用的双工模式。 有效值如下表所示。 只读。|
|副本|Int32|应打印的份数。 只读。|
|colorMode|printColorMode|打印机打印作业时应使用的颜色模式。 有效值如下表所示。 只读。|
|inputBin|String|打印时使用的送纸盒（送纸器）。 请参阅打印机的[功能](../api/printer-getcapabilities.md)，获取受支持的输入纸盒的列表。|
|outputBin|String|要放置的输出纸盒已完成打印。 请参阅打印机的[功能](../api/printer-getcapabilities.md)，获取受支持的输出箱列表。|
|mediaSize|String|打印时使用的媒体 sizeto。 支持 ISO 和 ANSI 媒体大小的标准大小名称，以及关联打印机支持的任何自定义大小。|
|页脚|[printMargin](printmargin.md)|打印时使用的页边距设置。|
|群组|String|打印文档时所用的默认媒体（如纸）类型。 有效值如下表所述。|
|finishings|printFinishing 集合|完成打印时要使用的进程。|
|pagesPerSheet|Int32|要在每张纸上打印的文档页面的数量。
|multipageLayout|printMultipageLayout|每个工作表打印多个页面时对页面进行布局的方向。 有效值如下表所述。|
|collate|Boolean|打印机是否应逐份打印多页文档的多个副本时 wehen 页面。|
|能力|printScaling|指定打印机应如何缩放文档数据以适应请求的媒体。 有效值如下表所述。|

### <a name="printquality-values"></a>printQuality 值

|成员|值|说明|
|:---|:---|
|降低|0|打印机将使用低（通常称为 "草稿"）质量打印作业。|
|中等|1 |打印机将使用 medim （通常称为 "普通"）质量打印作业。|
|高效|2 |打印机将使用 "高" （通常称为 "最佳" 或 "精细"）质量打印作业。|
|向 unknownfuturevalue|3 |Evolvable 枚举 sentinel 值。 请勿使用。|

## <a name="printerfeeddirection-values"></a>printerFeedDirection 值

|成员|值|说明|
|:---|:---|
|longEdgeFirst|0|打印机将使用 "横向" 方向的活动栏中的工作表，并在工作表的长边先进行处理。|
|shortEdgeFirst|1 |打印机将使用 "纵向" 方向的活动托盘中的工作表，并在工作表中先短边。|
|向 unknownfuturevalue|2 |Evolvable 枚举 sentinel 值。 请勿使用。|

## <a name="printorientation-values"></a>printOrientation 值

|成员|值|说明|
|:---|:---|:---|
|纵|3 |打印机将在 "纵向" 方向上打印为印记。|
|现状|4 |打印机将在 "横向" 方向上打印为印记。|
|reverseLandscape|5 |打印机将在 "翻转横向" 方向上打印为印记。|
|reversePortrait|6 |打印机将在 "反转纵向" 方向上打印为印记。|

### <a name="printduplexmode-values"></a>printDuplexMode 值

|成员|值|说明|
|:---|:---|:---|
|flipOnLongEdge|0|打印机将双面打印，并且将沿长边翻转文档。|
|flipOnShortEdge|1 |打印机将双面打印，并且将沿短边翻转文档。|
|oneSided|2 |打印机将单面打印。|

### <a name="printcolormode-values"></a>printColorMode 值

|成员|值|说明|
|:---|:---|:---|
|blackAndWhite|0|黑色和白色（仅使用黑色标记材料。）|
|灰度|1 |灰度（可能使用某些颜色标记材料。）|
|颜色|2 |颜色（使用标记材料的任意组合来创建颜色印象）。|
|自动|3 |让打印机决定要使用哪种颜色模式。|

### <a name="printfinishing-values"></a>printFinishing 值

|成员|值|说明|
|:---|:---|:---|
|无|3 |无 finishings。 包括此值等效于提供空的 finishings 集合。|
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
|向 unknownfuturevalue|32|Evolvable 枚举 sentinel 值。 请勿使用。|

### <a name="printmultipagelayout-values"></a>printMultipageLayout 值

|成员|值|说明|
|:---|:---|:---|
|clockwiseFromTopLeft|0|从左上角开始沿顺时针方向的网格排列页面。|
|counterClockwiseFromTopLeft|1 |在从左上角开始的逆时针网格中排列页面。|
|counterClockwiseFromTopRight|2 |从右上部开始以逆时针网格线排列页面。|
|clockwiseFromTopRight|3 |从右上部开始沿顺时针网格排列页面。|
|counterClockwiseFromBottomLeft|4 |从左下角开始以逆时针网格线排列页面。|
|clockwiseFromBottomLeft|5 |从左下角开始沿顺时针方向的网格排列页面。|
|counterClockwiseFromBottomRight|6 |从右下角开始以逆时针网格线排列页面。|
|clockwiseFromBottomRight|7 |从右下角开始沿顺时针方向的网格排列页面。|

### <a name="printscaling-values"></a>printScaling 值

|成员|值|说明|
|:---|:---|:---|
|自动|0|如果文档大于所请求的媒体，且边距不为零，则打印机会缩放**文档，如 printScaling。** 否则，打印机将使用**填充**printScaling 对文档进行缩放。 如果文档小于请求的媒体，则使用 "无" printScaling。|
|shrinkToFit|1 |如果文档比请求的媒体大，则打印机会缩放文档，**如 printScaling。** 否则，打印机会缩放文档，如**none** printScaling。|
|fill|2 |打印机缩放文档以填充请求的媒体大小，并保留其纵横比，但可能会裁剪文档的某些部分。|
|尺寸|3 |打印机缩放文档以匹配请求媒体大小的可打印区域，并保留文档数据的纵横比而不裁剪文档。|
|无|4 |打印机不会缩放文档以适应请求的媒体大小。 如果文档大于请求的媒体，打印机会居中并剪辑生成的输出。 如果文档小于请求的媒体，则打印机会将结果输出居中。|
|向 unknownfuturevalue|5 |Evolvable 枚举 sentinel 值。 请勿使用。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerDocumentConfiguration"
}-->

```json
{
  "pageRanges": [{"@odata.type": "microsoft.graph.integerRange"}],
  "quality": {"@odata.type": "microsoft.graph.printQuality"},
  "dpi": 12345,
  "feedDirection": {"@odata.type": "microsoft.graph.printerFeedDirection"},
  "orientation": {"@odata.type": "microsoft.graph.printOrientation"},
  "duplexMode": {"@odata.type": "microsoft.graph.printDuplexMode"},
  "copies": 12345,
  "colorMode": {"@odata.type": "microsoft.graph.printColorMode"},
  "inputBin": "",
  "outputBin": "",
  "mediaSize": "",
  "margin": {"@odata.type": "microsoft.graph.printMargin"},
  "mediaType": "",
  "finishings": [{"@odata.type": "microsoft.graph.printFinishing"}],
  "pagesPerSheet": 12345,
  "multipageLayout": {"@odata.type": "microsoft.graph.printMultipageLayout"},
  "collate": true,
  "scaling": {"@odata.type": "microsoft.graph.printScaling"}
}

```
