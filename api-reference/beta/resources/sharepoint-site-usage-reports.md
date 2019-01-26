---
title: SharePoint 网站使用情况报表
description: 您可以获取来自 SharePoint 的用户存储在 SharePoint 网站、 多少文件主动正在被使用，和存储在所有这些网站使用的文件总数方面得到的值的高级视图。 然后，您可以深化到的 SharePoint 网站使用率报告，以便了解趋势和每个网站的所有站点级别的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f25d752a179eac68b34465010ce6f2cb7fab08e8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575277"
---
# <a name="sharepoint-site-usage-reports"></a><span data-ttu-id="69c13-104">SharePoint 网站使用情况报表</span><span class="sxs-lookup"><span data-stu-id="69c13-104">SharePoint site usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69c13-105">您可以获取来自 SharePoint 的用户存储在 SharePoint 网站、 多少文件主动正在被使用，和存储在所有这些网站使用的文件总数方面得到的值的高级视图。</span><span class="sxs-lookup"><span data-stu-id="69c13-105">You can get a high level view of the value you are getting from SharePoint in terms of the total number of files that users store in SharePoint sites, how many files are actively being used, and the storage consumed across all these sites.</span></span> <span data-ttu-id="69c13-106">然后，您可以深化到的 SharePoint 网站使用率报告，以便了解趋势和每个网站的所有站点级别的详细信息。</span><span class="sxs-lookup"><span data-stu-id="69c13-106">Then, you can drill into the SharePoint site usage report to understand the trends and per site level details for all sites.</span></span>

> <span data-ttu-id="69c13-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="69c13-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="reports"></a><span data-ttu-id="69c13-108">报表</span><span class="sxs-lookup"><span data-stu-id="69c13-108">Reports</span></span>

| <span data-ttu-id="69c13-109">函数</span><span class="sxs-lookup"><span data-stu-id="69c13-109">Function</span></span>                                 | <span data-ttu-id="69c13-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="69c13-110">CSV return type</span></span> | <span data-ttu-id="69c13-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="69c13-111">JSON return type</span></span>                         | <span data-ttu-id="69c13-112">说明</span><span class="sxs-lookup"><span data-stu-id="69c13-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="69c13-113">获取网站详细信息</span><span class="sxs-lookup"><span data-stu-id="69c13-113">Get site detail</span></span>](../api/reportroot-getsharepointsiteusagedetail.md) | <span data-ttu-id="69c13-114">Stream</span><span class="sxs-lookup"><span data-stu-id="69c13-114">Stream</span></span>          | [<span data-ttu-id="69c13-115">sharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="69c13-115">sharePointSiteUsageDetail</span></span>](../resources/sharepointsiteusagedetail.md) | <span data-ttu-id="69c13-116">获取 SharePoint 网站使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="69c13-116">Get details about SharePoint site usage.</span></span> |
| [<span data-ttu-id="69c13-117">获取文件数</span><span class="sxs-lookup"><span data-stu-id="69c13-117">Get file counts</span></span>](../api/reportroot-getsharepointsiteusagefilecounts.md) | <span data-ttu-id="69c13-118">Stream</span><span class="sxs-lookup"><span data-stu-id="69c13-118">Stream</span></span>          | [<span data-ttu-id="69c13-119">sharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="69c13-119">sharePointSiteUsageFileCounts</span></span>](../resources/sharepointsiteusagefilecounts.md) | <span data-ttu-id="69c13-120">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="69c13-120">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="69c13-121">如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。</span><span class="sxs-lookup"><span data-stu-id="69c13-121">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span> |
| [<span data-ttu-id="69c13-122">获取网站数</span><span class="sxs-lookup"><span data-stu-id="69c13-122">Get site counts</span></span>](../api/reportroot-getsharepointsiteusagesitecounts.md) | <span data-ttu-id="69c13-123">Stream</span><span class="sxs-lookup"><span data-stu-id="69c13-123">Stream</span></span>          | [<span data-ttu-id="69c13-124">sharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="69c13-124">sharePointSiteUsageSiteCounts</span></span>](../resources/sharepointsiteusagesitecounts.md) | <span data-ttu-id="69c13-125">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="69c13-125">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="69c13-126">如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。</span><span class="sxs-lookup"><span data-stu-id="69c13-126">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span> |
| [<span data-ttu-id="69c13-127">获取存储</span><span class="sxs-lookup"><span data-stu-id="69c13-127">Get storage</span></span>](../api/reportroot-getsharepointsiteusagestorage.md) | <span data-ttu-id="69c13-128">Stream</span><span class="sxs-lookup"><span data-stu-id="69c13-128">Stream</span></span>          | [<span data-ttu-id="69c13-129">siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="69c13-129">siteUsageStorage</span></span>](../resources/siteusagestorage.md) | <span data-ttu-id="69c13-130">获取报表周期内分配和使用的存储趋势。</span><span class="sxs-lookup"><span data-stu-id="69c13-130">Get the trend of storage allocated and consumed during the reporting period.</span></span> |
| [<span data-ttu-id="69c13-131">获取页面数</span><span class="sxs-lookup"><span data-stu-id="69c13-131">Get pages</span></span>](../api/reportroot-getsharepointsiteusagepages.md) | <span data-ttu-id="69c13-132">Stream</span><span class="sxs-lookup"><span data-stu-id="69c13-132">Stream</span></span>          | [<span data-ttu-id="69c13-133">sharePointSiteUsagePages</span><span class="sxs-lookup"><span data-stu-id="69c13-133">sharePointSiteUsagePages</span></span>](../resources/sharepointsiteusagepages.md) | <span data-ttu-id="69c13-134">获取跨所有网站浏览的页面数。</span><span class="sxs-lookup"><span data-stu-id="69c13-134">Get the number of pages viewed across all sites.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-site-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
