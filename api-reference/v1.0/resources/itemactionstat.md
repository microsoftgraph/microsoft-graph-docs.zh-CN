---
author: daspek
ms.author: dspektor
title: itemActionStat 资源类型
description: ItemActionStat 对象提供有关一段时间内的操作的聚合详细信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 7eda0f6ddbed16dadf1eac4a3ea737cdd7fd2c89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036755"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="8eda2-103">itemActionStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="8eda2-103">itemActionStat resource type</span></span>

<span data-ttu-id="8eda2-104">**ItemActionStat**资源提供有关一段时间内的操作的聚合详细信息。</span><span class="sxs-lookup"><span data-stu-id="8eda2-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="8eda2-105">属性</span><span class="sxs-lookup"><span data-stu-id="8eda2-105">Properties</span></span>

| <span data-ttu-id="8eda2-106">属性</span><span class="sxs-lookup"><span data-stu-id="8eda2-106">Property</span></span>    | <span data-ttu-id="8eda2-107">类型</span><span class="sxs-lookup"><span data-stu-id="8eda2-107">Type</span></span>  | <span data-ttu-id="8eda2-108">说明</span><span class="sxs-lookup"><span data-stu-id="8eda2-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="8eda2-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="8eda2-109">actionCount</span></span> | <span data-ttu-id="8eda2-110">Int32</span><span class="sxs-lookup"><span data-stu-id="8eda2-110">Int32</span></span> | <span data-ttu-id="8eda2-111">操作发生次数。</span><span class="sxs-lookup"><span data-stu-id="8eda2-111">The number of times the action took place.</span></span> <span data-ttu-id="8eda2-112">只读。</span><span class="sxs-lookup"><span data-stu-id="8eda2-112">Read-only.</span></span>
| <span data-ttu-id="8eda2-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="8eda2-113">actorCount</span></span>  | <span data-ttu-id="8eda2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="8eda2-114">Int32</span></span> | <span data-ttu-id="8eda2-115">执行此操作的不同参与者的数量。</span><span class="sxs-lookup"><span data-stu-id="8eda2-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="8eda2-116">只读。</span><span class="sxs-lookup"><span data-stu-id="8eda2-116">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8eda2-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8eda2-117">JSON representation</span></span>

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
