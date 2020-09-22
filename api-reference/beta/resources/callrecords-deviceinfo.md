---
title: deviceInfo 资源类型
description: DeviceInfo 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 944e827e0e7827190b3ff879a2f62d52d6fa15c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071529"
---
# <a name="deviceinfo-resource-type"></a>deviceInfo 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关呼叫中使用的设备 (麦克风、扬声器、相机等 ) 的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|captureDeviceDriver|String|媒体终结点使用的捕获设备驱动程序的名称。|
|captureDeviceName|String|媒体终结点使用的捕获设备的名称。|
|captureNotFunctioningEventRatio|双精度|媒体终结点检测到捕获设备的呼叫的小部分工作不正常。|
|cpuInsufficentEventRatio|双精度|媒体终结点检测到可用 CPU 资源不足并导致发送和接收的音频质量不佳的调用的一小部分。|
|deviceClippingEventRatio|双精度|媒体终结点在捕获的音频中检测到的剪辑在导致发送的音频质量较差时检测到的呼叫的一小部分。|
|deviceGlitchEventRatio|双精度|媒体终结点检测到或捕获的音频中由于导致发送或接收的音频质量较差而发生了故障或间隙的呼叫的一小部分。|
|howlingEventCount|Int32|呼叫期间媒体终结点检测到 howling 或 screeching 音频的次数。|
|initialSignalLevelRootMeanSquare|双精度|最高为呼叫的前30秒的传入信号的根平均平方 (RMS) 。|
|lowSpeechLevelEventRatio|双精度|媒体终结点检测到较低语音级别导致发送音频质量较差的呼叫的小部分。|
|lowSpeechToNoiseEventRatio|双精度|媒体终结点检测到的流量较低的流量的小到噪音级别导致音频质量较差的呼叫。|
|micGlitchRate|双精度|媒体终结点麦克风的每5分钟间隔一次的故障次数。|
|receivedNoiseLevel|Int32|被分类为单声道噪音或由媒体终结点的立体声噪音的左声道的音频的平均能量水平。|
|receivedSignalLevel|Int32|被分类为单声道语音或左声道立体声语音（由媒体终结点）的音频的接收音频的平均能量水平。|
|renderDeviceDriver|String|媒体终结点使用的呈现设备驱动程序的名称。|
|renderDeviceName|String|媒体终结点使用的呈现设备的名称。|
|renderMuteEventRatio|双精度|媒体终结点检测到设备呈现的一小部分的呼叫已静音。|
|renderNotFunctioningEventRatio|双精度|媒体终结点检测到呈现设备的呼叫的分数未正常运行。|
|renderZeroVolumeEventRatio|双精度|媒体终结点检测到的设备呈现卷的呼叫数设置为0。|
|sentNoiseLevel|Int32|媒体终结点被分类为单声道噪音或左声道立体声噪音的音频的已发送音频的平均能量水平。|
|sentSignalLevel|Int32|被分类为单声道语音或左声道立体声语音（由媒体终结点进行分类）的音频的已发送音频的平均能量水平。|
|speakerGlitchRate|双精度|媒体终结点的扬声器内部每5分钟的故障。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.deviceInfo",
  "baseType": null
}-->

```json
{
  "captureDeviceDriver": "String",
  "captureDeviceName": "String",
  "captureNotFunctioningEventRatio": "Double",
  "cpuInsufficentEventRatio": "Double",
  "deviceClippingEventRatio": "Double",
  "deviceGlitchEventRatio": "Double",
  "howlingEventCount": 1024,
  "initialSignalLevelRootMeanSquare": "Double",
  "lowSpeechLevelEventRatio": "Double",
  "lowSpeechToNoiseEventRatio": "Double",
  "micGlitchRate": "Double",
  "receivedNoiseLevel": 1024,
  "receivedSignalLevel": 1024,
  "renderDeviceDriver": "String",
  "renderDeviceName": "String",
  "renderMuteEventRatio": "Double",
  "renderNotFunctioningEventRatio": "Double",
  "renderZeroVolumeEventRatio": "Double",
  "sentNoiseLevel": 1024,
  "sentSignalLevel": 1024,
  "speakerGlitchRate": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

