---
author: JeremyKelley
ms.date: 09/10/2017
title: 视频
localization_priority: Normal
description: 视频资源将与视频相关的数据项分组到一个单一结构。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7f79ca080182a4439277c4eb32a2ccccb4df2928
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238979"
---
# <a name="video-resource-type"></a><span data-ttu-id="7c713-103">Video 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c713-103">Video resource type</span></span>

<span data-ttu-id="7c713-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c713-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c713-105">**视频** 资源将与视频相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="7c713-105">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="7c713-p101">如果 [**DriveItem**](driveitem.md) 具有一个非 null **视频** 方面，则该项表示一个视频文件。通过从文件中提取元数据对 **视频** 资源的属性进行填充。</span><span class="sxs-lookup"><span data-stu-id="7c713-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c713-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c713-108">JSON representation</span></span>

<span data-ttu-id="7c713-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c713-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="7c713-110">属性</span><span class="sxs-lookup"><span data-stu-id="7c713-110">Properties</span></span>

| <span data-ttu-id="7c713-111">属性名称</span><span class="sxs-lookup"><span data-stu-id="7c713-111">Property name</span></span>             | <span data-ttu-id="7c713-112">类型</span><span class="sxs-lookup"><span data-stu-id="7c713-112">Type</span></span>   | <span data-ttu-id="7c713-113">说明</span><span class="sxs-lookup"><span data-stu-id="7c713-113">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="7c713-114">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="7c713-114">**audioBitsPerSample**</span></span>    | <span data-ttu-id="7c713-115">Int32</span><span class="sxs-lookup"><span data-stu-id="7c713-115">Int32</span></span>  | <span data-ttu-id="7c713-116">每个样本的音频位数。</span><span class="sxs-lookup"><span data-stu-id="7c713-116">Number of audio bits per sample.</span></span>
| <span data-ttu-id="7c713-117">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="7c713-117">**audioChannels**</span></span>         | <span data-ttu-id="7c713-118">Int32</span><span class="sxs-lookup"><span data-stu-id="7c713-118">Int32</span></span>  | <span data-ttu-id="7c713-119">音频频道数。</span><span class="sxs-lookup"><span data-stu-id="7c713-119">Number of audio channels.</span></span>
| <span data-ttu-id="7c713-120">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="7c713-120">**audioFormat**</span></span>           | <span data-ttu-id="7c713-121">string</span><span class="sxs-lookup"><span data-stu-id="7c713-121">string</span></span> | <span data-ttu-id="7c713-122">音频格式名称（AAC、MP3 等）。</span><span class="sxs-lookup"><span data-stu-id="7c713-122">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="7c713-123">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="7c713-123">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="7c713-124">Int32</span><span class="sxs-lookup"><span data-stu-id="7c713-124">Int32</span></span>  | <span data-ttu-id="7c713-125">每秒音频采样数。</span><span class="sxs-lookup"><span data-stu-id="7c713-125">Number of audio samples per second.</span></span>
| <span data-ttu-id="7c713-126">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="7c713-126">**bitrate**</span></span>               | <span data-ttu-id="7c713-127">Int32</span><span class="sxs-lookup"><span data-stu-id="7c713-127">Int32</span></span>  | <span data-ttu-id="7c713-128">视频比特率（以位/秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="7c713-128">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="7c713-129">**duration**</span><span class="sxs-lookup"><span data-stu-id="7c713-129">**duration**</span></span>              | <span data-ttu-id="7c713-130">Int64</span><span class="sxs-lookup"><span data-stu-id="7c713-130">Int64</span></span>  | <span data-ttu-id="7c713-131">文件时长（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="7c713-131">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="7c713-132">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="7c713-132">**fourCC**</span></span>                | <span data-ttu-id="7c713-133">string</span><span class="sxs-lookup"><span data-stu-id="7c713-133">string</span></span> | <span data-ttu-id="7c713-134">视频格式的“四个字符代码”名称。</span><span class="sxs-lookup"><span data-stu-id="7c713-134">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="7c713-135">**frameRate**</span><span class="sxs-lookup"><span data-stu-id="7c713-135">**frameRate**</span></span>             | <span data-ttu-id="7c713-136">double</span><span class="sxs-lookup"><span data-stu-id="7c713-136">double</span></span> | <span data-ttu-id="7c713-137">视频的帧速率。</span><span class="sxs-lookup"><span data-stu-id="7c713-137">Frame rate of the video.</span></span>
| <span data-ttu-id="7c713-138">**height**</span><span class="sxs-lookup"><span data-stu-id="7c713-138">**height**</span></span>                | <span data-ttu-id="7c713-139">Int32</span><span class="sxs-lookup"><span data-stu-id="7c713-139">Int32</span></span>  | <span data-ttu-id="7c713-140">视频高度（以像素为单位）。</span><span class="sxs-lookup"><span data-stu-id="7c713-140">Height of the video, in pixels.</span></span>
| <span data-ttu-id="7c713-141">**width**</span><span class="sxs-lookup"><span data-stu-id="7c713-141">**width**</span></span>                 | <span data-ttu-id="7c713-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7c713-142">Int32</span></span>  | <span data-ttu-id="7c713-143">视频的宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="7c713-143">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="7c713-144">注解</span><span class="sxs-lookup"><span data-stu-id="7c713-144">Remarks</span></span>

<span data-ttu-id="7c713-145">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="7c713-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->

