---
title: audioSourceLevel 资源类型
description: 其他源的级别配置。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bc2b0c11b18a3cf8120cab0bb9c745ae8880cfc6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339025"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="ee56c-103">audioSourceLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee56c-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee56c-104">其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="ee56c-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="ee56c-105">属性</span><span class="sxs-lookup"><span data-stu-id="ee56c-105">Properties</span></span>

| <span data-ttu-id="ee56c-106">属性</span><span class="sxs-lookup"><span data-stu-id="ee56c-106">Property</span></span>               | <span data-ttu-id="ee56c-107">类型</span><span class="sxs-lookup"><span data-stu-id="ee56c-107">Type</span></span>    | <span data-ttu-id="ee56c-108">说明</span><span class="sxs-lookup"><span data-stu-id="ee56c-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ee56c-109">duckOthers</span><span class="sxs-lookup"><span data-stu-id="ee56c-109">duckOthers</span></span>             | <span data-ttu-id="ee56c-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee56c-110">Boolean</span></span> | <span data-ttu-id="ee56c-111">允许此源在活动时有其他源。</span><span class="sxs-lookup"><span data-stu-id="ee56c-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="ee56c-112">如果设置为 true, 则必须设置 ducking 级别。</span><span class="sxs-lookup"><span data-stu-id="ee56c-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="ee56c-113">块级</span><span class="sxs-lookup"><span data-stu-id="ee56c-113">level</span></span>                  | <span data-ttu-id="ee56c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ee56c-114">Int64</span></span>   | <span data-ttu-id="ee56c-115">源的 Ducking 级别 (如果`duckOthers`设置为`true`)。</span><span class="sxs-lookup"><span data-stu-id="ee56c-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="ee56c-116">参与者</span><span class="sxs-lookup"><span data-stu-id="ee56c-116">participant</span></span>            | <span data-ttu-id="ee56c-117">String</span><span class="sxs-lookup"><span data-stu-id="ee56c-117">String</span></span>  | <span data-ttu-id="ee56c-118">源参与者音频流。</span><span class="sxs-lookup"><span data-stu-id="ee56c-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="ee56c-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee56c-119">JSON representation</span></span>

<span data-ttu-id="ee56c-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee56c-120">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
