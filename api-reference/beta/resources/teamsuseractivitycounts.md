---
title: teamsUserActivityCounts 资源类型
description: 表示按类型表示的活动枚举。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7e931d3488fce488710c638a0155ef0c5dd3a521
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766089"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="87f01-103">teamsUserActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="87f01-103">teamsUserActivityCounts resource type</span></span>

<span data-ttu-id="87f01-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87f01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87f01-105">表示按类型表示的活动枚举。</span><span class="sxs-lookup"><span data-stu-id="87f01-105">Represents numers of activities by type.</span></span>

## <a name="properties"></a><span data-ttu-id="87f01-106">属性</span><span class="sxs-lookup"><span data-stu-id="87f01-106">Properties</span></span>

| <span data-ttu-id="87f01-107">属性</span><span class="sxs-lookup"><span data-stu-id="87f01-107">Property</span></span>            | <span data-ttu-id="87f01-108">类型</span><span class="sxs-lookup"><span data-stu-id="87f01-108">Type</span></span>   | <span data-ttu-id="87f01-109">说明</span><span class="sxs-lookup"><span data-stu-id="87f01-109">Description</span></span>                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="87f01-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="87f01-110">reportRefreshDate</span></span>   | <span data-ttu-id="87f01-111">日期</span><span class="sxs-lookup"><span data-stu-id="87f01-111">Date</span></span>   | <span data-ttu-id="87f01-112">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="87f01-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="87f01-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="87f01-113">reportDate</span></span>          | <span data-ttu-id="87f01-114">日期</span><span class="sxs-lookup"><span data-stu-id="87f01-114">Date</span></span>   | <span data-ttu-id="87f01-115">用户执行活动的日期。</span><span class="sxs-lookup"><span data-stu-id="87f01-115">The date on which the users performed the activities.</span></span>        |
| <span data-ttu-id="87f01-116">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="87f01-116">teamChatMessages</span></span>    | <span data-ttu-id="87f01-117">Int64</span><span class="sxs-lookup"><span data-stu-id="87f01-117">Int64</span></span>  | <span data-ttu-id="87f01-118">用户在团队聊天中发布的唯一消息数。</span><span class="sxs-lookup"><span data-stu-id="87f01-118">The number of unique messages that users posted in a team chat.</span></span> |
| <span data-ttu-id="87f01-119">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="87f01-119">privateChatMessages</span></span> | <span data-ttu-id="87f01-120">Int64</span><span class="sxs-lookup"><span data-stu-id="87f01-120">Int64</span></span>  | <span data-ttu-id="87f01-121">用户在私人聊天中发布的唯一消息数。</span><span class="sxs-lookup"><span data-stu-id="87f01-121">The number of unique messages that users posted in a private chat.</span></span> |
| <span data-ttu-id="87f01-122">calls</span><span class="sxs-lookup"><span data-stu-id="87f01-122">calls</span></span>               | <span data-ttu-id="87f01-123">Int64</span><span class="sxs-lookup"><span data-stu-id="87f01-123">Int64</span></span>  | <span data-ttu-id="87f01-124">用户参与的唯一 1：1 呼叫数。</span><span class="sxs-lookup"><span data-stu-id="87f01-124">The number of unique 1:1 calls that users participated in.</span></span>   |
| <span data-ttu-id="87f01-125">会议</span><span class="sxs-lookup"><span data-stu-id="87f01-125">meetings</span></span>            | <span data-ttu-id="87f01-126">Int64</span><span class="sxs-lookup"><span data-stu-id="87f01-126">Int64</span></span>  | <span data-ttu-id="87f01-127">用户参与的唯一联机会议的数量。</span><span class="sxs-lookup"><span data-stu-id="87f01-127">The number of unique online meetings that users participated in.</span></span> |
| <span data-ttu-id="87f01-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="87f01-128">reportPeriod</span></span>        | <span data-ttu-id="87f01-129">String</span><span class="sxs-lookup"><span data-stu-id="87f01-129">String</span></span> | <span data-ttu-id="87f01-130">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="87f01-130">The number of days the report covers.</span></span>                        |


## <a name="json-representation"></a><span data-ttu-id="87f01-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87f01-131">JSON representation</span></span>

<span data-ttu-id="87f01-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87f01-132">The following is a JSON representation of the resource.</span></span>

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


