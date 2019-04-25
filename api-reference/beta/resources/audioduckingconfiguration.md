---
title: audioDuckingConfiguration 资源类型
description: 其他源的 ducking 参数 (逐步淘汰 in 和其他来源。)
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d61e4150250df25e020f45a65676d1c55c0e4c9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544098"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="20b97-103">audioDuckingConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="20b97-103">audioDuckingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20b97-104">其他源的 ducking 参数 (逐步淘汰 in 和其他来源。)</span><span class="sxs-lookup"><span data-stu-id="20b97-104">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="20b97-105">属性</span><span class="sxs-lookup"><span data-stu-id="20b97-105">Properties</span></span>

| <span data-ttu-id="20b97-106">属性</span><span class="sxs-lookup"><span data-stu-id="20b97-106">Property</span></span>      | <span data-ttu-id="20b97-107">类型</span><span class="sxs-lookup"><span data-stu-id="20b97-107">Type</span></span>     | <span data-ttu-id="20b97-108">说明</span><span class="sxs-lookup"><span data-stu-id="20b97-108">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="20b97-109">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="20b97-109">lowerLevel</span></span>    | <span data-ttu-id="20b97-110">Int64</span><span class="sxs-lookup"><span data-stu-id="20b97-110">Int64</span></span>    | <span data-ttu-id="20b97-111">源正在 ducked 时, 源的数量 (以百分比为单位)。</span><span class="sxs-lookup"><span data-stu-id="20b97-111">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="20b97-112">rampActive</span><span class="sxs-lookup"><span data-stu-id="20b97-112">rampActive</span></span>    | <span data-ttu-id="20b97-113">Int64</span><span class="sxs-lookup"><span data-stu-id="20b97-113">Int64</span></span>    | <span data-ttu-id="20b97-114">ducked 源到 "淡出" 所需的时间量 (以毫秒为单位)。</span><span class="sxs-lookup"><span data-stu-id="20b97-114">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="20b97-115">rampInactive</span><span class="sxs-lookup"><span data-stu-id="20b97-115">rampInactive</span></span>  | <span data-ttu-id="20b97-116">Int64</span><span class="sxs-lookup"><span data-stu-id="20b97-116">Int64</span></span>    | <span data-ttu-id="20b97-117">ducked 源到 "淡入" 所需的时间 (以毫秒为单位)。</span><span class="sxs-lookup"><span data-stu-id="20b97-117">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="20b97-118">upperLevel</span><span class="sxs-lookup"><span data-stu-id="20b97-118">upperLevel</span></span>    | <span data-ttu-id="20b97-119">Int64</span><span class="sxs-lookup"><span data-stu-id="20b97-119">Int64</span></span>    | <span data-ttu-id="20b97-120">源未 ducked 时的源数量 (以百分比为单位)。</span><span class="sxs-lookup"><span data-stu-id="20b97-120">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="20b97-121">**注意:** 斜向持续时间不能超过5000毫秒。</span><span class="sxs-lookup"><span data-stu-id="20b97-121">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="20b97-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20b97-122">JSON representation</span></span>

<span data-ttu-id="20b97-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20b97-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioduckingconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
