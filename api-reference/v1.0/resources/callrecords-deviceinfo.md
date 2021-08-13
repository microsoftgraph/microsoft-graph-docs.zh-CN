---
title: deviceInfo 资源类型
description: deviceInfo 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6d4897d861c23721a8132badc28295b3e78855cb6e02bd8bd50c24f99475e0b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180898"
---
# <a name="deviceinfo-resource-type"></a>deviceInfo 资源类型

命名空间：microsoft.graph.callRecords

表示有关呼叫中使用的 (麦克风、扬声器、相机) 设备的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|captureDeviceDriver|String|媒体终结点使用的捕获设备驱动程序的名称。|
|captureDeviceName|String|媒体终结点使用的捕获设备的名称。|
|captureNotFunctioningEventRatio|双精度|媒体终结点检测到捕获设备未正常工作的通话的一小部分。|
|cpuInsufficentEventRatio|双精度|满足以下比例的通话：媒体终结点检测到可用 CPU 资源不足，导致已发送和已接收音频的质量差。|
|deviceClippingEventRatio|双精度|媒体终结点在捕获的音频中检测到剪辑导致发送的音频质量差的通话的一小部分。|
|deviceGlitchEventRatio|双精度|媒体终结点检测到播放或捕获的音频出现故障或缺陷导致发送或接收的音频质量差的通话的一小部分。|
|howlingEventCount|Int32|在呼叫期间，媒体终结点检测到声声或叫声音频次数。|
|initialSignalLevelRootMeanSquare|双精度|根平均值 (RMS) 呼叫前 30 秒传入信号的平均值。|
|lowSpeechLevelEventRatio|双精度|媒体终结点检测到语音级别低（导致发送的音频质量差）的通话的一小部分。|
|lowSpeechToNoiseEventRatio|双精度|媒体终结点检测到语音级别低到噪音级别导致发送的音频质量差的呼叫的一小部分。|
|micGlitchRate|双精度|媒体终结点的麦克风每 5 分钟发生一次故障。|
|receivedNoiseLevel|Int32|对于被分类为单声道噪音或左声道立体声噪音的音频，媒体终结点接收的音频的平均能量水平。|
|receivedSignalLevel|Int32|对于被分类为单声道语音或左声道立体声语音的音频，媒体终结点接收的音频的平均能量水平。|
|renderDeviceDriver|String|媒体终结点使用的呈现设备驱动程序的名称。|
|renderDeviceName|String|媒体终结点使用的呈现设备的名称。|
|renderMuteEventRatio|双精度|媒体终结点检测到设备呈现被静音的通话的一小部分。|
|renderNotFunctioningEventRatio|双精度|媒体终结点检测到呈现设备未正常工作的通话的一小部分。|
|renderZeroVolumeEventRatio|双精度|媒体终结点检测到设备呈现音量设置为 0 的通话的一小部分。|
|sentNoiseLevel|Int32|对于媒体终结点分类为单声道噪音或左声道立体声噪音的音频，发送的音频的平均能量水平。|
|sentSignalLevel|Int32|对于被分类为单声道语音或左声道立体声语音的音频，媒体终结点发送的音频的平均能量水平。|
|speakerGlitchRate|双精度|媒体终结点的扬声器每 5 分钟内部故障一次。|


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
