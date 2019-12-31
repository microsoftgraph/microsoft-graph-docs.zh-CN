---
author: ananmishr
ms.date: 09/10/2017
title: 音频
localization_priority: Normal
ms.prod: microsoft-teams
description: Audio 资源将与音频相关的属性分组到一个单一结构。
doc_type: resourcePageType
ms.openlocfilehash: 1351ae9dcd363d156997fd5cc75e7e3387a0fb38
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913483"
---
# <a name="audio-facet"></a><span data-ttu-id="062a1-103">Audio Facet</span><span class="sxs-lookup"><span data-stu-id="062a1-103">Audio facet</span></span>

<span data-ttu-id="062a1-104">**Audio** 资源将与音频相关的属性分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="062a1-104">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="062a1-p101">如果 [**DriveItem**](driveitem.md) 具有一个非 null **音频** facet，则该项表示一个音频文件。通过从文件中提取元数据来填充**音频**资源的属性。</span><span class="sxs-lookup"><span data-stu-id="062a1-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="062a1-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="062a1-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="062a1-108">属性</span><span class="sxs-lookup"><span data-stu-id="062a1-108">Properties</span></span>

| <span data-ttu-id="062a1-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="062a1-109">Property name</span></span>         | <span data-ttu-id="062a1-110">类型</span><span class="sxs-lookup"><span data-stu-id="062a1-110">Type</span></span>    | <span data-ttu-id="062a1-111">说明</span><span class="sxs-lookup"><span data-stu-id="062a1-111">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="062a1-112">**album**</span><span class="sxs-lookup"><span data-stu-id="062a1-112">**album**</span></span>             | <span data-ttu-id="062a1-113">string</span><span class="sxs-lookup"><span data-stu-id="062a1-113">string</span></span>  | <span data-ttu-id="062a1-114">此音频文件的专辑标题。</span><span class="sxs-lookup"><span data-stu-id="062a1-114">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="062a1-115">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="062a1-115">**albumArtist**</span></span>       | <span data-ttu-id="062a1-116">string</span><span class="sxs-lookup"><span data-stu-id="062a1-116">string</span></span>  | <span data-ttu-id="062a1-117">此音频文件的专辑上的艺术家。</span><span class="sxs-lookup"><span data-stu-id="062a1-117">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="062a1-118">**artist**</span><span class="sxs-lookup"><span data-stu-id="062a1-118">**artist**</span></span>            | <span data-ttu-id="062a1-119">string</span><span class="sxs-lookup"><span data-stu-id="062a1-119">string</span></span>  | <span data-ttu-id="062a1-120">此音频文件的表演艺术家。</span><span class="sxs-lookup"><span data-stu-id="062a1-120">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="062a1-121">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="062a1-121">**bitrate**</span></span>           | <span data-ttu-id="062a1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="062a1-122">Int64</span></span>   | <span data-ttu-id="062a1-123">比特率（以 kbps 为单位）。</span><span class="sxs-lookup"><span data-stu-id="062a1-123">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="062a1-124">**composers**</span><span class="sxs-lookup"><span data-stu-id="062a1-124">**composers**</span></span>         | <span data-ttu-id="062a1-125">string</span><span class="sxs-lookup"><span data-stu-id="062a1-125">string</span></span>  | <span data-ttu-id="062a1-126">此音频文件的作曲者姓名。</span><span class="sxs-lookup"><span data-stu-id="062a1-126">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="062a1-127">**copyright**</span><span class="sxs-lookup"><span data-stu-id="062a1-127">**copyright**</span></span>         | <span data-ttu-id="062a1-128">string</span><span class="sxs-lookup"><span data-stu-id="062a1-128">string</span></span>  | <span data-ttu-id="062a1-129">此音频文件的版权信息。</span><span class="sxs-lookup"><span data-stu-id="062a1-129">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="062a1-130">**disc**</span><span class="sxs-lookup"><span data-stu-id="062a1-130">**disc**</span></span>              | <span data-ttu-id="062a1-131">Int16</span><span class="sxs-lookup"><span data-stu-id="062a1-131">Int16</span></span>   | <span data-ttu-id="062a1-132">此音频文件源自的光盘编号。</span><span class="sxs-lookup"><span data-stu-id="062a1-132">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="062a1-133">**discCount**</span><span class="sxs-lookup"><span data-stu-id="062a1-133">**discCount**</span></span>         | <span data-ttu-id="062a1-134">Int16</span><span class="sxs-lookup"><span data-stu-id="062a1-134">Int16</span></span>   | <span data-ttu-id="062a1-135">此专辑中的光盘总数。</span><span class="sxs-lookup"><span data-stu-id="062a1-135">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="062a1-136">**duration**</span><span class="sxs-lookup"><span data-stu-id="062a1-136">**duration**</span></span>          | <span data-ttu-id="062a1-137">Int64</span><span class="sxs-lookup"><span data-stu-id="062a1-137">Int64</span></span>   | <span data-ttu-id="062a1-138">此音频文件的持续时间（以毫秒为单位）</span><span class="sxs-lookup"><span data-stu-id="062a1-138">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="062a1-139">**genre**</span><span class="sxs-lookup"><span data-stu-id="062a1-139">**genre**</span></span>             | <span data-ttu-id="062a1-140">string</span><span class="sxs-lookup"><span data-stu-id="062a1-140">string</span></span>  | <span data-ttu-id="062a1-141">此音频文件的流派。</span><span class="sxs-lookup"><span data-stu-id="062a1-141">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="062a1-142">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="062a1-142">**hasDrm**</span></span>            | <span data-ttu-id="062a1-143">boolean</span><span class="sxs-lookup"><span data-stu-id="062a1-143">boolean</span></span> | <span data-ttu-id="062a1-144">指明此文件是否受数字版权管理的保护。</span><span class="sxs-lookup"><span data-stu-id="062a1-144">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="062a1-145">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="062a1-145">**isVariableBitrate**</span></span> | <span data-ttu-id="062a1-146">boolean</span><span class="sxs-lookup"><span data-stu-id="062a1-146">boolean</span></span> | <span data-ttu-id="062a1-147">指明此文件是否已经过可变比特率编码。</span><span class="sxs-lookup"><span data-stu-id="062a1-147">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="062a1-148">**title**</span><span class="sxs-lookup"><span data-stu-id="062a1-148">**title**</span></span>             | <span data-ttu-id="062a1-149">string</span><span class="sxs-lookup"><span data-stu-id="062a1-149">string</span></span>  | <span data-ttu-id="062a1-150">此音频文件的标题。</span><span class="sxs-lookup"><span data-stu-id="062a1-150">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="062a1-151">**track**</span><span class="sxs-lookup"><span data-stu-id="062a1-151">**track**</span></span>             | <span data-ttu-id="062a1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="062a1-152">Int32</span></span>   | <span data-ttu-id="062a1-153">此音频文件在原始光盘上的曲目编号。</span><span class="sxs-lookup"><span data-stu-id="062a1-153">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="062a1-154">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="062a1-154">**trackCount**</span></span>        | <span data-ttu-id="062a1-155">Int32</span><span class="sxs-lookup"><span data-stu-id="062a1-155">Int32</span></span>   | <span data-ttu-id="062a1-156">此音频文件的原始光盘上的曲目总数。</span><span class="sxs-lookup"><span data-stu-id="062a1-156">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="062a1-157">**year**</span><span class="sxs-lookup"><span data-stu-id="062a1-157">**year**</span></span>              | <span data-ttu-id="062a1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="062a1-158">Int32</span></span>   | <span data-ttu-id="062a1-159">此音频文件的录制年份。</span><span class="sxs-lookup"><span data-stu-id="062a1-159">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="062a1-160">注解</span><span class="sxs-lookup"><span data-stu-id="062a1-160">Remarks</span></span>

<span data-ttu-id="062a1-161">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="062a1-161">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
