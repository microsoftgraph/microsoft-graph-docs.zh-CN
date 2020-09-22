---
title: teleconferenceDeviceMediaQuality 资源类型
description: 视频电话会议设备媒体质量数据。
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a01dd135c85288fd511975cce8781912f2975f4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046308"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a><span data-ttu-id="12398-103">teleconferenceDeviceMediaQuality 资源类型</span><span class="sxs-lookup"><span data-stu-id="12398-103">teleconferenceDeviceMediaQuality resource type</span></span>

<span data-ttu-id="12398-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12398-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12398-105">表示视频电话会议设备媒体质量数据。</span><span class="sxs-lookup"><span data-stu-id="12398-105">Represents video teleconferencing device media quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="12398-106">属性</span><span class="sxs-lookup"><span data-stu-id="12398-106">Properties</span></span>

| <span data-ttu-id="12398-107">属性</span><span class="sxs-lookup"><span data-stu-id="12398-107">Property</span></span>     | <span data-ttu-id="12398-108">类型</span><span class="sxs-lookup"><span data-stu-id="12398-108">Type</span></span>        | <span data-ttu-id="12398-109">说明</span><span class="sxs-lookup"><span data-stu-id="12398-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="12398-110">averageInboundJitter</span><span class="sxs-lookup"><span data-stu-id="12398-110">averageInboundJitter</span></span>|<span data-ttu-id="12398-111">持续时间</span><span class="sxs-lookup"><span data-stu-id="12398-111">Duration</span></span>|<span data-ttu-id="12398-112">平均入站流网络抖动。</span><span class="sxs-lookup"><span data-stu-id="12398-112">The average inbound stream network jitter.</span></span>|
|<span data-ttu-id="12398-113">averageInboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="12398-113">averageInboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="12398-114">双精度</span><span class="sxs-lookup"><span data-stu-id="12398-114">Double</span></span>|<span data-ttu-id="12398-115">以 (0-100) 为单位的平均入站流数据包丢失率（百分比）。</span><span class="sxs-lookup"><span data-stu-id="12398-115">The average inbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="12398-116">例如，0.01 表示0.01%。</span><span class="sxs-lookup"><span data-stu-id="12398-116">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="12398-117">averageInboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="12398-117">averageInboundRoundTripDelay</span></span>|<span data-ttu-id="12398-118">持续时间</span><span class="sxs-lookup"><span data-stu-id="12398-118">Duration</span></span>|<span data-ttu-id="12398-119">平均入站流网络往返延迟。</span><span class="sxs-lookup"><span data-stu-id="12398-119">The average inbound stream network round trip delay.</span></span>|
|<span data-ttu-id="12398-120">averageOutboundJitter</span><span class="sxs-lookup"><span data-stu-id="12398-120">averageOutboundJitter</span></span>|<span data-ttu-id="12398-121">持续时间</span><span class="sxs-lookup"><span data-stu-id="12398-121">Duration</span></span>|<span data-ttu-id="12398-122">平均出站流网络抖动。</span><span class="sxs-lookup"><span data-stu-id="12398-122">The average outbound stream network jitter.</span></span>|
|<span data-ttu-id="12398-123">averageOutboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="12398-123">averageOutboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="12398-124">双精度</span><span class="sxs-lookup"><span data-stu-id="12398-124">Double</span></span>|<span data-ttu-id="12398-125">平均出站流数据包丢失率 (0-100) 的百分比。</span><span class="sxs-lookup"><span data-stu-id="12398-125">The average outbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="12398-126">例如，0.01 表示0.01%。</span><span class="sxs-lookup"><span data-stu-id="12398-126">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="12398-127">averageOutboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="12398-127">averageOutboundRoundTripDelay</span></span>|<span data-ttu-id="12398-128">持续时间</span><span class="sxs-lookup"><span data-stu-id="12398-128">Duration</span></span>|<span data-ttu-id="12398-129">平均出站流网络往返延迟。</span><span class="sxs-lookup"><span data-stu-id="12398-129">The average outbound stream network round trip delay.</span></span>|
|<span data-ttu-id="12398-130">channelIndex</span><span class="sxs-lookup"><span data-stu-id="12398-130">channelIndex</span></span>|<span data-ttu-id="12398-131">Int32</span><span class="sxs-lookup"><span data-stu-id="12398-131">Int32</span></span>|<span data-ttu-id="12398-132">媒体的通道索引。</span><span class="sxs-lookup"><span data-stu-id="12398-132">The channel index of media.</span></span> <span data-ttu-id="12398-133">索引从1开始。</span><span class="sxs-lookup"><span data-stu-id="12398-133">Indexing begins with 1.</span></span>  <span data-ttu-id="12398-134">如果媒体会话包含3个视频形式，通道索引将为1、2和3。</span><span class="sxs-lookup"><span data-stu-id="12398-134">If a media session contains 3 video modalities, channel indexes will be 1, 2, and 3.</span></span>|
|<span data-ttu-id="12398-135">inboundPackets</span><span class="sxs-lookup"><span data-stu-id="12398-135">inboundPackets</span></span>|<span data-ttu-id="12398-136">Int64</span><span class="sxs-lookup"><span data-stu-id="12398-136">Int64</span></span>|<span data-ttu-id="12398-137">入站数据包的总数。</span><span class="sxs-lookup"><span data-stu-id="12398-137">The total number of the inbound packets.</span></span>|
|<span data-ttu-id="12398-138">localIPAddress</span><span class="sxs-lookup"><span data-stu-id="12398-138">localIPAddress</span></span>|<span data-ttu-id="12398-139">String</span><span class="sxs-lookup"><span data-stu-id="12398-139">String</span></span>|<span data-ttu-id="12398-140">媒体会话的本地 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="12398-140">the local IP address for the media session.</span></span>|
|<span data-ttu-id="12398-141">localPort</span><span class="sxs-lookup"><span data-stu-id="12398-141">localPort</span></span>|<span data-ttu-id="12398-142">Int32</span><span class="sxs-lookup"><span data-stu-id="12398-142">Int32</span></span>|<span data-ttu-id="12398-143">本地媒体端口。</span><span class="sxs-lookup"><span data-stu-id="12398-143">The local media port.</span></span>|
|<span data-ttu-id="12398-144">maximumInboundJitter</span><span class="sxs-lookup"><span data-stu-id="12398-144">maximumInboundJitter</span></span>|<span data-ttu-id="12398-145">持续时间</span><span class="sxs-lookup"><span data-stu-id="12398-145">Duration</span></span>|<span data-ttu-id="12398-146">最大入站流网络抖动。</span><span class="sxs-lookup"><span data-stu-id="12398-146">The maximum inbound stream network jitter.</span></span>|
|<span data-ttu-id="12398-147">maximumInboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="12398-147">maximumInboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="12398-148">双精度</span><span class="sxs-lookup"><span data-stu-id="12398-148">Double</span></span>|<span data-ttu-id="12398-149">以 (0-100) 的百分比表示的最大入站流数据包丢失率。</span><span class="sxs-lookup"><span data-stu-id="12398-149">The maximum inbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="12398-150">例如，0.01 表示0.01%。</span><span class="sxs-lookup"><span data-stu-id="12398-150">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="12398-151">maximumInboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="12398-151">maximumInboundRoundTripDelay</span></span>|<span data-ttu-id="12398-152">持续时间</span><span class="sxs-lookup"><span data-stu-id="12398-152">Duration</span></span>|<span data-ttu-id="12398-153">入站流网络的最大往返延迟。</span><span class="sxs-lookup"><span data-stu-id="12398-153">The maximum inbound stream network round trip delay.</span></span>|
|<span data-ttu-id="12398-154">maximumOutboundJitter</span><span class="sxs-lookup"><span data-stu-id="12398-154">maximumOutboundJitter</span></span>|<span data-ttu-id="12398-155">持续时间</span><span class="sxs-lookup"><span data-stu-id="12398-155">Duration</span></span>|<span data-ttu-id="12398-156">最大出站流网络抖动。</span><span class="sxs-lookup"><span data-stu-id="12398-156">The maximum outbound stream network jitter.</span></span>|
|<span data-ttu-id="12398-157">maximumOutboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="12398-157">maximumOutboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="12398-158">双精度</span><span class="sxs-lookup"><span data-stu-id="12398-158">Double</span></span>|<span data-ttu-id="12398-159">以 (0-100) 的百分比表示的最大出站流数据包丢失率。</span><span class="sxs-lookup"><span data-stu-id="12398-159">The maximum outbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="12398-160">例如，0.01 表示0.01%。</span><span class="sxs-lookup"><span data-stu-id="12398-160">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="12398-161">maximumOutboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="12398-161">maximumOutboundRoundTripDelay</span></span>|<span data-ttu-id="12398-162">持续时间</span><span class="sxs-lookup"><span data-stu-id="12398-162">Duration</span></span>|<span data-ttu-id="12398-163">最大出站流网络往返延迟。</span><span class="sxs-lookup"><span data-stu-id="12398-163">The maximum outbound stream network round trip delay.</span></span>|
|<span data-ttu-id="12398-164">mediaDuration</span><span class="sxs-lookup"><span data-stu-id="12398-164">mediaDuration</span></span>|<span data-ttu-id="12398-165">持续时间</span><span class="sxs-lookup"><span data-stu-id="12398-165">Duration</span></span>|<span data-ttu-id="12398-166">整个模态的持续时间。</span><span class="sxs-lookup"><span data-stu-id="12398-166">The total modality duration.</span></span> <span data-ttu-id="12398-167">如果启用和禁用媒体多次，则 MediaDuration 将的所有持续时间的总和。</span><span class="sxs-lookup"><span data-stu-id="12398-167">If the media enabled and disabled multiple times, MediaDuration will the summation of all of the durations.</span></span>|
|<span data-ttu-id="12398-168">networkLinkSpeedInBytes</span><span class="sxs-lookup"><span data-stu-id="12398-168">networkLinkSpeedInBytes</span></span>|<span data-ttu-id="12398-169">Int64</span><span class="sxs-lookup"><span data-stu-id="12398-169">Int64</span></span>|<span data-ttu-id="12398-170">网络链接速度（以字节为单位）</span><span class="sxs-lookup"><span data-stu-id="12398-170">The network link speed in bytes</span></span>|
|<span data-ttu-id="12398-171">outboundPackets</span><span class="sxs-lookup"><span data-stu-id="12398-171">outboundPackets</span></span>|<span data-ttu-id="12398-172">Int64</span><span class="sxs-lookup"><span data-stu-id="12398-172">Int64</span></span>|<span data-ttu-id="12398-173">出站数据包的总数。</span><span class="sxs-lookup"><span data-stu-id="12398-173">The total number of the outbound packets.</span></span>|
|<span data-ttu-id="12398-174">remoteIPAddress</span><span class="sxs-lookup"><span data-stu-id="12398-174">remoteIPAddress</span></span>|<span data-ttu-id="12398-175">String</span><span class="sxs-lookup"><span data-stu-id="12398-175">String</span></span>|<span data-ttu-id="12398-176">媒体会话的远程 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="12398-176">The remote IP address for the media session.</span></span>|
|<span data-ttu-id="12398-177">remotePort</span><span class="sxs-lookup"><span data-stu-id="12398-177">remotePort</span></span>|<span data-ttu-id="12398-178">Int32</span><span class="sxs-lookup"><span data-stu-id="12398-178">Int32</span></span>|<span data-ttu-id="12398-179">远程媒体端口。</span><span class="sxs-lookup"><span data-stu-id="12398-179">The remote media port.</span></span>|

### <a name="derived-types"></a><span data-ttu-id="12398-180">派生类型</span><span class="sxs-lookup"><span data-stu-id="12398-180">Derived types</span></span>

| <span data-ttu-id="12398-181">类型</span><span class="sxs-lookup"><span data-stu-id="12398-181">Type</span></span>                                                 | <span data-ttu-id="12398-182">说明</span><span class="sxs-lookup"><span data-stu-id="12398-182">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="12398-183">teleconferenceDeviceAudioQuality</span><span class="sxs-lookup"><span data-stu-id="12398-183">teleconferenceDeviceAudioQuality</span></span>](teleconferencedeviceaudioquality.md)    | <span data-ttu-id="12398-184">视频电话会议设备音频质量数据。</span><span class="sxs-lookup"><span data-stu-id="12398-184">Video teleconferencing device audio quality data.</span></span>                          |
| [<span data-ttu-id="12398-185">teleconferenceDeviceVideoQuality</span><span class="sxs-lookup"><span data-stu-id="12398-185">teleconferenceDeviceVideoQuality</span></span>](teleconferencedevicevideoquality.md)    | <span data-ttu-id="12398-186">视频电话会议设备视频质量数据。</span><span class="sxs-lookup"><span data-stu-id="12398-186">Video teleconferencing device video quality data.</span></span>                          |
| [<span data-ttu-id="12398-187">teleconferenceDeviceScreenSharingQuality</span><span class="sxs-lookup"><span data-stu-id="12398-187">teleconferenceDeviceScreenSharingQuality</span></span>](teleconferencedevicescreensharingquality.md)    | <span data-ttu-id="12398-188">视频电话会议设备屏幕-共享质量数据。</span><span class="sxs-lookup"><span data-stu-id="12398-188">Video teleconferencing device screen-sharing quality data.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="12398-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12398-189">JSON representation</span></span>

<span data-ttu-id="12398-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12398-190">The following is a JSON representation of the resource.</span></span>

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


