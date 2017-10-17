---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Audio
ms.openlocfilehash: 43b9999ecfb472a82e00a12ca820fdf8548eec64
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="audio-facet"></a><span data-ttu-id="f705d-102">Audio Facet</span><span class="sxs-lookup"><span data-stu-id="f705d-102">Audio facet</span></span>

<span data-ttu-id="f705d-103">**Audio** 资源将与音频相关的属性分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="f705d-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="f705d-104">如果 [**DriveItem**](driveitem.md) 具有一个非 null **audio** facet，则该项表示一个音频文件。</span><span class="sxs-lookup"><span data-stu-id="f705d-104">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the Audio resource are populated by extracting metadata from the file.</span></span>
<span data-ttu-id="f705d-105">通过从文件中提取元数据来填充 **Audio** 资源的属性。</span><span class="sxs-lookup"><span data-stu-id="f705d-105">If a DriveItem has a non-null audio facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="f705d-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f705d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f705d-107">属性</span><span class="sxs-lookup"><span data-stu-id="f705d-107">Properties</span></span>

| <span data-ttu-id="f705d-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="f705d-108">Property name</span></span>         | <span data-ttu-id="f705d-109">类型</span><span class="sxs-lookup"><span data-stu-id="f705d-109">Type</span></span>    | <span data-ttu-id="f705d-110">说明</span><span class="sxs-lookup"><span data-stu-id="f705d-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="f705d-111">**album**</span><span class="sxs-lookup"><span data-stu-id="f705d-111">**album**</span></span>             | <span data-ttu-id="f705d-112">string</span><span class="sxs-lookup"><span data-stu-id="f705d-112">string</span></span>  | <span data-ttu-id="f705d-113">此音频文件的专辑标题。</span><span class="sxs-lookup"><span data-stu-id="f705d-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="f705d-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="f705d-114">**albumArtist**</span></span>       | <span data-ttu-id="f705d-115">string</span><span class="sxs-lookup"><span data-stu-id="f705d-115">string</span></span>  | <span data-ttu-id="f705d-116">此音频文件的专辑上的艺术家。</span><span class="sxs-lookup"><span data-stu-id="f705d-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="f705d-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="f705d-117">**artist**</span></span>            | <span data-ttu-id="f705d-118">string</span><span class="sxs-lookup"><span data-stu-id="f705d-118">string</span></span>  | <span data-ttu-id="f705d-119">此音频文件的表演艺术家。</span><span class="sxs-lookup"><span data-stu-id="f705d-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="f705d-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="f705d-120">**bitrate**</span></span>           | <span data-ttu-id="f705d-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f705d-121">Int32</span></span>   | <span data-ttu-id="f705d-122">比特率（以 kbps 为单位）。</span><span class="sxs-lookup"><span data-stu-id="f705d-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="f705d-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="f705d-123">**composers**</span></span>         | <span data-ttu-id="f705d-124">string</span><span class="sxs-lookup"><span data-stu-id="f705d-124">string</span></span>  | <span data-ttu-id="f705d-125">此音频文件的作曲者姓名。</span><span class="sxs-lookup"><span data-stu-id="f705d-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="f705d-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="f705d-126">**copyright**</span></span>         | <span data-ttu-id="f705d-127">string</span><span class="sxs-lookup"><span data-stu-id="f705d-127">string</span></span>  | <span data-ttu-id="f705d-128">此音频文件的版权信息。</span><span class="sxs-lookup"><span data-stu-id="f705d-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="f705d-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="f705d-129">**disc**</span></span>              | <span data-ttu-id="f705d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="f705d-130">Int32</span></span>   | <span data-ttu-id="f705d-131">此音频文件源自的光盘编号。</span><span class="sxs-lookup"><span data-stu-id="f705d-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="f705d-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="f705d-132">**discCount**</span></span>         | <span data-ttu-id="f705d-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f705d-133">Int32</span></span>   | <span data-ttu-id="f705d-134">此专辑中的光盘总数。</span><span class="sxs-lookup"><span data-stu-id="f705d-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="f705d-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="f705d-135">**duration**</span></span>          | <span data-ttu-id="f705d-136">Int64</span><span class="sxs-lookup"><span data-stu-id="f705d-136">Int64</span></span>   | <span data-ttu-id="f705d-137">此音频文件的持续时间（以毫秒为单位）</span><span class="sxs-lookup"><span data-stu-id="f705d-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="f705d-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="f705d-138">**genre**</span></span>             | <span data-ttu-id="f705d-139">string</span><span class="sxs-lookup"><span data-stu-id="f705d-139">string</span></span>  | <span data-ttu-id="f705d-140">此音频文件的流派。</span><span class="sxs-lookup"><span data-stu-id="f705d-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="f705d-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="f705d-141">**hasDrm**</span></span>            | <span data-ttu-id="f705d-142">boolean</span><span class="sxs-lookup"><span data-stu-id="f705d-142">boolean</span></span> | <span data-ttu-id="f705d-143">指明此文件是否受数字版权管理的保护。</span><span class="sxs-lookup"><span data-stu-id="f705d-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="f705d-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="f705d-144">**isVariableBitrate**</span></span> | <span data-ttu-id="f705d-145">boolean</span><span class="sxs-lookup"><span data-stu-id="f705d-145">boolean</span></span> | <span data-ttu-id="f705d-146">指明此文件是否已经过可变比特率编码。</span><span class="sxs-lookup"><span data-stu-id="f705d-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="f705d-147">**title**</span><span class="sxs-lookup"><span data-stu-id="f705d-147">**title**</span></span>             | <span data-ttu-id="f705d-148">string</span><span class="sxs-lookup"><span data-stu-id="f705d-148">string</span></span>  | <span data-ttu-id="f705d-149">此音频文件的标题。</span><span class="sxs-lookup"><span data-stu-id="f705d-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="f705d-150">**track**</span><span class="sxs-lookup"><span data-stu-id="f705d-150">**track**</span></span>             | <span data-ttu-id="f705d-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f705d-151">Int32</span></span>   | <span data-ttu-id="f705d-152">此音频文件在原始光盘上的曲目编号。</span><span class="sxs-lookup"><span data-stu-id="f705d-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="f705d-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="f705d-153">**trackCount**</span></span>        | <span data-ttu-id="f705d-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f705d-154">Int32</span></span>   | <span data-ttu-id="f705d-155">此音频文件的原始光盘上的曲目总数。</span><span class="sxs-lookup"><span data-stu-id="f705d-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="f705d-156">**year**</span><span class="sxs-lookup"><span data-stu-id="f705d-156">**year**</span></span>              | <span data-ttu-id="f705d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f705d-157">Int32</span></span>   | <span data-ttu-id="f705d-158">此音频文件的录制年份。</span><span class="sxs-lookup"><span data-stu-id="f705d-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="f705d-159">注解</span><span class="sxs-lookup"><span data-stu-id="f705d-159">Remarks</span></span>

<span data-ttu-id="f705d-160">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="f705d-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
