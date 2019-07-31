---
title: Microsoft Teams 用户活动报告
description: 使用 Microsoft 团队用户活动报告可深入了解组织中的 Microsoft 团队用户活动。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: ca8d1f772744b33aa5fee60fc3b843bf60b0be9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009634"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="91d91-103">Microsoft Teams 用户活动报告</span><span class="sxs-lookup"><span data-stu-id="91d91-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91d91-104">使用 Microsoft 团队用户活动报告可深入了解组织中的 Microsoft 团队用户活动。</span><span class="sxs-lookup"><span data-stu-id="91d91-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="91d91-105">方法</span><span class="sxs-lookup"><span data-stu-id="91d91-105">Methods</span></span>

| <span data-ttu-id="91d91-106">方法</span><span class="sxs-lookup"><span data-stu-id="91d91-106">Method</span></span>                                   | <span data-ttu-id="91d91-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="91d91-107">Return Type</span></span>                              | <span data-ttu-id="91d91-108">说明</span><span class="sxs-lookup"><span data-stu-id="91d91-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="91d91-109">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="91d91-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="91d91-110">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="91d91-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="91d91-111">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="91d91-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="91d91-112">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="91d91-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="91d91-113">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="91d91-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="91d91-114">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="91d91-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="91d91-115">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="91d91-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="91d91-116">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="91d91-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="91d91-117">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="91d91-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="91d91-118">按活动类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="91d91-118">Get the number of users by activity type.</span></span> <span data-ttu-id="91d91-119">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="91d91-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
