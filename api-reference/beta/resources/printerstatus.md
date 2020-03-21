---
title: printerStatus 资源类型
description: 表示打印机的处理状态，包括任何错误。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4fff364cced30e46d50bbef9ef5b8b50e4a058f5
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895606"
---
# <a name="printerstatus-resource-type"></a>printerStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印机的处理状态，包括任何错误。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|processingState|printerProcessingState|当前的处理状态。 有效值如下表所述。 只读。|
|processingStateReasons|printerProcessingStateReason 集合|描述打印机处于当前状态的原因的列表。 有效值如下表所述。 只读。|
|processingStateDescription|String|打印机当前处理状态的人可读说明。 只读。|

### <a name="printerprocessingstate-values"></a>printerProcessingState 值

|成员|值|说明|
|:---|:---|:---|
|unknown|0|打印机报告的处理状态未知。|
|待机|1|打印机处于空闲状态，并已准备好接受新的打印作业。|
|处理|双面|打印机当前正在处理打印作业，并将在完成时处理任何挂起的作业。|
|停止|第三章|打印机遇到问题（例如，在当前送纸器中缺纸），无法继续使用当前的打印作业，直到问题得到解决。 有关详细信息，请参阅**printerProcessingStateReasons**值或**printerProcessingStateDescription**值。|
|向 unknownfuturevalue|4 |Evolvable 枚举 sentinel 值。 请勿使用。|

### <a name="printerprocessingstatereason-values"></a>printerProcessingStateReason 值

|成员|值|说明|
|:---|:---|:---|
|停留|0| 正在进行的打印作业已暂停。|
|被|1|与打印机的连接丢失或无法建立连接。|
|mediaJam|双面|一个或多个纸盒中的介质卡纸。|
|mediaNeeded|第三章|必须先替换当前使用的输入送纸器中的媒体，然后才能继续执行作业。|
|mediaLow|4 |一个或多个送纸器中的媒体几乎耗尽。|
|mediaEmpty|5 |一个或多个托盘中的媒体已耗尽。|
|coverOpen|6 |打开了一个或多个封面。|
|interlockOpen|7 |一个或多个互锁设备已打开。|
|queueFull|8 |打印机的后台打印程序队列已满，无法排队新的作业。|
|outputTrayMissing|9 |一个或多个输出送纸器丢失。|
|outputAreaFull|10 |一个或多个输出托盘已满，无法接受更多的媒体。|
|markerSupplyLow|11x17|一个或多个标记源（例如，墨迹、墨粉或功能区）不足。|
|markerSupplyEmpty|12 |一个或多个标记源（例如，墨迹、墨粉或功能区）已耗尽。|
|inputTrayMissing|13 |一个或多个输入送纸器不在设备中。|
|outputAlmostFull|14 |一个或多个输出区域几乎已满（例如，送纸器、堆栈器、排序程序）。|
|markerWasteAlmostFull|15 |设备标记供应废物容器几乎已满。|
|markerWasteFull|16 |设备标记供应废物容器已满。|
|fuserOverTemp|17 |热熔器温度高于正常水平。|
|fuserUnderTemp|18 |热熔器温度低于正常水平。|
|相互|合|不属于其余原因的任何其他原因。|
|向 unknownfuturevalue|20|Evolvable 枚举 sentinel 值。 请勿使用。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerStatus"
}-->

```json
{
    "processingState": "String",
    "processingStateReasons": ["String"],
    "processingStateDescription": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->