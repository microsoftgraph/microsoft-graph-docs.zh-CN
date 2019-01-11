---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
ms.openlocfilehash: 1d2ab438e7aaf5b0a6aede99290394a9a4ea7f0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879525"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="fb5dd-102">itemActionStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb5dd-102">itemActionStat resource type</span></span>

> <span data-ttu-id="fb5dd-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb5dd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb5dd-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb5dd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb5dd-105">**ItemActionStat**资源提供有关操作的时间段的聚合详细信息。</span><span class="sxs-lookup"><span data-stu-id="fb5dd-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb5dd-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb5dd-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fb5dd-107">属性</span><span class="sxs-lookup"><span data-stu-id="fb5dd-107">Properties</span></span>

| <span data-ttu-id="fb5dd-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb5dd-108">Property</span></span>    | <span data-ttu-id="fb5dd-109">类型</span><span class="sxs-lookup"><span data-stu-id="fb5dd-109">Type</span></span>  | <span data-ttu-id="fb5dd-110">Description</span><span class="sxs-lookup"><span data-stu-id="fb5dd-110">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="fb5dd-111">actionCount</span><span class="sxs-lookup"><span data-stu-id="fb5dd-111">actionCount</span></span> | <span data-ttu-id="fb5dd-112">Int32</span><span class="sxs-lookup"><span data-stu-id="fb5dd-112">Int32</span></span> | <span data-ttu-id="fb5dd-113">操作发生次数。</span><span class="sxs-lookup"><span data-stu-id="fb5dd-113">The number of times the action took place.</span></span> <span data-ttu-id="fb5dd-114">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="fb5dd-114">Read-only.</span></span>
| <span data-ttu-id="fb5dd-115">actorCount</span><span class="sxs-lookup"><span data-stu-id="fb5dd-115">actorCount</span></span>  | <span data-ttu-id="fb5dd-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fb5dd-116">Int32</span></span> | <span data-ttu-id="fb5dd-117">执行操作的不同参与者数。</span><span class="sxs-lookup"><span data-stu-id="fb5dd-117">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="fb5dd-118">只读。</span><span class="sxs-lookup"><span data-stu-id="fb5dd-118">Read-only.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat"
} -->
