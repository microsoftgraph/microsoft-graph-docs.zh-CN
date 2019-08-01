---
title: Skype for Business 组织者活动报表
description: Skype for Business 组织者活动报表可用于获取整个组织中组织会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: d914e1af08a2afc85a1d263b1c55098f6d8457fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034102"
---
# <a name="skype-for-business-organizer-activity-reports"></a><span data-ttu-id="e1154-104">Skype for Business 组织者活动报表</span><span class="sxs-lookup"><span data-stu-id="e1154-104">Skype for Business organizer activity reports</span></span>

<span data-ttu-id="e1154-105">Skype for Business 组织者活动报表可用于获取整个组织中组织会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e1154-105">You can use the Skype for Business organizer activity reports to get details on organized conferences activity across your organization.</span></span> <span data-ttu-id="e1154-106">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="e1154-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="e1154-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="e1154-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="reports"></a><span data-ttu-id="e1154-108">报表</span><span class="sxs-lookup"><span data-stu-id="e1154-108">Reports</span></span>

| <span data-ttu-id="e1154-109">函数</span><span class="sxs-lookup"><span data-stu-id="e1154-109">Function</span></span>                                 | <span data-ttu-id="e1154-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e1154-110">Return Type</span></span> | <span data-ttu-id="e1154-111">说明</span><span class="sxs-lookup"><span data-stu-id="e1154-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="e1154-112">获取活动数</span><span class="sxs-lookup"><span data-stu-id="e1154-112">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | <span data-ttu-id="e1154-113">流</span><span class="sxs-lookup"><span data-stu-id="e1154-113">Stream</span></span>      | <span data-ttu-id="e1154-114">获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="e1154-114">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="e1154-115">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="e1154-115">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="e1154-116">获取用户数</span><span class="sxs-lookup"><span data-stu-id="e1154-116">Get user counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | <span data-ttu-id="e1154-117">Stream</span><span class="sxs-lookup"><span data-stu-id="e1154-117">Stream</span></span>      | <span data-ttu-id="e1154-118">获取使用情况趋势，即组织中用户召开和组织的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="e1154-118">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="e1154-119">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="e1154-119">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="e1154-120">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="e1154-120">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | <span data-ttu-id="e1154-121">Stream</span><span class="sxs-lookup"><span data-stu-id="e1154-121">Stream</span></span>      | <span data-ttu-id="e1154-122">获取使用情况趋势，即组织中用户召开和组织的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="e1154-122">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="e1154-123">会议会话类型包括音频/视频和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="e1154-123">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span> |
