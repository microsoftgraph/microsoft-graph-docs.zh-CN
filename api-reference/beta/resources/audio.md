---
author: ananmishr
description: Audio 资源将与音频相关的属性分组到一个单一结构。
ms.date: 09/10/2017
title: 音频
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 944ad03a3ab70be5131e64f7d96c2a14ffea06ea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508127"
---
# <a name="audio-facet"></a><span data-ttu-id="8436c-103">Audio Facet</span><span class="sxs-lookup"><span data-stu-id="8436c-103">Audio facet</span></span>

<span data-ttu-id="8436c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8436c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8436c-105">**Audio** 资源将与音频相关的属性分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="8436c-105">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="8436c-p101">如果 [**DriveItem**](driveitem.md) 具有一个非 null **音频** facet，则该项表示一个音频文件。通过从文件中提取元数据来填充**音频**资源的属性。</span><span class="sxs-lookup"><span data-stu-id="8436c-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="8436c-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8436c-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.audio" } -->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 128,
  "composers": "string",
  "copyright": "string",
  "disc": 0,
  "discCount": 0,
  "duration": 567,
  "genre": "string",
  "hasDrm": false,
  "isVariableBitrate": false,
  "title": "string",
  "track": 1,
  "trackCount": 16,
  "year": 2014
}
```

## <a name="properties"></a><span data-ttu-id="8436c-109">属性</span><span class="sxs-lookup"><span data-stu-id="8436c-109">Properties</span></span>

| <span data-ttu-id="8436c-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="8436c-110">Property name</span></span>         | <span data-ttu-id="8436c-111">类型</span><span class="sxs-lookup"><span data-stu-id="8436c-111">Type</span></span>    | <span data-ttu-id="8436c-112">说明</span><span class="sxs-lookup"><span data-stu-id="8436c-112">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="8436c-113">**album**</span><span class="sxs-lookup"><span data-stu-id="8436c-113">**album**</span></span>             | <span data-ttu-id="8436c-114">string</span><span class="sxs-lookup"><span data-stu-id="8436c-114">string</span></span>  | <span data-ttu-id="8436c-115">此音频文件的专辑标题。</span><span class="sxs-lookup"><span data-stu-id="8436c-115">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="8436c-116">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="8436c-116">**albumArtist**</span></span>       | <span data-ttu-id="8436c-117">string</span><span class="sxs-lookup"><span data-stu-id="8436c-117">string</span></span>  | <span data-ttu-id="8436c-118">此音频文件的专辑上的艺术家。</span><span class="sxs-lookup"><span data-stu-id="8436c-118">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="8436c-119">**artist**</span><span class="sxs-lookup"><span data-stu-id="8436c-119">**artist**</span></span>            | <span data-ttu-id="8436c-120">string</span><span class="sxs-lookup"><span data-stu-id="8436c-120">string</span></span>  | <span data-ttu-id="8436c-121">此音频文件的表演艺术家。</span><span class="sxs-lookup"><span data-stu-id="8436c-121">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="8436c-122">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="8436c-122">**bitrate**</span></span>           | <span data-ttu-id="8436c-123">Int32</span><span class="sxs-lookup"><span data-stu-id="8436c-123">Int32</span></span>   | <span data-ttu-id="8436c-124">比特率（以 kbps 为单位）。</span><span class="sxs-lookup"><span data-stu-id="8436c-124">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="8436c-125">**composers**</span><span class="sxs-lookup"><span data-stu-id="8436c-125">**composers**</span></span>         | <span data-ttu-id="8436c-126">string</span><span class="sxs-lookup"><span data-stu-id="8436c-126">string</span></span>  | <span data-ttu-id="8436c-127">此音频文件的作曲者姓名。</span><span class="sxs-lookup"><span data-stu-id="8436c-127">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="8436c-128">**copyright**</span><span class="sxs-lookup"><span data-stu-id="8436c-128">**copyright**</span></span>         | <span data-ttu-id="8436c-129">string</span><span class="sxs-lookup"><span data-stu-id="8436c-129">string</span></span>  | <span data-ttu-id="8436c-130">此音频文件的版权信息。</span><span class="sxs-lookup"><span data-stu-id="8436c-130">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="8436c-131">**disc**</span><span class="sxs-lookup"><span data-stu-id="8436c-131">**disc**</span></span>              | <span data-ttu-id="8436c-132">Int32</span><span class="sxs-lookup"><span data-stu-id="8436c-132">Int32</span></span>   | <span data-ttu-id="8436c-133">此音频文件源自的光盘编号。</span><span class="sxs-lookup"><span data-stu-id="8436c-133">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="8436c-134">**discCount**</span><span class="sxs-lookup"><span data-stu-id="8436c-134">**discCount**</span></span>         | <span data-ttu-id="8436c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="8436c-135">Int32</span></span>   | <span data-ttu-id="8436c-136">此专辑中的光盘总数。</span><span class="sxs-lookup"><span data-stu-id="8436c-136">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="8436c-137">**duration**</span><span class="sxs-lookup"><span data-stu-id="8436c-137">**duration**</span></span>          | <span data-ttu-id="8436c-138">Int64</span><span class="sxs-lookup"><span data-stu-id="8436c-138">Int64</span></span>   | <span data-ttu-id="8436c-139">此音频文件的持续时间（以毫秒为单位）</span><span class="sxs-lookup"><span data-stu-id="8436c-139">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="8436c-140">**genre**</span><span class="sxs-lookup"><span data-stu-id="8436c-140">**genre**</span></span>             | <span data-ttu-id="8436c-141">string</span><span class="sxs-lookup"><span data-stu-id="8436c-141">string</span></span>  | <span data-ttu-id="8436c-142">此音频文件的流派。</span><span class="sxs-lookup"><span data-stu-id="8436c-142">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="8436c-143">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="8436c-143">**hasDrm**</span></span>            | <span data-ttu-id="8436c-144">boolean</span><span class="sxs-lookup"><span data-stu-id="8436c-144">boolean</span></span> | <span data-ttu-id="8436c-145">指明此文件是否受数字版权管理的保护。</span><span class="sxs-lookup"><span data-stu-id="8436c-145">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="8436c-146">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="8436c-146">**isVariableBitrate**</span></span> | <span data-ttu-id="8436c-147">boolean</span><span class="sxs-lookup"><span data-stu-id="8436c-147">boolean</span></span> | <span data-ttu-id="8436c-148">指明此文件是否已经过可变比特率编码。</span><span class="sxs-lookup"><span data-stu-id="8436c-148">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="8436c-149">**title**</span><span class="sxs-lookup"><span data-stu-id="8436c-149">**title**</span></span>             | <span data-ttu-id="8436c-150">string</span><span class="sxs-lookup"><span data-stu-id="8436c-150">string</span></span>  | <span data-ttu-id="8436c-151">此音频文件的标题。</span><span class="sxs-lookup"><span data-stu-id="8436c-151">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="8436c-152">**track**</span><span class="sxs-lookup"><span data-stu-id="8436c-152">**track**</span></span>             | <span data-ttu-id="8436c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8436c-153">Int32</span></span>   | <span data-ttu-id="8436c-154">此音频文件在原始光盘上的曲目编号。</span><span class="sxs-lookup"><span data-stu-id="8436c-154">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="8436c-155">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="8436c-155">**trackCount**</span></span>        | <span data-ttu-id="8436c-156">Int32</span><span class="sxs-lookup"><span data-stu-id="8436c-156">Int32</span></span>   | <span data-ttu-id="8436c-157">此音频文件的原始光盘上的曲目总数。</span><span class="sxs-lookup"><span data-stu-id="8436c-157">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="8436c-158">**year**</span><span class="sxs-lookup"><span data-stu-id="8436c-158">**year**</span></span>              | <span data-ttu-id="8436c-159">Int32</span><span class="sxs-lookup"><span data-stu-id="8436c-159">Int32</span></span>   | <span data-ttu-id="8436c-160">此音频文件的录制年份。</span><span class="sxs-lookup"><span data-stu-id="8436c-160">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="8436c-161">注解</span><span class="sxs-lookup"><span data-stu-id="8436c-161">Remarks</span></span>

<span data-ttu-id="8436c-162">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="8436c-162">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio",
  "suppressions": []
}
-->
