---
title: printerStatus 资源类型
description: 表示打印机的处理状态，包括任何错误。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 726fba10b91edb98d41eac47779c86749a173e48
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617001"
---
# <a name="printerstatus-resource-type"></a>printerStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印机的处理状态，包括任何错误。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|state|printerProcessingState|当前的处理状态。 有效值如下表所述。 只读。|
|详细信息|printerProcessingStateDetail 集合|描述打印机处于当前状态的原因的详细信息列表。 有效值如下表所述。 只读。|
|说明|String|打印机当前处理状态的人可读说明。 只读。|

### <a name="printerprocessingstate-values"></a>printerProcessingState 值

|成员|值|说明|
|:---|:---|:---|
|unknown|0|打印机报告的处理状态未知。|
|待机|1 |打印机处于空闲状态，并已准备好接受新的打印作业。|
|处理|2 |打印机当前正在处理打印作业，并将在完成时处理任何挂起的作业。|
|停止|3 |打印机遇到问题 (例如，在活动纸盒中缺纸) ，并且在解决问题之前无法继续当前的打印作业。 有关详细信息，请参阅 (s) 的 **详细** 信息值或 **描述** 值。|
|向 unknownfuturevalue|4 |Evolvable 枚举 sentinel 值。 请勿使用。|

### <a name="printerprocessingstatedetail-values"></a>printerProcessingStateDetail 值

|成员|值|说明|
|:---|:---|:---|
|停留|0| 正在进行的打印作业已暂停。|
|mediaJam|2 |一个或多个纸盒中的介质卡纸。|
|mediaNeeded|3 |必须先替换当前使用的输入送纸器中的媒体，然后才能继续执行作业。|
|mediaLow|4 |一个或多个送纸器中的媒体几乎耗尽。|
|mediaEmpty|5 |一个或多个托盘中的媒体已耗尽。|
|coverOpen|6 |打开了一个或多个封面。|
|interlockOpen|7 |一个或多个互锁设备已打开。|
|outputTrayMissing|9 |一个或多个输出送纸器丢失。|
|outputAreaFull|10 |一个或多个输出托盘已满，无法接受更多的媒体。|
|markerSupplyLow|11 |一个或多个标记源 (例如，墨水、墨粉或功能区) 不足。|
|markerSupplyEmpty|12 |一个或多个标记源 (例如，墨水、墨粉或功能区) 耗尽。|
|inputTrayMissing|13 |一个或多个输入送纸器不在设备中。|
|outputAreaAlmostFull|14 |一个或多个输出区域几乎已满 (例如，"任务栏"、"堆栈器"、"排序程序") 。|
|markerWasteAlmostFull|15 |设备标记供应废物容器几乎已满。|
|markerWasteFull|16 |设备标记供应废物容器已满。|
|fuserOverTemp|17 |热熔器温度高于正常水平。|
|fuserUnderTemp|18 |热熔器温度低于正常水平。|
|相互|合|不属于其余原因的任何其他原因。|
|无|20|无原因。|
|movingToPaused| 21|某人使用 Pause-Printer 操作暂停了打印机。|
|关闭|22|某人从服务中删除了一个打印机对象，并且该设备可能已断电或已物理删除。|
|connectingToDevice|上午|打印机正处于连接到共享网络输出设备的过程中。|
|timedOut|24|服务器无法从输出设备获取响应。|
|停止|word|打印机对象正处于停止设备的过程中。|
|stoppedPartially|26|一个或多个输出设备已停止。|
|tonerLow|27|设备墨粉不足。|
|tonerEmpty|28|设备缺墨粉。|
|spoolAreaFull|29|已达到为后台处理分配的永久存储限制。|
|doorOpen|30|设备上的一个或多个门处于打开状态。|
|opticalPhotoConductorNearEndOfLife|31|光学照片导线在生命周期快要结束。|
|opticalPhotoConductorLifeOver|32|光学照片导线不再正常工作。|
|developerLow|33|设备的开发人员不足。|
|developerEmpty|34|设备不在开发人员的开发中。|
|interpreterResourceUnavailable|35|解释器资源不可用 (例如字体、窗体) 。|
|向 unknownfuturevalue|36|Evolvable 枚举 sentinel 值。 请勿使用。|

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
    "state": "String",
    "details": ["String"],
    "description": "String"
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

