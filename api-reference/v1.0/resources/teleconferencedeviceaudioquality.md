---
title: teleconferenceDeviceAudioQuality 资源类型
description: 视频电话会议设备音频质量数据。
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8c2d5cb6201f035065e5f46278dce60c70f876e4
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082716"
---
# <a name="teleconferencedeviceaudioquality-resource-type"></a><span data-ttu-id="f5e16-103">teleconferenceDeviceAudioQuality 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5e16-103">teleconferenceDeviceAudioQuality resource type</span></span>

<span data-ttu-id="f5e16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5e16-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5e16-105">表示视频电话会议设备音频质量数据。</span><span class="sxs-lookup"><span data-stu-id="f5e16-105">Represents video teleconferencing device audio quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="f5e16-106">属性</span><span class="sxs-lookup"><span data-stu-id="f5e16-106">Properties</span></span>

<span data-ttu-id="f5e16-107">**teleconferenceDeviceAudioQuality**继承[teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)资源的所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5e16-107">**teleconferenceDeviceAudioQuality** inherits all the properties of the [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5e16-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5e16-108">JSON representation</span></span>

<span data-ttu-id="f5e16-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5e16-109">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceAudioQuality",
  "baseType": "microsoft.graph.teleconferenceDeviceMediaQuality"
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
  "description": "teleconferenceDeviceAudioQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
