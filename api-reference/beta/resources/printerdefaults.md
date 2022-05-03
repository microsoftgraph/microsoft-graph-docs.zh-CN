---
title: printerDefaults 资源类型
description: 表示打印机的默认设置。 检查打印机的功能，查看它支持的所有值。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: b6450b1293a1b5f5b5a7a019df01b9cfb4dd4ef8
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176689"
---
# <a name="printerdefaults-resource-type"></a>printerDefaults 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印机的默认设置。 检查打印机的 [功能](printercapabilities.md) ，查看它支持的所有值。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|copiesPerJob|Int32|每个作业打印的默认副本数。|
|contentType|String|处理文档时要使用的默认内容 (MIME) 类型。|
|finishings|printFinishing 集合|要应用于打印作业的默认完成集。 下表描述了有效值。|
|mediaColor|String|要打印文档的默认媒体 (（如纸张) 颜色）。|
|mediaType|String|要打印文档的默认媒体 (（如纸张) 类型）。|
|mediaSize|String|要使用的默认媒体大小。 支持 ISO 和 ANSI 媒体大小的标准大小名称。 有效值列在 [printerCapabilities](printercapabilities.md#mediasizes-values) 主题中。|
|pagesPerSheet|Int32|每个工作表上要打印的文档页的默认数目。
|orientation|printOrientation|打印文档时要使用的默认方向。 下表描述了有效值。|
|inputBin|String|用作纸张源的默认输入箱。|
|outputBin|String|要将已完成打印放入其中的默认输出箱。 有关支持的输出箱列表，请参阅打印机的 [功能](printercapabilities.md) 。|
|fitPdfToPage|Boolean|默认的 fitPdfToPage 设置。 如此 若要将 PDF 文档的每个页面安装到物理媒体表中，则为 True;false，让打印机决定如何布置印象。|
|multipageLayout|printMultipageLayout|每张工作表打印多个页面时布局页面的默认方向。 下表描述了有效值。|
|colorMode|printColorMode|打印文档时要使用的默认颜色模式。 下表描述了有效值。|
|质量|printQuality|打印文档时要使用的默认质量。 下表描述了有效值。|
|duplexMode|printDuplexMode|打印文档时要使用的默认双面 (双面) 配置。 下表描述了有效值。|
|dpi|Int32|打印作业时要使用的 DPI 中的默认分辨率。|
|scaling|printScaling|指定打印机如何缩放文档数据以适应请求的媒体。 下表描述了有效值。|

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

### <a name="printquality-values"></a>printQuality 值

|成员|值|Description|
|:---|:---|
|低|0|打印机将使用低 (通常称为“草稿”) 质量打印作业。|
|中等|1|打印机将使用 medim 打印作业 (通常称为“普通”) 质量。|
|高|2|打印机将使用高 (通常称为“最佳”或“精细”) 质量来打印作业。|
|unknownFutureValue|3|可变枚举 sentinel 值。 请勿使用。|

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

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerDefaults"
}-->

```json
{
  "copiesPerJob": 123456,
  "contentType": "String",
  "finishings": ["String"],
  "mediaColor": "String",
  "mediaSize": "String",
  "pagesPerSheet": 123456,
  "orientation": "String",
  "outputBin": "String",
  "fitPdfToPage": true,
  "multipageLayout": "String",
  "colorMode": "String",
  "quality": "String",
  "duplexMode": "String"
}

```

## <a name="see-also"></a>另请参阅

* [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerDefaults resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

