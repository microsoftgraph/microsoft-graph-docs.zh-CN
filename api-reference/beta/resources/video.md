---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: a9bf228d814526d089fb102444e6952558b07e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048273"
---
# <a name="video-resource-type"></a><span data-ttu-id="6e711-102">Video 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e711-102">Video resource type</span></span>

> <span data-ttu-id="6e711-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6e711-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e711-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6e711-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e711-105">**视频**资源将与视频相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="6e711-105">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="6e711-p102">如果 [**DriveItem**](driveitem.md) 具有一个非 null **视频**方面，则该项表示一个视频文件。通过从文件中提取元数据对**视频**资源的属性进行填充。</span><span class="sxs-lookup"><span data-stu-id="6e711-p102">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e711-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e711-108">JSON representation</span></span>

<span data-ttu-id="6e711-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e711-109">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.video"
}-->

```json
{
  "audioBitsPerSample": 16,
  "audioChannels": 1,
  "audioFormat": "AAC",
  "audioSamplesPerSecond": 44100,
  "bitrate": 39101896,
  "duration": 8053,
  "fourCC": "H264",
  "frameRate": 239.877,
  "height": 1280,
  "width": 720
}
```

## <a name="properties"></a><span data-ttu-id="6e711-110">属性</span><span class="sxs-lookup"><span data-stu-id="6e711-110">Properties</span></span>

| <span data-ttu-id="6e711-111">属性名称</span><span class="sxs-lookup"><span data-stu-id="6e711-111">Property name</span></span>             | <span data-ttu-id="6e711-112">类型</span><span class="sxs-lookup"><span data-stu-id="6e711-112">Type</span></span>   | <span data-ttu-id="6e711-113">说明</span><span class="sxs-lookup"><span data-stu-id="6e711-113">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="6e711-114">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="6e711-114">**audioBitsPerSample**</span></span>    | <span data-ttu-id="6e711-115">Int32</span><span class="sxs-lookup"><span data-stu-id="6e711-115">Int32</span></span>  | <span data-ttu-id="6e711-116">每个样本的音频位数。</span><span class="sxs-lookup"><span data-stu-id="6e711-116">Number of audio bits per sample.</span></span>
| <span data-ttu-id="6e711-117">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="6e711-117">**audioChannels**</span></span>         | <span data-ttu-id="6e711-118">Int32</span><span class="sxs-lookup"><span data-stu-id="6e711-118">Int32</span></span>  | <span data-ttu-id="6e711-119">音频频道数。</span><span class="sxs-lookup"><span data-stu-id="6e711-119">Number of audio channels.</span></span>
| <span data-ttu-id="6e711-120">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="6e711-120">**audioFormat**</span></span>           | <span data-ttu-id="6e711-121">string</span><span class="sxs-lookup"><span data-stu-id="6e711-121">string</span></span> | <span data-ttu-id="6e711-122">音频格式名称（AAC、MP3 等）。</span><span class="sxs-lookup"><span data-stu-id="6e711-122">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="6e711-123">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="6e711-123">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="6e711-124">Int32</span><span class="sxs-lookup"><span data-stu-id="6e711-124">Int32</span></span>  | <span data-ttu-id="6e711-125">每秒音频采样数。</span><span class="sxs-lookup"><span data-stu-id="6e711-125">Number of audio samples per second.</span></span>
| <span data-ttu-id="6e711-126">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="6e711-126">**bitrate**</span></span>               | <span data-ttu-id="6e711-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6e711-127">Int32</span></span>  | <span data-ttu-id="6e711-128">视频比特率（以位/秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="6e711-128">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="6e711-129">**duration**</span><span class="sxs-lookup"><span data-stu-id="6e711-129">**duration**</span></span>              | <span data-ttu-id="6e711-130">Int64</span><span class="sxs-lookup"><span data-stu-id="6e711-130">Int64</span></span>  | <span data-ttu-id="6e711-131">文件时长（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="6e711-131">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="6e711-132">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="6e711-132">**fourCC**</span></span>                | <span data-ttu-id="6e711-133">string</span><span class="sxs-lookup"><span data-stu-id="6e711-133">string</span></span> | <span data-ttu-id="6e711-134">视频格式的“四个字符代码”名称。</span><span class="sxs-lookup"><span data-stu-id="6e711-134">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="6e711-135">**framerate**</span><span class="sxs-lookup"><span data-stu-id="6e711-135">**framerate**</span></span>             | <span data-ttu-id="6e711-136">double</span><span class="sxs-lookup"><span data-stu-id="6e711-136">double</span></span> | <span data-ttu-id="6e711-137">视频的帧速率。</span><span class="sxs-lookup"><span data-stu-id="6e711-137">Frame rate of the video.</span></span>
| <span data-ttu-id="6e711-138">**height**</span><span class="sxs-lookup"><span data-stu-id="6e711-138">**height**</span></span>                | <span data-ttu-id="6e711-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6e711-139">Int32</span></span>  | <span data-ttu-id="6e711-140">视频高度（以像素为单位）。</span><span class="sxs-lookup"><span data-stu-id="6e711-140">Height of the video, in pixels.</span></span>
| <span data-ttu-id="6e711-141">**width**</span><span class="sxs-lookup"><span data-stu-id="6e711-141">**width**</span></span>                 | <span data-ttu-id="6e711-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6e711-142">Int32</span></span>  | <span data-ttu-id="6e711-143">视频的宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="6e711-143">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="6e711-144">注解</span><span class="sxs-lookup"><span data-stu-id="6e711-144">Remarks</span></span>

<span data-ttu-id="6e711-145">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="6e711-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": ""
}-->
