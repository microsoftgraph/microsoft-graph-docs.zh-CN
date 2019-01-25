---
title: audioSourceLevel 资源类型
description: 对于其他源的级别配置。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528373"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="7956e-103">audioSourceLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="7956e-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7956e-104">对于其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="7956e-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="7956e-105">属性</span><span class="sxs-lookup"><span data-stu-id="7956e-105">Properties</span></span>

| <span data-ttu-id="7956e-106">属性</span><span class="sxs-lookup"><span data-stu-id="7956e-106">Property</span></span>               | <span data-ttu-id="7956e-107">类型</span><span class="sxs-lookup"><span data-stu-id="7956e-107">Type</span></span>    | <span data-ttu-id="7956e-108">说明</span><span class="sxs-lookup"><span data-stu-id="7956e-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7956e-109">duckOthers</span><span class="sxs-lookup"><span data-stu-id="7956e-109">duckOthers</span></span>             | <span data-ttu-id="7956e-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="7956e-110">Boolean</span></span> | <span data-ttu-id="7956e-111">允许此源回避活动时的其他源。</span><span class="sxs-lookup"><span data-stu-id="7956e-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="7956e-112">如果设置为 true，放掉级别设置。</span><span class="sxs-lookup"><span data-stu-id="7956e-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="7956e-113">level</span><span class="sxs-lookup"><span data-stu-id="7956e-113">level</span></span>                  | <span data-ttu-id="7956e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7956e-114">Int64</span></span>   | <span data-ttu-id="7956e-115">如果放掉源的级别`duckOthers`设置为`true`。</span><span class="sxs-lookup"><span data-stu-id="7956e-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="7956e-116">参与者</span><span class="sxs-lookup"><span data-stu-id="7956e-116">participant</span></span>            | <span data-ttu-id="7956e-117">String</span><span class="sxs-lookup"><span data-stu-id="7956e-117">String</span></span>  | <span data-ttu-id="7956e-118">源参与者音频流。</span><span class="sxs-lookup"><span data-stu-id="7956e-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="7956e-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7956e-119">JSON representation</span></span>

<span data-ttu-id="7956e-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7956e-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audiosourcelevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
