---
title: teamsUserActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c7351795f6b3dafbac996844fc1ac11cd24bbc03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886588"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="9d93e-103">teamsUserActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d93e-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9d93e-104">属性</span><span class="sxs-lookup"><span data-stu-id="9d93e-104">Properties</span></span>

| <span data-ttu-id="9d93e-105">属性</span><span class="sxs-lookup"><span data-stu-id="9d93e-105">Property</span></span>            | <span data-ttu-id="9d93e-106">类型</span><span class="sxs-lookup"><span data-stu-id="9d93e-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="9d93e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9d93e-107">reportRefreshDate</span></span>   | <span data-ttu-id="9d93e-108">日期</span><span class="sxs-lookup"><span data-stu-id="9d93e-108">Date</span></span>   |
| <span data-ttu-id="9d93e-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="9d93e-109">reportDate</span></span>          | <span data-ttu-id="9d93e-110">日期</span><span class="sxs-lookup"><span data-stu-id="9d93e-110">Date</span></span>   |
| <span data-ttu-id="9d93e-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="9d93e-111">teamChatMessages</span></span>    | <span data-ttu-id="9d93e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="9d93e-112">Int64</span></span>  |
| <span data-ttu-id="9d93e-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="9d93e-113">privateChatMessages</span></span> | <span data-ttu-id="9d93e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="9d93e-114">Int64</span></span>  |
| <span data-ttu-id="9d93e-115">呼叫</span><span class="sxs-lookup"><span data-stu-id="9d93e-115">calls</span></span>               | <span data-ttu-id="9d93e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="9d93e-116">Int64</span></span>  |
| <span data-ttu-id="9d93e-117">会议</span><span class="sxs-lookup"><span data-stu-id="9d93e-117">meetings</span></span>            | <span data-ttu-id="9d93e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="9d93e-118">Int64</span></span>  |
| <span data-ttu-id="9d93e-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9d93e-119">reportPeriod</span></span>        | <span data-ttu-id="9d93e-120">String</span><span class="sxs-lookup"><span data-stu-id="9d93e-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9d93e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d93e-121">JSON representation</span></span>

<span data-ttu-id="9d93e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d93e-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```
