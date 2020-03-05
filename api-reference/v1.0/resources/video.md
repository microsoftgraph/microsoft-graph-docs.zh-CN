---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 视频
localization_priority: Normal
description: 视频资源将与视频相关的数据项分组到一个单一结构。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2982dbad8f1e06a2f1288bd499c88c77a4ef2fda
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446763"
---
# <a name="video-resource-type"></a><span data-ttu-id="0937f-103">Video 资源类型</span><span class="sxs-lookup"><span data-stu-id="0937f-103">Video resource type</span></span>

<span data-ttu-id="0937f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0937f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0937f-105">**视频**资源将与视频相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="0937f-105">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="0937f-p101">如果 [**DriveItem**](driveitem.md) 具有一个非 null **视频**方面，则该项表示一个视频文件。通过从文件中提取元数据对**视频**资源的属性进行填充。</span><span class="sxs-lookup"><span data-stu-id="0937f-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0937f-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0937f-108">JSON representation</span></span>

<span data-ttu-id="0937f-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0937f-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="0937f-110">属性</span><span class="sxs-lookup"><span data-stu-id="0937f-110">Properties</span></span>

| <span data-ttu-id="0937f-111">属性名称</span><span class="sxs-lookup"><span data-stu-id="0937f-111">Property name</span></span>             | <span data-ttu-id="0937f-112">类型</span><span class="sxs-lookup"><span data-stu-id="0937f-112">Type</span></span>   | <span data-ttu-id="0937f-113">说明</span><span class="sxs-lookup"><span data-stu-id="0937f-113">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="0937f-114">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="0937f-114">**audioBitsPerSample**</span></span>    | <span data-ttu-id="0937f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="0937f-115">Int32</span></span>  | <span data-ttu-id="0937f-116">每个样本的音频位数。</span><span class="sxs-lookup"><span data-stu-id="0937f-116">Number of audio bits per sample.</span></span>
| <span data-ttu-id="0937f-117">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="0937f-117">**audioChannels**</span></span>         | <span data-ttu-id="0937f-118">Int32</span><span class="sxs-lookup"><span data-stu-id="0937f-118">Int32</span></span>  | <span data-ttu-id="0937f-119">音频频道数。</span><span class="sxs-lookup"><span data-stu-id="0937f-119">Number of audio channels.</span></span>
| <span data-ttu-id="0937f-120">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="0937f-120">**audioFormat**</span></span>           | <span data-ttu-id="0937f-121">string</span><span class="sxs-lookup"><span data-stu-id="0937f-121">string</span></span> | <span data-ttu-id="0937f-122">音频格式名称（AAC、MP3 等）。</span><span class="sxs-lookup"><span data-stu-id="0937f-122">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="0937f-123">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="0937f-123">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="0937f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="0937f-124">Int32</span></span>  | <span data-ttu-id="0937f-125">每秒音频采样数。</span><span class="sxs-lookup"><span data-stu-id="0937f-125">Number of audio samples per second.</span></span>
| <span data-ttu-id="0937f-126">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="0937f-126">**bitrate**</span></span>               | <span data-ttu-id="0937f-127">Int32</span><span class="sxs-lookup"><span data-stu-id="0937f-127">Int32</span></span>  | <span data-ttu-id="0937f-128">视频比特率（以位/秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="0937f-128">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="0937f-129">**duration**</span><span class="sxs-lookup"><span data-stu-id="0937f-129">**duration**</span></span>              | <span data-ttu-id="0937f-130">Int64</span><span class="sxs-lookup"><span data-stu-id="0937f-130">Int64</span></span>  | <span data-ttu-id="0937f-131">文件时长（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="0937f-131">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="0937f-132">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="0937f-132">**fourCC**</span></span>                | <span data-ttu-id="0937f-133">string</span><span class="sxs-lookup"><span data-stu-id="0937f-133">string</span></span> | <span data-ttu-id="0937f-134">视频格式的“四个字符代码”名称。</span><span class="sxs-lookup"><span data-stu-id="0937f-134">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="0937f-135">**frameRate**</span><span class="sxs-lookup"><span data-stu-id="0937f-135">**frameRate**</span></span>             | <span data-ttu-id="0937f-136">double</span><span class="sxs-lookup"><span data-stu-id="0937f-136">double</span></span> | <span data-ttu-id="0937f-137">视频的帧速率。</span><span class="sxs-lookup"><span data-stu-id="0937f-137">Frame rate of the video.</span></span>
| <span data-ttu-id="0937f-138">**height**</span><span class="sxs-lookup"><span data-stu-id="0937f-138">**height**</span></span>                | <span data-ttu-id="0937f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0937f-139">Int32</span></span>  | <span data-ttu-id="0937f-140">视频高度（以像素为单位）。</span><span class="sxs-lookup"><span data-stu-id="0937f-140">Height of the video, in pixels.</span></span>
| <span data-ttu-id="0937f-141">**width**</span><span class="sxs-lookup"><span data-stu-id="0937f-141">**width**</span></span>                 | <span data-ttu-id="0937f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="0937f-142">Int32</span></span>  | <span data-ttu-id="0937f-143">视频的宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="0937f-143">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="0937f-144">注解</span><span class="sxs-lookup"><span data-stu-id="0937f-144">Remarks</span></span>

<span data-ttu-id="0937f-145">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="0937f-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
