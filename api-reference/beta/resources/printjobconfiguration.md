---
title: printJobConfiguration 资源类型
description: 打印机应用于打印作业的一组设置。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 3579a8ca5e8bc7fa238456fc3d368d3c101acdca
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176949"
---
# <a name="printjobconfiguration-resource-type"></a>printJobConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

打印机应用于打印作业的一组设置。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|pageRanges|[integerRange](integerrange.md) 集合|要打印的页面范围。 只读。|
|质量|printQuality|打印作业时要使用的打印质量。 下表描述了有效值。 只读。|
|dpi|Int32|打印作业时要使用的分辨率，以每英寸点表示 (DPI) 。 只读。|
|feedOrientation|printerFeedOrientation|将媒体馈送到打印机时要使用的方向。 下表描述了有效值。 只读。|
|orientation|printOrientation|打印作业时打印打印机应使用的方向设置。 下表描述了有效值。|
|duplexMode|printDuplexMode|打印作业时打印机应使用的双工模式。 下表描述了有效值。 只读。|
|副本|Int32|应打印的副本数。 只读。|
|colorMode|printColorMode|打印机应用于打印作业的颜色模式。 下表描述了有效值。 只读。|
|inputBin|String|输入箱 () 打印时使用的托盘。 有关支持的输入箱列表，请参阅打印机的 [功能](printercapabilities.md) 。|
|outputBin|字符串|要将已完成打印放入其中的输出箱。 有关支持的输出箱列表，请参阅打印机的 [功能](printercapabilities.md) 。|
|mediaSize|字符串|打印时要使用的媒体大小。 支持 ISO 和 ANSI 媒体大小的标准大小名称。 有效值列在 [printerCapabilities](printercapabilities.md#mediasizes-values) 主题中。|
|margin|[printMargin](printmargin.md)|打印时要使用的边距设置。|
|mediaType|String|要打印文档的默认媒体 (（如纸张) 类型）。|
|finishings|printFinishing 集合|打印时要使用的完成过程。|
|pagesPerSheet|Int32|每张工作表上要打印的文档页数。
|multipageLayout|printMultipageLayout|每张工作表打印多个页面时布局页面的方向。 下表描述了有效值。|
|collate|Boolean|打印机是否应对打印多页文档的多个副本的页面进行排序。|
|scaling|printScaling|指定打印机应如何缩放文档数据以适应请求的媒体。 下表描述了有效值。|

### <a name="printquality-values"></a>printQuality 值

|成员|值|Description|
|:---|:---|:---|
|低|0|打印机将使用低 (通常称为“草稿”) 质量打印作业。|
|中等|1|打印机将使用 medim 打印作业 (通常称为“普通”) 质量。|
|高|2|打印机将使用高 (通常称为“最佳”或“精细”) 质量来打印作业。|
|unknownFutureValue|3|可变枚举 sentinel 值。 请勿使用。|

### <a name="printerfeedorientation-values"></a>printerFeedOrientation 值

|成员|值|Description|
|:---|:---|:---|
|longEdgeFirst|0|打印机将在“横向”方向使用活动托盘中的工作表，其中首先使用工作表的长边缘。|
|shortEdgeFirst|1|打印机将以“纵向”方向使用活动托盘中的工作表，并首先使用工作表的短边缘。|
|unknownFutureValue|2|可变枚举 sentinel 值。 请勿使用。|

### <a name="printorientation-values"></a>printOrientation 值

|成员|值|Description|
|:---|:---|:---|
|肖像|3|打印机将以“纵向”方向打印印象。|
|景观|4|打印机将以“横向”方向打印印象。|
|reverseLandscape|5|打印机将以“反向横向”方向打印印象。|
|reversePortrait|6 |打印机将以“反向纵向”方向打印印象。|

### <a name="printduplexmode-values"></a>printDuplexMode 值

|成员|值|Description|
|:---|:---|:---|
|flipOnLongEdge|0|打印机将双面打印，并将沿长边缘翻转文档。|
|flipOnShortEdge|1|打印机将双面打印，并将沿短边缘翻转文档。|
|oneSided|2|打印机将单面打印。|

### <a name="printcolormode-values"></a>printColorMode 值

|成员|值|Description|
|:---|:---|:---|
|blackAndWhite|0|黑白 (只使用黑色标记材料。) |
|灰度|1|灰度 (可能使用一些颜色标记材料。) |
|颜色|2|颜色 (使用标记材料的任何组合来创建颜色印象) 。|
|自动|3|让打印机决定要使用的颜色模式。|

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

### <a name="printmultipagelayout-values"></a>printMultipageLayout 值

|成员|值|Description|
|:---|:---|:---|
|clockwiseFromTopLeft|0|从左上角开始，在顺时针网格中排列页面。|
|counterClockwiseFromTopLeft|1|从左上角开始，在逆时针网格中排列页面。|
|counterClockwiseFromTopRight|2|从右上角开始，在逆时针网格中排列页面。|
|clockwiseFromTopRight|3|从右上角开始，在顺时针网格中排列页面。|
|counterClockwiseFromBottomLeft|4|从左下角开始，在逆时针网格中排列页面。|
|clockwiseFromBottomLeft|5|从左下角开始，在顺时针网格中排列页面。|
|counterClockwiseFromBottomRight|6 |从右下角开始，在逆时针网格中排列页面。|
|clockwiseFromBottomRight|7 |从右下角开始，在顺时针网格中排列页面。|

### <a name="printscaling-values"></a>printScaling 值

|成员|值|Description|
|:---|:---|:---|
|自动|0|如果文档大于请求的媒体且边距为非零，则打印机会缩放文档，如 **拟合** printScaling。 否则，打印机将使用 **填充** printScaling 缩放文档。 如果文档小于请求的媒体，则使用“无”printScaling。|
|shrinkToFit|1|如果文档大于请求的媒体，打印机会缩放文档，如 **拟合** printScaling。 否则，打印机会缩放文档，就像 **无** 打印缩放一样。|
|fill|2|打印机缩放文档以填充请求的媒体大小，保留其纵横比，但可能会裁剪文档的部分。|
|适合|3|打印机缩放文档以适应所请求媒体大小的可打印区域，在不裁剪文档的情况下保留文档数据的纵横比。|
|无|4|打印机不缩放文档以适应所请求的媒体大小。 如果文档大于请求的媒体，打印机会居中并剪辑生成的输出。 如果文档小于请求的媒体，打印机将生成的输出居中。|
|unknownFutureValue|5|可变枚举 sentinel 值。 请勿使用。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobConfiguration"
}-->

```json
{
  "pageRanges": [{"@odata.type": "microsoft.graph.integerRange"}],
  "quality": {"@odata.type": "microsoft.graph.printQuality"},
  "dpi": 12345,
  "feedOrientation": {"@odata.type": "microsoft.graph.printerFeedOrientation"},
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


