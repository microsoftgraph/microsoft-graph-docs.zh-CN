---
title: Skype for Business 活动报表
description: 你可以获取有关整个组织活动的详细信息。 这些详细信息有助于为组织调查、计划和制定其他业务决策。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 0fe3236fc8c4f29357e2ae3fae45c80969c353db
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980645"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="a2d6c-104">Skype for Business 活动报告</span><span class="sxs-lookup"><span data-stu-id="a2d6c-104">Skype for Business activity reports</span></span>

<span data-ttu-id="a2d6c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2d6c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2d6c-106">你可以获取有关整个组织活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a2d6c-106">You can get details on activity across your organization.</span></span> <span data-ttu-id="a2d6c-107">这些详细信息有助于为组织调查、计划和制定其他业务决策。</span><span class="sxs-lookup"><span data-stu-id="a2d6c-107">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="a2d6c-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="a2d6c-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="a2d6c-109">报告</span><span class="sxs-lookup"><span data-stu-id="a2d6c-109">Reports</span></span>

| <span data-ttu-id="a2d6c-110">函数</span><span class="sxs-lookup"><span data-stu-id="a2d6c-110">Function</span></span>                                 | <span data-ttu-id="a2d6c-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="a2d6c-111">CSV return type</span></span> | <span data-ttu-id="a2d6c-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="a2d6c-112">JSON return type</span></span>                         | <span data-ttu-id="a2d6c-113">说明</span><span class="sxs-lookup"><span data-stu-id="a2d6c-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="a2d6c-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="a2d6c-114">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="a2d6c-115">Stream</span><span class="sxs-lookup"><span data-stu-id="a2d6c-115">Stream</span></span>          | [<span data-ttu-id="a2d6c-116">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="a2d6c-116">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="a2d6c-117">获取用户执行的 Skype for Business 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a2d6c-117">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="a2d6c-118">获取活动数</span><span class="sxs-lookup"><span data-stu-id="a2d6c-118">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="a2d6c-119">Stream</span><span class="sxs-lookup"><span data-stu-id="a2d6c-119">Stream</span></span>          | [<span data-ttu-id="a2d6c-120">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="a2d6c-120">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="a2d6c-121">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="a2d6c-121">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="a2d6c-122">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="a2d6c-122">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="a2d6c-123">获取用户数</span><span class="sxs-lookup"><span data-stu-id="a2d6c-123">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="a2d6c-124">Stream</span><span class="sxs-lookup"><span data-stu-id="a2d6c-124">Stream</span></span>          | [<span data-ttu-id="a2d6c-125">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="a2d6c-125">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="a2d6c-126">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="a2d6c-126">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="a2d6c-127">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="a2d6c-127">The report also includes the number of peer-to-peer sessions.</span></span> |


