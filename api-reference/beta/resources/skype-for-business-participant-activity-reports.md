---
title: Skype for Business 参与者活动报表
description: 你可以在组织中获取有关会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 41cfa3d848cf5dcf6537a94b5adab0cf649dc21f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997639"
---
# <a name="skype-for-business-participant-activity-reports"></a><span data-ttu-id="d4aa2-104">Skype for Business 参与者活动报表</span><span class="sxs-lookup"><span data-stu-id="d4aa2-104">Skype for Business participant activity reports</span></span>

<span data-ttu-id="d4aa2-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4aa2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4aa2-106">你可以在组织中获取有关会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d4aa2-106">You can get details on conferencing activity across your organization.</span></span> <span data-ttu-id="d4aa2-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="d4aa2-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="d4aa2-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 reports-Skype For business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="d4aa2-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="reports"></a><span data-ttu-id="d4aa2-109">报表</span><span class="sxs-lookup"><span data-stu-id="d4aa2-109">Reports</span></span>

| <span data-ttu-id="d4aa2-110">函数</span><span class="sxs-lookup"><span data-stu-id="d4aa2-110">Function</span></span>                                 | <span data-ttu-id="d4aa2-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="d4aa2-111">CSV return type</span></span> | <span data-ttu-id="d4aa2-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="d4aa2-112">JSON return type</span></span>                         | <span data-ttu-id="d4aa2-113">说明</span><span class="sxs-lookup"><span data-stu-id="d4aa2-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="d4aa2-114">获取活动数</span><span class="sxs-lookup"><span data-stu-id="d4aa2-114">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="d4aa2-115">Stream</span><span class="sxs-lookup"><span data-stu-id="d4aa2-115">Stream</span></span>          | [<span data-ttu-id="d4aa2-116">skypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="d4aa2-116">skypeForBusinessParticipantActivityCounts</span></span>](../resources/skypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="d4aa2-117">获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="d4aa2-117">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="d4aa2-118">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="d4aa2-118">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="d4aa2-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="d4aa2-119">Get user counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="d4aa2-120">Stream</span><span class="sxs-lookup"><span data-stu-id="d4aa2-120">Stream</span></span>          | [<span data-ttu-id="d4aa2-121">skypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="d4aa2-121">skypeForBusinessParticipantActivityUserCounts</span></span>](../resources/skypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="d4aa2-122">获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="d4aa2-122">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="d4aa2-123">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="d4aa2-123">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="d4aa2-124">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="d4aa2-124">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="d4aa2-125">Stream</span><span class="sxs-lookup"><span data-stu-id="d4aa2-125">Stream</span></span>          | [<span data-ttu-id="d4aa2-126">skypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="d4aa2-126">skypeForBusinessParticipantActivityMinuteCounts</span></span>](../resources/skypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="d4aa2-127">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="d4aa2-127">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="d4aa2-128">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="d4aa2-128">Types of conference sessions include audio/video.</span></span> |


