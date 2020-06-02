---
title: deviceInfo 资源类型
description: DeviceInfo 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8387926d7b6c8b0f5bf2ea774dc8d248d956c916
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491950"
---
# <a name="deviceinfo-resource-type"></a><span data-ttu-id="bd5c7-103">deviceInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd5c7-103">deviceInfo resource type</span></span>

<span data-ttu-id="bd5c7-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="bd5c7-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="bd5c7-105">表示有关呼叫中使用的设备（麦克风、扬声器、相机等）的信息。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-105">Represents information about a device (microphone, speaker, camera, etc.) used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="bd5c7-106">属性</span><span class="sxs-lookup"><span data-stu-id="bd5c7-106">Properties</span></span>

| <span data-ttu-id="bd5c7-107">属性</span><span class="sxs-lookup"><span data-stu-id="bd5c7-107">Property</span></span>     | <span data-ttu-id="bd5c7-108">类型</span><span class="sxs-lookup"><span data-stu-id="bd5c7-108">Type</span></span>        | <span data-ttu-id="bd5c7-109">Description</span><span class="sxs-lookup"><span data-stu-id="bd5c7-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bd5c7-110">captureDeviceDriver</span><span class="sxs-lookup"><span data-stu-id="bd5c7-110">captureDeviceDriver</span></span>|<span data-ttu-id="bd5c7-111">String</span><span class="sxs-lookup"><span data-stu-id="bd5c7-111">String</span></span>|<span data-ttu-id="bd5c7-112">媒体终结点使用的捕获设备驱动程序的名称。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-112">Name of the capture device driver used by the media endpoint.</span></span>|
|<span data-ttu-id="bd5c7-113">captureDeviceName</span><span class="sxs-lookup"><span data-stu-id="bd5c7-113">captureDeviceName</span></span>|<span data-ttu-id="bd5c7-114">String</span><span class="sxs-lookup"><span data-stu-id="bd5c7-114">String</span></span>|<span data-ttu-id="bd5c7-115">媒体终结点使用的捕获设备的名称。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-115">Name of the capture device used by the media endpoint.</span></span>|
|<span data-ttu-id="bd5c7-116">captureNotFunctioningEventRatio</span><span class="sxs-lookup"><span data-stu-id="bd5c7-116">captureNotFunctioningEventRatio</span></span>|<span data-ttu-id="bd5c7-117">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-117">Double</span></span>|<span data-ttu-id="bd5c7-118">媒体终结点检测到捕获设备的呼叫的小部分工作不正常。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-118">Fraction of the call that the media endpoint detected the capture device was not working properly.</span></span>|
|<span data-ttu-id="bd5c7-119">cpuInsufficentEventRatio</span><span class="sxs-lookup"><span data-stu-id="bd5c7-119">cpuInsufficentEventRatio</span></span>|<span data-ttu-id="bd5c7-120">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-120">Double</span></span>|<span data-ttu-id="bd5c7-121">媒体终结点检测到可用 CPU 资源不足并导致发送和接收的音频质量不佳的调用的一小部分。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-121">Fraction of the call that the media endpoint detected the CPU resources available were insufficient and caused poor quality of the audio sent and received.</span></span>|
|<span data-ttu-id="bd5c7-122">deviceClippingEventRatio</span><span class="sxs-lookup"><span data-stu-id="bd5c7-122">deviceClippingEventRatio</span></span>|<span data-ttu-id="bd5c7-123">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-123">Double</span></span>|<span data-ttu-id="bd5c7-124">媒体终结点在捕获的音频中检测到的剪辑在导致发送的音频质量较差时检测到的呼叫的一小部分。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-124">Fraction of the call that the media endpoint detected clipping in the captured audio that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="bd5c7-125">deviceGlitchEventRatio</span><span class="sxs-lookup"><span data-stu-id="bd5c7-125">deviceGlitchEventRatio</span></span>|<span data-ttu-id="bd5c7-126">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-126">Double</span></span>|<span data-ttu-id="bd5c7-127">媒体终结点检测到或捕获的音频中由于导致发送或接收的音频质量较差而发生了故障或间隙的呼叫的一小部分。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-127">Fraction of the call that the media endpoint detected glitches or gaps in the audio played or captured that caused poor quality of the audio being sent or received.</span></span>|
|<span data-ttu-id="bd5c7-128">howlingEventCount</span><span class="sxs-lookup"><span data-stu-id="bd5c7-128">howlingEventCount</span></span>|<span data-ttu-id="bd5c7-129">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5c7-129">Int32</span></span>|<span data-ttu-id="bd5c7-130">呼叫期间媒体终结点检测到 howling 或 screeching 音频的次数。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-130">Number of times during the call that the media endpoint detected howling or screeching audio.</span></span>|
|<span data-ttu-id="bd5c7-131">initialSignalLevelRootMeanSquare</span><span class="sxs-lookup"><span data-stu-id="bd5c7-131">initialSignalLevelRootMeanSquare</span></span>|<span data-ttu-id="bd5c7-132">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-132">Double</span></span>|<span data-ttu-id="bd5c7-133">呼叫的前30秒内传入信号的根平均平方（RMS）。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-133">The root mean square (RMS) of the incoming signal of up to the first 30 seconds of the call.</span></span>|
|<span data-ttu-id="bd5c7-134">lowSpeechLevelEventRatio</span><span class="sxs-lookup"><span data-stu-id="bd5c7-134">lowSpeechLevelEventRatio</span></span>|<span data-ttu-id="bd5c7-135">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-135">Double</span></span>|<span data-ttu-id="bd5c7-136">媒体终结点检测到较低语音级别导致发送音频质量较差的呼叫的小部分。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-136">Fraction of the call that the media endpoint detected low speech level that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="bd5c7-137">lowSpeechToNoiseEventRatio</span><span class="sxs-lookup"><span data-stu-id="bd5c7-137">lowSpeechToNoiseEventRatio</span></span>|<span data-ttu-id="bd5c7-138">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-138">Double</span></span>|<span data-ttu-id="bd5c7-139">媒体终结点检测到的流量较低的流量的小到噪音级别导致音频质量较差的呼叫。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-139">Fraction of the call that the media endpoint detected low speech to noise level that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="bd5c7-140">micGlitchRate</span><span class="sxs-lookup"><span data-stu-id="bd5c7-140">micGlitchRate</span></span>|<span data-ttu-id="bd5c7-141">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-141">Double</span></span>|<span data-ttu-id="bd5c7-142">媒体终结点麦克风的每5分钟间隔一次的故障次数。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-142">Glitches per 5 minute interval for the media endpoint's microphone.</span></span>|
|<span data-ttu-id="bd5c7-143">receivedNoiseLevel</span><span class="sxs-lookup"><span data-stu-id="bd5c7-143">receivedNoiseLevel</span></span>|<span data-ttu-id="bd5c7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5c7-144">Int32</span></span>|<span data-ttu-id="bd5c7-145">被分类为单声道噪音或由媒体终结点的立体声噪音的左声道的音频的平均能量水平。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-145">Average energy level of received audio for audio classified as mono noise or left channel of stereo noise by the media endpoint.</span></span>|
|<span data-ttu-id="bd5c7-146">receivedSignalLevel</span><span class="sxs-lookup"><span data-stu-id="bd5c7-146">receivedSignalLevel</span></span>|<span data-ttu-id="bd5c7-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5c7-147">Int32</span></span>|<span data-ttu-id="bd5c7-148">被分类为单声道语音或左声道立体声语音（由媒体终结点）的音频的接收音频的平均能量水平。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-148">Average energy level of received audio for audio classified as mono speech, or left channel of stereo speech by the media endpoint.</span></span>|
|<span data-ttu-id="bd5c7-149">renderDeviceDriver</span><span class="sxs-lookup"><span data-stu-id="bd5c7-149">renderDeviceDriver</span></span>|<span data-ttu-id="bd5c7-150">String</span><span class="sxs-lookup"><span data-stu-id="bd5c7-150">String</span></span>|<span data-ttu-id="bd5c7-151">媒体终结点使用的呈现设备驱动程序的名称。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-151">Name of the render device driver used by the media endpoint.</span></span>|
|<span data-ttu-id="bd5c7-152">renderDeviceName</span><span class="sxs-lookup"><span data-stu-id="bd5c7-152">renderDeviceName</span></span>|<span data-ttu-id="bd5c7-153">String</span><span class="sxs-lookup"><span data-stu-id="bd5c7-153">String</span></span>|<span data-ttu-id="bd5c7-154">媒体终结点使用的呈现设备的名称。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-154">Name of the render device used by the media endpoint.</span></span>|
|<span data-ttu-id="bd5c7-155">renderMuteEventRatio</span><span class="sxs-lookup"><span data-stu-id="bd5c7-155">renderMuteEventRatio</span></span>|<span data-ttu-id="bd5c7-156">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-156">Double</span></span>|<span data-ttu-id="bd5c7-157">媒体终结点检测到设备呈现的一小部分的呼叫已静音。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-157">Fraction of the call that media endpoint detected device render is muted.</span></span>|
|<span data-ttu-id="bd5c7-158">renderNotFunctioningEventRatio</span><span class="sxs-lookup"><span data-stu-id="bd5c7-158">renderNotFunctioningEventRatio</span></span>|<span data-ttu-id="bd5c7-159">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-159">Double</span></span>|<span data-ttu-id="bd5c7-160">媒体终结点检测到呈现设备的呼叫的分数未正常运行。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-160">Fraction of the call that the media endpoint detected the render device was not working properly.</span></span>|
|<span data-ttu-id="bd5c7-161">renderZeroVolumeEventRatio</span><span class="sxs-lookup"><span data-stu-id="bd5c7-161">renderZeroVolumeEventRatio</span></span>|<span data-ttu-id="bd5c7-162">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-162">Double</span></span>|<span data-ttu-id="bd5c7-163">媒体终结点检测到的设备呈现卷的呼叫数设置为0。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-163">Fraction of the call that media endpoint detected device render volume is set to 0.</span></span>|
|<span data-ttu-id="bd5c7-164">sentNoiseLevel</span><span class="sxs-lookup"><span data-stu-id="bd5c7-164">sentNoiseLevel</span></span>|<span data-ttu-id="bd5c7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5c7-165">Int32</span></span>|<span data-ttu-id="bd5c7-166">媒体终结点被分类为单声道噪音或左声道立体声噪音的音频的已发送音频的平均能量水平。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-166">Average energy level of sent audio for audio classified as mono noise or left channel of stereo noise by the media endpoint.</span></span>|
|<span data-ttu-id="bd5c7-167">sentSignalLevel</span><span class="sxs-lookup"><span data-stu-id="bd5c7-167">sentSignalLevel</span></span>|<span data-ttu-id="bd5c7-168">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5c7-168">Int32</span></span>|<span data-ttu-id="bd5c7-169">被分类为单声道语音或左声道立体声语音（由媒体终结点进行分类）的音频的已发送音频的平均能量水平。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-169">Average energy level of sent audio for audio classified as mono speech, or left channel of stereo speech by the media endpoint.</span></span>|
|<span data-ttu-id="bd5c7-170">speakerGlitchRate</span><span class="sxs-lookup"><span data-stu-id="bd5c7-170">speakerGlitchRate</span></span>|<span data-ttu-id="bd5c7-171">双精度</span><span class="sxs-lookup"><span data-stu-id="bd5c7-171">Double</span></span>|<span data-ttu-id="bd5c7-172">媒体终结点的扬声器内部每5分钟的故障。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-172">Glitches per 5 minute internal for the media endpoint's loudspeaker.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bd5c7-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd5c7-173">JSON representation</span></span>

<span data-ttu-id="bd5c7-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd5c7-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.deviceInfo",
  "baseType": null
}-->

```json
{
  "captureDeviceDriver": "String",
  "captureDeviceName": "String",
  "captureNotFunctioningEventRatio": "Double",
  "cpuInsufficentEventRatio": "Double",
  "deviceClippingEventRatio": "Double",
  "deviceGlitchEventRatio": "Double",
  "howlingEventCount": 1024,
  "initialSignalLevelRootMeanSquare": "Double",
  "lowSpeechLevelEventRatio": "Double",
  "lowSpeechToNoiseEventRatio": "Double",
  "micGlitchRate": "Double",
  "receivedNoiseLevel": 1024,
  "receivedSignalLevel": 1024,
  "renderDeviceDriver": "String",
  "renderDeviceName": "String",
  "renderMuteEventRatio": "Double",
  "renderNotFunctioningEventRatio": "Double",
  "renderZeroVolumeEventRatio": "Double",
  "sentNoiseLevel": 1024,
  "sentSignalLevel": 1024,
  "speakerGlitchRate": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->