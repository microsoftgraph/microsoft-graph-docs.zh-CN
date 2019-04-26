---
title: Skype for Business 参与者活动报表
description: 你可以在组织中获取有关会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 31810a7ca5df52724089783efe208e5a28bf0cfb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554861"
---
# <a name="skype-for-business-participant-activity-reports"></a><span data-ttu-id="40f54-104">Skype for Business 参与者活动报表</span><span class="sxs-lookup"><span data-stu-id="40f54-104">Skype for Business participant activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40f54-105">你可以在组织中获取有关会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="40f54-105">You can get details on conferencing activity across your organization.</span></span> <span data-ttu-id="40f54-106">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="40f54-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="40f54-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="40f54-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="reports"></a><span data-ttu-id="40f54-108">报表</span><span class="sxs-lookup"><span data-stu-id="40f54-108">Reports</span></span>

| <span data-ttu-id="40f54-109">函数</span><span class="sxs-lookup"><span data-stu-id="40f54-109">Function</span></span>                                 | <span data-ttu-id="40f54-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="40f54-110">CSV return type</span></span> | <span data-ttu-id="40f54-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="40f54-111">JSON return type</span></span>                         | <span data-ttu-id="40f54-112">说明</span><span class="sxs-lookup"><span data-stu-id="40f54-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="40f54-113">获取活动数</span><span class="sxs-lookup"><span data-stu-id="40f54-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="40f54-114">Stream</span><span class="sxs-lookup"><span data-stu-id="40f54-114">Stream</span></span>          | [<span data-ttu-id="40f54-115">skypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="40f54-115">skypeForBusinessParticipantActivityCounts</span></span>](../resources/skypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="40f54-116">获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="40f54-116">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="40f54-117">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="40f54-117">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="40f54-118">获取用户数</span><span class="sxs-lookup"><span data-stu-id="40f54-118">Get user counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="40f54-119">Stream</span><span class="sxs-lookup"><span data-stu-id="40f54-119">Stream</span></span>          | [<span data-ttu-id="40f54-120">skypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="40f54-120">skypeForBusinessParticipantActivityUserCounts</span></span>](../resources/skypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="40f54-121">获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="40f54-121">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="40f54-122">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="40f54-122">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="40f54-123">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="40f54-123">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="40f54-124">Stream</span><span class="sxs-lookup"><span data-stu-id="40f54-124">Stream</span></span>          | [<span data-ttu-id="40f54-125">skypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="40f54-125">skypeForBusinessParticipantActivityMinuteCounts</span></span>](../resources/skypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="40f54-126">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="40f54-126">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="40f54-127">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="40f54-127">Types of conference sessions include audio/video.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-participant-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
