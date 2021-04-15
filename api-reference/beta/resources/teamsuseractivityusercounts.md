---
title: teamsUserActivityUserCounts 资源类型
description: 表示按活动类型表示的每日用户数。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f1ddb3e6e5e6a0b6fbb5c9973bec7e29f4492089
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766439"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="69244-103">teamsUserActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="69244-103">teamsUserActivityUserCounts resource type</span></span>

<span data-ttu-id="69244-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69244-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69244-105">表示按活动类型表示的每日用户数。</span><span class="sxs-lookup"><span data-stu-id="69244-105">Represents numbers of daily users by activity type.</span></span>

## <a name="properties"></a><span data-ttu-id="69244-106">属性</span><span class="sxs-lookup"><span data-stu-id="69244-106">Properties</span></span>

| <span data-ttu-id="69244-107">属性</span><span class="sxs-lookup"><span data-stu-id="69244-107">Property</span></span>            | <span data-ttu-id="69244-108">类型</span><span class="sxs-lookup"><span data-stu-id="69244-108">Type</span></span>   | <span data-ttu-id="69244-109">说明</span><span class="sxs-lookup"><span data-stu-id="69244-109">Description</span></span>                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="69244-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="69244-110">reportRefreshDate</span></span>   | <span data-ttu-id="69244-111">日期</span><span class="sxs-lookup"><span data-stu-id="69244-111">Date</span></span>   | <span data-ttu-id="69244-112">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="69244-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="69244-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="69244-113">reportDate</span></span>          | <span data-ttu-id="69244-114">日期</span><span class="sxs-lookup"><span data-stu-id="69244-114">Date</span></span>   | <span data-ttu-id="69244-115">用户执行活动的日期。</span><span class="sxs-lookup"><span data-stu-id="69244-115">The date on which the users performed the activities.</span></span>        |
| <span data-ttu-id="69244-116">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="69244-116">teamChatMessages</span></span>    | <span data-ttu-id="69244-117">Int64</span><span class="sxs-lookup"><span data-stu-id="69244-117">Int64</span></span>  | <span data-ttu-id="69244-118">在团队聊天中发布消息的用户数量。</span><span class="sxs-lookup"><span data-stu-id="69244-118">The number of users who posted message in a team chat.</span></span>       |
| <span data-ttu-id="69244-119">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="69244-119">privateChatMessages</span></span> | <span data-ttu-id="69244-120">Int64</span><span class="sxs-lookup"><span data-stu-id="69244-120">Int64</span></span>  | <span data-ttu-id="69244-121">在私人聊天中发布消息的用户数量。</span><span class="sxs-lookup"><span data-stu-id="69244-121">The number of users who posted message in a private chat.</span></span>    |
| <span data-ttu-id="69244-122">calls</span><span class="sxs-lookup"><span data-stu-id="69244-122">calls</span></span>               | <span data-ttu-id="69244-123">Int64</span><span class="sxs-lookup"><span data-stu-id="69244-123">Int64</span></span>  | <span data-ttu-id="69244-124">参与一对一呼叫的用户数。</span><span class="sxs-lookup"><span data-stu-id="69244-124">The number of users who participated in 1:1 calls.</span></span>           |
| <span data-ttu-id="69244-125">会议</span><span class="sxs-lookup"><span data-stu-id="69244-125">meetings</span></span>            | <span data-ttu-id="69244-126">Int64</span><span class="sxs-lookup"><span data-stu-id="69244-126">Int64</span></span>  | <span data-ttu-id="69244-127">参与联机会议的用户数。</span><span class="sxs-lookup"><span data-stu-id="69244-127">The number of users who participated in online meetings.</span></span>     |
| <span data-ttu-id="69244-128">otherActions</span><span class="sxs-lookup"><span data-stu-id="69244-128">otherActions</span></span>        | <span data-ttu-id="69244-129">Int64</span><span class="sxs-lookup"><span data-stu-id="69244-129">Int64</span></span>  | <span data-ttu-id="69244-130">除报告中提供的公开操作类型外，处于活动状态但执行了其他活动的用户数 (发送或回复频道消息和聊天消息、安排或参与 1：1 呼叫和会议) 。</span><span class="sxs-lookup"><span data-stu-id="69244-130">The number of users who were active but performed other activities than exposed action types offered in the report (sending or replying to channel messages and chat messages, scheduling or participating in 1:1 calls and meetings).</span></span> <span data-ttu-id="69244-131">示例操作包括用户更改 Teams 状态或 Teams 状态消息或打开频道消息帖子但不回复的情况。</span><span class="sxs-lookup"><span data-stu-id="69244-131">Examples actions are when a user changes the Teams status or the Teams status message or opens a Channel Message post but does not reply.</span></span> |
| <span data-ttu-id="69244-132">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="69244-132">reportPeriod</span></span>        | <span data-ttu-id="69244-133">String</span><span class="sxs-lookup"><span data-stu-id="69244-133">String</span></span> | <span data-ttu-id="69244-134">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="69244-134">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="69244-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69244-135">JSON representation</span></span>

<span data-ttu-id="69244-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69244-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```


