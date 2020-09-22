---
title: Skype for Business 组织者活动报表
description: 你可以在组织中获取有关组织的会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 9f239845c96da851c72a7b3503d68dfd85edffe0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997646"
---
# <a name="skype-for-business-organizer-activity-reports"></a><span data-ttu-id="e69f9-104">Skype for Business 组织者活动报表</span><span class="sxs-lookup"><span data-stu-id="e69f9-104">Skype for Business organizer activity reports</span></span>

<span data-ttu-id="e69f9-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e69f9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e69f9-106">你可以在组织中获取有关组织的会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e69f9-106">You can get details on organized conferences activity across your organization.</span></span> <span data-ttu-id="e69f9-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="e69f9-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="e69f9-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 reports-Skype For business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="e69f9-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="reports"></a><span data-ttu-id="e69f9-109">报表</span><span class="sxs-lookup"><span data-stu-id="e69f9-109">Reports</span></span>

| <span data-ttu-id="e69f9-110">函数</span><span class="sxs-lookup"><span data-stu-id="e69f9-110">Function</span></span>                                 | <span data-ttu-id="e69f9-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="e69f9-111">CSV return type</span></span> | <span data-ttu-id="e69f9-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="e69f9-112">JSON return type</span></span>                         | <span data-ttu-id="e69f9-113">说明</span><span class="sxs-lookup"><span data-stu-id="e69f9-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="e69f9-114">获取活动数</span><span class="sxs-lookup"><span data-stu-id="e69f9-114">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | <span data-ttu-id="e69f9-115">Stream</span><span class="sxs-lookup"><span data-stu-id="e69f9-115">Stream</span></span>          | [<span data-ttu-id="e69f9-116">skypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="e69f9-116">skypeForBusinessOrganizerActivityCounts</span></span>](../resources/skypeforbusinessorganizeractivitycounts.md) | <span data-ttu-id="e69f9-117">获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="e69f9-117">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="e69f9-118">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="e69f9-118">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="e69f9-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="e69f9-119">Get user counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | <span data-ttu-id="e69f9-120">Stream</span><span class="sxs-lookup"><span data-stu-id="e69f9-120">Stream</span></span>          | [<span data-ttu-id="e69f9-121">skypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="e69f9-121">skypeForBusinessOrganizerActivityUserCounts</span></span>](../resources/skypeforbusinessorganizeractivityusercounts.md) | <span data-ttu-id="e69f9-122">获取使用情况趋势，即组织中用户召开和组织的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="e69f9-122">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="e69f9-123">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="e69f9-123">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="e69f9-124">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="e69f9-124">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | <span data-ttu-id="e69f9-125">Stream</span><span class="sxs-lookup"><span data-stu-id="e69f9-125">Stream</span></span>          | [<span data-ttu-id="e69f9-126">skypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="e69f9-126">skypeForBusinessOrganizerActivityMinuteCounts</span></span>](../resources/skypeforbusinessorganizeractivityminutecounts.md) | <span data-ttu-id="e69f9-127">获取使用情况趋势，即组织中用户召开和组织的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="e69f9-127">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="e69f9-128">会议会话类型包括音频/视频和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="e69f9-128">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span> |


