---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Audio
localization_priority: Normal
ms.openlocfilehash: ead665ee4977a563ebb6b24636b627d72a2428dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871587"
---
# <a name="audio-facet"></a><span data-ttu-id="967ea-102">Audio Facet</span><span class="sxs-lookup"><span data-stu-id="967ea-102">Audio facet</span></span>

> <span data-ttu-id="967ea-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="967ea-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="967ea-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="967ea-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="967ea-105">**Audio** 资源将与音频相关的属性分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="967ea-105">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="967ea-p102">如果 [**DriveItem**](driveitem.md) 具有一个非 null **音频** facet，则该项表示一个音频文件。通过从文件中提取元数据来填充**音频**资源的属性。</span><span class="sxs-lookup"><span data-stu-id="967ea-p102">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="967ea-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="967ea-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="967ea-109">属性</span><span class="sxs-lookup"><span data-stu-id="967ea-109">Properties</span></span>

| <span data-ttu-id="967ea-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="967ea-110">Property name</span></span>         | <span data-ttu-id="967ea-111">类型</span><span class="sxs-lookup"><span data-stu-id="967ea-111">Type</span></span>    | <span data-ttu-id="967ea-112">说明</span><span class="sxs-lookup"><span data-stu-id="967ea-112">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="967ea-113">**album**</span><span class="sxs-lookup"><span data-stu-id="967ea-113">**album**</span></span>             | <span data-ttu-id="967ea-114">string</span><span class="sxs-lookup"><span data-stu-id="967ea-114">string</span></span>  | <span data-ttu-id="967ea-115">此音频文件的专辑标题。</span><span class="sxs-lookup"><span data-stu-id="967ea-115">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="967ea-116">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="967ea-116">**albumArtist**</span></span>       | <span data-ttu-id="967ea-117">string</span><span class="sxs-lookup"><span data-stu-id="967ea-117">string</span></span>  | <span data-ttu-id="967ea-118">此音频文件的专辑上的艺术家。</span><span class="sxs-lookup"><span data-stu-id="967ea-118">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="967ea-119">**artist**</span><span class="sxs-lookup"><span data-stu-id="967ea-119">**artist**</span></span>            | <span data-ttu-id="967ea-120">string</span><span class="sxs-lookup"><span data-stu-id="967ea-120">string</span></span>  | <span data-ttu-id="967ea-121">此音频文件的表演艺术家。</span><span class="sxs-lookup"><span data-stu-id="967ea-121">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="967ea-122">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="967ea-122">**bitrate**</span></span>           | <span data-ttu-id="967ea-123">Int32</span><span class="sxs-lookup"><span data-stu-id="967ea-123">Int32</span></span>   | <span data-ttu-id="967ea-124">比特率（以 kbps 为单位）。</span><span class="sxs-lookup"><span data-stu-id="967ea-124">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="967ea-125">**composers**</span><span class="sxs-lookup"><span data-stu-id="967ea-125">**composers**</span></span>         | <span data-ttu-id="967ea-126">string</span><span class="sxs-lookup"><span data-stu-id="967ea-126">string</span></span>  | <span data-ttu-id="967ea-127">此音频文件的作曲者姓名。</span><span class="sxs-lookup"><span data-stu-id="967ea-127">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="967ea-128">**copyright**</span><span class="sxs-lookup"><span data-stu-id="967ea-128">**copyright**</span></span>         | <span data-ttu-id="967ea-129">string</span><span class="sxs-lookup"><span data-stu-id="967ea-129">string</span></span>  | <span data-ttu-id="967ea-130">此音频文件的版权信息。</span><span class="sxs-lookup"><span data-stu-id="967ea-130">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="967ea-131">**disc**</span><span class="sxs-lookup"><span data-stu-id="967ea-131">**disc**</span></span>              | <span data-ttu-id="967ea-132">Int32</span><span class="sxs-lookup"><span data-stu-id="967ea-132">Int32</span></span>   | <span data-ttu-id="967ea-133">此音频文件源自的光盘编号。</span><span class="sxs-lookup"><span data-stu-id="967ea-133">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="967ea-134">**discCount**</span><span class="sxs-lookup"><span data-stu-id="967ea-134">**discCount**</span></span>         | <span data-ttu-id="967ea-135">Int32</span><span class="sxs-lookup"><span data-stu-id="967ea-135">Int32</span></span>   | <span data-ttu-id="967ea-136">此专辑中的光盘总数。</span><span class="sxs-lookup"><span data-stu-id="967ea-136">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="967ea-137">**duration**</span><span class="sxs-lookup"><span data-stu-id="967ea-137">**duration**</span></span>          | <span data-ttu-id="967ea-138">Int64</span><span class="sxs-lookup"><span data-stu-id="967ea-138">Int64</span></span>   | <span data-ttu-id="967ea-139">此音频文件的持续时间（以毫秒为单位）</span><span class="sxs-lookup"><span data-stu-id="967ea-139">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="967ea-140">**genre**</span><span class="sxs-lookup"><span data-stu-id="967ea-140">**genre**</span></span>             | <span data-ttu-id="967ea-141">string</span><span class="sxs-lookup"><span data-stu-id="967ea-141">string</span></span>  | <span data-ttu-id="967ea-142">此音频文件的流派。</span><span class="sxs-lookup"><span data-stu-id="967ea-142">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="967ea-143">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="967ea-143">**hasDrm**</span></span>            | <span data-ttu-id="967ea-144">boolean</span><span class="sxs-lookup"><span data-stu-id="967ea-144">boolean</span></span> | <span data-ttu-id="967ea-145">指明此文件是否受数字版权管理的保护。</span><span class="sxs-lookup"><span data-stu-id="967ea-145">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="967ea-146">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="967ea-146">**isVariableBitrate**</span></span> | <span data-ttu-id="967ea-147">boolean</span><span class="sxs-lookup"><span data-stu-id="967ea-147">boolean</span></span> | <span data-ttu-id="967ea-148">指明此文件是否已经过可变比特率编码。</span><span class="sxs-lookup"><span data-stu-id="967ea-148">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="967ea-149">**title**</span><span class="sxs-lookup"><span data-stu-id="967ea-149">**title**</span></span>             | <span data-ttu-id="967ea-150">string</span><span class="sxs-lookup"><span data-stu-id="967ea-150">string</span></span>  | <span data-ttu-id="967ea-151">此音频文件的标题。</span><span class="sxs-lookup"><span data-stu-id="967ea-151">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="967ea-152">**track**</span><span class="sxs-lookup"><span data-stu-id="967ea-152">**track**</span></span>             | <span data-ttu-id="967ea-153">Int32</span><span class="sxs-lookup"><span data-stu-id="967ea-153">Int32</span></span>   | <span data-ttu-id="967ea-154">此音频文件在原始光盘上的曲目编号。</span><span class="sxs-lookup"><span data-stu-id="967ea-154">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="967ea-155">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="967ea-155">**trackCount**</span></span>        | <span data-ttu-id="967ea-156">Int32</span><span class="sxs-lookup"><span data-stu-id="967ea-156">Int32</span></span>   | <span data-ttu-id="967ea-157">此音频文件的原始光盘上的曲目总数。</span><span class="sxs-lookup"><span data-stu-id="967ea-157">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="967ea-158">**year**</span><span class="sxs-lookup"><span data-stu-id="967ea-158">**year**</span></span>              | <span data-ttu-id="967ea-159">Int32</span><span class="sxs-lookup"><span data-stu-id="967ea-159">Int32</span></span>   | <span data-ttu-id="967ea-160">此音频文件的录制年份。</span><span class="sxs-lookup"><span data-stu-id="967ea-160">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="967ea-161">注解</span><span class="sxs-lookup"><span data-stu-id="967ea-161">Remarks</span></span>

<span data-ttu-id="967ea-162">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="967ea-162">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
