---
title: Skype for Business 组织者活动报表
description: Skype for Business 组织者活动报表可用于获取整个组织中组织会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 24e57eec7a7ff7c401028e8798d06ab26d038991
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897958"
---
# <a name="skype-for-business-organizer-activity-reports"></a><span data-ttu-id="dfb60-104">Skype for Business 组织者活动报表</span><span class="sxs-lookup"><span data-stu-id="dfb60-104">Skype for Business organizer activity reports</span></span>

<span data-ttu-id="dfb60-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfb60-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfb60-106">Skype for Business 组织者活动报表可用于获取整个组织中组织会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dfb60-106">You can use the Skype for Business organizer activity reports to get details on organized conferences activity across your organization.</span></span> <span data-ttu-id="dfb60-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="dfb60-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="dfb60-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-Skype For business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="dfb60-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="reports"></a><span data-ttu-id="dfb60-109">报表</span><span class="sxs-lookup"><span data-stu-id="dfb60-109">Reports</span></span>

| <span data-ttu-id="dfb60-110">函数</span><span class="sxs-lookup"><span data-stu-id="dfb60-110">Function</span></span>                                 | <span data-ttu-id="dfb60-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="dfb60-111">Return Type</span></span> | <span data-ttu-id="dfb60-112">说明</span><span class="sxs-lookup"><span data-stu-id="dfb60-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="dfb60-113">获取活动数</span><span class="sxs-lookup"><span data-stu-id="dfb60-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | <span data-ttu-id="dfb60-114">Stream</span><span class="sxs-lookup"><span data-stu-id="dfb60-114">Stream</span></span>      | <span data-ttu-id="dfb60-115">获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="dfb60-115">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="dfb60-116">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="dfb60-116">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="dfb60-117">获取用户数</span><span class="sxs-lookup"><span data-stu-id="dfb60-117">Get user counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | <span data-ttu-id="dfb60-118">Stream</span><span class="sxs-lookup"><span data-stu-id="dfb60-118">Stream</span></span>      | <span data-ttu-id="dfb60-119">获取使用情况趋势，即组织中用户召开和组织的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="dfb60-119">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="dfb60-120">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="dfb60-120">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="dfb60-121">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="dfb60-121">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | <span data-ttu-id="dfb60-122">Stream</span><span class="sxs-lookup"><span data-stu-id="dfb60-122">Stream</span></span>      | <span data-ttu-id="dfb60-123">获取使用情况趋势，即组织中用户召开和组织的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="dfb60-123">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="dfb60-124">会议会话类型包括音频/视频和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="dfb60-124">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span> |
