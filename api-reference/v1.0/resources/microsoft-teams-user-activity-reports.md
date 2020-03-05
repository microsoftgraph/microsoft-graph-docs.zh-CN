---
title: Microsoft Teams 用户活动报告
description: 使用 Microsoft Teams 活动报告了解组织中的 Microsoft Teams 用户活动。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: adde0eecbfe468b5eac45bf0c0d496d430947284
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447386"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="1d1ca-103">Microsoft Teams 用户活动报告</span><span class="sxs-lookup"><span data-stu-id="1d1ca-103">Microsoft Teams user activity reports</span></span>

<span data-ttu-id="1d1ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d1ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d1ca-105">使用 Microsoft Teams 活动报告了解组织中的 Microsoft Teams 用户活动。</span><span class="sxs-lookup"><span data-stu-id="1d1ca-105">Use the Microsoft Teams activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="1d1ca-106">方法</span><span class="sxs-lookup"><span data-stu-id="1d1ca-106">Methods</span></span>

| <span data-ttu-id="1d1ca-107">方法</span><span class="sxs-lookup"><span data-stu-id="1d1ca-107">Method</span></span>                                   | <span data-ttu-id="1d1ca-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d1ca-108">Return Type</span></span> | <span data-ttu-id="1d1ca-109">说明</span><span class="sxs-lookup"><span data-stu-id="1d1ca-109">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="1d1ca-110">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="1d1ca-110">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | <span data-ttu-id="1d1ca-111">Stream</span><span class="sxs-lookup"><span data-stu-id="1d1ca-111">Stream</span></span>      | <span data-ttu-id="1d1ca-112">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1d1ca-112">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="1d1ca-113">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="1d1ca-113">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | <span data-ttu-id="1d1ca-114">Stream</span><span class="sxs-lookup"><span data-stu-id="1d1ca-114">Stream</span></span>      | <span data-ttu-id="1d1ca-115">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="1d1ca-115">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="1d1ca-116">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="1d1ca-116">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="1d1ca-117">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="1d1ca-117">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | <span data-ttu-id="1d1ca-118">Stream</span><span class="sxs-lookup"><span data-stu-id="1d1ca-118">Stream</span></span>      | <span data-ttu-id="1d1ca-119">按活动类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="1d1ca-119">Get the number of users by activity type.</span></span> <span data-ttu-id="1d1ca-120">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="1d1ca-120">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
