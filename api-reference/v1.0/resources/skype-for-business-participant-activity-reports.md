---
title: Skype for Business 参与者活动报表
description: Skype for Business 参与者活动报表可用于获取整个组织中参与会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5cfb5412cb2be03dcd3463714346e5f23ca6a5cf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576442"
---
# <a name="skype-for-business-participant-activity-reports"></a><span data-ttu-id="b08e8-104">Skype for Business 参与者活动报表</span><span class="sxs-lookup"><span data-stu-id="b08e8-104">Skype for Business participant activity reports</span></span>

<span data-ttu-id="b08e8-105">Skype for Business 参与者活动报表可用于获取整个组织中参与会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b08e8-105">You can use the Skype for Business participant activity reports to get details on conferencing activity across your organization.</span></span> <span data-ttu-id="b08e8-106">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="b08e8-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="b08e8-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="b08e8-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="reports"></a><span data-ttu-id="b08e8-108">报表</span><span class="sxs-lookup"><span data-stu-id="b08e8-108">Reports</span></span>

| <span data-ttu-id="b08e8-109">函数</span><span class="sxs-lookup"><span data-stu-id="b08e8-109">Function</span></span>                                 | <span data-ttu-id="b08e8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b08e8-110">Return Type</span></span> | <span data-ttu-id="b08e8-111">说明</span><span class="sxs-lookup"><span data-stu-id="b08e8-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="b08e8-112">获取活动数</span><span class="sxs-lookup"><span data-stu-id="b08e8-112">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="b08e8-113">Stream</span><span class="sxs-lookup"><span data-stu-id="b08e8-113">Stream</span></span>      | <span data-ttu-id="b08e8-114">获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="b08e8-114">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="b08e8-115">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="b08e8-115">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="b08e8-116">获取用户数</span><span class="sxs-lookup"><span data-stu-id="b08e8-116">Get user counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="b08e8-117">Stream</span><span class="sxs-lookup"><span data-stu-id="b08e8-117">Stream</span></span>      | <span data-ttu-id="b08e8-118">获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="b08e8-118">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="b08e8-119">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="b08e8-119">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="b08e8-120">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="b08e8-120">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="b08e8-121">Stream</span><span class="sxs-lookup"><span data-stu-id="b08e8-121">Stream</span></span>      | <span data-ttu-id="b08e8-122">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="b08e8-122">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="b08e8-123">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="b08e8-123">Types of conference sessions include audio/video.</span></span> |
