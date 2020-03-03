---
title: mediaStream 资源类型
description: MediaStream 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0c75b49c25f0344fa64d56493523c0828d9794a8
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394699"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="f4498-103">mediaStream 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4498-103">mediaStream resource type</span></span>

<span data-ttu-id="f4498-104">命名空间： callRecords</span><span class="sxs-lookup"><span data-stu-id="f4498-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4498-105">表示有关呼叫中两个终结点之间的媒体流的信息。</span><span class="sxs-lookup"><span data-stu-id="f4498-105">Represents information about a media stream between two endpoints in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="f4498-106">属性</span><span class="sxs-lookup"><span data-stu-id="f4498-106">Properties</span></span>

| <span data-ttu-id="f4498-107">属性</span><span class="sxs-lookup"><span data-stu-id="f4498-107">Property</span></span>     | <span data-ttu-id="f4498-108">类型</span><span class="sxs-lookup"><span data-stu-id="f4498-108">Type</span></span>        | <span data-ttu-id="f4498-109">说明</span><span class="sxs-lookup"><span data-stu-id="f4498-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4498-110">averageAudioDegradation</span><span class="sxs-lookup"><span data-stu-id="f4498-110">averageAudioDegradation</span></span>|<span data-ttu-id="f4498-111">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-111">Double</span></span>|<span data-ttu-id="f4498-112">流的平均网络平均意见分数下降。</span><span class="sxs-lookup"><span data-stu-id="f4498-112">Average Network Mean Opinion Score degradation for stream.</span></span> <span data-ttu-id="f4498-113">表示网络丢失和抖动对接收的音频质量有多少影响。</span><span class="sxs-lookup"><span data-stu-id="f4498-113">Represents how much the network loss and jitter has impacted the quality of received audio.</span></span>|
|<span data-ttu-id="f4498-114">averageAudioNetworkJitter</span><span class="sxs-lookup"><span data-stu-id="f4498-114">averageAudioNetworkJitter</span></span>|<span data-ttu-id="f4498-115">持续时间</span><span class="sxs-lookup"><span data-stu-id="f4498-115">Duration</span></span>|<span data-ttu-id="f4498-116">根据[RFC 3550][]中指定的流计算的平均抖动（以[ISO 8601][]格式表示）。</span><span class="sxs-lookup"><span data-stu-id="f4498-116">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="f4498-117">例如，1秒表示为`'PT1S'`，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="f4498-117">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="f4498-118">averageBandwidthEstimate</span><span class="sxs-lookup"><span data-stu-id="f4498-118">averageBandwidthEstimate</span></span>|<span data-ttu-id="f4498-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f4498-119">Int64</span></span>|<span data-ttu-id="f4498-120">两个终结点之间的平均估计可用带宽（以位/秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f4498-120">Average estimated bandwidth available between two endpoints in bits per second.</span></span>|
|<span data-ttu-id="f4498-121">averageJitter</span><span class="sxs-lookup"><span data-stu-id="f4498-121">averageJitter</span></span>|<span data-ttu-id="f4498-122">持续时间</span><span class="sxs-lookup"><span data-stu-id="f4498-122">Duration</span></span>|<span data-ttu-id="f4498-123">根据[RFC 3550][]中指定的流计算的平均抖动（以[ISO 8601][]格式表示）。</span><span class="sxs-lookup"><span data-stu-id="f4498-123">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="f4498-124">例如，1秒表示为`'PT1S'`，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="f4498-124">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="f4498-125">averagePacketLossRate</span><span class="sxs-lookup"><span data-stu-id="f4498-125">averagePacketLossRate</span></span>|<span data-ttu-id="f4498-126">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-126">Double</span></span>|<span data-ttu-id="f4498-127">流的平均数据包丢失率。</span><span class="sxs-lookup"><span data-stu-id="f4498-127">Average packet loss rate for stream.</span></span>|
|<span data-ttu-id="f4498-128">averageRatioOfConcealedSamples</span><span class="sxs-lookup"><span data-stu-id="f4498-128">averageRatioOfConcealedSamples</span></span>|<span data-ttu-id="f4498-129">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-129">Double</span></span>|<span data-ttu-id="f4498-130">包含由数据包丢失含有丢生成的样本的音频帧数与音频帧总数的比值。</span><span class="sxs-lookup"><span data-stu-id="f4498-130">Ratio of the number of audio frames with samples generated by packet loss concealment to the total number of audio frames.</span></span>|
|<span data-ttu-id="f4498-131">averageReceivedFrameRate</span><span class="sxs-lookup"><span data-stu-id="f4498-131">averageReceivedFrameRate</span></span>|<span data-ttu-id="f4498-132">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-132">Double</span></span>|<span data-ttu-id="f4498-133">在会话持续期间计算出的所有视频流每秒接收的平均帧数。</span><span class="sxs-lookup"><span data-stu-id="f4498-133">Average frames per second received for all video streams computed over the duration of the session.</span></span>|
|<span data-ttu-id="f4498-134">averageRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="f4498-134">averageRoundTripTime</span></span>|<span data-ttu-id="f4498-135">持续时间</span><span class="sxs-lookup"><span data-stu-id="f4498-135">Duration</span></span>|<span data-ttu-id="f4498-136">[RFC 3550][]中指定的计算出的平均网络传播往返时间，以[ISO 8601][]格式表示。</span><span class="sxs-lookup"><span data-stu-id="f4498-136">Average network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="f4498-137">例如，1秒表示为`'PT1S'`，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="f4498-137">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="f4498-138">averageVideoFrameLossPercentage</span><span class="sxs-lookup"><span data-stu-id="f4498-138">averageVideoFrameLossPercentage</span></span>|<span data-ttu-id="f4498-139">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-139">Double</span></span>|<span data-ttu-id="f4498-140">向用户显示的视频帧丢失的平均百分比。</span><span class="sxs-lookup"><span data-stu-id="f4498-140">Average percentage of video frames lost as displayed to the user.</span></span>|
|<span data-ttu-id="f4498-141">averageVideoFrameRate</span><span class="sxs-lookup"><span data-stu-id="f4498-141">averageVideoFrameRate</span></span>|<span data-ttu-id="f4498-142">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-142">Double</span></span>|<span data-ttu-id="f4498-143">视频流每秒接收的平均帧数，在会话持续期间计算。</span><span class="sxs-lookup"><span data-stu-id="f4498-143">Average frames per second received for a video stream, computed over the duration of the session.</span></span>|
|<span data-ttu-id="f4498-144">averageVideoPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="f4498-144">averageVideoPacketLossRate</span></span>|<span data-ttu-id="f4498-145">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-145">Double</span></span>|<span data-ttu-id="f4498-146">在[RFC 3550][]中指定的数据包丢失的平均分数，在会话持续期间计算。</span><span class="sxs-lookup"><span data-stu-id="f4498-146">Average fraction of packets lost, as specified in [RFC 3550][], computed over the duration of the session.</span></span>|
|<span data-ttu-id="f4498-147">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f4498-147">endDateTime</span></span>|<span data-ttu-id="f4498-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4498-148">DateTimeOffset</span></span>|<span data-ttu-id="f4498-149">流结束时的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f4498-149">UTC time when the stream ended.</span></span> <span data-ttu-id="f4498-150">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f4498-150">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4498-151">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f4498-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f4498-152">lowFrameRateRatio</span><span class="sxs-lookup"><span data-stu-id="f4498-152">lowFrameRateRatio</span></span>|<span data-ttu-id="f4498-153">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-153">Double</span></span>|<span data-ttu-id="f4498-154">帧速率小于每秒7.5 帧数的呼叫分数。</span><span class="sxs-lookup"><span data-stu-id="f4498-154">Fraction of the call where frame rate is less than 7.5 frames per second.</span></span>|
|<span data-ttu-id="f4498-155">lowVideoProcessingCapabilityRatio</span><span class="sxs-lookup"><span data-stu-id="f4498-155">lowVideoProcessingCapabilityRatio</span></span>|<span data-ttu-id="f4498-156">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-156">Double</span></span>|<span data-ttu-id="f4498-157">客户端运行时间小于70% 的预期视频处理功能的分数。</span><span class="sxs-lookup"><span data-stu-id="f4498-157">Fraction of the call that the client is running less than 70% expected video processing capability.</span></span>|
|<span data-ttu-id="f4498-158">maxAudioNetworkJitter</span><span class="sxs-lookup"><span data-stu-id="f4498-158">maxAudioNetworkJitter</span></span>|<span data-ttu-id="f4498-159">持续时间</span><span class="sxs-lookup"><span data-stu-id="f4498-159">Duration</span></span>|<span data-ttu-id="f4498-160">在会话期间，每个20秒窗口计算出的音频网络抖动最大值，以[ISO 8601][]格式表示。</span><span class="sxs-lookup"><span data-stu-id="f4498-160">Maximum of audio network jitter computed over each of the 20 second windows during the session, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="f4498-161">例如，1秒表示为`'PT1S'`，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="f4498-161">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="f4498-162">maxJitter</span><span class="sxs-lookup"><span data-stu-id="f4498-162">maxJitter</span></span>|<span data-ttu-id="f4498-163">持续时间</span><span class="sxs-lookup"><span data-stu-id="f4498-163">Duration</span></span>|<span data-ttu-id="f4498-164">根据 RFC 3550 中指定的流计算的最大抖动（以[ISO 8601][]格式表示）。</span><span class="sxs-lookup"><span data-stu-id="f4498-164">Maximum jitter for the stream computed as specified in RFC 3550, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="f4498-165">例如，1秒表示为`'PT1S'`，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="f4498-165">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="f4498-166">maxPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="f4498-166">maxPacketLossRate</span></span>|<span data-ttu-id="f4498-167">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-167">Double</span></span>|<span data-ttu-id="f4498-168">流的最大数据包丢失率。</span><span class="sxs-lookup"><span data-stu-id="f4498-168">Maximum packet loss rate for the stream.</span></span>|
|<span data-ttu-id="f4498-169">maxRatioOfConcealedSamples</span><span class="sxs-lookup"><span data-stu-id="f4498-169">maxRatioOfConcealedSamples</span></span>|<span data-ttu-id="f4498-170">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-170">Double</span></span>|<span data-ttu-id="f4498-171">由修复程序隐藏的数据包的最大比率。</span><span class="sxs-lookup"><span data-stu-id="f4498-171">Maximum ratio of packets concealed by the healer.</span></span>|
|<span data-ttu-id="f4498-172">maxRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="f4498-172">maxRoundTripTime</span></span>|<span data-ttu-id="f4498-173">持续时间</span><span class="sxs-lookup"><span data-stu-id="f4498-173">Duration</span></span>|<span data-ttu-id="f4498-174">[RFC 3550][]中指定的计算的最大网络传播往返时间（以[ISO 8601][]格式表示）。</span><span class="sxs-lookup"><span data-stu-id="f4498-174">Maximum network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="f4498-175">例如，1秒表示为`'PT1S'`，其中 ' P ' 是持续时间指示器，' t ' 是时间指示器，' 是第二个指示符。</span><span class="sxs-lookup"><span data-stu-id="f4498-175">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="f4498-176">packetUtilization</span><span class="sxs-lookup"><span data-stu-id="f4498-176">packetUtilization</span></span>|<span data-ttu-id="f4498-177">Int64</span><span class="sxs-lookup"><span data-stu-id="f4498-177">Int64</span></span>|<span data-ttu-id="f4498-178">流的数据包计数。</span><span class="sxs-lookup"><span data-stu-id="f4498-178">Packet count for the stream.</span></span>|
|<span data-ttu-id="f4498-179">postForwardErrorCorrectionPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="f4498-179">postForwardErrorCorrectionPacketLossRate</span></span>|<span data-ttu-id="f4498-180">双精度</span><span class="sxs-lookup"><span data-stu-id="f4498-180">Double</span></span>|<span data-ttu-id="f4498-181">在所有视频流和编码解码器中应用 FEC 后的数据包丢失率。</span><span class="sxs-lookup"><span data-stu-id="f4498-181">Packet loss rate after FEC has been applied aggregated across all video streams and codecs.</span></span>|
|<span data-ttu-id="f4498-182">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f4498-182">startDateTime</span></span>|<span data-ttu-id="f4498-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4498-183">DateTimeOffset</span></span>|<span data-ttu-id="f4498-184">流启动时的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f4498-184">UTC time when the stream started.</span></span> <span data-ttu-id="f4498-185">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f4498-185">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4498-186">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f4498-186">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f4498-187">streamDirection</span><span class="sxs-lookup"><span data-stu-id="f4498-187">streamDirection</span></span>|<span data-ttu-id="f4498-188">String</span><span class="sxs-lookup"><span data-stu-id="f4498-188">String</span></span>|<span data-ttu-id="f4498-189">指示媒体流的方向。</span><span class="sxs-lookup"><span data-stu-id="f4498-189">Indicates the direction of the media stream.</span></span> <span data-ttu-id="f4498-190">可取值为：`callerToCallee`、`calleeToCaller`。</span><span class="sxs-lookup"><span data-stu-id="f4498-190">Possible values are: `callerToCallee`, `calleeToCaller`.</span></span>|
|<span data-ttu-id="f4498-191">streamId</span><span class="sxs-lookup"><span data-stu-id="f4498-191">streamId</span></span>|<span data-ttu-id="f4498-192">String</span><span class="sxs-lookup"><span data-stu-id="f4498-192">String</span></span>|<span data-ttu-id="f4498-193">流的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f4498-193">Unique identifier for the stream.</span></span>|
|<span data-ttu-id="f4498-194">wasMediaBypassed</span><span class="sxs-lookup"><span data-stu-id="f4498-194">wasMediaBypassed</span></span>|<span data-ttu-id="f4498-195">布尔</span><span class="sxs-lookup"><span data-stu-id="f4498-195">Boolean</span></span>|<span data-ttu-id="f4498-196">如此如果媒体流绕过中介服务器并直接在客户端和 PSTN 网关/PBX 之间进行，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="f4498-196">True if the media stream bypassed the Mediation Server and went straight between client and PSTN Gateway/PBX, false otherwise.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f4498-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4498-197">JSON representation</span></span>

<span data-ttu-id="f4498-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4498-198">The following is a JSON representation of the resource.</span></span>

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