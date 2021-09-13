---
title: teleconferenceDeviceVideoQuality 资源类型
description: 表示视频电话会议设备视频质量数据。
ms.localizationpriority: medium
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aabb72c315d08068c0450777ca914770171c75d6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128058"
---
# <a name="teleconferencedevicevideoquality-resource-type"></a>teleconferenceDeviceVideoQuality 资源类型

命名空间：microsoft.graph

表示视频电话会议设备视频质量数据。

## <a name="properties"></a>属性

**teleconferenceDeviceVideoQuality** 资源从 [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)继承属性，并包括以下附加属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|averageInboundBitRate|双精度|平均入站流视频比特率/秒。|
|averageInboundFrameRate|双精度|平均入站流视频帧速率/秒。|
|averageOutboundBitRate|双精度|平均出站流视频比特率/秒。|
|averageOutboundFrameRate|双精度|平均出站流视频帧速率/秒。|

### <a name="derived-types"></a>派生类型

| 类型                                                 | 说明                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [teleconferenceDeviceScreenSharingQuality](teleconferencedevicescreensharingquality.md)    | 视频电话会议设备屏幕共享质量数据。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceVideoQuality",
  "baseType": "microsoft.graph.teleconferenceDeviceMediaQuality"
}-->

```json
{
  "averageInboundBitRate": 1024,
  "averageInboundFrameRate": 1024,
  "averageInboundJitter": "String (ISO 8601 duration)",
  "averageInboundPacketLossRateInPercentage": 10,
  "averageInboundRoundTripDelay": "String (ISO 8601 duration)",
  "averageOutboundBitRate": 1024,
  "averageOutboundFrameRate": 1024,
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
  "description": "teleconferenceDeviceVideoQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

