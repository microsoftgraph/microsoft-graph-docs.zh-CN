---
author: daspek
ms.author: dspektor
title: itemActionStat 资源类型
description: ItemActionStat 对象提供有关一段时间内的操作的聚合详细信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f1be83bef880b967758a803e694b068df9bfaebf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041265"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="d064d-103">itemActionStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="d064d-103">itemActionStat resource type</span></span>

<span data-ttu-id="d064d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d064d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d064d-105">**ItemActionStat**资源提供有关一段时间内的操作的聚合详细信息。</span><span class="sxs-lookup"><span data-stu-id="d064d-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="d064d-106">属性</span><span class="sxs-lookup"><span data-stu-id="d064d-106">Properties</span></span>

| <span data-ttu-id="d064d-107">属性</span><span class="sxs-lookup"><span data-stu-id="d064d-107">Property</span></span>    | <span data-ttu-id="d064d-108">类型</span><span class="sxs-lookup"><span data-stu-id="d064d-108">Type</span></span>  | <span data-ttu-id="d064d-109">说明</span><span class="sxs-lookup"><span data-stu-id="d064d-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="d064d-110">actionCount</span><span class="sxs-lookup"><span data-stu-id="d064d-110">actionCount</span></span> | <span data-ttu-id="d064d-111">Int32</span><span class="sxs-lookup"><span data-stu-id="d064d-111">Int32</span></span> | <span data-ttu-id="d064d-112">操作发生次数。</span><span class="sxs-lookup"><span data-stu-id="d064d-112">The number of times the action took place.</span></span> <span data-ttu-id="d064d-113">只读。</span><span class="sxs-lookup"><span data-stu-id="d064d-113">Read-only.</span></span>
| <span data-ttu-id="d064d-114">actorCount</span><span class="sxs-lookup"><span data-stu-id="d064d-114">actorCount</span></span>  | <span data-ttu-id="d064d-115">Int32</span><span class="sxs-lookup"><span data-stu-id="d064d-115">Int32</span></span> | <span data-ttu-id="d064d-116">执行此操作的不同参与者的数量。</span><span class="sxs-lookup"><span data-stu-id="d064d-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="d064d-117">只读。</span><span class="sxs-lookup"><span data-stu-id="d064d-117">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d064d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d064d-118">JSON representation</span></span>

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

