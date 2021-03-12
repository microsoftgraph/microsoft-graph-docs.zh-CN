---
title: mediaStream 资源类型
description: mediaStream 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f30aef10b29d2880b1c892522e9d91218c0b081b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721556"
---
# <a name="mediastream-resource-type"></a>mediaStream 资源类型

命名空间：microsoft.graph.callRecords

表示有关通话中两个终结点之间的媒体流的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|averageAudioDegradation|双精度|流降级的网络平均意见得分平均值。 表示网络丢失和抖动对接收的音频质量的影响。|
|averageAudioNetworkJitter|持续时间|按 [RFC 3550][]指定的流的平均抖动，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。|
|averageBandwidthEstimate|Int64|两个终结点之间的可用平均估计带宽（以位/秒为单位）。|
|averageJitter|持续时间|按 [RFC 3550][]指定的流的平均抖动，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。|
|averagePacketLossRate|双精度|流的平均数据包丢失率。|
|averageRatioOfConcealedSamples|双精度|丢包隐藏生成的样本的音频帧数与音频帧总数的比率。|
|averageReceivedFrameRate|双精度|在会话持续时间内计算的所有视频流每秒接收的平均帧数。|
|averageRoundTripTime|持续时间|按 [RFC 3550][]指定的平均网络传播往返时间，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。|
|averageVideoFrameLossPercentage|双精度|向用户显示的视频帧丢失的平均百分比。|
|averageVideoFrameRate|双精度|在会话持续期间计算的视频流每秒接收的平均帧数。|
|averageVideoPacketLossRate|双精度|按 [RFC 3550][]中指定的，数据包丢失的平均百分数在会话持续时间内计算。|
|endDateTime|DateTimeOffset|流结束时的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|lowFrameRateRatio|双精度|帧速率小于每秒 7.5 帧的通话的分数。|
|lowVideoProcessingCapabilityRatio|双精度|客户端运行低于预期视频处理容量的 70% 的通话的一小部分。|
|maxAudioNetworkJitter|持续时间|在会话期间，在 20 秒窗口中每个窗口计算的最大音频网络抖动，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。|
|maxJitter|持续时间|RFC 3550 中指定的流的最大抖动，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。|
|maxPacketLossRate|双精度|流的最大数据包丢失率。|
|maxRatioOfConcealedSamples|双精度|修复程序隐藏的数据包的最大比率。|
|maxRoundTripTime|持续时间|按 [RFC 3550][]指定的最大网络传播往返时间，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。|
|packetUtilization|Int64|流的数据包计数。|
|postForwardErrorCorrectionPacketLossRate|双精度|应用 FEC 后跨所有视频流和编解码器聚合的丢包率。|
|startDateTime|DateTimeOffset|流启动的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|streamDirection|microsoft.graph.callRecords.mediaStreamDirection|指示媒体流的方向。 可取值为：`callerToCallee`、`calleeToCaller`。|
|streamId|字符串|流的唯一标识符。|
|wasMediaBypassed|布尔值|如果媒体流绕过中介服务器，直接在客户端和 PSTN 网关/PBX 之间传输，则其为 True，否则为 false。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.mediaStream",
  "baseType": null
}-->

```json
{
  "averageAudioDegradation": "Double",
  "averageAudioNetworkJitter": "String (duration)",
  "averageBandwidthEstimate": 1024,
  "averageJitter": "String (duration)",
  "averagePacketLossRate": "Double",
  "averageRatioOfConcealedSamples": "Double",
  "averageReceivedFrameRate": "Double",
  "averageRoundTripTime": "String (duration)",
  "averageVideoFrameLossPercentage": "Double",
  "averageVideoFrameRate": "Double",
  "averageVideoPacketLossRate": "Double",
  "endDateTime": "String (timestamp)",
  "lowFrameRateRatio": "Double",
  "lowVideoProcessingCapabilityRatio": "Double",
  "maxAudioNetworkJitter": "String (duration)",
  "maxJitter": "String (duration)",
  "maxPacketLossRate": "Double",
  "maxRatioOfConcealedSamples": "Double",
  "maxRoundTripTime": "String (duration)",
  "packetUtilization": 1024,
  "postForwardErrorCorrectionPacketLossRate": "Double",
  "startDateTime": "String (timestamp)",
  "streamDirection": "String",
  "streamId": "String",
  "wasMediaBypassed": true
}
```

[ISO 8601]: https://www.iso.org/iso/iso8601
[RFC 3550]: https://tools.ietf.org/html/rfc3550

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
