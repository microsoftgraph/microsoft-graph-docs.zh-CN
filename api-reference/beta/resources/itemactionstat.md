---
author: daspek
description: ItemActionStat 资源提供有关一段时间内的操作的聚合详细信息。
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 719a443af65fd9642feee3bc8ddbc832eb3964c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010110"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="f8cba-103">itemActionStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8cba-103">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8cba-104">**ItemActionStat**资源提供有关一段时间内的操作的聚合详细信息。</span><span class="sxs-lookup"><span data-stu-id="f8cba-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8cba-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8cba-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f8cba-106">属性</span><span class="sxs-lookup"><span data-stu-id="f8cba-106">Properties</span></span>

| <span data-ttu-id="f8cba-107">属性</span><span class="sxs-lookup"><span data-stu-id="f8cba-107">Property</span></span>    | <span data-ttu-id="f8cba-108">类型</span><span class="sxs-lookup"><span data-stu-id="f8cba-108">Type</span></span>  | <span data-ttu-id="f8cba-109">说明</span><span class="sxs-lookup"><span data-stu-id="f8cba-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="f8cba-110">actionCount</span><span class="sxs-lookup"><span data-stu-id="f8cba-110">actionCount</span></span> | <span data-ttu-id="f8cba-111">Int32</span><span class="sxs-lookup"><span data-stu-id="f8cba-111">Int32</span></span> | <span data-ttu-id="f8cba-112">操作发生次数。</span><span class="sxs-lookup"><span data-stu-id="f8cba-112">The number of times the action took place.</span></span> <span data-ttu-id="f8cba-113">只读。</span><span class="sxs-lookup"><span data-stu-id="f8cba-113">Read-only.</span></span>
| <span data-ttu-id="f8cba-114">actorCount</span><span class="sxs-lookup"><span data-stu-id="f8cba-114">actorCount</span></span>  | <span data-ttu-id="f8cba-115">Int32</span><span class="sxs-lookup"><span data-stu-id="f8cba-115">Int32</span></span> | <span data-ttu-id="f8cba-116">执行此操作的不同参与者的数量。</span><span class="sxs-lookup"><span data-stu-id="f8cba-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="f8cba-117">只读。</span><span class="sxs-lookup"><span data-stu-id="f8cba-117">Read-only.</span></span>

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
