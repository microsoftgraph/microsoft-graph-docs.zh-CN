---
title: teleconferenceDeviceVideoQuality 资源类型
description: 表示视频电话会议设备视频质量数据。
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 33b781a5b32285f30b4be1c5941fa75bf836fac3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763226"
---
# <a name="teleconferencedevicevideoquality-resource-type"></a><span data-ttu-id="952f9-103">teleconferenceDeviceVideoQuality 资源类型</span><span class="sxs-lookup"><span data-stu-id="952f9-103">teleconferenceDeviceVideoQuality resource type</span></span>

<span data-ttu-id="952f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="952f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="952f9-105">表示视频电话会议设备视频质量数据。</span><span class="sxs-lookup"><span data-stu-id="952f9-105">Represents video teleconferencing device video quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="952f9-106">属性</span><span class="sxs-lookup"><span data-stu-id="952f9-106">Properties</span></span>

<span data-ttu-id="952f9-107">**TeleconferenceDeviceVideoQuality**资源继承[teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)中的属性，并包含以下其他属性。</span><span class="sxs-lookup"><span data-stu-id="952f9-107">The **teleconferenceDeviceVideoQuality** resource inherits the properties from [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md), and includes the following additional properties.</span></span>

| <span data-ttu-id="952f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="952f9-108">Property</span></span>     | <span data-ttu-id="952f9-109">类型</span><span class="sxs-lookup"><span data-stu-id="952f9-109">Type</span></span>        | <span data-ttu-id="952f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="952f9-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="952f9-111">averageInboundBitRate</span><span class="sxs-lookup"><span data-stu-id="952f9-111">averageInboundBitRate</span></span>|<span data-ttu-id="952f9-112">双精度</span><span class="sxs-lookup"><span data-stu-id="952f9-112">Double</span></span>|<span data-ttu-id="952f9-113">每秒平均入站流视频比特率。</span><span class="sxs-lookup"><span data-stu-id="952f9-113">The average inbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="952f9-114">averageInboundFrameRate</span><span class="sxs-lookup"><span data-stu-id="952f9-114">averageInboundFrameRate</span></span>|<span data-ttu-id="952f9-115">双精度</span><span class="sxs-lookup"><span data-stu-id="952f9-115">Double</span></span>|<span data-ttu-id="952f9-116">每秒平均入站流视频帧速率。</span><span class="sxs-lookup"><span data-stu-id="952f9-116">The average inbound stream video frame rate per second.</span></span>|
|<span data-ttu-id="952f9-117">averageOutboundBitRate</span><span class="sxs-lookup"><span data-stu-id="952f9-117">averageOutboundBitRate</span></span>|<span data-ttu-id="952f9-118">双精度</span><span class="sxs-lookup"><span data-stu-id="952f9-118">Double</span></span>|<span data-ttu-id="952f9-119">每秒的平均出站流视频比特率。</span><span class="sxs-lookup"><span data-stu-id="952f9-119">The average outbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="952f9-120">averageOutboundFrameRate</span><span class="sxs-lookup"><span data-stu-id="952f9-120">averageOutboundFrameRate</span></span>|<span data-ttu-id="952f9-121">双精度</span><span class="sxs-lookup"><span data-stu-id="952f9-121">Double</span></span>|<span data-ttu-id="952f9-122">每秒的平均出站流视频帧速率。</span><span class="sxs-lookup"><span data-stu-id="952f9-122">The average outbound stream video frame rate per second.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="952f9-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="952f9-123">JSON representation</span></span>

<span data-ttu-id="952f9-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="952f9-124">The following is a JSON representation of the resource.</span></span>

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
