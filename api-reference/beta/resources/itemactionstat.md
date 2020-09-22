---
author: daspek
description: ItemActionStat 资源提供有关一段时间内的操作的聚合详细信息。
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8316239a7e00cdc74921c42b70431eba60cdc2d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075670"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="8e82e-103">itemActionStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e82e-103">itemActionStat resource type</span></span>

<span data-ttu-id="8e82e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e82e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e82e-105">**ItemActionStat**资源提供有关一段时间内的操作的聚合详细信息。</span><span class="sxs-lookup"><span data-stu-id="8e82e-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e82e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e82e-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8e82e-107">属性</span><span class="sxs-lookup"><span data-stu-id="8e82e-107">Properties</span></span>

| <span data-ttu-id="8e82e-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e82e-108">Property</span></span>    | <span data-ttu-id="8e82e-109">类型</span><span class="sxs-lookup"><span data-stu-id="8e82e-109">Type</span></span>  | <span data-ttu-id="8e82e-110">说明</span><span class="sxs-lookup"><span data-stu-id="8e82e-110">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="8e82e-111">actionCount</span><span class="sxs-lookup"><span data-stu-id="8e82e-111">actionCount</span></span> | <span data-ttu-id="8e82e-112">Int32</span><span class="sxs-lookup"><span data-stu-id="8e82e-112">Int32</span></span> | <span data-ttu-id="8e82e-113">操作发生次数。</span><span class="sxs-lookup"><span data-stu-id="8e82e-113">The number of times the action took place.</span></span> <span data-ttu-id="8e82e-114">只读。</span><span class="sxs-lookup"><span data-stu-id="8e82e-114">Read-only.</span></span>
| <span data-ttu-id="8e82e-115">actorCount</span><span class="sxs-lookup"><span data-stu-id="8e82e-115">actorCount</span></span>  | <span data-ttu-id="8e82e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8e82e-116">Int32</span></span> | <span data-ttu-id="8e82e-117">执行此操作的不同参与者的数量。</span><span class="sxs-lookup"><span data-stu-id="8e82e-117">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="8e82e-118">只读。</span><span class="sxs-lookup"><span data-stu-id="8e82e-118">Read-only.</span></span>

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


