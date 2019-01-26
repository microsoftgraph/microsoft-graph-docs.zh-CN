---
title: SharePoint 活动报表
description: 您可以获取许可的可供 SharePoint 看它们与文件的交互的每个用户的活动。 也可以查看以共享文件数为依据的协作级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 98d0393545963a73852197f5bd78241cfb958a22
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577114"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="254fa-104">SharePoint 活动报表</span><span class="sxs-lookup"><span data-stu-id="254fa-104">SharePoint activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="254fa-105">您可以获取许可的可供 SharePoint 看它们与文件的交互的每个用户的活动。</span><span class="sxs-lookup"><span data-stu-id="254fa-105">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="254fa-106">也可以查看以共享文件数为依据的协作级别。</span><span class="sxs-lookup"><span data-stu-id="254fa-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="254fa-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="254fa-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="254fa-108">报表</span><span class="sxs-lookup"><span data-stu-id="254fa-108">Reports</span></span>

| <span data-ttu-id="254fa-109">函数</span><span class="sxs-lookup"><span data-stu-id="254fa-109">Function</span></span>                                 | <span data-ttu-id="254fa-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="254fa-110">CSV Return Type</span></span> | <span data-ttu-id="254fa-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="254fa-111">JSON Return Type</span></span>                         | <span data-ttu-id="254fa-112">说明</span><span class="sxs-lookup"><span data-stu-id="254fa-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="254fa-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="254fa-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="254fa-114">Stream</span><span class="sxs-lookup"><span data-stu-id="254fa-114">Stream</span></span>          | [<span data-ttu-id="254fa-115">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="254fa-115">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="254fa-116">获取用户执行的 SharePoint 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="254fa-116">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="254fa-117">获取文件数</span><span class="sxs-lookup"><span data-stu-id="254fa-117">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="254fa-118">Stream</span><span class="sxs-lookup"><span data-stu-id="254fa-118">Stream</span></span>          | [<span data-ttu-id="254fa-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="254fa-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="254fa-120">获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="254fa-120">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="254fa-121">获取用户数</span><span class="sxs-lookup"><span data-stu-id="254fa-121">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="254fa-122">Stream</span><span class="sxs-lookup"><span data-stu-id="254fa-122">Stream</span></span>          | [<span data-ttu-id="254fa-123">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="254fa-123">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="254fa-124">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="254fa-124">Get the trend in the number of active users.</span></span> <span data-ttu-id="254fa-125">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="254fa-125">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="254fa-126">获取页面数</span><span class="sxs-lookup"><span data-stu-id="254fa-126">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="254fa-127">Stream</span><span class="sxs-lookup"><span data-stu-id="254fa-127">Stream</span></span>          | [<span data-ttu-id="254fa-128">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="254fa-128">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="254fa-129">获取用户访问的唯一页面数。</span><span class="sxs-lookup"><span data-stu-id="254fa-129">Get the number of unique pages visited by users.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
