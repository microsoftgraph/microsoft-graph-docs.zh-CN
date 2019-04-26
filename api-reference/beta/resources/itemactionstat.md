---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
ms.openlocfilehash: 39209671b63b991a8fb3ccf1c830c8557fce27c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569975"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="28030-102">itemActionStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="28030-102">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28030-103">**itemActionStat**资源提供有关一段时间内的操作的聚合详细信息。</span><span class="sxs-lookup"><span data-stu-id="28030-103">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="28030-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28030-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="28030-105">属性</span><span class="sxs-lookup"><span data-stu-id="28030-105">Properties</span></span>

| <span data-ttu-id="28030-106">属性</span><span class="sxs-lookup"><span data-stu-id="28030-106">Property</span></span>    | <span data-ttu-id="28030-107">类型</span><span class="sxs-lookup"><span data-stu-id="28030-107">Type</span></span>  | <span data-ttu-id="28030-108">说明</span><span class="sxs-lookup"><span data-stu-id="28030-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="28030-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="28030-109">actionCount</span></span> | <span data-ttu-id="28030-110">Int32</span><span class="sxs-lookup"><span data-stu-id="28030-110">Int32</span></span> | <span data-ttu-id="28030-111">操作发生次数。</span><span class="sxs-lookup"><span data-stu-id="28030-111">The number of times the action took place.</span></span> <span data-ttu-id="28030-112">只读。</span><span class="sxs-lookup"><span data-stu-id="28030-112">Read-only.</span></span>
| <span data-ttu-id="28030-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="28030-113">actorCount</span></span>  | <span data-ttu-id="28030-114">Int32</span><span class="sxs-lookup"><span data-stu-id="28030-114">Int32</span></span> | <span data-ttu-id="28030-115">执行此操作的不同参与者的数量。</span><span class="sxs-lookup"><span data-stu-id="28030-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="28030-116">只读。</span><span class="sxs-lookup"><span data-stu-id="28030-116">Read-only.</span></span>

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
