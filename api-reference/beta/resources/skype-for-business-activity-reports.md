---
title: Skype for Business 活动报表
description: 您的组织内，可以在活动上获取详细信息。 这些详细信息有助于为组织调查、计划和做出其他业务决策。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a81e27d58316cb415d6296b4f77519a3f2125643
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512393"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="de866-104">Skype for Business 活动报表</span><span class="sxs-lookup"><span data-stu-id="de866-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de866-105">您的组织内，可以在活动上获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="de866-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="de866-106">这些详细信息有助于为组织调查、计划和做出其他业务决策。</span><span class="sxs-lookup"><span data-stu-id="de866-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="de866-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="de866-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="de866-108">报表</span><span class="sxs-lookup"><span data-stu-id="de866-108">Reports</span></span>

| <span data-ttu-id="de866-109">函数</span><span class="sxs-lookup"><span data-stu-id="de866-109">Function</span></span>                                 | <span data-ttu-id="de866-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="de866-110">CSV return type</span></span> | <span data-ttu-id="de866-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="de866-111">JSON return type</span></span>                         | <span data-ttu-id="de866-112">说明</span><span class="sxs-lookup"><span data-stu-id="de866-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="de866-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="de866-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="de866-114">Stream</span><span class="sxs-lookup"><span data-stu-id="de866-114">Stream</span></span>          | [<span data-ttu-id="de866-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="de866-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="de866-116">获取用户执行的 Skype for Business 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="de866-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="de866-117">获取活动数</span><span class="sxs-lookup"><span data-stu-id="de866-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="de866-118">Stream</span><span class="sxs-lookup"><span data-stu-id="de866-118">Stream</span></span>          | [<span data-ttu-id="de866-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="de866-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="de866-120">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="de866-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="de866-121">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="de866-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="de866-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="de866-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="de866-123">Stream</span><span class="sxs-lookup"><span data-stu-id="de866-123">Stream</span></span>          | [<span data-ttu-id="de866-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="de866-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="de866-125">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="de866-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="de866-126">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="de866-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
