---
title: Skype for Business 活动报表
description: 你可以在组织中获取活动的详细信息。 这些详细信息有助于为组织调查、计划和制定其他业务决策。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: fcd23201732f1e0988853ae33cf08a24295a2647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008241"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="2846e-104">Skype for Business 活动报告</span><span class="sxs-lookup"><span data-stu-id="2846e-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2846e-105">你可以在组织中获取活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2846e-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="2846e-106">这些详细信息有助于为组织调查、计划和做出其他业务决策。</span><span class="sxs-lookup"><span data-stu-id="2846e-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="2846e-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="2846e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="2846e-108">报表</span><span class="sxs-lookup"><span data-stu-id="2846e-108">Reports</span></span>

| <span data-ttu-id="2846e-109">函数</span><span class="sxs-lookup"><span data-stu-id="2846e-109">Function</span></span>                                 | <span data-ttu-id="2846e-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="2846e-110">CSV return type</span></span> | <span data-ttu-id="2846e-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="2846e-111">JSON return type</span></span>                         | <span data-ttu-id="2846e-112">说明</span><span class="sxs-lookup"><span data-stu-id="2846e-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="2846e-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="2846e-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="2846e-114">流</span><span class="sxs-lookup"><span data-stu-id="2846e-114">Stream</span></span>          | [<span data-ttu-id="2846e-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="2846e-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="2846e-116">获取用户执行的 Skype for Business 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2846e-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="2846e-117">获取活动数</span><span class="sxs-lookup"><span data-stu-id="2846e-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="2846e-118">Stream</span><span class="sxs-lookup"><span data-stu-id="2846e-118">Stream</span></span>          | [<span data-ttu-id="2846e-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="2846e-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="2846e-120">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="2846e-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="2846e-121">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="2846e-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="2846e-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="2846e-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="2846e-123">Stream</span><span class="sxs-lookup"><span data-stu-id="2846e-123">Stream</span></span>          | [<span data-ttu-id="2846e-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="2846e-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="2846e-125">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="2846e-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="2846e-126">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="2846e-126">The report also includes the number of peer-to-peer sessions.</span></span> |
