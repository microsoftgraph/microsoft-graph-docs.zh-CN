---
title: Skype for Business 活动报表
description: Skype for Business 活动报表可用于获取整个组织中活动的详细信息。 这些详细信息有助于为组织调查、计划和制定其他业务决策。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 953c62e5747176c7eace8c8ee4baa82d0d48d6d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533670"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="e6cc2-104">Skype for Business 活动报告</span><span class="sxs-lookup"><span data-stu-id="e6cc2-104">Skype for Business activity reports</span></span>

<span data-ttu-id="e6cc2-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6cc2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6cc2-106">Skype for Business 活动报表可用于获取整个组织中活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e6cc2-106">You can use the Skype for Business activity reports to get details on activity across your organization.</span></span> <span data-ttu-id="e6cc2-107">这些详细信息有助于为组织调查、计划和做出其他业务决策。</span><span class="sxs-lookup"><span data-stu-id="e6cc2-107">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="e6cc2-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="e6cc2-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="e6cc2-109">报表</span><span class="sxs-lookup"><span data-stu-id="e6cc2-109">Reports</span></span>

| <span data-ttu-id="e6cc2-110">函数</span><span class="sxs-lookup"><span data-stu-id="e6cc2-110">Function</span></span>                                 | <span data-ttu-id="e6cc2-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="e6cc2-111">Return Type</span></span> | <span data-ttu-id="e6cc2-112">说明</span><span class="sxs-lookup"><span data-stu-id="e6cc2-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="e6cc2-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="e6cc2-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="e6cc2-114">Stream</span><span class="sxs-lookup"><span data-stu-id="e6cc2-114">Stream</span></span>      | <span data-ttu-id="e6cc2-115">获取用户执行的 Skype for Business 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e6cc2-115">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="e6cc2-116">获取活动数</span><span class="sxs-lookup"><span data-stu-id="e6cc2-116">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="e6cc2-117">Stream</span><span class="sxs-lookup"><span data-stu-id="e6cc2-117">Stream</span></span>      | <span data-ttu-id="e6cc2-118">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="e6cc2-118">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="e6cc2-119">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="e6cc2-119">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="e6cc2-120">获取用户数</span><span class="sxs-lookup"><span data-stu-id="e6cc2-120">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="e6cc2-121">Stream</span><span class="sxs-lookup"><span data-stu-id="e6cc2-121">Stream</span></span>      | <span data-ttu-id="e6cc2-122">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="e6cc2-122">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="e6cc2-123">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="e6cc2-123">The report also includes the number of peer-to-peer sessions.</span></span> |
