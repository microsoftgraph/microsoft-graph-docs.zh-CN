---
title: Microsoft Teams 用户活动报告
description: 使用 Microsoft 团队用户活动报告您的组织中获取的 Microsoft 团队用户活动见解。
ms.openlocfilehash: 26af58ad88541fb4e9e0f64159505846bfe90bb5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042383"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="d1da8-103">Microsoft Teams 用户活动报告</span><span class="sxs-lookup"><span data-stu-id="d1da8-103">Microsoft Teams user activity reports</span></span>

> <span data-ttu-id="d1da8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d1da8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1da8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d1da8-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="d1da8-106">在 Microsoft Graph 中国由 21Vianet 不支持这些 Api。</span><span class="sxs-lookup"><span data-stu-id="d1da8-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="d1da8-107">使用 Microsoft 团队用户活动报告您的组织中获取的 Microsoft 团队用户活动见解。</span><span class="sxs-lookup"><span data-stu-id="d1da8-107">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="d1da8-108">方法</span><span class="sxs-lookup"><span data-stu-id="d1da8-108">Methods</span></span>

| <span data-ttu-id="d1da8-109">方法</span><span class="sxs-lookup"><span data-stu-id="d1da8-109">Method</span></span>                                   | <span data-ttu-id="d1da8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d1da8-110">Return Type</span></span>                              | <span data-ttu-id="d1da8-111">说明</span><span class="sxs-lookup"><span data-stu-id="d1da8-111">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="d1da8-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="d1da8-112">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="d1da8-113">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d1da8-113">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="d1da8-114">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d1da8-114">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="d1da8-115">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="d1da8-115">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="d1da8-116">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="d1da8-116">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="d1da8-117">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="d1da8-117">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="d1da8-118">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="d1da8-118">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="d1da8-119">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="d1da8-119">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="d1da8-120">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="d1da8-120">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="d1da8-121">按活动类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="d1da8-121">Get the number of users by activity type.</span></span> <span data-ttu-id="d1da8-122">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="d1da8-122">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
