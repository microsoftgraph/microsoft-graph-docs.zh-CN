---
title: audioSourceLevel 资源类型
description: 对于其他源的级别配置。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 79ad56c11e8b277a1354ffc3a6292a0434466c8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947650"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="70259-103">audioSourceLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="70259-103">audioSourceLevel resource type</span></span>

> <span data-ttu-id="70259-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="70259-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70259-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="70259-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70259-106">对于其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="70259-106">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="70259-107">属性</span><span class="sxs-lookup"><span data-stu-id="70259-107">Properties</span></span>

| <span data-ttu-id="70259-108">属性</span><span class="sxs-lookup"><span data-stu-id="70259-108">Property</span></span>               | <span data-ttu-id="70259-109">类型</span><span class="sxs-lookup"><span data-stu-id="70259-109">Type</span></span>    | <span data-ttu-id="70259-110">Description</span><span class="sxs-lookup"><span data-stu-id="70259-110">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="70259-111">duckOthers</span><span class="sxs-lookup"><span data-stu-id="70259-111">duckOthers</span></span>             | <span data-ttu-id="70259-112">布尔</span><span class="sxs-lookup"><span data-stu-id="70259-112">Boolean</span></span> | <span data-ttu-id="70259-113">允许此源回避活动时的其他源。</span><span class="sxs-lookup"><span data-stu-id="70259-113">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="70259-114">如果设置为 true，放掉级别设置。</span><span class="sxs-lookup"><span data-stu-id="70259-114">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="70259-115">level</span><span class="sxs-lookup"><span data-stu-id="70259-115">level</span></span>                  | <span data-ttu-id="70259-116">Int64</span><span class="sxs-lookup"><span data-stu-id="70259-116">Int64</span></span>   | <span data-ttu-id="70259-117">如果放掉源的级别`duckOthers`设置为`true`。</span><span class="sxs-lookup"><span data-stu-id="70259-117">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="70259-118">参与者</span><span class="sxs-lookup"><span data-stu-id="70259-118">participant</span></span>            | <span data-ttu-id="70259-119">字符串</span><span class="sxs-lookup"><span data-stu-id="70259-119">String</span></span>  | <span data-ttu-id="70259-120">源参与者音频流。</span><span class="sxs-lookup"><span data-stu-id="70259-120">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="70259-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70259-121">JSON representation</span></span>

<span data-ttu-id="70259-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70259-122">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
