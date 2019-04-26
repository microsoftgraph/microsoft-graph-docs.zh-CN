---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
ms.openlocfilehash: a0e3bc3f217308d96eaadf6ab367431c7f1b8c3e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345434"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="6cc04-102">itemActionStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="6cc04-102">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cc04-103">**itemActionStat**资源提供有关一段时间内的操作的聚合详细信息。</span><span class="sxs-lookup"><span data-stu-id="6cc04-103">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6cc04-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6cc04-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6cc04-105">属性</span><span class="sxs-lookup"><span data-stu-id="6cc04-105">Properties</span></span>

| <span data-ttu-id="6cc04-106">属性</span><span class="sxs-lookup"><span data-stu-id="6cc04-106">Property</span></span>    | <span data-ttu-id="6cc04-107">类型</span><span class="sxs-lookup"><span data-stu-id="6cc04-107">Type</span></span>  | <span data-ttu-id="6cc04-108">说明</span><span class="sxs-lookup"><span data-stu-id="6cc04-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="6cc04-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="6cc04-109">actionCount</span></span> | <span data-ttu-id="6cc04-110">Int32</span><span class="sxs-lookup"><span data-stu-id="6cc04-110">Int32</span></span> | <span data-ttu-id="6cc04-111">操作发生次数。</span><span class="sxs-lookup"><span data-stu-id="6cc04-111">The number of times the action took place.</span></span> <span data-ttu-id="6cc04-112">只读。</span><span class="sxs-lookup"><span data-stu-id="6cc04-112">Read-only.</span></span>
| <span data-ttu-id="6cc04-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="6cc04-113">actorCount</span></span>  | <span data-ttu-id="6cc04-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6cc04-114">Int32</span></span> | <span data-ttu-id="6cc04-115">执行此操作的不同参与者的数量。</span><span class="sxs-lookup"><span data-stu-id="6cc04-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="6cc04-116">只读。</span><span class="sxs-lookup"><span data-stu-id="6cc04-116">Read-only.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat",
  "suppressions": []
}
-->
