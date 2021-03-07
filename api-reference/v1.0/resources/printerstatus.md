---
title: printerStatus 资源类型
description: 表示打印机的处理状态，包括任何错误。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 52972a673ae75ad82def76f92bc1bc59932b202f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517297"
---
# <a name="printerstatus-resource-type"></a>printerStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示打印机的处理状态，包括任何错误。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|state|printerProcessingState|当前处理状态。 下表介绍了有效值。 只读。|
|详细信息|printerProcessingStateDetail 集合|描述打印机为何当前状态的详细信息列表。 下表介绍了有效值。 只读。|
|说明|String|打印机当前处理状态的人读说明。 只读。|

### <a name="printerprocessingstate-values"></a>printerProcessingState 值

|成员|值|Description|
|:---|:---|:---|
|unknown|0|打印机报告的处理状态未知。|
|idle|1 |打印机处于空闲状态并准备接受新的打印作业。|
|processing|2 |打印机当前正在处理打印作业，在完成时将处理所有挂起的作业。|
|已停止|3 |打印机遇到问题 (例如，活动纸盒中的纸张) 无法继续当前打印作业，直到问题得到解决。 有关详细信息 **，** 请参阅 () **或说明值** 的详细信息。|
|unknownFutureValue|4 |可发展枚举 sentinel 值。 请勿使用。|

### <a name="printerprocessingstatedetail-values"></a>printerProcessingStateDetail 值

|成员|值|Description|
|:---|:---|:---|
|paused|0| 正在进行的打印作业已暂停。|
|mediaJam|2 |一个或多个纸盒中的媒体被卡住。|
|mediaNeeded|3 |需要替换当前使用的输入纸盒中的媒体，然后才能继续作业。|
|mediaLow|4 |一个或多个纸盒中的媒体几乎耗尽。|
|mediaEmpty|5 |一个或多个纸盒中的媒体已耗尽。|
|coverOpen|6 |一个或多个覆盖已打开。|
|interlockOpen|7 |一个或多个互锁设备已打开。|
|outputTrayMissing|9 |缺少一个或多个输出纸盒。|
|outputAreaFull|10  |一个或多个输出纸盒已满，无法接受更多媒体。|
|markerSupplyLow|11|一个或多个标记源 (，例如墨迹、toner 或功能区) 较低。|
|markerSupplyEmpty|12 |一个或多个标记源 (，例如墨迹、toner 或功能区) 用尽。|
|inputTrayMissing|13 |一个或多个输入纸盒不在设备中。|
|outputAreaAlmostFull|14 |一个或多个输出区域几乎已满， (纸盒、堆叠器、整理器) 。|
|markerWasteAlmostFull|15 |设备标记提供垃圾容器几乎已满。|
|markerWasteFull|16 |设备标记提供垃圾容器已满。|
|fuserOverTemp|17 |合成器温度高于正常。|
|fuserUnderTemp|18 |合成器温度低于正常值。|
|other|19|任何其他原因不属于其余原因。|
|无|20|无原因。|
|movingToPaused| 21|有人使用"打印"操作Pause-Printer打印机。|
|shutdown|22|某人从服务中删除了 Printer 对象，设备可能关闭或实际删除。|
|connectingToDevice|23|打印机正在连接到共享网络输出设备。|
|timedOut|24|服务器无法从输出设备获取响应。|
|停止|25|Printer 对象正在停止设备。|
|stoppedPartially|26|一个或多个输出设备已停止。|
|tonerLow|27|设备在 Toner 上较低。|
|tonerEmpty|28|设备已外出。|
|spoolAreaFull|29|已达到分配给后台打印的永久存储的限制。|
|doorOpen|30|设备上一个或多个门已打开。|
|opticalPhotoConductorNearEndOfLife|31|光学照片的检测接近生命周期的结束。|
|opticalPhotoConductorLifeOver|32|光学照片的放大功能不再起作用。|
|developerLow|33|设备在开发人员中较低。|
|developerEmpty|34|设备不是开发人员。|
|interpreterResourceUnavailable|35|解释器资源不可用 (如字体、窗体) 。|
|unknownFutureValue|36|可发展枚举 sentinel 值。 请勿使用。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerStatus",
  "state": "String",
  "details": [
    "String"
  ],
  "description": "String"
}
```

