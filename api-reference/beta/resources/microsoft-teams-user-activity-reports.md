---
title: Microsoft Teams 用户活动报告
description: 使用 Microsoft 团队用户活动报告您的组织中获取的 Microsoft 团队用户活动见解。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4a071fb38ce9fd76aff4ccdc648201f91a600f24
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574717"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="0d09b-103">Microsoft Teams 用户活动报告</span><span class="sxs-lookup"><span data-stu-id="0d09b-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d09b-104">使用 Microsoft 团队用户活动报告您的组织中获取的 Microsoft 团队用户活动见解。</span><span class="sxs-lookup"><span data-stu-id="0d09b-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="0d09b-105">方法</span><span class="sxs-lookup"><span data-stu-id="0d09b-105">Methods</span></span>

| <span data-ttu-id="0d09b-106">方法</span><span class="sxs-lookup"><span data-stu-id="0d09b-106">Method</span></span>                                   | <span data-ttu-id="0d09b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="0d09b-107">Return Type</span></span>                              | <span data-ttu-id="0d09b-108">说明</span><span class="sxs-lookup"><span data-stu-id="0d09b-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="0d09b-109">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="0d09b-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="0d09b-110">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="0d09b-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="0d09b-111">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0d09b-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="0d09b-112">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="0d09b-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="0d09b-113">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="0d09b-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="0d09b-114">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="0d09b-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="0d09b-115">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="0d09b-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="0d09b-116">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="0d09b-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="0d09b-117">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="0d09b-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="0d09b-118">按活动类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="0d09b-118">Get the number of users by activity type.</span></span> <span data-ttu-id="0d09b-119">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="0d09b-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-user-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
