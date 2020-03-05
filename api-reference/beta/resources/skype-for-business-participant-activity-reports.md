---
title: Skype for Business 参与者活动报表
description: 你可以在组织中获取有关会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 9ef31521125a7b4a8443002847ccf27cd8f265a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520469"
---
# <a name="skype-for-business-participant-activity-reports"></a><span data-ttu-id="1248c-104">Skype for Business 参与者活动报表</span><span class="sxs-lookup"><span data-stu-id="1248c-104">Skype for Business participant activity reports</span></span>

<span data-ttu-id="1248c-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1248c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1248c-106">你可以在组织中获取有关会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1248c-106">You can get details on conferencing activity across your organization.</span></span> <span data-ttu-id="1248c-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="1248c-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="1248c-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="1248c-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="reports"></a><span data-ttu-id="1248c-109">报表</span><span class="sxs-lookup"><span data-stu-id="1248c-109">Reports</span></span>

| <span data-ttu-id="1248c-110">函数</span><span class="sxs-lookup"><span data-stu-id="1248c-110">Function</span></span>                                 | <span data-ttu-id="1248c-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="1248c-111">CSV return type</span></span> | <span data-ttu-id="1248c-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="1248c-112">JSON return type</span></span>                         | <span data-ttu-id="1248c-113">说明</span><span class="sxs-lookup"><span data-stu-id="1248c-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="1248c-114">获取活动数</span><span class="sxs-lookup"><span data-stu-id="1248c-114">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="1248c-115">Stream</span><span class="sxs-lookup"><span data-stu-id="1248c-115">Stream</span></span>          | [<span data-ttu-id="1248c-116">skypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="1248c-116">skypeForBusinessParticipantActivityCounts</span></span>](../resources/skypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="1248c-117">获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="1248c-117">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="1248c-118">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="1248c-118">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="1248c-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="1248c-119">Get user counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="1248c-120">Stream</span><span class="sxs-lookup"><span data-stu-id="1248c-120">Stream</span></span>          | [<span data-ttu-id="1248c-121">skypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="1248c-121">skypeForBusinessParticipantActivityUserCounts</span></span>](../resources/skypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="1248c-122">获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="1248c-122">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="1248c-123">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="1248c-123">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="1248c-124">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="1248c-124">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="1248c-125">Stream</span><span class="sxs-lookup"><span data-stu-id="1248c-125">Stream</span></span>          | [<span data-ttu-id="1248c-126">skypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="1248c-126">skypeForBusinessParticipantActivityMinuteCounts</span></span>](../resources/skypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="1248c-127">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="1248c-127">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="1248c-128">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="1248c-128">Types of conference sessions include audio/video.</span></span> |
