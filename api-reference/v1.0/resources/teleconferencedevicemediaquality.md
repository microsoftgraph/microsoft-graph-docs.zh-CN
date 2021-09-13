---
title: teleconferenceDeviceMediaQuality 资源类型
description: 视频电话会议设备媒体质量数据。
ms.localizationpriority: medium
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 45ca9d4bdc34077ea19bdcbac866495a198ea5ab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128128"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a>teleconferenceDeviceMediaQuality 资源类型

命名空间：microsoft.graph

表示视频电话会议设备媒体质量数据。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|averageInboundJitter|期限|平均入站流网络抖动。|
|averageInboundPacketLossRateInPercentage|双精度|平均入站流数据包丢失率（以百分比表示 (0-100) 。 例如，0.01 表示 0.01%。|
|averageInboundRoundTripDelay|期限|平均入站流网络往返延迟。|
|averageOutboundJitter|期限|平均出站流网络抖动。|
|averageOutboundPacketLossRateInPercentage|双精度|从 0 到 100 (的平均出站流数据包丢失) 。 例如，0.01 表示 0.01%。|
|averageOutboundRoundTripDelay|期限|平均出站流网络往返延迟。|
|channelIndex|Int32|媒体的频道索引。 索引从 1 开始。  如果媒体会话包含 3 种视频形式，则频道索引将为 1、2 和 3。|
|inboundPackets|Int64|入站数据包的总数。|
|localIPAddress|String|媒体会话的本地 IP 地址。|
|localPort|Int32|本地媒体端口。|
|maximumInboundJitter|期限|最大入站流网络抖动。|
|maximumInboundPacketLossRateInPercentage|双精度|最大入站流数据包丢失率（以百分比表示 (0-100) 。 例如，0.01 表示 0.01%。|
|maximumInboundRoundTripDelay|期限|最大入站流网络往返延迟。|
|maximumOutboundJitter|期限|最大出站流网络抖动。|
|maximumOutboundPacketLossRateInPercentage|双精度|最大出站流数据包丢失率（以百分比表示 (0-100) 。 例如，0.01 表示 0.01%。|
|maximumOutboundRoundTripDelay|期限|最大出站流网络往返延迟。|
|mediaDuration|期限|总形式持续时间。 如果多次启用和禁用媒体，MediaDuration 将汇总所有持续时间。|
|networkLinkSpeedInBytes|Int64|网络链接速度（以字节为单位）|
|outboundPackets|Int64|出站数据包的总数。|
|remoteIPAddress|String|媒体会话的远程 IP 地址。|
|remotePort|Int32|远程媒体端口。|

### <a name="derived-types"></a>派生类型

| 类型                                                 | 说明                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [teleconferenceDeviceAudioQuality](teleconferencedeviceaudioquality.md)    | 视频电话会议设备音频质量数据。                          |
| [teleconferenceDeviceVideoQuality](teleconferencedevicevideoquality.md)    | 视频电话会议设备视频质量数据。                          |
| [teleconferenceDeviceScreenSharingQuality](teleconferencedevicescreensharingquality.md)    | 视频电话会议设备屏幕共享质量数据。 |

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

