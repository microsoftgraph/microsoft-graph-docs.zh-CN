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
# <a name="mediastream-resource-type"></a><span data-ttu-id="b6040-103">mediaStream 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6040-103">mediaStream resource type</span></span>

<span data-ttu-id="b6040-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="b6040-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="b6040-105">表示有关通话中两个终结点之间的媒体流的信息。</span><span class="sxs-lookup"><span data-stu-id="b6040-105">Represents information about a media stream between two endpoints in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="b6040-106">属性</span><span class="sxs-lookup"><span data-stu-id="b6040-106">Properties</span></span>

| <span data-ttu-id="b6040-107">属性</span><span class="sxs-lookup"><span data-stu-id="b6040-107">Property</span></span>     | <span data-ttu-id="b6040-108">类型</span><span class="sxs-lookup"><span data-stu-id="b6040-108">Type</span></span>        | <span data-ttu-id="b6040-109">说明</span><span class="sxs-lookup"><span data-stu-id="b6040-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6040-110">averageAudioDegradation</span><span class="sxs-lookup"><span data-stu-id="b6040-110">averageAudioDegradation</span></span>|<span data-ttu-id="b6040-111">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-111">Double</span></span>|<span data-ttu-id="b6040-112">流降级的网络平均意见得分平均值。</span><span class="sxs-lookup"><span data-stu-id="b6040-112">Average Network Mean Opinion Score degradation for stream.</span></span> <span data-ttu-id="b6040-113">表示网络丢失和抖动对接收的音频质量的影响。</span><span class="sxs-lookup"><span data-stu-id="b6040-113">Represents how much the network loss and jitter has impacted the quality of received audio.</span></span>|
|<span data-ttu-id="b6040-114">averageAudioNetworkJitter</span><span class="sxs-lookup"><span data-stu-id="b6040-114">averageAudioNetworkJitter</span></span>|<span data-ttu-id="b6040-115">持续时间</span><span class="sxs-lookup"><span data-stu-id="b6040-115">Duration</span></span>|<span data-ttu-id="b6040-116">按 [RFC 3550][]指定的流的平均抖动，以 [ISO 8601][] 格式表示。</span><span class="sxs-lookup"><span data-stu-id="b6040-116">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="b6040-117">例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="b6040-117">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="b6040-118">averageBandwidthEstimate</span><span class="sxs-lookup"><span data-stu-id="b6040-118">averageBandwidthEstimate</span></span>|<span data-ttu-id="b6040-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b6040-119">Int64</span></span>|<span data-ttu-id="b6040-120">两个终结点之间的可用平均估计带宽（以位/秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="b6040-120">Average estimated bandwidth available between two endpoints in bits per second.</span></span>|
|<span data-ttu-id="b6040-121">averageJitter</span><span class="sxs-lookup"><span data-stu-id="b6040-121">averageJitter</span></span>|<span data-ttu-id="b6040-122">持续时间</span><span class="sxs-lookup"><span data-stu-id="b6040-122">Duration</span></span>|<span data-ttu-id="b6040-123">按 [RFC 3550][]指定的流的平均抖动，以 [ISO 8601][] 格式表示。</span><span class="sxs-lookup"><span data-stu-id="b6040-123">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="b6040-124">例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="b6040-124">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="b6040-125">averagePacketLossRate</span><span class="sxs-lookup"><span data-stu-id="b6040-125">averagePacketLossRate</span></span>|<span data-ttu-id="b6040-126">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-126">Double</span></span>|<span data-ttu-id="b6040-127">流的平均数据包丢失率。</span><span class="sxs-lookup"><span data-stu-id="b6040-127">Average packet loss rate for stream.</span></span>|
|<span data-ttu-id="b6040-128">averageRatioOfConcealedSamples</span><span class="sxs-lookup"><span data-stu-id="b6040-128">averageRatioOfConcealedSamples</span></span>|<span data-ttu-id="b6040-129">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-129">Double</span></span>|<span data-ttu-id="b6040-130">丢包隐藏生成的样本的音频帧数与音频帧总数的比率。</span><span class="sxs-lookup"><span data-stu-id="b6040-130">Ratio of the number of audio frames with samples generated by packet loss concealment to the total number of audio frames.</span></span>|
|<span data-ttu-id="b6040-131">averageReceivedFrameRate</span><span class="sxs-lookup"><span data-stu-id="b6040-131">averageReceivedFrameRate</span></span>|<span data-ttu-id="b6040-132">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-132">Double</span></span>|<span data-ttu-id="b6040-133">在会话持续时间内计算的所有视频流每秒接收的平均帧数。</span><span class="sxs-lookup"><span data-stu-id="b6040-133">Average frames per second received for all video streams computed over the duration of the session.</span></span>|
|<span data-ttu-id="b6040-134">averageRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="b6040-134">averageRoundTripTime</span></span>|<span data-ttu-id="b6040-135">持续时间</span><span class="sxs-lookup"><span data-stu-id="b6040-135">Duration</span></span>|<span data-ttu-id="b6040-136">按 [RFC 3550][]指定的平均网络传播往返时间，以 [ISO 8601][] 格式表示。</span><span class="sxs-lookup"><span data-stu-id="b6040-136">Average network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="b6040-137">例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="b6040-137">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="b6040-138">averageVideoFrameLossPercentage</span><span class="sxs-lookup"><span data-stu-id="b6040-138">averageVideoFrameLossPercentage</span></span>|<span data-ttu-id="b6040-139">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-139">Double</span></span>|<span data-ttu-id="b6040-140">向用户显示的视频帧丢失的平均百分比。</span><span class="sxs-lookup"><span data-stu-id="b6040-140">Average percentage of video frames lost as displayed to the user.</span></span>|
|<span data-ttu-id="b6040-141">averageVideoFrameRate</span><span class="sxs-lookup"><span data-stu-id="b6040-141">averageVideoFrameRate</span></span>|<span data-ttu-id="b6040-142">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-142">Double</span></span>|<span data-ttu-id="b6040-143">在会话持续期间计算的视频流每秒接收的平均帧数。</span><span class="sxs-lookup"><span data-stu-id="b6040-143">Average frames per second received for a video stream, computed over the duration of the session.</span></span>|
|<span data-ttu-id="b6040-144">averageVideoPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="b6040-144">averageVideoPacketLossRate</span></span>|<span data-ttu-id="b6040-145">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-145">Double</span></span>|<span data-ttu-id="b6040-146">按 [RFC 3550][]中指定的，数据包丢失的平均百分数在会话持续时间内计算。</span><span class="sxs-lookup"><span data-stu-id="b6040-146">Average fraction of packets lost, as specified in [RFC 3550][], computed over the duration of the session.</span></span>|
|<span data-ttu-id="b6040-147">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b6040-147">endDateTime</span></span>|<span data-ttu-id="b6040-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6040-148">DateTimeOffset</span></span>|<span data-ttu-id="b6040-149">流结束时的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b6040-149">UTC time when the stream ended.</span></span> <span data-ttu-id="b6040-150">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b6040-150">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b6040-151">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b6040-151">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b6040-152">lowFrameRateRatio</span><span class="sxs-lookup"><span data-stu-id="b6040-152">lowFrameRateRatio</span></span>|<span data-ttu-id="b6040-153">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-153">Double</span></span>|<span data-ttu-id="b6040-154">帧速率小于每秒 7.5 帧的通话的分数。</span><span class="sxs-lookup"><span data-stu-id="b6040-154">Fraction of the call where frame rate is less than 7.5 frames per second.</span></span>|
|<span data-ttu-id="b6040-155">lowVideoProcessingCapabilityRatio</span><span class="sxs-lookup"><span data-stu-id="b6040-155">lowVideoProcessingCapabilityRatio</span></span>|<span data-ttu-id="b6040-156">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-156">Double</span></span>|<span data-ttu-id="b6040-157">客户端运行低于预期视频处理容量的 70% 的通话的一小部分。</span><span class="sxs-lookup"><span data-stu-id="b6040-157">Fraction of the call that the client is running less than 70% expected video processing capability.</span></span>|
|<span data-ttu-id="b6040-158">maxAudioNetworkJitter</span><span class="sxs-lookup"><span data-stu-id="b6040-158">maxAudioNetworkJitter</span></span>|<span data-ttu-id="b6040-159">持续时间</span><span class="sxs-lookup"><span data-stu-id="b6040-159">Duration</span></span>|<span data-ttu-id="b6040-160">在会话期间，在 20 秒窗口中每个窗口计算的最大音频网络抖动，以 [ISO 8601][] 格式表示。</span><span class="sxs-lookup"><span data-stu-id="b6040-160">Maximum of audio network jitter computed over each of the 20 second windows during the session, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="b6040-161">例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="b6040-161">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="b6040-162">maxJitter</span><span class="sxs-lookup"><span data-stu-id="b6040-162">maxJitter</span></span>|<span data-ttu-id="b6040-163">持续时间</span><span class="sxs-lookup"><span data-stu-id="b6040-163">Duration</span></span>|<span data-ttu-id="b6040-164">RFC 3550 中指定的流的最大抖动，以 [ISO 8601][] 格式表示。</span><span class="sxs-lookup"><span data-stu-id="b6040-164">Maximum jitter for the stream computed as specified in RFC 3550, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="b6040-165">例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="b6040-165">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="b6040-166">maxPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="b6040-166">maxPacketLossRate</span></span>|<span data-ttu-id="b6040-167">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-167">Double</span></span>|<span data-ttu-id="b6040-168">流的最大数据包丢失率。</span><span class="sxs-lookup"><span data-stu-id="b6040-168">Maximum packet loss rate for the stream.</span></span>|
|<span data-ttu-id="b6040-169">maxRatioOfConcealedSamples</span><span class="sxs-lookup"><span data-stu-id="b6040-169">maxRatioOfConcealedSamples</span></span>|<span data-ttu-id="b6040-170">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-170">Double</span></span>|<span data-ttu-id="b6040-171">修复程序隐藏的数据包的最大比率。</span><span class="sxs-lookup"><span data-stu-id="b6040-171">Maximum ratio of packets concealed by the healer.</span></span>|
|<span data-ttu-id="b6040-172">maxRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="b6040-172">maxRoundTripTime</span></span>|<span data-ttu-id="b6040-173">持续时间</span><span class="sxs-lookup"><span data-stu-id="b6040-173">Duration</span></span>|<span data-ttu-id="b6040-174">按 [RFC 3550][]指定的最大网络传播往返时间，以 [ISO 8601][] 格式表示。</span><span class="sxs-lookup"><span data-stu-id="b6040-174">Maximum network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="b6040-175">例如，1 秒表示为 ，其中"P"是持续时间指示符 `'PT1S'` ，"T"是时间指示符，"S"是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="b6040-175">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="b6040-176">packetUtilization</span><span class="sxs-lookup"><span data-stu-id="b6040-176">packetUtilization</span></span>|<span data-ttu-id="b6040-177">Int64</span><span class="sxs-lookup"><span data-stu-id="b6040-177">Int64</span></span>|<span data-ttu-id="b6040-178">流的数据包计数。</span><span class="sxs-lookup"><span data-stu-id="b6040-178">Packet count for the stream.</span></span>|
|<span data-ttu-id="b6040-179">postForwardErrorCorrectionPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="b6040-179">postForwardErrorCorrectionPacketLossRate</span></span>|<span data-ttu-id="b6040-180">双精度</span><span class="sxs-lookup"><span data-stu-id="b6040-180">Double</span></span>|<span data-ttu-id="b6040-181">应用 FEC 后跨所有视频流和编解码器聚合的丢包率。</span><span class="sxs-lookup"><span data-stu-id="b6040-181">Packet loss rate after FEC has been applied aggregated across all video streams and codecs.</span></span>|
|<span data-ttu-id="b6040-182">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b6040-182">startDateTime</span></span>|<span data-ttu-id="b6040-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6040-183">DateTimeOffset</span></span>|<span data-ttu-id="b6040-184">流启动的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b6040-184">UTC time when the stream started.</span></span> <span data-ttu-id="b6040-185">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b6040-185">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b6040-186">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b6040-186">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b6040-187">streamDirection</span><span class="sxs-lookup"><span data-stu-id="b6040-187">streamDirection</span></span>|<span data-ttu-id="b6040-188">microsoft.graph.callRecords.mediaStreamDirection</span><span class="sxs-lookup"><span data-stu-id="b6040-188">microsoft.graph.callRecords.mediaStreamDirection</span></span>|<span data-ttu-id="b6040-189">指示媒体流的方向。</span><span class="sxs-lookup"><span data-stu-id="b6040-189">Indicates the direction of the media stream.</span></span> <span data-ttu-id="b6040-190">可取值为：`callerToCallee`、`calleeToCaller`。</span><span class="sxs-lookup"><span data-stu-id="b6040-190">Possible values are: `callerToCallee`, `calleeToCaller`.</span></span>|
|<span data-ttu-id="b6040-191">streamId</span><span class="sxs-lookup"><span data-stu-id="b6040-191">streamId</span></span>|<span data-ttu-id="b6040-192">字符串</span><span class="sxs-lookup"><span data-stu-id="b6040-192">String</span></span>|<span data-ttu-id="b6040-193">流的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b6040-193">Unique identifier for the stream.</span></span>|
|<span data-ttu-id="b6040-194">wasMediaBypassed</span><span class="sxs-lookup"><span data-stu-id="b6040-194">wasMediaBypassed</span></span>|<span data-ttu-id="b6040-195">布尔值</span><span class="sxs-lookup"><span data-stu-id="b6040-195">Boolean</span></span>|<span data-ttu-id="b6040-196">如果媒体流绕过中介服务器，直接在客户端和 PSTN 网关/PBX 之间传输，则其为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="b6040-196">True if the media stream bypassed the Mediation Server and went straight between client and PSTN Gateway/PBX, false otherwise.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b6040-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6040-197">JSON representation</span></span>

<span data-ttu-id="b6040-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6040-198">The following is a JSON representation of the resource.</span></span>

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
