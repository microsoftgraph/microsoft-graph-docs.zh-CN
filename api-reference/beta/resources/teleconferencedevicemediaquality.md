---
title: teleconferenceDeviceMediaQuality 资源类型
description: 视频电话会议设备媒体质量数据。
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6fa0bc09f2f6038dd49c8c804420ce042bd5ec93
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510581"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a>teleconferenceDeviceMediaQuality 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示视频电话会议设备媒体质量数据。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|averageInboundJitter|持续时间|平均入站流网络抖动。|
|averageInboundPacketLossRateInPercentage|双精度|以百分比表示的平均入站流数据包丢失率（0-100）。 例如，0.01 表示0.01%。|
|averageInboundRoundTripDelay|持续时间|平均入站流网络往返延迟。|
|averageOutboundJitter|持续时间|平均出站流网络抖动。|
|averageOutboundPacketLossRateInPercentage|双精度|以百分比表示的平均出站流数据包丢失率（0-100）。 例如，0.01 表示0.01%。|
|averageOutboundRoundTripDelay|持续时间|平均出站流网络往返延迟。|
|channelIndex|Int32|媒体的通道索引。 索引从1开始。  如果媒体会话包含3个视频形式，通道索引将为1、2和3。|
|inboundPackets|Int64|入站数据包的总数。|
|localIPAddress|String|媒体会话的本地 IP 地址。|
|localPort|Int32|本地媒体端口。|
|maximumInboundJitter|持续时间|最大入站流网络抖动。|
|maximumInboundPacketLossRateInPercentage|双精度|以百分比表示的最大入站流数据包丢失率（0-100）。 例如，0.01 表示0.01%。|
|maximumInboundRoundTripDelay|持续时间|入站流网络的最大往返延迟。|
|maximumOutboundJitter|持续时间|最大出站流网络抖动。|
|maximumOutboundPacketLossRateInPercentage|双精度|以百分比表示的最大出站流数据包丢失率（0-100）。 例如，0.01 表示0.01%。|
|maximumOutboundRoundTripDelay|持续时间|最大出站流网络往返延迟。|
|mediaDuration|持续时间|整个模态的持续时间。 如果启用和禁用媒体多次，则 MediaDuration 将的所有持续时间的总和。|
|networkLinkSpeedInBytes|Int64|网络链接速度（以字节为单位）|
|outboundPackets|Int64|出站数据包的总数。|
|remoteIPAddress|String|媒体会话的远程 IP 地址。|
|remotePort|Int32|远程媒体端口。|

### <a name="derived-types"></a>派生类型

| 类型                                                 | 说明                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [teleconferenceDeviceAudioQuality](teleconferencedeviceaudioquality.md)    | 视频电话会议设备音频质量数据。                          |
| [teleconferenceDeviceVideoQuality](teleconferencedevicevideoquality.md)    | 视频电话会议设备视频质量数据。                          |
| [teleconferenceDeviceScreenSharingQuality](teleconferencedevicescreensharingquality.md)    | 视频电话会议设备屏幕-共享质量数据。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceMediaQuality",
  "baseType": null
}-->

```json
{
  "averageInboundJitter": "String (ISO 8601 duration)",
  "averageInboundPacketLossRateInPercentage": 10,
  "averageInboundRoundTripDelay": "String (ISO 8601 duration)",
  "averageOutboundJitter": "String (ISO 8601 duration)",
  "averageOutboundPacketLossRateInPercentage": 10,
  "averageOutboundRoundTripDelay": "String (ISO 8601 duration)",
  "channelIndex": 1,
  "inboundPackets": 1024,
  "localIPAddress": "String",
  "localPort": 2000,
  "maximumInboundJitter": "String (ISO 8601 duration)",
  "maximumInboundPacketLossRateInPercentage": 12,
  "maximumInboundRoundTripDelay": "String (ISO 8601 duration)",
  "maximumOutboundJitter": "String (ISO 8601 duration)",
  "maximumOutboundPacketLossRateInPercentage": 12,
  "maximumOutboundRoundTripDelay": "String (ISO 8601 duration)",
  "mediaDuration": "String (ISO 8601 duration)",
  "networkLinkSpeedInBytes": 1000000,
  "outboundPackets": 1024,
  "remoteIPAddress": "String",
  "remotePort": 3000
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teleconferenceDeviceMediaQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
