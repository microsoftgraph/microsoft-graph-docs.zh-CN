---
title: Skype for Business 参与者活动报表
description: Skype for Business 参与者活动报表可用于获取整个组织中参与会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: ee077a84f010058cf398a271680698e5bc2c327f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897951"
---
# <a name="skype-for-business-participant-activity-reports"></a><span data-ttu-id="f990a-104">Skype for Business 参与者活动报表</span><span class="sxs-lookup"><span data-stu-id="f990a-104">Skype for Business participant activity reports</span></span>

<span data-ttu-id="f990a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f990a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f990a-106">Skype for Business 参与者活动报表可用于获取整个组织中参与会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f990a-106">You can use the Skype for Business participant activity reports to get details on conferencing activity across your organization.</span></span> <span data-ttu-id="f990a-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="f990a-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="f990a-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-Skype For business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="f990a-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="reports"></a><span data-ttu-id="f990a-109">报表</span><span class="sxs-lookup"><span data-stu-id="f990a-109">Reports</span></span>

| <span data-ttu-id="f990a-110">函数</span><span class="sxs-lookup"><span data-stu-id="f990a-110">Function</span></span>                                 | <span data-ttu-id="f990a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="f990a-111">Return Type</span></span> | <span data-ttu-id="f990a-112">说明</span><span class="sxs-lookup"><span data-stu-id="f990a-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="f990a-113">获取活动数</span><span class="sxs-lookup"><span data-stu-id="f990a-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="f990a-114">Stream</span><span class="sxs-lookup"><span data-stu-id="f990a-114">Stream</span></span>      | <span data-ttu-id="f990a-115">获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="f990a-115">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="f990a-116">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="f990a-116">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="f990a-117">获取用户数</span><span class="sxs-lookup"><span data-stu-id="f990a-117">Get user counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="f990a-118">Stream</span><span class="sxs-lookup"><span data-stu-id="f990a-118">Stream</span></span>      | <span data-ttu-id="f990a-119">获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="f990a-119">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="f990a-120">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="f990a-120">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="f990a-121">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="f990a-121">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="f990a-122">Stream</span><span class="sxs-lookup"><span data-stu-id="f990a-122">Stream</span></span>      | <span data-ttu-id="f990a-123">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="f990a-123">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="f990a-124">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="f990a-124">Types of conference sessions include audio/video.</span></span> |
