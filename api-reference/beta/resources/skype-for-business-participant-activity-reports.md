---
title: Skype for Business 参与者活动报表
description: 您可以在整个组织会议活动获取详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 31810a7ca5df52724089783efe208e5a28bf0cfb
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576743"
---
# <a name="skype-for-business-participant-activity-reports"></a><span data-ttu-id="baeae-104">Skype for Business 参与者活动报表</span><span class="sxs-lookup"><span data-stu-id="baeae-104">Skype for Business participant activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baeae-105">您可以在整个组织会议活动获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="baeae-105">You can get details on conferencing activity across your organization.</span></span> <span data-ttu-id="baeae-106">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="baeae-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="baeae-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="baeae-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="reports"></a><span data-ttu-id="baeae-108">报表</span><span class="sxs-lookup"><span data-stu-id="baeae-108">Reports</span></span>

| <span data-ttu-id="baeae-109">函数</span><span class="sxs-lookup"><span data-stu-id="baeae-109">Function</span></span>                                 | <span data-ttu-id="baeae-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="baeae-110">CSV return type</span></span> | <span data-ttu-id="baeae-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="baeae-111">JSON return type</span></span>                         | <span data-ttu-id="baeae-112">说明</span><span class="sxs-lookup"><span data-stu-id="baeae-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="baeae-113">获取活动数</span><span class="sxs-lookup"><span data-stu-id="baeae-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="baeae-114">Stream</span><span class="sxs-lookup"><span data-stu-id="baeae-114">Stream</span></span>          | [<span data-ttu-id="baeae-115">skypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="baeae-115">skypeForBusinessParticipantActivityCounts</span></span>](../resources/skypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="baeae-116">获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="baeae-116">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="baeae-117">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="baeae-117">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="baeae-118">获取用户数</span><span class="sxs-lookup"><span data-stu-id="baeae-118">Get user counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="baeae-119">Stream</span><span class="sxs-lookup"><span data-stu-id="baeae-119">Stream</span></span>          | [<span data-ttu-id="baeae-120">skypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="baeae-120">skypeForBusinessParticipantActivityUserCounts</span></span>](../resources/skypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="baeae-121">获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="baeae-121">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="baeae-122">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="baeae-122">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="baeae-123">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="baeae-123">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="baeae-124">Stream</span><span class="sxs-lookup"><span data-stu-id="baeae-124">Stream</span></span>          | [<span data-ttu-id="baeae-125">skypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="baeae-125">skypeForBusinessParticipantActivityMinuteCounts</span></span>](../resources/skypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="baeae-126">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="baeae-126">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="baeae-127">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="baeae-127">Types of conference sessions include audio/video.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-participant-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
