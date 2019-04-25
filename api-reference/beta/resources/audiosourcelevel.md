---
title: audioSourceLevel 资源类型
description: 其他源的级别配置。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535576"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="4fa33-103">audioSourceLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="4fa33-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fa33-104">其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="4fa33-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="4fa33-105">属性</span><span class="sxs-lookup"><span data-stu-id="4fa33-105">Properties</span></span>

| <span data-ttu-id="4fa33-106">属性</span><span class="sxs-lookup"><span data-stu-id="4fa33-106">Property</span></span>               | <span data-ttu-id="4fa33-107">类型</span><span class="sxs-lookup"><span data-stu-id="4fa33-107">Type</span></span>    | <span data-ttu-id="4fa33-108">说明</span><span class="sxs-lookup"><span data-stu-id="4fa33-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4fa33-109">duckOthers</span><span class="sxs-lookup"><span data-stu-id="4fa33-109">duckOthers</span></span>             | <span data-ttu-id="4fa33-110">布尔值</span><span class="sxs-lookup"><span data-stu-id="4fa33-110">Boolean</span></span> | <span data-ttu-id="4fa33-111">允许此源在活动时有其他源。</span><span class="sxs-lookup"><span data-stu-id="4fa33-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="4fa33-112">如果设置为 true, 则必须设置 ducking 级别。</span><span class="sxs-lookup"><span data-stu-id="4fa33-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="4fa33-113">块级</span><span class="sxs-lookup"><span data-stu-id="4fa33-113">level</span></span>                  | <span data-ttu-id="4fa33-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4fa33-114">Int64</span></span>   | <span data-ttu-id="4fa33-115">源的 Ducking 级别 (如果`duckOthers`设置为`true`)。</span><span class="sxs-lookup"><span data-stu-id="4fa33-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="4fa33-116">参与者</span><span class="sxs-lookup"><span data-stu-id="4fa33-116">participant</span></span>            | <span data-ttu-id="4fa33-117">String</span><span class="sxs-lookup"><span data-stu-id="4fa33-117">String</span></span>  | <span data-ttu-id="4fa33-118">源参与者音频流。</span><span class="sxs-lookup"><span data-stu-id="4fa33-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="4fa33-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4fa33-119">JSON representation</span></span>

<span data-ttu-id="4fa33-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4fa33-120">The following is a JSON representation of the resource.</span></span>

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
