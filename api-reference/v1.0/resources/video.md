---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 视频
localization_priority: Normal
description: 视频资源将与视频相关的数据项分组到一个单一结构。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 24af35fff4e867caa8e7052c821cb44d1f2c3755
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033430"
---
# <a name="video-resource-type"></a><span data-ttu-id="f1a03-103">Video 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1a03-103">Video resource type</span></span>

<span data-ttu-id="f1a03-104">**视频**资源将与视频相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="f1a03-104">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="f1a03-p101">如果 [**DriveItem**](driveitem.md) 具有一个非 null **视频**方面，则该项表示一个视频文件。通过从文件中提取元数据对**视频**资源的属性进行填充。</span><span class="sxs-lookup"><span data-stu-id="f1a03-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1a03-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1a03-107">JSON representation</span></span>

<span data-ttu-id="f1a03-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1a03-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="f1a03-109">属性</span><span class="sxs-lookup"><span data-stu-id="f1a03-109">Properties</span></span>

| <span data-ttu-id="f1a03-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="f1a03-110">Property name</span></span>             | <span data-ttu-id="f1a03-111">类型</span><span class="sxs-lookup"><span data-stu-id="f1a03-111">Type</span></span>   | <span data-ttu-id="f1a03-112">说明</span><span class="sxs-lookup"><span data-stu-id="f1a03-112">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="f1a03-113">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="f1a03-113">**audioBitsPerSample**</span></span>    | <span data-ttu-id="f1a03-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a03-114">Int32</span></span>  | <span data-ttu-id="f1a03-115">每个样本的音频位数。</span><span class="sxs-lookup"><span data-stu-id="f1a03-115">Number of audio bits per sample.</span></span>
| <span data-ttu-id="f1a03-116">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="f1a03-116">**audioChannels**</span></span>         | <span data-ttu-id="f1a03-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a03-117">Int32</span></span>  | <span data-ttu-id="f1a03-118">音频频道数。</span><span class="sxs-lookup"><span data-stu-id="f1a03-118">Number of audio channels.</span></span>
| <span data-ttu-id="f1a03-119">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="f1a03-119">**audioFormat**</span></span>           | <span data-ttu-id="f1a03-120">string</span><span class="sxs-lookup"><span data-stu-id="f1a03-120">string</span></span> | <span data-ttu-id="f1a03-121">音频格式名称（AAC、MP3 等）。</span><span class="sxs-lookup"><span data-stu-id="f1a03-121">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="f1a03-122">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="f1a03-122">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="f1a03-123">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a03-123">Int32</span></span>  | <span data-ttu-id="f1a03-124">每秒音频采样数。</span><span class="sxs-lookup"><span data-stu-id="f1a03-124">Number of audio samples per second.</span></span>
| <span data-ttu-id="f1a03-125">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="f1a03-125">**bitrate**</span></span>               | <span data-ttu-id="f1a03-126">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a03-126">Int32</span></span>  | <span data-ttu-id="f1a03-127">视频比特率（以位/秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f1a03-127">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="f1a03-128">**duration**</span><span class="sxs-lookup"><span data-stu-id="f1a03-128">**duration**</span></span>              | <span data-ttu-id="f1a03-129">Int64</span><span class="sxs-lookup"><span data-stu-id="f1a03-129">Int64</span></span>  | <span data-ttu-id="f1a03-130">文件时长（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f1a03-130">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="f1a03-131">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="f1a03-131">**fourCC**</span></span>                | <span data-ttu-id="f1a03-132">string</span><span class="sxs-lookup"><span data-stu-id="f1a03-132">string</span></span> | <span data-ttu-id="f1a03-133">视频格式的“四个字符代码”名称。</span><span class="sxs-lookup"><span data-stu-id="f1a03-133">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="f1a03-134">**frameRate**</span><span class="sxs-lookup"><span data-stu-id="f1a03-134">**frameRate**</span></span>             | <span data-ttu-id="f1a03-135">double</span><span class="sxs-lookup"><span data-stu-id="f1a03-135">double</span></span> | <span data-ttu-id="f1a03-136">视频的帧速率。</span><span class="sxs-lookup"><span data-stu-id="f1a03-136">Frame rate of the video.</span></span>
| <span data-ttu-id="f1a03-137">**height**</span><span class="sxs-lookup"><span data-stu-id="f1a03-137">**height**</span></span>                | <span data-ttu-id="f1a03-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a03-138">Int32</span></span>  | <span data-ttu-id="f1a03-139">视频高度（以像素为单位）。</span><span class="sxs-lookup"><span data-stu-id="f1a03-139">Height of the video, in pixels.</span></span>
| <span data-ttu-id="f1a03-140">**width**</span><span class="sxs-lookup"><span data-stu-id="f1a03-140">**width**</span></span>                 | <span data-ttu-id="f1a03-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a03-141">Int32</span></span>  | <span data-ttu-id="f1a03-142">视频的宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="f1a03-142">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="f1a03-143">注解</span><span class="sxs-lookup"><span data-stu-id="f1a03-143">Remarks</span></span>

<span data-ttu-id="f1a03-144">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="f1a03-144">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
