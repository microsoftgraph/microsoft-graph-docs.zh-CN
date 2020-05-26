---
title: mediaStream 资源类型
description: MediaStream 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 018fb6c036225c743f679deca7d2ccd9132f76e7
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353537"
---
# <a name="mediastream-resource-type"></a>mediaStream 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关呼叫中两个终结点之间的媒体流的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|averageAudioDegradation|双精度|流的平均网络平均意见分数下降。 表示网络丢失和抖动对接收的音频质量有多少影响。|
|averageAudioNetworkJitter|持续时间|根据[RFC 3550][]中指定的流计算的平均抖动（以[ISO 8601][]格式表示）。 例如，1秒表示为 `'PT1S'` ，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。|
|averageBandwidthEstimate|Int64|两个终结点之间的平均估计可用带宽（以位/秒为单位）。|
|averageJitter|持续时间|根据[RFC 3550][]中指定的流计算的平均抖动（以[ISO 8601][]格式表示）。 例如，1秒表示为 `'PT1S'` ，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。|
|averagePacketLossRate|双精度|流的平均数据包丢失率。|
|averageRatioOfConcealedSamples|双精度|包含由数据包丢失含有丢生成的样本的音频帧数与音频帧总数的比值。|
|averageReceivedFrameRate|双精度|在会话持续期间计算出的所有视频流每秒接收的平均帧数。|
|averageRoundTripTime|持续时间|[RFC 3550][]中指定的计算出的平均网络传播往返时间，以[ISO 8601][]格式表示。 例如，1秒表示为 `'PT1S'` ，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。|
|averageVideoFrameLossPercentage|双精度|向用户显示的视频帧丢失的平均百分比。|
|averageVideoFrameRate|双精度|视频流每秒接收的平均帧数，在会话持续期间计算。|
|averageVideoPacketLossRate|双精度|在[RFC 3550][]中指定的数据包丢失的平均分数，在会话持续期间计算。|
|endDateTime|DateTimeOffset|流结束时的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|lowFrameRateRatio|双精度|帧速率小于每秒7.5 帧数的呼叫分数。|
|lowVideoProcessingCapabilityRatio|双精度|客户端运行时间小于70% 的预期视频处理功能的分数。|
|maxAudioNetworkJitter|持续时间|在会话期间，每个20秒窗口计算出的音频网络抖动最大值，以[ISO 8601][]格式表示。 例如，1秒表示为 `'PT1S'` ，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。|
|maxJitter|持续时间|根据 RFC 3550 中指定的流计算的最大抖动（以[ISO 8601][]格式表示）。 例如，1秒表示为 `'PT1S'` ，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。|
|maxPacketLossRate|双精度|流的最大数据包丢失率。|
|maxRatioOfConcealedSamples|双精度|由修复程序隐藏的数据包的最大比率。|
|maxRoundTripTime|持续时间|[RFC 3550][]中指定的计算的最大网络传播往返时间（以[ISO 8601][]格式表示）。 例如，1秒表示为 `'PT1S'` ，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。|
|packetUtilization|Int64|流的数据包计数。|
|postForwardErrorCorrectionPacketLossRate|双精度|在所有视频流和编码解码器中应用 FEC 后的数据包丢失率。|
|startDateTime|DateTimeOffset|流启动时的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|streamDirection|callRecords。 mediaStreamDirection|指示媒体流的方向。 可取值为：`callerToCallee`、`calleeToCaller`。|
|streamId|字符串|流的唯一标识符。|
|wasMediaBypassed|Boolean|如此如果媒体流绕过中介服务器并直接在客户端和 PSTN 网关/PBX 之间进行，否则为 false。|


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