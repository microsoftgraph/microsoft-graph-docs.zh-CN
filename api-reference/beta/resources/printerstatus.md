---
title: printerStatus 资源类型
description: 表示打印机的处理状态，包括任何错误。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b06d121f54361e5c49364220be55e5285188be03
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108724"
---
# <a name="printerstatus-resource-type"></a>printerStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印机的处理状态，包括任何错误。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|state|printerProcessingState|当前处理状态。 下表介绍了有效值。 只读。|
|详细信息|printerProcessingStateDetail 集合|描述打印机为何当前状态的详细信息列表。 下表介绍了有效值。 只读。|
|说明|字符串|打印机当前处理状态可读的说明。 只读。|

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
|alertRemovalOfBinaryChangeEntry|36|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderAdded|37|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderAlmostEmpty|38|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderAlmostFull|39|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderAtLimit|40|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderClosed|41|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderConfigurationChange|42|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderCoverClosed|43|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderCoverOpen|44|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderEmpty|45|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderFull|46|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderInterlockClosed|47|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderInterlockOpen|48|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderJam|49|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderLifeAlmostOver|50|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderLifeOver|51|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderMemoryExtedted|52|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderMissing|53|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderMotorFailure|54|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderNearLimit|55|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderOffline|56|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderOpened|57|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderOverTemperature|58|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderPowerSaver|59|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderRecoverableFailure|60|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderRecoverableStorage|61|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderRemoved|62|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderResourceAdded|63|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderResourceRemoved|64|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderThermistorFailure|65|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderTimingFailure|66|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderTurnedOff|67|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderTurnedOn|68|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderUnderTemperature|69|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderUnrecoverableFailure|70|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderUnrecoverableStorageError|71|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|banderWarmingUp|72|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderAdded|73|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderAlmostEmpty|74|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderAlmostFull|75|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderAtLimit|76|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderClosed|77|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderConfigurationChange|78|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderCoverClosed|79|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderCoverOpen|80|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderEmpty|81|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderFull|82|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderInterlockClosed|83|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderInterlockOpen|84|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderJam|85|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderLifeAlmostOver|86|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderLifeOver|87|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderMemoryExtedted|88|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderMissing|89|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderMotorFailure|90|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderNearLimit|91|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderOffline|92|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderOpened|93|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderOverTemperature|94|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderPowerSaver|95|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderRecoverableFailure|96|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderRecoverableStorage|97|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderRemoved|98|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderResourceAdded|99|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderResourceRemoved|100|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderThermistorFailure|101|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderTimingFailure|102|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderTurnedOff|103|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderTurnedOn|104|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderUnderTemperature|105|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderUnrecoverableFailure|106|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderUnrecoverableStorageError|107|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|binderWarmingUp|108|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|cameraFailure|109|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|将cooling|110|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|将进行配置|111|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|heatHeating|112|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|将temperatureHigh|113|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|将temperatureLow|114|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|cleanerLifeAlmostOver|115|这是 PWG5100.13 中描述的标准 IPP 打印机属性值。|
|cleanerLifeOver|116|这是 PWG5100.13 中描述的标准 IPP 打印机属性值。|
|configurationChange|117|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|deactivated|118|这是 RFC3998 中描述的标准 IPP 打印机属性值。|
|deleted|119|这是 PWG5100.22 中描述的标准 IPP 打印机属性值。|
|utterCutterAdded|120|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterAlmostEmpty|121|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterAlmostFull|122|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterAtLimit|123|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterClosed|124|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterConfigurationChange|125|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterCoverClosed|126|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterCoverOpen|127|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterEmpty|128|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterFull|129|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterInterlockClosed|130|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterInterlockOpen|131|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterJam|132|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterLifeAlmostOver|133|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterLifeOver|134|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterMemoryExtedted|135|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterMissing|136|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterMotorFailure|137|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterNearLimit|138|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterOffline|139|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterOpened|140|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterOverTemperature|141|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterPowerSaver|142|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterRecoverableFailure|143|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterRecoverableStorage|144|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterRemoved|145|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterResourceAdded|146|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterResourceRemoved|147|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterThermistorFailure|148|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterTimingFailure|149|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterTurnedOff|150|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterTurnedOn|151|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterUnderTemperature|152|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterUnrecoverableFailure|153|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterUnrecoverableStorageError|154|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|utterCutterWarmingUp|155|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|extruderCooling|156|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|extruderFailure|157|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|extruderHeating|158|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|extruderJam|159|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|extruderTemperatureHigh|160|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|extruderTemperatureLow|161|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|fanFailure|162|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|faxModemLifeAlmostOver|163|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|faxModemLifeOver|164|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|faxModemMissing|165|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|faxModemTurnedOff|166|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|faxModemTurnedOn|167|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|folderAdded|168|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderAlmostEmpty|169|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderAlmostFull|170|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderAtLimit|171|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderClosed|172|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderConfigurationChange|173|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderCoverClosed|174|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderCoverOpen|175|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderEmpty|176|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderFull|177|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderInterlockClosed|178|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderInterlockOpen|179|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderJam|180|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderLifeAlmostOver|181|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderLifeOver|182|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderMemoryExtedted|183|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderMissing|184|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderMotorFailure|185|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderNearLimit|186|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderOffline|187|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderOpened|188|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderOverTemperature|189|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderPowerSaver|190|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderRecoverableFailure|191|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderRecoverableStorage|192|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderRemoved|193|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderResourceAdded|194|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderResourceRemoved|195|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderThermistorFailure|196|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderTimingFailure|197|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderTurnedOff|198|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderTurnedOn|199|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderUnderTemperature|200|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderUnrecoverableFailure|201|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderUnrecoverableStorageError|202|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|folderWarmingUp|203|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|休眠|204|这是 PWG5106.4 中描述的标准 IPP 打印机属性值。|
|holdNewJobs|205|这是 RFC3998 中描述的标准 IPP 打印机属性值。|
|identifyPrinterRequested|206|这是 PWG5100.18 中描述的标准 IPP 打印机属性值。|
|imprinterAdded|207|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterAlmostEmpty|208|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterAlmostFull|209|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterAtLimit|210|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterClosed|211|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterConfigurationChange|212|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterCoverClosed|213|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterCoverOpen|214|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterEmpty|215|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterFull|216|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterInterlockClosed|217|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterInterlockOpen|218|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterJam|219|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterLifeAlmostOver|220|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterLifeOver|221|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterMemoryExtedted|222|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterMissing|223|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterMotorFailure|224|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterNearLimit|225|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterOffline|226|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterOpened|227|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterOverTemperature|228|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterPowerSaver|229|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterRecoverableFailure|230|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterRecoverableStorage|231|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterRemoved|232|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterResourceAdded|233|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterResourceRemoved|234|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterThermistorFailure|235|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterTimingFailure|236|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterTurnedOff|237|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterTurnedOn|238|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterUnderTemperature|239|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterUnrecoverableFailure|240|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterUnrecoverableStorageError|241|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|imprinterWarmingUp|242|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inputCannotFeedSizeSelected|243|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inputManualInputRequest|244|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inputMediaColorChange|245|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inputMediaFormPartsChange|246|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inputMediaSizeChange|247|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inputMediaTrayFailure|248|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|inputMediaTrayFeedError|249|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|inputMediaTrayJam|250|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|inputMediaTypeChange|251|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inputMediaWeightChange|252|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inputPickRollerFailure|253|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|inputPickRollerLifeOver|254|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|inputPickRollerLifeWarn|255|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|inputPickRollerMissing|256|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|inputTrayElevationFailure|257|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inputTrayPositionFailure|258|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterAdded|259|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterAlmostEmpty|260|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterAlmostFull|261|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterAtLimit|262|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterClosed|263|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterConfigurationChange|264|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterCoverClosed|265|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterCoverOpen|266|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterEmpty|267|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterFull|268|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterInterlockClosed|269|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterInterlockOpen|270|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterJam|271|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterLifeAlmostOver|272|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterLifeOver|273|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterMemoryExtedted|274|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterMissing|275|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterMotorFailure|276|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterNearLimit|277|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterOffline|278|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterOpened|279|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterOverTemperature|280|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterPowerSaver|281|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterRecoverableFailure|282|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterRecoverableStorage|283|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterRemoved|284|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterResourceAdded|285|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterResourceRemoved|286|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterThermistorFailure|287|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterTimingFailure|288|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterTurnedOff|289|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterTurnedOn|290|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterUnderTemperature|291|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterUnrecoverableFailure|292|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterUnrecoverableStorageError|293|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|inserterWarmingUp|294|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|interlockClosed|295|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将cartridgeAdded|296|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将cartridgeDeleted|297|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将complexPageEncountered|298|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|interpreterMemoryDecrease|299|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将memoryIncrease|300|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|interpreterResourceAdded|301|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|interpreterResourceDeleted|302|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|lampAtEol|303|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|lampFailure|304|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|lampNearEol|305|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|laserAtEol|306|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|laserFailure|307|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|laserNearEol|308|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeAdded|309|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeAlmostEmpty|310|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeAlmostFull|311|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeAtLimit|312|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeClosed|313|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeConfigurationChange|314|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeCoverClosed|315|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeCoverOpen|316|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeEmpty|317|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeFull|318|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeInterlockClosed|319|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeInterlockOpen|320|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeJam|321|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeLifeAlmostOver|322|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeLifeOver|323|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeMemoryExtedted|324|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeMissing|325|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeMotorFailure|326|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeNearLimit|327|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeOffline|328|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeOpened|329|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeOverTemperature|330|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopePowerSaver|331|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeRecoverableFailure|332|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeRecoverableStorage|333|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeRemoved|334|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeResourceAdded|335|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeResourceRemoved|336|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeThermistorFailure|337|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeTimingFailure|338|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeTurnedOff|339|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeTurnedOn|340|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeUnderTemperature|341|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeUnrecoverableFailure|342|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeUnrecoverableStorageError|343|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|makeEnvelopeWarmingUp|344|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerAdjustingPrintQuality|345|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerCleanerMissing|346|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|markerDeveloperAlmostEmpty|347|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerDeveloperEmpty|348|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerDeveloperMissing|349|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|markerFuserMissing|350|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|markerFuserThermistorFailure|351|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerFuserTimingFailure|352|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerInkAlmostEmpty|353|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerInkEmpty|354|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerInkMissing|355|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|markerOpcMissing|356|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|markerPrintRibbonAlmostEmpty|357|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerPrintRibbonEmpty|358|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerPrintRibbonMissing|359|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|markerSupplyAlmostEmpty|360|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|markerSupplyMissing|361|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|markerTonerCartridgeMissing|362|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerTonerMissing|363|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|markerWasteInkReceptacleAlmostFull|364|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerWasteInkReceptacleFull|365|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerWasteInkReceptacleMissing|366|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|markerWasteMissing|367|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|markerWasteTonerReceptacleAlmostFull|368|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerWasteTonerReceptacleFull|369|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|markerWasteTonerReceptacleMissing|370|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|materialEmpty|371|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|materialLow|372|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|materialNeeded|373|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|mediaDrying|374|这是 HP20181213 中描述的标准 IPP 打印机属性值。|
|mediaPathCannotDuplexMediaSelected|375|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|mediaPathFailure|376|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathInputEmpty|377|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathInputFeedError|378|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathInputJam|379|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathInputRequest|380|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathJam|381|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathMediaTrayAlmostFull|382|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|mediaPathMediaTrayFull|383|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|mediaPathMediaTrayMissing|384|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|mediaPathOutputFeedError|385|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathOutputFull|386|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathOutputJam|387|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathPickRollerFailure|388|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathPickRollerLifeOver|389|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathPickRollerLifeWarn|390|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|mediaPathPickRollerMissing|391|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|motorFailure|392|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|outputMailboxSelectFailure|393|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|outputMediaTrayFailure|394|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|outputMediaTrayFeedError|395|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|outputMediaTrayJam|396|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|perforaterAdded|397|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterAlmostEmpty|398|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterAlmostFull|399|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterAtLimit|400|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterClosed|401|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterConfigurationChange|402|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterCoverClosed|403|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterCoverOpen|404|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterEmpty|405|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterFull|406|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterInterlockClosed|407|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterInterlockOpen|408|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterJam|409|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterLifeAlmostOver|410|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterLifeOver|411|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterMemoryExtedted|412|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterMissing|413|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterMotorFailure|414|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterNearLimit|415|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterOffline|416|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterOpened|417|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterOverTemperature|418|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterPowerSaver|419|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterRecoverableFailure|420|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterRecoverableStorage|421|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterRemoved|422|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterResourceAdded|423|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterResourceRemoved|424|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterThermistorFailure|425|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterTimingFailure|426|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterTurnedOff|427|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterTurnedOn|428|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterUnderTemperature|429|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterUnrecoverableFailure|430|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterUnrecoverableStorageError|431|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|perforaterWarmingUp|432|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|platformCooling|433|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|platformFailure|434|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|platformHeating|435|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|platformTemperatureHigh|436|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|platformTemperatureLow|437|这是 PWG5100.21 中描述的标准 IPP 打印机属性值。|
|powerDown|438|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|powerUp|439|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|printerManualReset|440|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|printerNmsReset|441|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|printerReadyToPrint|442|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|443|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一部分|444|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将almostFull|445|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|446|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|447|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些应用程序|448|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将coverClosed|449|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将covererCoverOpen|450|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|451|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|452|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|453|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一个功能区|454|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|455|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将lifeAlmostOver|456|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|457|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|458|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|459|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一个功能区|460|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一个 2013 年 1 月 2 日|461|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|462|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|463|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|puncherOverTemperature|464|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|465|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将recoverableFailure|466|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|covererRecoverableStorage|467|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|468|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将resourceAdded|469|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将resourceRemoved|470|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|471|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将timingFailure|472|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将turnederTurnedOff|473|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将turnederTurnedOn|474|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|475|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|476|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|477|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一个功能区|478|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|resuming|479|这是 PWG5100.22 中描述的标准 IPP 打印机属性值。|
|scanMediaPathFailure|480|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathInputEmpty|481|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathInputFeedError|482|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathInputJam|483|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathInputRequest|484|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathJam|485|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathOutputFeedError|486|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathOutputFull|487|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathOutputJam|488|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathPickRollerFailure|489|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathPickRollerLifeOver|490|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathPickRollerLifeWarn|491|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathPickRollerMissing|492|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathTrayAlmostFull|493|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathTrayFull|494|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scanMediaPathTrayMissing|495|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scannerLightFailure|496|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scannerLightLifeAlmostOver|497|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scannerLightLifeOver|498|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scannerLightMissing|499|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scannerSensorFailure|500|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scannerSensorLifeAlmostOver|501|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scannerSensorLifeOver|502|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|scannerSensorMissing|503|这是 PWG5107.3 中描述的标准 IPP 打印机属性值。|
|separationCutterAdded|504|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterAlmostEmpty|505|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterAlmostFull|506|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterAtLimit|507|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterClosed|508|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterConfigurationChange|509|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterCoverClosed|510|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterCoverOpen|511|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterEmpty|512|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterFull|513|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterInterlockClosed|514|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterInterlockOpen|515|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterJam|516|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterLifeAlmostOver|517|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterLifeOver|518|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterMemoryExtedted|519|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterMissing|520|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterMotorFailure|521|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterNearLimit|522|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterOffline|523|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterOpened|524|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterOverTemperature|525|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterPowerSaver|526|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterRecoverableFailure|527|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterRecoverableStorage|528|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterRemoved|529|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterResourceAdded|530|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterResourceRemoved|531|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterThermistorFailure|532|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterTimingFailure|533|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterTurnedOff|534|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterTurnedOn|535|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterUnderTemperature|536|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterUnrecoverableFailure|537|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterUnrecoverableStorageError|538|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|separationCutterWarmingUp|539|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorAdded|540|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorAlmostEmpty|541|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorAlmostFull|542|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorAtLimit|543|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorClosed|544|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorConfigurationChange|545|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorCoverClosed|546|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorCoverOpen|547|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorEmpty|548|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorFull|549|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorInterlockClosed|550|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorInterlockOpen|551|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorJam|552|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorLifeAlmostOver|553|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorLifeOver|554|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorMemoryExtedted|555|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorMissing|556|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorMotorFailure|557|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorNearLimit|558|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorOffline|559|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorOpened|560|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorOverTemperature|561|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorPowerSaver|562|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorRecoverableFailure|563|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorRecoverableStorage|564|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorRemoved|565|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorResourceAdded|566|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorResourceRemoved|567|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorThermistorFailure|568|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorTimingFailure|569|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorTurnedOff|570|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorTurnedOn|571|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorUnderTemperature|572|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorUnrecoverableFailure|573|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorUnrecoverableStorageError|574|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|sheetRotatorWarmingUp|575|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterAdded|576|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterAlmostEmpty|577|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterAlmostFull|578|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterAtLimit|579|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterClosed|580|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterConfigurationChange|581|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterCoverClosed|582|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterCoverOpen|583|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterEmpty|584|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterFull|585|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterInterlockClosed|586|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterInterlockOpen|587|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterJam|588|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterLifeAlmostOver|589|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterLifeOver|590|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterMemoryExtedted|591|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterMissing|592|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterMotorFailure|593|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterNearLimit|594|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterOffline|595|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterOpened|596|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterOverTemperature|597|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterPowerSaver|598|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterRecoverableFailure|599|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterRecoverableStorage|600|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterRemoved|601|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterResourceAdded|602|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterResourceRemoved|603|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterThermistorFailure|604|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterTimingFailure|605|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterTurnedOff|606|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterTurnedOn|607|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterUnderTemperature|608|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterUnrecoverableFailure|609|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterUnrecoverableStorageError|610|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|slitterWarmingUp|611|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerAdded|612|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerAlmostEmpty|613|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerAlmostFull|614|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerAtLimit|615|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerClosed|616|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerConfigurationChange|617|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerCoverClosed|618|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerCoverOpen|619|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerEmpty|620|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerFull|621|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerInterlockClosed|622|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerInterlockOpen|623|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerJam|624|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerLifeAlmostOver|625|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerLifeOver|626|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerMemoryExtedted|627|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerMissing|628|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerMotorFailure|629|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerNearLimit|630|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerOffline|631|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerOpened|632|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerOverTemperature|633|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerPowerSaver|634|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerRecoverableFailure|635|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerRecoverableStorage|636|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerRemoved|637|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerResourceAdded|638|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerResourceRemoved|639|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerThermistorFailure|640|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerTimingFailure|641|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerTurnedOff|642|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerTurnedOn|643|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerUnderTemperature|644|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerUnrecoverableFailure|645|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerUnrecoverableStorageError|646|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|stackerWarmingUp|647|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|备用|648|这是 PWG5106.4 中描述的标准 IPP 打印机属性值。|
|装订器Added|649|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerAlmostEmpty|650|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerAlmostFull|651|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerAtLimit|652|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器Closed|653|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器ConfigurationChange|654|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器CoverClosed|655|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器CoverOpen|656|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerEmpty|657|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器Full|658|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器InterlockClosed|659|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器InterlockOpen|660|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器Jam|661|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerLifeAlmostOver|662|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器LifeOver|663|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerMemoryExtedted|664|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerMissing|665|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器MotorFailure|666|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerNearLimit|667|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订线|668|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器Opened|669|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerOverTemperature|670|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器PowerSaver|671|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器RecoverableFailure|672|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器RecoverableStorage|673|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器Removed|674|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器ResourceAdded|675|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器ResourceRemoved|676|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerThermistorFailure|677|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器TimingFailure|678|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器TurnedOff|679|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器TurnedOn|680|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerUnderTemperature|681|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|装订器UnrecoverableFailure|682|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerUnrecoverableStorageError|683|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|staplerWarmingUp|684|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|685|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一部分|686|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将almostFull|687|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|688|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|689|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些应用程序|690|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将covererCoverClosed|691|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将covererCoverOpen|692|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|693|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一台或多张|694|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一台或多张|695|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一键式打开|696|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|697|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将lifeAlmostOver|698|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|699|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|700|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将missing|701|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一个 2013 年 1 月 2 日|702|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一个 2013|703|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|704|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|705|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将overTemperature|706|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一个 2013 年 1 月 2 日|707|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|covererRecoverableFailure|708|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|covererRecoverableStorage|709|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一台或多张|710|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将resourceAdded|711|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将resourceRemoved|712|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一台或多张|713|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将timingFailure|714|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|turnederTurnedOff|715|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|将turnederTurnedOn|716|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一些|717|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|covererUnrecoverableFailure|718|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|covererUnrecoverableStorageError|719|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|一个|720|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitAdded|721|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitAlmostEmpty|722|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitAlmostFull|723|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitAtLimit|724|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitClosed|725|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitCoolingDown|726|这是 HPINC20180215 中描述的标准 IPP 打印机属性值。|
|subunitEmpty|727|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitFull|728|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitLifeAlmostOver|729|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitLifeOver|730|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitMemoryExtedted|731|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitMissing|732|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitMotorFailure|733|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitNearLimit|734|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitOffline|735|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitOpened|736|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitOverTemperature|737|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitPowerSaver|738|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitRecoverableFailure|739|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitRecoverableStorage|740|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitRemoved|741|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitResourceAdded|742|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitResourceRemoved|743|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitThermistorFailure|744|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitTimingFailure|745|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitTurnedOff|746|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitTurnedOn|747|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitUnderTemperature|748|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitUnrecoverableFailure|749|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitUnrecoverableStorage|750|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|subunitWarmingUp|751|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|suspend|752|这是 PWG5106.4 中描述的标准 IPP 打印机属性值。|
|测试|753|这是 PWG5100.22 中描述的标准 IPP 打印机属性值。|
|trimmerAdded|754|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerAlmostEmpty|755|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerAlmostFull|756|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerAtLimit|757|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerClosed|758|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerConfigurationChange|759|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerCoverClosed|760|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerCoverOpen|761|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerEmpty|762|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerFull|763|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerInterlockClosed|764|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerInterlockOpen|765|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerJam|766|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerLifeAlmostOver|767|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerLifeOver|768|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerMemoryExtedted|769|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerMissing|770|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerMotorFailure|771|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerNearLimit|772|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerOffline|773|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerOpened|774|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerOverTemperature|775|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerPowerSaver|776|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerRecoverableFailure|777|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerRecoverableStorage|778|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerRemoved|779|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerResourceAdded|780|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerResourceRemoved|781|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerThermistorFailure|782|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerTimingFailure|783|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerTurnedOff|784|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerTurnedOn|785|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerUnderTemperature|786|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerUnrecoverableFailure|787|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerUnrecoverableStorageError|788|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|trimmerWarmingUp|789|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|unknown|790|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperAdded|791|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperAlmostEmpty|792|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperAlmostFull|793|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperAtLimit|794|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperClosed|795|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperConfigurationChange|796|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperCoverClosed|797|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperCoverOpen|798|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperEmpty|799|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperFull|800|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperInterlockClosed|801|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperInterlockOpen|802|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperJam|803|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperLifeAlmostOver|804|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperLifeOver|805|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperMemoryExtedted|806|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperMissing|807|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperMotorFailure|808|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperNearLimit|809|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperOffline|810|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperOpened|811|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperOverTemperature|812|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperPowerSaver|813|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperRecoverableFailure|814|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperRecoverableStorage|815|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperRemoved|816|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperResourceAdded|817|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperResourceRemoved|818|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperThermistorFailure|819|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperTimingFailure|820|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperTurnedOff|821|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperTurnedOn|822|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperUnderTemperature|823|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperUnrecoverableFailure|824|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperUnrecoverableStorageError|825|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|wrapperWarmingUp|826|这是 PWG5100.9 中描述的标准 IPP 打印机属性值。|
|unknownFutureValue|827|可发展枚举 sentinel 值。 请勿使用。|

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

