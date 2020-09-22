---
title: audioSourceLevel 资源类型
description: 其他源的级别配置。
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: eb98e434540dd00529963c48ff3f3296e17e0c01
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998948"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="9ebbe-103">audioSourceLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ebbe-103">audioSourceLevel resource type</span></span>

<span data-ttu-id="9ebbe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ebbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ebbe-105">其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="9ebbe-105">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="9ebbe-106">属性</span><span class="sxs-lookup"><span data-stu-id="9ebbe-106">Properties</span></span>

| <span data-ttu-id="9ebbe-107">属性</span><span class="sxs-lookup"><span data-stu-id="9ebbe-107">Property</span></span>               | <span data-ttu-id="9ebbe-108">类型</span><span class="sxs-lookup"><span data-stu-id="9ebbe-108">Type</span></span>    | <span data-ttu-id="9ebbe-109">说明</span><span class="sxs-lookup"><span data-stu-id="9ebbe-109">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9ebbe-110">duckOthers</span><span class="sxs-lookup"><span data-stu-id="9ebbe-110">duckOthers</span></span>             | <span data-ttu-id="9ebbe-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ebbe-111">Boolean</span></span> | <span data-ttu-id="9ebbe-112">允许此源在活动时有其他源。</span><span class="sxs-lookup"><span data-stu-id="9ebbe-112">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="9ebbe-113">如果设置为 true，则必须设置 ducking 级别。</span><span class="sxs-lookup"><span data-stu-id="9ebbe-113">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="9ebbe-114">块级</span><span class="sxs-lookup"><span data-stu-id="9ebbe-114">level</span></span>                  | <span data-ttu-id="9ebbe-115">Int64</span><span class="sxs-lookup"><span data-stu-id="9ebbe-115">Int64</span></span>   | <span data-ttu-id="9ebbe-116">源的 Ducking 级别（如果 `duckOthers` 设置为） `true` 。</span><span class="sxs-lookup"><span data-stu-id="9ebbe-116">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="9ebbe-117">参与者</span><span class="sxs-lookup"><span data-stu-id="9ebbe-117">participant</span></span>            | <span data-ttu-id="9ebbe-118">String</span><span class="sxs-lookup"><span data-stu-id="9ebbe-118">String</span></span>  | <span data-ttu-id="9ebbe-119">源参与者音频流。</span><span class="sxs-lookup"><span data-stu-id="9ebbe-119">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="9ebbe-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ebbe-120">JSON representation</span></span>

<span data-ttu-id="9ebbe-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ebbe-121">The following is a JSON representation of the resource.</span></span>

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


