---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: dd6ece46ce54fe791c0e6b5801287e2abad4fe48
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="video-resource-type"></a><span data-ttu-id="38d37-102">Video 资源类型</span><span class="sxs-lookup"><span data-stu-id="38d37-102">Video resource type</span></span>

<span data-ttu-id="38d37-103">**视频**资源将与视频相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="38d37-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="38d37-104">如果 [**DriveItem**](driveitem.md) 具有一个非 null **video** facet，则该项表示一个视频文件。</span><span class="sxs-lookup"><span data-stu-id="38d37-104">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the Video resource are populated by extracting metadata from the file.</span></span>
<span data-ttu-id="38d37-105">通过从文件中提取元数据填充 **Video** 资源的属性。</span><span class="sxs-lookup"><span data-stu-id="38d37-105">If a DriveItem has a non-null video facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38d37-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38d37-106">JSON representation</span></span>

<span data-ttu-id="38d37-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38d37-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="38d37-108">属性</span><span class="sxs-lookup"><span data-stu-id="38d37-108">Properties</span></span>

| <span data-ttu-id="38d37-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="38d37-109">Property name</span></span>             | <span data-ttu-id="38d37-110">类型</span><span class="sxs-lookup"><span data-stu-id="38d37-110">Type</span></span>   | <span data-ttu-id="38d37-111">说明</span><span class="sxs-lookup"><span data-stu-id="38d37-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="38d37-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="38d37-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="38d37-113">Int32</span><span class="sxs-lookup"><span data-stu-id="38d37-113">Int32</span></span>  | <span data-ttu-id="38d37-114">每个样本的音频位数。</span><span class="sxs-lookup"><span data-stu-id="38d37-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="38d37-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="38d37-115">**audioChannels**</span></span>         | <span data-ttu-id="38d37-116">Int32</span><span class="sxs-lookup"><span data-stu-id="38d37-116">Int32</span></span>  | <span data-ttu-id="38d37-117">音频频道数。</span><span class="sxs-lookup"><span data-stu-id="38d37-117">Number of audio channels.</span></span>
| <span data-ttu-id="38d37-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="38d37-118">**audioFormat**</span></span>           | <span data-ttu-id="38d37-119">string</span><span class="sxs-lookup"><span data-stu-id="38d37-119">string</span></span> | <span data-ttu-id="38d37-120">音频格式名称（AAC、MP3 等）。</span><span class="sxs-lookup"><span data-stu-id="38d37-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="38d37-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="38d37-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="38d37-122">Int32</span><span class="sxs-lookup"><span data-stu-id="38d37-122">Int32</span></span>  | <span data-ttu-id="38d37-123">每秒音频采样数。</span><span class="sxs-lookup"><span data-stu-id="38d37-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="38d37-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="38d37-124">**bitrate**</span></span>               | <span data-ttu-id="38d37-125">Int32</span><span class="sxs-lookup"><span data-stu-id="38d37-125">Int32</span></span>  | <span data-ttu-id="38d37-126">视频比特率（以位/秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="38d37-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="38d37-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="38d37-127">**duration**</span></span>              | <span data-ttu-id="38d37-128">Int64</span><span class="sxs-lookup"><span data-stu-id="38d37-128">Int64</span></span>  | <span data-ttu-id="38d37-129">文件时长（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="38d37-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="38d37-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="38d37-130">**fourCC**</span></span>                | <span data-ttu-id="38d37-131">string</span><span class="sxs-lookup"><span data-stu-id="38d37-131">string</span></span> | <span data-ttu-id="38d37-132">视频格式的“四个字符代码”名称。</span><span class="sxs-lookup"><span data-stu-id="38d37-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="38d37-133">**framerate**</span><span class="sxs-lookup"><span data-stu-id="38d37-133">**framerate**</span></span>             | <span data-ttu-id="38d37-134">double</span><span class="sxs-lookup"><span data-stu-id="38d37-134">double</span></span> | <span data-ttu-id="38d37-135">视频的帧速率。</span><span class="sxs-lookup"><span data-stu-id="38d37-135">Frame rate of the video.</span></span>
| <span data-ttu-id="38d37-136">**height**</span><span class="sxs-lookup"><span data-stu-id="38d37-136">**height**</span></span>                | <span data-ttu-id="38d37-137">Int32</span><span class="sxs-lookup"><span data-stu-id="38d37-137">Int32</span></span>  | <span data-ttu-id="38d37-138">视频的高度（以像素为单位）。</span><span class="sxs-lookup"><span data-stu-id="38d37-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="38d37-139">**width**</span><span class="sxs-lookup"><span data-stu-id="38d37-139">**width**</span></span>                 | <span data-ttu-id="38d37-140">Int32</span><span class="sxs-lookup"><span data-stu-id="38d37-140">Int32</span></span>  | <span data-ttu-id="38d37-141">视频的宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="38d37-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="38d37-142">注解</span><span class="sxs-lookup"><span data-stu-id="38d37-142">Remarks</span></span>

<span data-ttu-id="38d37-143">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="38d37-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
