---
title: Skype for Business 组织者活动报表
description: Skype for Business 组织者活动报表可用于获取整个组织中组织会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: d77addaee5acd610979d50ab308a04dbb96a06f4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533657"
---
# <a name="skype-for-business-organizer-activity-reports"></a><span data-ttu-id="cca56-104">Skype for Business 组织者活动报表</span><span class="sxs-lookup"><span data-stu-id="cca56-104">Skype for Business organizer activity reports</span></span>

<span data-ttu-id="cca56-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cca56-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cca56-106">Skype for Business 组织者活动报表可用于获取整个组织中组织会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cca56-106">You can use the Skype for Business organizer activity reports to get details on organized conferences activity across your organization.</span></span> <span data-ttu-id="cca56-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="cca56-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="cca56-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="cca56-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="reports"></a><span data-ttu-id="cca56-109">报表</span><span class="sxs-lookup"><span data-stu-id="cca56-109">Reports</span></span>

| <span data-ttu-id="cca56-110">函数</span><span class="sxs-lookup"><span data-stu-id="cca56-110">Function</span></span>                                 | <span data-ttu-id="cca56-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="cca56-111">Return Type</span></span> | <span data-ttu-id="cca56-112">说明</span><span class="sxs-lookup"><span data-stu-id="cca56-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="cca56-113">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="cca56-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | <span data-ttu-id="cca56-114">Stream</span><span class="sxs-lookup"><span data-stu-id="cca56-114">Stream</span></span>      | <span data-ttu-id="cca56-115">获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="cca56-115">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="cca56-116">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="cca56-116">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="cca56-117">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="cca56-117">Get user counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | <span data-ttu-id="cca56-118">Stream</span><span class="sxs-lookup"><span data-stu-id="cca56-118">Stream</span></span>      | <span data-ttu-id="cca56-119">获取使用情况趋势，即组织中用户召开和组织的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="cca56-119">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="cca56-120">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="cca56-120">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="cca56-121">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="cca56-121">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | <span data-ttu-id="cca56-122">Stream</span><span class="sxs-lookup"><span data-stu-id="cca56-122">Stream</span></span>      | <span data-ttu-id="cca56-123">获取使用情况趋势，即组织中用户召开和组织的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="cca56-123">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="cca56-124">会议会话类型包括音频/视频和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="cca56-124">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span> |
