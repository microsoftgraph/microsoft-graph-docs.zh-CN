---
title: SharePoint 活动报表
description: 您可以获取许可的可供 SharePoint 看它们与文件的交互的每个用户的活动。 也可以查看以共享文件数为依据的协作级别。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 55013b3ada74e876734a83acf512a532e32cc4be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522194"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="551b2-104">SharePoint 活动报表</span><span class="sxs-lookup"><span data-stu-id="551b2-104">SharePoint activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="551b2-105">您可以获取许可的可供 SharePoint 看它们与文件的交互的每个用户的活动。</span><span class="sxs-lookup"><span data-stu-id="551b2-105">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="551b2-106">也可以查看以共享文件数为依据的协作级别。</span><span class="sxs-lookup"><span data-stu-id="551b2-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="551b2-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="551b2-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="551b2-108">报表</span><span class="sxs-lookup"><span data-stu-id="551b2-108">Reports</span></span>

| <span data-ttu-id="551b2-109">函数</span><span class="sxs-lookup"><span data-stu-id="551b2-109">Function</span></span>                                 | <span data-ttu-id="551b2-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="551b2-110">CSV Return Type</span></span> | <span data-ttu-id="551b2-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="551b2-111">JSON Return Type</span></span>                         | <span data-ttu-id="551b2-112">说明</span><span class="sxs-lookup"><span data-stu-id="551b2-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="551b2-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="551b2-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="551b2-114">Stream</span><span class="sxs-lookup"><span data-stu-id="551b2-114">Stream</span></span>          | [<span data-ttu-id="551b2-115">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="551b2-115">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="551b2-116">获取用户执行的 SharePoint 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="551b2-116">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="551b2-117">获取文件数</span><span class="sxs-lookup"><span data-stu-id="551b2-117">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="551b2-118">Stream</span><span class="sxs-lookup"><span data-stu-id="551b2-118">Stream</span></span>          | [<span data-ttu-id="551b2-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="551b2-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="551b2-120">获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="551b2-120">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="551b2-121">获取用户数</span><span class="sxs-lookup"><span data-stu-id="551b2-121">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="551b2-122">Stream</span><span class="sxs-lookup"><span data-stu-id="551b2-122">Stream</span></span>          | [<span data-ttu-id="551b2-123">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="551b2-123">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="551b2-124">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="551b2-124">Get the trend in the number of active users.</span></span> <span data-ttu-id="551b2-125">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="551b2-125">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="551b2-126">获取页面数</span><span class="sxs-lookup"><span data-stu-id="551b2-126">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="551b2-127">Stream</span><span class="sxs-lookup"><span data-stu-id="551b2-127">Stream</span></span>          | [<span data-ttu-id="551b2-128">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="551b2-128">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="551b2-129">获取用户访问的唯一页面数。</span><span class="sxs-lookup"><span data-stu-id="551b2-129">Get the number of unique pages visited by users.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
