---
title: plannerPlanContextDetails 资源类型
description: '**plannerPlanContextDetails**资源包含有关 plannerPlanContext 的其他信息。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 025e5b1623333d0235ae83e061e30247a3d130f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505947"
---
# <a name="plannerplancontextdetails-resource-type"></a><span data-ttu-id="7595b-103">plannerPlanContextDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="7595b-103">plannerPlanContextDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7595b-104">**plannerPlanContextDetails**资源包含有关[plannerPlanContext](plannerplancontext.md)的其他信息。</span><span class="sxs-lookup"><span data-stu-id="7595b-104">The **plannerPlanContextDetails** resource contains additional information about a [plannerPlanContext](plannerplancontext.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7595b-105">属性</span><span class="sxs-lookup"><span data-stu-id="7595b-105">Properties</span></span>
| <span data-ttu-id="7595b-106">属性</span><span class="sxs-lookup"><span data-stu-id="7595b-106">Property</span></span>     | <span data-ttu-id="7595b-107">类型</span><span class="sxs-lookup"><span data-stu-id="7595b-107">Type</span></span>   |<span data-ttu-id="7595b-108">说明</span><span class="sxs-lookup"><span data-stu-id="7595b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7595b-109">url</span><span class="sxs-lookup"><span data-stu-id="7595b-109">url</span></span>|<span data-ttu-id="7595b-110">String</span><span class="sxs-lookup"><span data-stu-id="7595b-110">String</span></span>|<span data-ttu-id="7595b-111">由关联的[plannerPlanContext](plannerplancontext.md)表示的用户体验的 URL。</span><span class="sxs-lookup"><span data-stu-id="7595b-111">URL of the user experience represented by the associated [plannerPlanContext](plannerplancontext.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7595b-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7595b-112">JSON representation</span></span>

<span data-ttu-id="7595b-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7595b-113">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextdetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
