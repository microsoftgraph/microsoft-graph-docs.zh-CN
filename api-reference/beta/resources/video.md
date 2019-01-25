---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
localization_priority: Normal
ms.openlocfilehash: db560abc31daecc6064820ef6ef958808ddbc297
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508543"
---
# <a name="video-resource-type"></a><span data-ttu-id="b5bd2-102">Video 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5bd2-102">Video resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5bd2-103">**视频**资源将与视频相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="b5bd2-p101">如果 DriveItem 具有一个非 null 视频方面，则该项表示一个视频文件。通过从文件中提取元数据对视频资源的属性进行填充。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5bd2-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5bd2-106">JSON representation</span></span>

<span data-ttu-id="b5bd2-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="b5bd2-108">属性</span><span class="sxs-lookup"><span data-stu-id="b5bd2-108">Properties</span></span>

| <span data-ttu-id="b5bd2-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="b5bd2-109">Property name</span></span>             | <span data-ttu-id="b5bd2-110">类型</span><span class="sxs-lookup"><span data-stu-id="b5bd2-110">Type</span></span>   | <span data-ttu-id="b5bd2-111">说明</span><span class="sxs-lookup"><span data-stu-id="b5bd2-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="b5bd2-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="b5bd2-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="b5bd2-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b5bd2-113">Int32</span></span>  | <span data-ttu-id="b5bd2-114">每个样本的音频位数。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="b5bd2-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="b5bd2-115">**audioChannels**</span></span>         | <span data-ttu-id="b5bd2-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b5bd2-116">Int32</span></span>  | <span data-ttu-id="b5bd2-117">音频频道数。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-117">Number of audio channels.</span></span>
| <span data-ttu-id="b5bd2-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="b5bd2-118">**audioFormat**</span></span>           | <span data-ttu-id="b5bd2-119">string</span><span class="sxs-lookup"><span data-stu-id="b5bd2-119">string</span></span> | <span data-ttu-id="b5bd2-120">音频格式名称（AAC、MP3 等）。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="b5bd2-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="b5bd2-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="b5bd2-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b5bd2-122">Int32</span></span>  | <span data-ttu-id="b5bd2-123">每秒音频采样数。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="b5bd2-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="b5bd2-124">**bitrate**</span></span>               | <span data-ttu-id="b5bd2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b5bd2-125">Int32</span></span>  | <span data-ttu-id="b5bd2-126">视频比特率（以位/秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="b5bd2-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="b5bd2-127">**duration**</span></span>              | <span data-ttu-id="b5bd2-128">Int64</span><span class="sxs-lookup"><span data-stu-id="b5bd2-128">Int64</span></span>  | <span data-ttu-id="b5bd2-129">文件时长（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="b5bd2-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="b5bd2-130">**fourCC**</span></span>                | <span data-ttu-id="b5bd2-131">string</span><span class="sxs-lookup"><span data-stu-id="b5bd2-131">string</span></span> | <span data-ttu-id="b5bd2-132">视频格式的“四个字符代码”名称。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="b5bd2-133">**framerate**</span><span class="sxs-lookup"><span data-stu-id="b5bd2-133">**framerate**</span></span>             | <span data-ttu-id="b5bd2-134">double</span><span class="sxs-lookup"><span data-stu-id="b5bd2-134">double</span></span> | <span data-ttu-id="b5bd2-135">视频的帧速率。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-135">Frame rate of the video.</span></span>
| <span data-ttu-id="b5bd2-136">**height**</span><span class="sxs-lookup"><span data-stu-id="b5bd2-136">**height**</span></span>                | <span data-ttu-id="b5bd2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b5bd2-137">Int32</span></span>  | <span data-ttu-id="b5bd2-138">视频高度（以像素为单位）。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="b5bd2-139">**width**</span><span class="sxs-lookup"><span data-stu-id="b5bd2-139">**width**</span></span>                 | <span data-ttu-id="b5bd2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b5bd2-140">Int32</span></span>  | <span data-ttu-id="b5bd2-141">视频的宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="b5bd2-142">注解</span><span class="sxs-lookup"><span data-stu-id="b5bd2-142">Remarks</span></span>

<span data-ttu-id="b5bd2-143">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b5bd2-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/video.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
