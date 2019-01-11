---
title: plannerPlanContextDetails 资源类型
description: '**PlannerPlanContextDetails**资源包含有关 plannerPlanContext 的其他信息。'
localization_priority: Normal
ms.openlocfilehash: ec35a83e5ba2d2648c512f31f838f19bd3ec2e02
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812052"
---
# <a name="plannerplancontextdetails-resource-type"></a><span data-ttu-id="1578d-103">plannerPlanContextDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="1578d-103">plannerPlanContextDetails resource type</span></span>

> <span data-ttu-id="1578d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1578d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1578d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1578d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1578d-106">**PlannerPlanContextDetails**资源包含有关[plannerPlanContext](plannerplancontext.md)的其他信息。</span><span class="sxs-lookup"><span data-stu-id="1578d-106">The **plannerPlanContextDetails** resource contains additional information about a [plannerPlanContext](plannerplancontext.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1578d-107">属性</span><span class="sxs-lookup"><span data-stu-id="1578d-107">Properties</span></span>
| <span data-ttu-id="1578d-108">属性</span><span class="sxs-lookup"><span data-stu-id="1578d-108">Property</span></span>     | <span data-ttu-id="1578d-109">类型</span><span class="sxs-lookup"><span data-stu-id="1578d-109">Type</span></span>   |<span data-ttu-id="1578d-110">说明</span><span class="sxs-lookup"><span data-stu-id="1578d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1578d-111">url</span><span class="sxs-lookup"><span data-stu-id="1578d-111">url</span></span>|<span data-ttu-id="1578d-112">String</span><span class="sxs-lookup"><span data-stu-id="1578d-112">String</span></span>|<span data-ttu-id="1578d-113">由关联[plannerPlanContext](plannerplancontext.md)的用户体验的 URL。</span><span class="sxs-lookup"><span data-stu-id="1578d-113">URL of the user experience represented by the associated [plannerPlanContext](plannerplancontext.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1578d-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1578d-114">JSON representation</span></span>

<span data-ttu-id="1578d-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1578d-115">The following is a JSON representation of the resource.</span></span>

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
