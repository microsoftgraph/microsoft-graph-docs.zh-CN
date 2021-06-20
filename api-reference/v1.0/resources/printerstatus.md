---
title: printerStatus 资源类型
description: 表示打印机的处理状态，包括任何错误。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 55374ff2cdb2ad26100fbc3440e4b542e763248b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030962"
---
# <a name="printerstatus-resource-type"></a>printerStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示打印机的处理状态，包括任何错误。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|state|printerProcessingState|当前处理状态。 下表介绍了有效值。 只读。|
|详细信息|printerProcessingStateDetail 集合|描述打印机为何当前状态的详细信息列表。 下表介绍了有效值。 只读。|
|说明|String|打印机当前处理状态可读的说明。 只读。|

### <a name="printerprocessingstate-values"></a>printerProcessingState 值

|成员|值|说明|
|:---|:---|:---|
|unknown|0|打印机报告的处理状态未知。|
|idle|1|打印机处于空闲状态并准备接受新的打印作业。|
|processing|2|打印机当前正在处理打印作业，并且将在完成时处理所有挂起的作业。|
|已停止|3|打印机遇到问题 (例如，活动纸盒中的纸张) 无法继续当前打印作业，直到问题得到解决。 有关详细信息 **，** 请参阅 (的详细信息) **或说明** 值。|
|unknownFutureValue|4 |可发展枚举 sentinel 值。 请勿使用。|

### <a name="printerprocessingstatedetail-values"></a>printerProcessingStateDetail 值

|成员|值|说明|
|:---|:---|:---|
|paused|0| 正在进行的打印作业已暂停。|
|mediaJam|2|一个或多个纸盒中的媒体被阻塞。|
|mediaNeeded|3|需要替换当前使用的输入纸盒中的媒体，然后作业才能继续。|
|mediaLow|4 |一个或多个纸盒中的媒体几乎耗尽。|
|mediaEmpty|5 |一个或多个纸盒中的媒体已耗尽。|
|coverOpen|6 |一个或多个覆盖已打开。|
|interlockOpen|7 |一个或多个互锁设备已打开。|
|outputTrayMissing|9 |缺少一个或多个输出纸盒。|
|outputAreaFull|10  |一个或多个输出纸盒已满，无法接受更多媒体。|
|markerSupplyLow|11|一个或多个标记源 (，例如墨迹、颜色笔或功能区) 较低。|
|markerSupplyEmpty|12 |一个或多个标记源 (，例如墨迹、颜色笔或功能区) 已耗尽。|
|inputTrayMissing|13|一个或多个输入纸盒不在设备中。|
|outputAreaAlmostFull|14 |一个或多个输出区域几乎已满， (纸盒、堆叠器、整理器) 。|
|markerWasteAlmostFull|15|设备标记提供浪费接受几乎已满。|
|markerWasteFull|16 |设备标记提供垃圾接受器已满。|
|将overTemp|17 |温度高于正常水平。|
|一些|18 |温度低于正常值。|
|other|19|其他原因不包括在其余原因中。|
|无|20|无原因。|
|movingToPaused| 21|有人使用"打印机"Pause-Printer打印机。|
|shutdown|22|某人从服务中删除了 Printer 对象，设备可能断电或实际移除。|
|connectingToDevice|23|打印机正在连接到共享网络输出设备。|
|timedOut|24|服务器无法从输出设备获取响应。|
|stopping|25|Printer 对象正在停止设备。|
|stoppedPartially|26|一个或多个输出设备已停止。|
|tonerLow|27|设备在 Toner 上较低。|
|tonerEmpty|28|设备已外出。|
|spoolAreaFull|29|已达到分配给后台处理程序的持久性存储的限制。|
|doorOpen|30|设备上一个或多个门已打开。|
|opticalPhotoConductorNearEndOfLife|31|光学照片的光学镜头即将结束。|
|opticalPhotoConductorLifeOver|32|光学照片的光学镜头不再起作用。|
|developerLow|33|设备对开发人员影响较低。|
|developerEmpty|34|设备不为开发人员使用。|
|interpreterResourceUnavailable|35|解释器资源 (字体、窗体和) 。|
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
