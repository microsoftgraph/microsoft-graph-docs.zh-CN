---
title: Skype for Business 参与者活动报表
description: Skype for Business 参与者活动报表可用于获取整个组织中参与会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 2b6596e7478632da773dc8839dafd722587e417d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034088"
---
# <a name="skype-for-business-participant-activity-reports"></a><span data-ttu-id="735d2-104">Skype for Business 参与者活动报表</span><span class="sxs-lookup"><span data-stu-id="735d2-104">Skype for Business participant activity reports</span></span>

<span data-ttu-id="735d2-105">Skype for Business 参与者活动报表可用于获取整个组织中参与会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="735d2-105">You can use the Skype for Business participant activity reports to get details on conferencing activity across your organization.</span></span> <span data-ttu-id="735d2-106">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="735d2-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="735d2-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="735d2-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="reports"></a><span data-ttu-id="735d2-108">报表</span><span class="sxs-lookup"><span data-stu-id="735d2-108">Reports</span></span>

| <span data-ttu-id="735d2-109">函数</span><span class="sxs-lookup"><span data-stu-id="735d2-109">Function</span></span>                                 | <span data-ttu-id="735d2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="735d2-110">Return Type</span></span> | <span data-ttu-id="735d2-111">说明</span><span class="sxs-lookup"><span data-stu-id="735d2-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="735d2-112">获取活动数</span><span class="sxs-lookup"><span data-stu-id="735d2-112">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="735d2-113">流</span><span class="sxs-lookup"><span data-stu-id="735d2-113">Stream</span></span>      | <span data-ttu-id="735d2-114">获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="735d2-114">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="735d2-115">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="735d2-115">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="735d2-116">获取用户数</span><span class="sxs-lookup"><span data-stu-id="735d2-116">Get user counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="735d2-117">Stream</span><span class="sxs-lookup"><span data-stu-id="735d2-117">Stream</span></span>      | <span data-ttu-id="735d2-118">获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="735d2-118">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="735d2-119">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="735d2-119">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="735d2-120">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="735d2-120">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="735d2-121">Stream</span><span class="sxs-lookup"><span data-stu-id="735d2-121">Stream</span></span>      | <span data-ttu-id="735d2-122">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="735d2-122">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="735d2-123">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="735d2-123">Types of conference sessions include audio/video.</span></span> |
