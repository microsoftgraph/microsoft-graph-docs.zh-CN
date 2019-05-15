---
author: daspek
ms.author: dspektor
title: itemActionStat 资源类型
description: ItemActionStat 对象提供有关一段时间内的操作的聚合详细信息。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1d5531fc969762219f4e2404787190649ecdaf11
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970636"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="38b6c-103">itemActionStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="38b6c-103">itemActionStat resource type</span></span>

<span data-ttu-id="38b6c-104">**ItemActionStat**资源提供有关一段时间内的操作的聚合详细信息。</span><span class="sxs-lookup"><span data-stu-id="38b6c-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="38b6c-105">属性</span><span class="sxs-lookup"><span data-stu-id="38b6c-105">Properties</span></span>

| <span data-ttu-id="38b6c-106">属性</span><span class="sxs-lookup"><span data-stu-id="38b6c-106">Property</span></span>    | <span data-ttu-id="38b6c-107">类型</span><span class="sxs-lookup"><span data-stu-id="38b6c-107">Type</span></span>  | <span data-ttu-id="38b6c-108">说明</span><span class="sxs-lookup"><span data-stu-id="38b6c-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="38b6c-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="38b6c-109">actionCount</span></span> | <span data-ttu-id="38b6c-110">Int32</span><span class="sxs-lookup"><span data-stu-id="38b6c-110">Int32</span></span> | <span data-ttu-id="38b6c-111">操作发生次数。</span><span class="sxs-lookup"><span data-stu-id="38b6c-111">The number of times the action took place.</span></span> <span data-ttu-id="38b6c-112">只读。</span><span class="sxs-lookup"><span data-stu-id="38b6c-112">Read-only.</span></span>
| <span data-ttu-id="38b6c-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="38b6c-113">actorCount</span></span>  | <span data-ttu-id="38b6c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="38b6c-114">Int32</span></span> | <span data-ttu-id="38b6c-115">执行此操作的不同参与者的数量。</span><span class="sxs-lookup"><span data-stu-id="38b6c-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="38b6c-116">只读。</span><span class="sxs-lookup"><span data-stu-id="38b6c-116">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38b6c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38b6c-117">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/itemActionStat",
  "suppressions": []
}
-->
