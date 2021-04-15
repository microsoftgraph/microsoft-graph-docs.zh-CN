---
title: teamsUserActivityDistributionUserCounts 资源类型
description: 表示选定时段内按活动类型表示的用户数。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3d4fa8b3aec98a03d7e51819db0dc4797367f499
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766921"
---
# <a name="teamsuseractivitydistributionusercounts-resource-type"></a><span data-ttu-id="6fc9f-103">teamsUserActivityDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fc9f-103">teamsUserActivityDistributionUserCounts resource type</span></span>

<span data-ttu-id="6fc9f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fc9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fc9f-105">表示选定时段内按活动类型表示的用户数。</span><span class="sxs-lookup"><span data-stu-id="6fc9f-105">Represents numbers of users by activity type over the selected time period.</span></span>

## <a name="properties"></a><span data-ttu-id="6fc9f-106">属性</span><span class="sxs-lookup"><span data-stu-id="6fc9f-106">Properties</span></span>

| <span data-ttu-id="6fc9f-107">属性</span><span class="sxs-lookup"><span data-stu-id="6fc9f-107">Property</span></span>            | <span data-ttu-id="6fc9f-108">类型</span><span class="sxs-lookup"><span data-stu-id="6fc9f-108">Type</span></span>   | <span data-ttu-id="6fc9f-109">说明</span><span class="sxs-lookup"><span data-stu-id="6fc9f-109">Description</span></span>                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="6fc9f-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6fc9f-110">reportRefreshDate</span></span>   | <span data-ttu-id="6fc9f-111">日期</span><span class="sxs-lookup"><span data-stu-id="6fc9f-111">Date</span></span>   | <span data-ttu-id="6fc9f-112">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="6fc9f-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="6fc9f-113">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="6fc9f-113">teamChatMessages</span></span>    | <span data-ttu-id="6fc9f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6fc9f-114">Int64</span></span>  | <span data-ttu-id="6fc9f-115">用户在团队聊天中发布的唯一消息数。</span><span class="sxs-lookup"><span data-stu-id="6fc9f-115">The number of unique messages that users posted in a team chat.</span></span> |
| <span data-ttu-id="6fc9f-116">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="6fc9f-116">privateChatMessages</span></span> | <span data-ttu-id="6fc9f-117">Int64</span><span class="sxs-lookup"><span data-stu-id="6fc9f-117">Int64</span></span>  | <span data-ttu-id="6fc9f-118">用户在私人聊天中发布的唯一消息数。</span><span class="sxs-lookup"><span data-stu-id="6fc9f-118">The number of unique messages that users posted in a private chat.</span></span> |
| <span data-ttu-id="6fc9f-119">calls</span><span class="sxs-lookup"><span data-stu-id="6fc9f-119">calls</span></span>               | <span data-ttu-id="6fc9f-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6fc9f-120">Int64</span></span>  | <span data-ttu-id="6fc9f-121">用户参与的唯一 1：1 呼叫数。</span><span class="sxs-lookup"><span data-stu-id="6fc9f-121">The number of unique 1:1 calls that users participated in.</span></span>   |
| <span data-ttu-id="6fc9f-122">会议</span><span class="sxs-lookup"><span data-stu-id="6fc9f-122">meetings</span></span>            | <span data-ttu-id="6fc9f-123">Int64</span><span class="sxs-lookup"><span data-stu-id="6fc9f-123">Int64</span></span>  | <span data-ttu-id="6fc9f-124">用户参与的唯一联机会议的数量。</span><span class="sxs-lookup"><span data-stu-id="6fc9f-124">The number of unique online meetings that users participated in.</span></span> |
| <span data-ttu-id="6fc9f-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6fc9f-125">reportPeriod</span></span>        | <span data-ttu-id="6fc9f-126">String</span><span class="sxs-lookup"><span data-stu-id="6fc9f-126">String</span></span> | <span data-ttu-id="6fc9f-127">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="6fc9f-127">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="6fc9f-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fc9f-128">JSON representation</span></span>

<span data-ttu-id="6fc9f-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fc9f-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```


