---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
ms.openlocfilehash: f7e9351bc4a394005cffc712aa444c999a51b363
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048266"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="69103-102">itemActionStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="69103-102">itemActionStat resource type</span></span>

> <span data-ttu-id="69103-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69103-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69103-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69103-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69103-105">**ItemActionStat**资源提供有关操作的时间段的聚合详细信息。</span><span class="sxs-lookup"><span data-stu-id="69103-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69103-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69103-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="69103-107">属性</span><span class="sxs-lookup"><span data-stu-id="69103-107">Properties</span></span>

| <span data-ttu-id="69103-108">属性</span><span class="sxs-lookup"><span data-stu-id="69103-108">Property</span></span>    | <span data-ttu-id="69103-109">类型</span><span class="sxs-lookup"><span data-stu-id="69103-109">Type</span></span>  | <span data-ttu-id="69103-110">说明</span><span class="sxs-lookup"><span data-stu-id="69103-110">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="69103-111">actionCount</span><span class="sxs-lookup"><span data-stu-id="69103-111">actionCount</span></span> | <span data-ttu-id="69103-112">Int32</span><span class="sxs-lookup"><span data-stu-id="69103-112">Int32</span></span> | <span data-ttu-id="69103-113">操作发生次数。</span><span class="sxs-lookup"><span data-stu-id="69103-113">The number of times the action took place.</span></span> <span data-ttu-id="69103-114">只读。</span><span class="sxs-lookup"><span data-stu-id="69103-114">Read-only.</span></span>
| <span data-ttu-id="69103-115">actorCount</span><span class="sxs-lookup"><span data-stu-id="69103-115">actorCount</span></span>  | <span data-ttu-id="69103-116">Int32</span><span class="sxs-lookup"><span data-stu-id="69103-116">Int32</span></span> | <span data-ttu-id="69103-117">执行操作的不同参与者数。</span><span class="sxs-lookup"><span data-stu-id="69103-117">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="69103-118">只读。</span><span class="sxs-lookup"><span data-stu-id="69103-118">Read-only.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat"
} -->
