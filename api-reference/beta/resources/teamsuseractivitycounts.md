---
title: teamsUserActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 68eb66cbd0e076d9cf2559170fee4c81dca1e65c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046340"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="497b2-103">teamsUserActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="497b2-103">teamsUserActivityCounts resource type</span></span>

<span data-ttu-id="497b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="497b2-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="497b2-105">属性</span><span class="sxs-lookup"><span data-stu-id="497b2-105">Properties</span></span>

| <span data-ttu-id="497b2-106">属性</span><span class="sxs-lookup"><span data-stu-id="497b2-106">Property</span></span>            | <span data-ttu-id="497b2-107">类型</span><span class="sxs-lookup"><span data-stu-id="497b2-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="497b2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="497b2-108">reportRefreshDate</span></span>   | <span data-ttu-id="497b2-109">日期</span><span class="sxs-lookup"><span data-stu-id="497b2-109">Date</span></span>   |
| <span data-ttu-id="497b2-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="497b2-110">reportDate</span></span>          | <span data-ttu-id="497b2-111">日期</span><span class="sxs-lookup"><span data-stu-id="497b2-111">Date</span></span>   |
| <span data-ttu-id="497b2-112">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="497b2-112">teamChatMessages</span></span>    | <span data-ttu-id="497b2-113">Int64</span><span class="sxs-lookup"><span data-stu-id="497b2-113">Int64</span></span>  |
| <span data-ttu-id="497b2-114">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="497b2-114">privateChatMessages</span></span> | <span data-ttu-id="497b2-115">Int64</span><span class="sxs-lookup"><span data-stu-id="497b2-115">Int64</span></span>  |
| <span data-ttu-id="497b2-116">calls</span><span class="sxs-lookup"><span data-stu-id="497b2-116">calls</span></span>               | <span data-ttu-id="497b2-117">Int64</span><span class="sxs-lookup"><span data-stu-id="497b2-117">Int64</span></span>  |
| <span data-ttu-id="497b2-118">会议</span><span class="sxs-lookup"><span data-stu-id="497b2-118">meetings</span></span>            | <span data-ttu-id="497b2-119">Int64</span><span class="sxs-lookup"><span data-stu-id="497b2-119">Int64</span></span>  |
| <span data-ttu-id="497b2-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="497b2-120">reportPeriod</span></span>        | <span data-ttu-id="497b2-121">String</span><span class="sxs-lookup"><span data-stu-id="497b2-121">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="497b2-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="497b2-122">JSON representation</span></span>

<span data-ttu-id="497b2-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="497b2-123">The following is a JSON representation of the resource.</span></span>

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


