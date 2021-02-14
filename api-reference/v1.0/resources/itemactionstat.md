---
author: daspek
title: itemActionStat 资源类型
description: itemActionStat 对象提供有关一段时间的操作的聚合详细信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 13bc306a1b14d7d59ec8eddda5b02a5cba84e649
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238524"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="cd09d-103">itemActionStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd09d-103">itemActionStat resource type</span></span>

<span data-ttu-id="cd09d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd09d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd09d-105">**itemActionStat** 资源提供一段时间内某个操作聚合的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cd09d-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="cd09d-106">属性</span><span class="sxs-lookup"><span data-stu-id="cd09d-106">Properties</span></span>

| <span data-ttu-id="cd09d-107">属性</span><span class="sxs-lookup"><span data-stu-id="cd09d-107">Property</span></span>    | <span data-ttu-id="cd09d-108">类型</span><span class="sxs-lookup"><span data-stu-id="cd09d-108">Type</span></span>  | <span data-ttu-id="cd09d-109">说明</span><span class="sxs-lookup"><span data-stu-id="cd09d-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="cd09d-110">actionCount</span><span class="sxs-lookup"><span data-stu-id="cd09d-110">actionCount</span></span> | <span data-ttu-id="cd09d-111">Int32</span><span class="sxs-lookup"><span data-stu-id="cd09d-111">Int32</span></span> | <span data-ttu-id="cd09d-112">操作发生次数。</span><span class="sxs-lookup"><span data-stu-id="cd09d-112">The number of times the action took place.</span></span> <span data-ttu-id="cd09d-113">只读。</span><span class="sxs-lookup"><span data-stu-id="cd09d-113">Read-only.</span></span>
| <span data-ttu-id="cd09d-114">actorCount</span><span class="sxs-lookup"><span data-stu-id="cd09d-114">actorCount</span></span>  | <span data-ttu-id="cd09d-115">Int32</span><span class="sxs-lookup"><span data-stu-id="cd09d-115">Int32</span></span> | <span data-ttu-id="cd09d-116">执行该操作不同操作者的数量。</span><span class="sxs-lookup"><span data-stu-id="cd09d-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="cd09d-117">只读。</span><span class="sxs-lookup"><span data-stu-id="cd09d-117">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd09d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd09d-118">JSON representation</span></span>

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

