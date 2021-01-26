---
title: Skype for Business 活动报表
description: Skype for Business 活动报表可用于获取整个组织中活动的详细信息。 这些详细信息有助于为组织调查、计划和制定其他业务决策。
localization_priority: Priority
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 1394ea6008d2514e091fa773db632f80d56e4b6e
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980946"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="7398e-104">Skype for Business 活动报告</span><span class="sxs-lookup"><span data-stu-id="7398e-104">Skype for Business activity reports</span></span>

<span data-ttu-id="7398e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7398e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7398e-106">Skype for Business 活动报表可用于获取整个组织中活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7398e-106">You can use the Skype for Business activity reports to get details on activity across your organization.</span></span> <span data-ttu-id="7398e-107">这些详细信息有助于为组织调查、计划和制定其他业务决策。</span><span class="sxs-lookup"><span data-stu-id="7398e-107">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="7398e-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="7398e-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="7398e-109">报告</span><span class="sxs-lookup"><span data-stu-id="7398e-109">Reports</span></span>

| <span data-ttu-id="7398e-110">函数</span><span class="sxs-lookup"><span data-stu-id="7398e-110">Function</span></span>                                 | <span data-ttu-id="7398e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7398e-111">Return Type</span></span> | <span data-ttu-id="7398e-112">说明</span><span class="sxs-lookup"><span data-stu-id="7398e-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="7398e-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="7398e-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="7398e-114">Stream</span><span class="sxs-lookup"><span data-stu-id="7398e-114">Stream</span></span>      | <span data-ttu-id="7398e-115">获取用户执行的 Skype for Business 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7398e-115">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="7398e-116">获取活动数</span><span class="sxs-lookup"><span data-stu-id="7398e-116">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="7398e-117">Stream</span><span class="sxs-lookup"><span data-stu-id="7398e-117">Stream</span></span>      | <span data-ttu-id="7398e-118">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="7398e-118">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="7398e-119">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="7398e-119">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="7398e-120">获取用户数</span><span class="sxs-lookup"><span data-stu-id="7398e-120">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="7398e-121">Stream</span><span class="sxs-lookup"><span data-stu-id="7398e-121">Stream</span></span>      | <span data-ttu-id="7398e-122">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="7398e-122">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="7398e-123">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="7398e-123">The report also includes the number of peer-to-peer sessions.</span></span> |

