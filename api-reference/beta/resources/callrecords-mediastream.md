---
title: mediaStream 资源类型
description: mediaStream 类型
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 180936a2a3bc36e1f7ccd9fe684439caf4531fd7
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924094"
---
# <a name="mediastream-resource-type"></a>mediaStream 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关调用中两个终结点之间的媒体流的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|audioCodec|microsoft.graph.callRecords.audioCodec|用于编码网络上传输音频的编解码器名称。 可能的值为：、、、、`pcma``pcmu`、`amrWide`、`g7221``g722`、、`g7221c`、`g729`、`muchv2``multiChannelAudio`、`opus`、`satin``satinFullband`、`rtAudio8`、`rtAudio16`、`silk`、`silkNarrow`、`silkWide`、、`siren`、、 `unknownFutureValue``xmsRTA``cn``invalid``unknown`|
|averageAudioDegradation|双精度|流的平均网络平均意见分数下降。 表示网络丢失和抖动对接收的音频质量的影响程度。|
|averageAudioNetworkJitter|期限|[RFC 3550][] 中指定的流的平均抖动，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 `'PT1S'`“P”是持续时间指定器，“T”是时间指定器，而“S”是第二个指定器。|
|averageBandwidthEstimate|Int64|两个终结点之间的平均估计带宽（以每秒位为单位）。|
|averageJitter|期限|[RFC 3550][] 中指定的流的平均抖动，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 `'PT1S'`“P”是持续时间指定器，“T”是时间指定器，而“S”是第二个指定器。|
|averagePacketLossRate|双精度|流的平均数据包丢失率。|
|averageRatioOfConcealedSamples|双精度|数据包丢失隐藏生成样本的音频帧数与音频帧总数之比。|
|averageReceivedFrameRate|双精度|在会话期间计算的所有视频流每秒接收的平均帧数。|
|averageRoundTripTime|期限|按 [RFC 3550][] 指定计算的平均网络传播往返时间，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 `'PT1S'`“P”是持续时间指定器，“T”是时间指定器，而“S”是第二个指定器。|
|averageVideoFrameLossPercentage|双精度|向用户显示的视频帧丢失的平均百分比。|
|averageVideoFrameRate|双精度|视频流每秒收到的平均帧数，在会话期间计算。|
|averageVideoPacketLossRate|双精度|在会话期间计算的 [RFC 3550][] 中指定的数据包丢失的平均分数。|
|endDateTime|DateTimeOffset|流结束时的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|lowFrameRateRatio|双精度|帧速率小于每秒 7.5 帧的调用的分数。|
|lowVideoProcessingCapabilityRatio|双精度|客户端运行的通话比例小于预期视频处理功能的 70%。|
|maxAudioNetworkJitter|期限|会话期间在每个 20 秒窗口上计算的音频网络抖动的最大值，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 `'PT1S'`“P”是持续时间指定器，“T”是时间指定器，而“S”是第二个指定器。|
|maxJitter|期限|RFC 3550 中指定的流的最大抖动，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 `'PT1S'`“P”是持续时间指定器，“T”是时间指定器，而“S”是第二个指定器。|
|maxPacketLossRate|双精度|流的最大数据包丢失率。|
|maxRatioOfConcealedSamples|双精度|由愈合器隐藏的数据包的最大比率。|
|maxRoundTripTime|期限|[RFC 3550][] 中指定的最大网络传播往返时间，以 [ISO 8601][] 格式表示。 例如，1 秒表示为 `'PT1S'`“P”是持续时间指定器，“T”是时间指定器，而“S”是第二个指定器。|
|packetUtilization|Int64|流的数据包计数。|
|postForwardErrorCorrectionPacketLossRate|双精度|在所有视频流和编解码器中应用 FEC 后的数据包丢失率。|
|startDateTime|DateTimeOffset|流启动时的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|streamDirection|microsoft.graph.callRecords.mediaStreamDirection|指示媒体流的方向。 可取值为：`callerToCallee`、`calleeToCaller`。|
|streamId|String|流的唯一标识符。|
|videoCodec|microsoft.graph.callRecords.videoCodec|用于编码视频以在网络上传输的编解码器名称。 可取值为：`unknown`、`invalid`、`av1`、`h263`、`h264`、`h264s`、`h264uc`、`h265`、`rtvc1`、`rtVideo`、`xrtvc1`、`unknownFutureValue`。|
|wasMediaBypassed|布尔值|如果媒体流绕过中介服务器并直接在客户端和 PSTN 网关/PBX 之间运行，则为 True，否则为 false。|


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
  "audioCodec": "String",
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
  "videoCodec": "String",
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
  "tocPath&quot;: &quot;"
}-->

