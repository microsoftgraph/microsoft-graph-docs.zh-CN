---
title: printerDefaults 资源类型
description: 表示打印机的默认设置。 检查打印机的功能以查看它支持的所有值。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: efc0c59774967a1ef135c0f90ec3e5c57b97b9c5
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944133"
---
# <a name="printerdefaults-resource-type"></a>printerDefaults 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印机的默认设置。 检查打印机 [的功能以查看](printercapabilities.md) 它支持的所有值。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|copiesPerJob|Int32|每个作业打印的默认副本数。|
|contentType|String|MIME (类型) 处理文档时使用。|
|finishings|printFinishing 集合|应用于打印作业的默认完成集。 下表介绍了有效值。|
|mediaColor|String|默认媒体 (，例如) 打印文档的纸张颜色。|
|mediaType|String|默认媒体 (，如) 打印文档的类型。|
|mediaSize|String|使用的默认媒体大小。 支持 ISO 和 ANSI 媒体大小的标准大小名称。 [printerCapabilities](printercapabilities.md#mediasizes-values)主题中列出了有效值。|
|pagesPerSheet|Int32|每张工作表上要打印的默认文档页数。
|orientation|printOrientation|打印文档时使用的默认方向。 下表介绍了有效值。|
|inputBin|String|作为纸张来源的默认输入箱。|
|outputBin|String|将已完成打印放入的默认输出箱。 有关受支持的 [输出箱](printercapabilities.md) 的列表，请参阅打印机的功能。|
|fitPdfToPage|布尔|默认 fitPdfToPage 设置。 如果为 True，将 PDF 文档的每一页都适合媒体的物理工作表;如果为 false，则打印机决定如何设置展示次数。|
|multipageLayout|printMultipageLayout|当每张工作表打印多个页面时，对页面进行布局的默认方向。 下表介绍了有效值。|
|colorMode|printColorMode|打印文档时使用的默认颜色模式。 下表介绍了有效值。|
|quality|printQuality|打印文档时使用的默认质量。 下表介绍了有效值。|
|duplexMode|printDuplexMode|默认双面 (双面) 打印文档时使用的配置。 下表介绍了有效值。|
|dpi|Int32|打印作业时使用的默认分辨率（以 DPI 表示）。|
|scaling|printScaling|指定打印机如何缩放文档数据以适应请求的媒体。 下表介绍了有效值。|

### <a name="printmultipagelayout-values"></a>printMultipageLayout 值

|成员|值|说明|
|:---|:---|:---|
|顺时针FromTopLeft|0|从左上开始按顺时针网格排列页面。|
|counterClockwiseFromTopLeft|1|从左上开始按逆时针网格排列页面。|
|counterClockwiseFromTopRight|2|从右上方开始按逆时针网格排列页面。|
|clockwiseFromTopRight|3|从右上开始按顺时针网格排列页面。|
|counterClockwiseFromBottomLeft|4 |从左下角开始按逆时针网格排列页面。|
|顺时针FromBottomLeft|5 |从左下角开始按顺时针网格排列页面。|
|counterClockwiseFromBottomRight|6 |从右下角开始按逆时针网格排列页面。|
|clockwiseFromBottomRight|7 |从右下角开始按顺时针网格排列页面。|

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

### <a name="printquality-values"></a>printQuality 值

|成员|值|说明|
|:---|:---|
|low|0|打印机使用通常称为"草稿 ("低质量打印) 作业。|
|中等|1|打印机使用 medim 打印作业 (通常称为"正常") 质量。|
|high|2|打印机会使用通常称为"最好"或 (质量"的高性能打印) 作业。|
|unknownFutureValue|3|可发展枚举 sentinel 值。 请勿使用。|

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

