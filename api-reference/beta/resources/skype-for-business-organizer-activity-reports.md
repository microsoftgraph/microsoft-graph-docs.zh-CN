---
title: Skype for Business 组织者活动报表
description: 你可以在组织中获取有关组织的会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8254221fc32b299b4d1a1de48165f6349b739f22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568185"
---
# <a name="skype-for-business-organizer-activity-reports"></a><span data-ttu-id="7b537-104">Skype for Business 组织者活动报表</span><span class="sxs-lookup"><span data-stu-id="7b537-104">Skype for Business organizer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b537-105">你可以在组织中获取有关组织的会议活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7b537-105">You can get details on organized conferences activity across your organization.</span></span> <span data-ttu-id="7b537-106">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="7b537-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="7b537-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="7b537-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="reports"></a><span data-ttu-id="7b537-108">报表</span><span class="sxs-lookup"><span data-stu-id="7b537-108">Reports</span></span>

| <span data-ttu-id="7b537-109">函数</span><span class="sxs-lookup"><span data-stu-id="7b537-109">Function</span></span>                                 | <span data-ttu-id="7b537-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="7b537-110">CSV return type</span></span> | <span data-ttu-id="7b537-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="7b537-111">JSON return type</span></span>                         | <span data-ttu-id="7b537-112">说明</span><span class="sxs-lookup"><span data-stu-id="7b537-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="7b537-113">获取活动数</span><span class="sxs-lookup"><span data-stu-id="7b537-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | <span data-ttu-id="7b537-114">Stream</span><span class="sxs-lookup"><span data-stu-id="7b537-114">Stream</span></span>          | [<span data-ttu-id="7b537-115">skypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="7b537-115">skypeForBusinessOrganizerActivityCounts</span></span>](../resources/skypeforbusinessorganizeractivitycounts.md) | <span data-ttu-id="7b537-116">获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="7b537-116">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="7b537-117">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="7b537-117">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="7b537-118">获取用户数</span><span class="sxs-lookup"><span data-stu-id="7b537-118">Get user counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | <span data-ttu-id="7b537-119">Stream</span><span class="sxs-lookup"><span data-stu-id="7b537-119">Stream</span></span>          | [<span data-ttu-id="7b537-120">skypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="7b537-120">skypeForBusinessOrganizerActivityUserCounts</span></span>](../resources/skypeforbusinessorganizeractivityusercounts.md) | <span data-ttu-id="7b537-121">获取使用情况趋势，即组织中用户召开和组织的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="7b537-121">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="7b537-122">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="7b537-122">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="7b537-123">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="7b537-123">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | <span data-ttu-id="7b537-124">Stream</span><span class="sxs-lookup"><span data-stu-id="7b537-124">Stream</span></span>          | [<span data-ttu-id="7b537-125">skypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="7b537-125">skypeForBusinessOrganizerActivityMinuteCounts</span></span>](../resources/skypeforbusinessorganizeractivityminutecounts.md) | <span data-ttu-id="7b537-126">获取使用情况趋势，即组织中用户召开和组织的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="7b537-126">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="7b537-127">会议会话类型包括音频/视频和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="7b537-127">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-organizer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
