---
title: Skype for Business 组织者活动报表
description: 您可以获取有关组织中组织的会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 6e52d37322bb5dbd67faac0b9b51f6e8afc3aeb2
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983060"
---
# <a name="skype-for-business-organizer-activity-reports"></a><span data-ttu-id="f21fe-104">Skype for Business 组织者活动报表</span><span class="sxs-lookup"><span data-stu-id="f21fe-104">Skype for Business organizer activity reports</span></span>

<span data-ttu-id="f21fe-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f21fe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f21fe-106">您可以获取有关组织中组织的会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f21fe-106">You can get details on organized conferences activity across your organization.</span></span> <span data-ttu-id="f21fe-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="f21fe-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="f21fe-108">**注意：** 有关不同报告视图和名称的详细信息，请参阅 [Microsoft 365 报告 - Skype for Business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="f21fe-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="reports"></a><span data-ttu-id="f21fe-109">报告</span><span class="sxs-lookup"><span data-stu-id="f21fe-109">Reports</span></span>

| <span data-ttu-id="f21fe-110">函数</span><span class="sxs-lookup"><span data-stu-id="f21fe-110">Function</span></span>                                 | <span data-ttu-id="f21fe-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="f21fe-111">CSV return type</span></span> | <span data-ttu-id="f21fe-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="f21fe-112">JSON return type</span></span>                         | <span data-ttu-id="f21fe-113">说明</span><span class="sxs-lookup"><span data-stu-id="f21fe-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="f21fe-114">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="f21fe-114">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | <span data-ttu-id="f21fe-115">Stream</span><span class="sxs-lookup"><span data-stu-id="f21fe-115">Stream</span></span>          | [<span data-ttu-id="f21fe-116">skypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="f21fe-116">skypeForBusinessOrganizerActivityCounts</span></span>](../resources/skypeforbusinessorganizeractivitycounts.md) | <span data-ttu-id="f21fe-117">获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="f21fe-117">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="f21fe-118">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="f21fe-118">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="f21fe-119">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="f21fe-119">Get user counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | <span data-ttu-id="f21fe-120">Stream</span><span class="sxs-lookup"><span data-stu-id="f21fe-120">Stream</span></span>          | [<span data-ttu-id="f21fe-121">skypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="f21fe-121">skypeForBusinessOrganizerActivityUserCounts</span></span>](../resources/skypeforbusinessorganizeractivityusercounts.md) | <span data-ttu-id="f21fe-122">获取使用情况趋势，即组织中用户召开和组织的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="f21fe-122">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="f21fe-123">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="f21fe-123">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="f21fe-124">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="f21fe-124">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | <span data-ttu-id="f21fe-125">Stream</span><span class="sxs-lookup"><span data-stu-id="f21fe-125">Stream</span></span>          | [<span data-ttu-id="f21fe-126">skypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="f21fe-126">skypeForBusinessOrganizerActivityMinuteCounts</span></span>](../resources/skypeforbusinessorganizeractivityminutecounts.md) | <span data-ttu-id="f21fe-127">获取使用情况趋势，即组织中用户召开和组织的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="f21fe-127">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="f21fe-128">会议会话类型包括音频/视频和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="f21fe-128">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span> |


