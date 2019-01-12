---
title: plannerPlanContextDetails 资源类型
description: '**PlannerPlanContextDetails**资源包含有关 plannerPlanContext 的其他信息。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e0f26bcb25bf77a0a9907ba7e0414e57ad738cae
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968216"
---
# <a name="plannerplancontextdetails-resource-type"></a><span data-ttu-id="c5274-103">plannerPlanContextDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5274-103">plannerPlanContextDetails resource type</span></span>

> <span data-ttu-id="c5274-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c5274-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5274-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c5274-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5274-106">**PlannerPlanContextDetails**资源包含有关[plannerPlanContext](plannerplancontext.md)的其他信息。</span><span class="sxs-lookup"><span data-stu-id="c5274-106">The **plannerPlanContextDetails** resource contains additional information about a [plannerPlanContext](plannerplancontext.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c5274-107">属性</span><span class="sxs-lookup"><span data-stu-id="c5274-107">Properties</span></span>
| <span data-ttu-id="c5274-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5274-108">Property</span></span>     | <span data-ttu-id="c5274-109">类型</span><span class="sxs-lookup"><span data-stu-id="c5274-109">Type</span></span>   |<span data-ttu-id="c5274-110">说明</span><span class="sxs-lookup"><span data-stu-id="c5274-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5274-111">url</span><span class="sxs-lookup"><span data-stu-id="c5274-111">url</span></span>|<span data-ttu-id="c5274-112">String</span><span class="sxs-lookup"><span data-stu-id="c5274-112">String</span></span>|<span data-ttu-id="c5274-113">由关联[plannerPlanContext](plannerplancontext.md)的用户体验的 URL。</span><span class="sxs-lookup"><span data-stu-id="c5274-113">URL of the user experience represented by the associated [plannerPlanContext](plannerplancontext.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5274-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5274-114">JSON representation</span></span>

<span data-ttu-id="c5274-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5274-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
