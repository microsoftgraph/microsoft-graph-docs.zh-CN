---
author: ananmishr
description: Audio 资源将与音频相关的属性分组到一个单一结构。
ms.date: 09/10/2017
title: 音频
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 146d9730c0a1c4e73ac16815abddd37eb729545b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034201"
---
# <a name="audio-facet"></a><span data-ttu-id="b41be-103">Audio Facet</span><span class="sxs-lookup"><span data-stu-id="b41be-103">Audio facet</span></span>

<span data-ttu-id="b41be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b41be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b41be-105">**Audio** 资源将与音频相关的属性分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="b41be-105">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="b41be-p101">如果 [**DriveItem**](driveitem.md) 具有一个非 null **音频** facet，则该项表示一个音频文件。通过从文件中提取元数据来填充**音频**资源的属性。</span><span class="sxs-lookup"><span data-stu-id="b41be-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="b41be-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b41be-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b41be-109">属性</span><span class="sxs-lookup"><span data-stu-id="b41be-109">Properties</span></span>

| <span data-ttu-id="b41be-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="b41be-110">Property name</span></span>         | <span data-ttu-id="b41be-111">类型</span><span class="sxs-lookup"><span data-stu-id="b41be-111">Type</span></span>    | <span data-ttu-id="b41be-112">说明</span><span class="sxs-lookup"><span data-stu-id="b41be-112">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="b41be-113">**album**</span><span class="sxs-lookup"><span data-stu-id="b41be-113">**album**</span></span>             | <span data-ttu-id="b41be-114">string</span><span class="sxs-lookup"><span data-stu-id="b41be-114">string</span></span>  | <span data-ttu-id="b41be-115">此音频文件的专辑标题。</span><span class="sxs-lookup"><span data-stu-id="b41be-115">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="b41be-116">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="b41be-116">**albumArtist**</span></span>       | <span data-ttu-id="b41be-117">string</span><span class="sxs-lookup"><span data-stu-id="b41be-117">string</span></span>  | <span data-ttu-id="b41be-118">此音频文件的专辑上的艺术家。</span><span class="sxs-lookup"><span data-stu-id="b41be-118">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="b41be-119">**artist**</span><span class="sxs-lookup"><span data-stu-id="b41be-119">**artist**</span></span>            | <span data-ttu-id="b41be-120">string</span><span class="sxs-lookup"><span data-stu-id="b41be-120">string</span></span>  | <span data-ttu-id="b41be-121">此音频文件的表演艺术家。</span><span class="sxs-lookup"><span data-stu-id="b41be-121">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="b41be-122">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="b41be-122">**bitrate**</span></span>           | <span data-ttu-id="b41be-123">Int32</span><span class="sxs-lookup"><span data-stu-id="b41be-123">Int32</span></span>   | <span data-ttu-id="b41be-124">比特率（以 kbps 为单位）。</span><span class="sxs-lookup"><span data-stu-id="b41be-124">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="b41be-125">**composers**</span><span class="sxs-lookup"><span data-stu-id="b41be-125">**composers**</span></span>         | <span data-ttu-id="b41be-126">string</span><span class="sxs-lookup"><span data-stu-id="b41be-126">string</span></span>  | <span data-ttu-id="b41be-127">此音频文件的作曲者姓名。</span><span class="sxs-lookup"><span data-stu-id="b41be-127">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="b41be-128">**copyright**</span><span class="sxs-lookup"><span data-stu-id="b41be-128">**copyright**</span></span>         | <span data-ttu-id="b41be-129">string</span><span class="sxs-lookup"><span data-stu-id="b41be-129">string</span></span>  | <span data-ttu-id="b41be-130">此音频文件的版权信息。</span><span class="sxs-lookup"><span data-stu-id="b41be-130">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="b41be-131">**disc**</span><span class="sxs-lookup"><span data-stu-id="b41be-131">**disc**</span></span>              | <span data-ttu-id="b41be-132">Int32</span><span class="sxs-lookup"><span data-stu-id="b41be-132">Int32</span></span>   | <span data-ttu-id="b41be-133">此音频文件源自的光盘编号。</span><span class="sxs-lookup"><span data-stu-id="b41be-133">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="b41be-134">**discCount**</span><span class="sxs-lookup"><span data-stu-id="b41be-134">**discCount**</span></span>         | <span data-ttu-id="b41be-135">Int32</span><span class="sxs-lookup"><span data-stu-id="b41be-135">Int32</span></span>   | <span data-ttu-id="b41be-136">此专辑中的光盘总数。</span><span class="sxs-lookup"><span data-stu-id="b41be-136">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="b41be-137">**duration**</span><span class="sxs-lookup"><span data-stu-id="b41be-137">**duration**</span></span>          | <span data-ttu-id="b41be-138">Int64</span><span class="sxs-lookup"><span data-stu-id="b41be-138">Int64</span></span>   | <span data-ttu-id="b41be-139">此音频文件的持续时间（以毫秒为单位）</span><span class="sxs-lookup"><span data-stu-id="b41be-139">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="b41be-140">**genre**</span><span class="sxs-lookup"><span data-stu-id="b41be-140">**genre**</span></span>             | <span data-ttu-id="b41be-141">string</span><span class="sxs-lookup"><span data-stu-id="b41be-141">string</span></span>  | <span data-ttu-id="b41be-142">此音频文件的流派。</span><span class="sxs-lookup"><span data-stu-id="b41be-142">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="b41be-143">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="b41be-143">**hasDrm**</span></span>            | <span data-ttu-id="b41be-144">boolean</span><span class="sxs-lookup"><span data-stu-id="b41be-144">boolean</span></span> | <span data-ttu-id="b41be-145">指明此文件是否受数字版权管理的保护。</span><span class="sxs-lookup"><span data-stu-id="b41be-145">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="b41be-146">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="b41be-146">**isVariableBitrate**</span></span> | <span data-ttu-id="b41be-147">boolean</span><span class="sxs-lookup"><span data-stu-id="b41be-147">boolean</span></span> | <span data-ttu-id="b41be-148">指明此文件是否已经过可变比特率编码。</span><span class="sxs-lookup"><span data-stu-id="b41be-148">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="b41be-149">**title**</span><span class="sxs-lookup"><span data-stu-id="b41be-149">**title**</span></span>             | <span data-ttu-id="b41be-150">string</span><span class="sxs-lookup"><span data-stu-id="b41be-150">string</span></span>  | <span data-ttu-id="b41be-151">此音频文件的标题。</span><span class="sxs-lookup"><span data-stu-id="b41be-151">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="b41be-152">**track**</span><span class="sxs-lookup"><span data-stu-id="b41be-152">**track**</span></span>             | <span data-ttu-id="b41be-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b41be-153">Int32</span></span>   | <span data-ttu-id="b41be-154">此音频文件在原始光盘上的曲目编号。</span><span class="sxs-lookup"><span data-stu-id="b41be-154">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="b41be-155">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="b41be-155">**trackCount**</span></span>        | <span data-ttu-id="b41be-156">Int32</span><span class="sxs-lookup"><span data-stu-id="b41be-156">Int32</span></span>   | <span data-ttu-id="b41be-157">此音频文件的原始光盘上的曲目总数。</span><span class="sxs-lookup"><span data-stu-id="b41be-157">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="b41be-158">**year**</span><span class="sxs-lookup"><span data-stu-id="b41be-158">**year**</span></span>              | <span data-ttu-id="b41be-159">Int32</span><span class="sxs-lookup"><span data-stu-id="b41be-159">Int32</span></span>   | <span data-ttu-id="b41be-160">此音频文件的录制年份。</span><span class="sxs-lookup"><span data-stu-id="b41be-160">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="b41be-161">注解</span><span class="sxs-lookup"><span data-stu-id="b41be-161">Remarks</span></span>

<span data-ttu-id="b41be-162">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b41be-162">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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


