---
title: Microsoft Teams 用户活动报告
description: 使用 Microsoft 团队用户活动报告您的组织中获取的 Microsoft 团队用户活动见解。
localization_priority: Normal
ms.openlocfilehash: 2fc2eee8243a338204687114d2f1de3d2e794a9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845519"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="b1cbb-103">Microsoft Teams 用户活动报告</span><span class="sxs-lookup"><span data-stu-id="b1cbb-103">Microsoft Teams user activity reports</span></span>

> <span data-ttu-id="b1cbb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b1cbb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1cbb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b1cbb-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="b1cbb-106">在 Microsoft Graph 中国由 21Vianet 不支持这些 Api。</span><span class="sxs-lookup"><span data-stu-id="b1cbb-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="b1cbb-107">使用 Microsoft 团队用户活动报告您的组织中获取的 Microsoft 团队用户活动见解。</span><span class="sxs-lookup"><span data-stu-id="b1cbb-107">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="b1cbb-108">方法</span><span class="sxs-lookup"><span data-stu-id="b1cbb-108">Methods</span></span>

| <span data-ttu-id="b1cbb-109">方法</span><span class="sxs-lookup"><span data-stu-id="b1cbb-109">Method</span></span>                                   | <span data-ttu-id="b1cbb-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1cbb-110">Return Type</span></span>                              | <span data-ttu-id="b1cbb-111">说明</span><span class="sxs-lookup"><span data-stu-id="b1cbb-111">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="b1cbb-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="b1cbb-112">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="b1cbb-113">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b1cbb-113">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="b1cbb-114">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b1cbb-114">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="b1cbb-115">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="b1cbb-115">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="b1cbb-116">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="b1cbb-116">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="b1cbb-117">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="b1cbb-117">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="b1cbb-118">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="b1cbb-118">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="b1cbb-119">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="b1cbb-119">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="b1cbb-120">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="b1cbb-120">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="b1cbb-121">按活动类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="b1cbb-121">Get the number of users by activity type.</span></span> <span data-ttu-id="b1cbb-122">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="b1cbb-122">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
