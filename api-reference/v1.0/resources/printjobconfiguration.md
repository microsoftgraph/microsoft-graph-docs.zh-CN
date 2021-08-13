---
title: printJobConfiguration 资源类型
description: 打印机用于打印作业的一组设置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 1e13d74fb7a9ed977a380050e49c8d3f267e045299474ca622aa408d738a4562
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223240"
---
# <a name="printjobconfiguration-resource-type"></a>printJobConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

打印机用于打印作业的一组设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|pageRanges|[integerRange](integerrange.md) 集合|要打印的页面范围。 只读。|
|quality|[printQuality](enums.md#printquality-values)|打印作业时使用的打印质量。 下表介绍了有效值。 只读。|
|dpi|Int32|打印作业时使用的分辨率，以每英寸点数表示 (DPI) 。 只读。|
|feedOrientation|printerFeedOrientation|将媒体馈送到打印机时使用的方向。 下表介绍了有效值。 只读。|
|orientation|[printOrientation](enums.md#printorientation-values)|打印作业时打印机应该使用的方向设置。 下表介绍了有效值。|
|duplexMode|[printDuplexMode](enums.md#printduplexmode-values)|打印作业时打印机应该使用的双面模式。 下表介绍了有效值。 只读。|
|copies|Int32|应打印的副本数。 只读。|
|colorMode|[printColorMode](enums.md#printcolormode-values)|打印机用于打印作业的颜色模式。 下表介绍了有效值。 只读。|
|inputBin|String|打印时 (纸盒) 纸盒。 有关受支持的 [输入箱](printercapabilities.md) 的列表，请参阅打印机的功能。|
|outputBin|String|要放入已完成打印输出的输出箱。 有关受支持的 [输出箱](printercapabilities.md) 的列表，请参阅打印机的功能。|
|mediaSize|String|打印时使用的媒体大小。 支持 ISO 和 ANSI 媒体大小的标准大小名称。 [printerCapabilities](printercapabilities.md#mediasizes-values)主题中列出的有效值。|
|margin|[printMargin](printmargin.md)|打印时使用的边距设置。|
|mediaType|String|默认媒体 (，如) 打印文档的类型。|
|finishings|[printFinishing](enums.md#printfinishing-values) 集合|完成打印时使用的过程。|
|pagesPerSheet|Int32|每张工作表上要打印的文档页数。
|multipageLayout|[printMultipageLayout](enums.md#printmultipagelayout-values)|每张工作表打印多个页面时布局页面的方向。 下表介绍了有效值。|
|collate|Boolean|打印多页文档的多个副本时，打印机是否应该整理页面。|
|scaling|[printScaling](enums.md#printscaling-values)|指定打印机如何缩放文档数据以适应请求的媒体。 下表介绍了有效值。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobConfiguration",
  "pageRanges": [
    {
      "@odata.type": "microsoft.graph.integerRange"
    }
  ],
  "quality": "String",
  "dpi": "Integer",
  "feedOrientation": "String",
  "orientation": "String",
  "duplexMode": "String",
  "copies": "Integer",
  "colorMode": "String",
  "inputBin": "String",
  "outputBin": "String",
  "mediaSize": "String",
  "margin": {
    "@odata.type": "microsoft.graph.printMargin"
  },
  "mediaType": "String",
  "finishings": [
    "String"
  ],
  "pagesPerSheet": "Integer",
  "multipageLayout": "String",
  "collate": "Boolean",
  "scaling": "String",
  "fitPdfToPage": "Boolean"
}
```

