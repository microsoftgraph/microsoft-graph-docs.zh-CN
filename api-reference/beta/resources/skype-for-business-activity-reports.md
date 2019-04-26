---
title: Skype for Business 活动报表
description: 你可以在组织中获取活动的详细信息。 这些详细信息有助于为组织调查、计划和制定其他业务决策。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3f843efc6834ee59872e7bf750174558cdb0a103
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551902"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="eec94-104">Skype for Business 活动报告</span><span class="sxs-lookup"><span data-stu-id="eec94-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eec94-105">你可以在组织中获取活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="eec94-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="eec94-106">这些详细信息有助于为组织调查、计划和做出其他业务决策。</span><span class="sxs-lookup"><span data-stu-id="eec94-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="eec94-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="eec94-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="eec94-108">报表</span><span class="sxs-lookup"><span data-stu-id="eec94-108">Reports</span></span>

| <span data-ttu-id="eec94-109">函数</span><span class="sxs-lookup"><span data-stu-id="eec94-109">Function</span></span>                                 | <span data-ttu-id="eec94-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="eec94-110">CSV return type</span></span> | <span data-ttu-id="eec94-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="eec94-111">JSON return type</span></span>                         | <span data-ttu-id="eec94-112">说明</span><span class="sxs-lookup"><span data-stu-id="eec94-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="eec94-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="eec94-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="eec94-114">Stream</span><span class="sxs-lookup"><span data-stu-id="eec94-114">Stream</span></span>          | [<span data-ttu-id="eec94-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="eec94-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="eec94-116">获取用户执行的 Skype for Business 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="eec94-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="eec94-117">获取活动数</span><span class="sxs-lookup"><span data-stu-id="eec94-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="eec94-118">Stream</span><span class="sxs-lookup"><span data-stu-id="eec94-118">Stream</span></span>          | [<span data-ttu-id="eec94-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="eec94-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="eec94-120">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="eec94-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="eec94-121">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="eec94-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="eec94-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="eec94-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="eec94-123">Stream</span><span class="sxs-lookup"><span data-stu-id="eec94-123">Stream</span></span>          | [<span data-ttu-id="eec94-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="eec94-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="eec94-125">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="eec94-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="eec94-126">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="eec94-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
