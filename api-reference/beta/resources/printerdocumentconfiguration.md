---
title: printerDocumentConfiguration 资源类型
description: 打印机打印文档时应使用的一组设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ff1da92894f8854bcdee2ce24d7a9d5cef6288e7
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895610"
---
# <a name="printerdocumentconfiguration-resource-type"></a>printerDocumentConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

打印机打印文档时应使用的一组设置。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|pageRanges|[printPageRange](printpagerange.md)集合|要打印的页面范围。 只读。|
|printQuality|printQuality|打印作业时使用的打印质量。 有效值如下表所示。 只读。|
|printResolutionInDpi|Int32|打印作业时要使用的分辨率，以每英寸点数（DPI）表示。 只读。|
|feedDirection|printerFeedDirection|将媒体送进打印机时使用的方向。 有效值如下表所述。 只读。|
|orientation|printOrientation|打印机打印作业时应使用的方向设置。 有效值如下表所述。|
|duplexConfiguration|printDuplexConfiguration|打印作业时打印机应使用的双工配置。 有效值如下表所示。 只读。|
|副本|Int32|应打印的份数。 只读。|
|colorConfiguration|printColorConfiguration|打印机打印作业时应使用的颜色配置。 有效值如下表所示。 只读。|

### <a name="printduplexconfiguration-values"></a>printDuplexConfiguration 值

|成员|值|说明|
|:---|:---|:---|
|twoSidedLongEdge|0|打印机将双面打印，并且将沿长边翻转文档。|
|twoSidedShortEdge|1|打印机将双面打印，并且将沿短边翻转文档。|
|oneSided|双面|打印机将单面打印。|

### <a name="printquality-values"></a>printQuality 值

|成员|说明|
|:---|:---|
|降低|打印机将使用低（通常称为 "草稿"）质量打印作业。|
|中等|打印机将使用 medim （通常称为 "普通"）质量打印作业。|
|高效|打印机将使用 "高" （通常称为 "最佳" 或 "精细"）质量打印作业。|

## <a name="printerfeeddirection-values"></a>printerFeedDirection 值

|成员|说明|
|:---|:---|
|longEdgeFirst|打印机将使用 "横向" 方向的活动栏中的工作表，并在工作表的长边先进行处理。|
|shortEdgeFirst|打印机将使用 "纵向" 方向的活动托盘中的工作表，并在工作表中先短边。|

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
  "@odata.type": "microsoft.graph.printerDocumentConfiguration"
}-->

```json
{
  "pageRanges": [{"@odata.type": "microsoft.graph.printPageRange"}],
  "printQuality": "String",
  "printResolutionInDpi": 123456,
  "feedDirection": "String",
  "orientation": "String",
  "duplexConfiguration": "String",
  "copies": 123456,
  "colorConfiguration": "String",
}

```
