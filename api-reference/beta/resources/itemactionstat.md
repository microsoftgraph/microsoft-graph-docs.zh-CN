---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
ms.openlocfilehash: 39209671b63b991a8fb3ccf1c830c8557fce27c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509635"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="5c0af-102">itemActionStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c0af-102">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c0af-103">**ItemActionStat**资源提供有关操作的时间段的聚合详细信息。</span><span class="sxs-lookup"><span data-stu-id="5c0af-103">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c0af-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c0af-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

## <a name="properties"></a><span data-ttu-id="5c0af-105">属性</span><span class="sxs-lookup"><span data-stu-id="5c0af-105">Properties</span></span>

| <span data-ttu-id="5c0af-106">属性</span><span class="sxs-lookup"><span data-stu-id="5c0af-106">Property</span></span>    | <span data-ttu-id="5c0af-107">类型</span><span class="sxs-lookup"><span data-stu-id="5c0af-107">Type</span></span>  | <span data-ttu-id="5c0af-108">说明</span><span class="sxs-lookup"><span data-stu-id="5c0af-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="5c0af-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="5c0af-109">actionCount</span></span> | <span data-ttu-id="5c0af-110">Int32</span><span class="sxs-lookup"><span data-stu-id="5c0af-110">Int32</span></span> | <span data-ttu-id="5c0af-111">操作发生次数。</span><span class="sxs-lookup"><span data-stu-id="5c0af-111">The number of times the action took place.</span></span> <span data-ttu-id="5c0af-112">只读。</span><span class="sxs-lookup"><span data-stu-id="5c0af-112">Read-only.</span></span>
| <span data-ttu-id="5c0af-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="5c0af-113">actorCount</span></span>  | <span data-ttu-id="5c0af-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5c0af-114">Int32</span></span> | <span data-ttu-id="5c0af-115">执行操作的不同参与者数。</span><span class="sxs-lookup"><span data-stu-id="5c0af-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="5c0af-116">只读。</span><span class="sxs-lookup"><span data-stu-id="5c0af-116">Read-only.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactionstat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
