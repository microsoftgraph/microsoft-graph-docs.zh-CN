---
title: SharePoint 网站使用情况报表
description: SharePoint 网站使用情况报表可用于大致了解 SharePoint 带来的价值，具体是以用户在 SharePoint 网站中存储的文件总数、使用的活跃文件数以及跨所有这些网站使用的存储为依据。 然后，可以向下钻取这些报表，了解所有网站的趋势以及每网站级别详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 08de7aff6f96a30632c9b639c7021414f7853663
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034305"
---
# <a name="sharepoint-site-usage-reports"></a><span data-ttu-id="b9736-104">SharePoint 网站使用情况报表</span><span class="sxs-lookup"><span data-stu-id="b9736-104">SharePoint site usage reports</span></span>

<span data-ttu-id="b9736-105">SharePoint 网站使用情况报表可用于大致了解 SharePoint 带来的价值，具体是以用户在 SharePoint 网站中存储的文件总数、使用的活跃文件数以及跨所有这些网站使用的存储为依据。</span><span class="sxs-lookup"><span data-stu-id="b9736-105">You can use the SharePoint site usage reports to gain a high level view of the value you are getting from SharePoint in terms of the total number of files that users store in SharePoint sites, how many files are actively being used, and the storage consumed across all these sites.</span></span> <span data-ttu-id="b9736-106">然后，可以向下钻取这些报表，了解所有网站的趋势以及每网站级别详细信息。</span><span class="sxs-lookup"><span data-stu-id="b9736-106">Then, you can drill into these reports to understand the trends and per site level details for all sites.</span></span>

> <span data-ttu-id="b9736-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="b9736-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="reports"></a><span data-ttu-id="b9736-108">报表</span><span class="sxs-lookup"><span data-stu-id="b9736-108">Reports</span></span>

| <span data-ttu-id="b9736-109">函数</span><span class="sxs-lookup"><span data-stu-id="b9736-109">Function</span></span>                                 | <span data-ttu-id="b9736-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b9736-110">Return Type</span></span> | <span data-ttu-id="b9736-111">说明</span><span class="sxs-lookup"><span data-stu-id="b9736-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="b9736-112">获取网站详细信息</span><span class="sxs-lookup"><span data-stu-id="b9736-112">Get site detail</span></span>](../api/reportroot-getsharepointsiteusagedetail.md) | <span data-ttu-id="b9736-113">流</span><span class="sxs-lookup"><span data-stu-id="b9736-113">Stream</span></span>      | <span data-ttu-id="b9736-114">获取 SharePoint 网站使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b9736-114">Get details about SharePoint site usage.</span></span> |
| [<span data-ttu-id="b9736-115">获取文件数</span><span class="sxs-lookup"><span data-stu-id="b9736-115">Get file counts</span></span>](../api/reportroot-getsharepointsiteusagefilecounts.md) | <span data-ttu-id="b9736-116">流</span><span class="sxs-lookup"><span data-stu-id="b9736-116">Stream</span></span>      | <span data-ttu-id="b9736-117">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="b9736-117">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="b9736-118">如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。</span><span class="sxs-lookup"><span data-stu-id="b9736-118">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span> |
| [<span data-ttu-id="b9736-119">获取网站数</span><span class="sxs-lookup"><span data-stu-id="b9736-119">Get site counts</span></span>](../api/reportroot-getsharepointsiteusagesitecounts.md) | <span data-ttu-id="b9736-120">Stream</span><span class="sxs-lookup"><span data-stu-id="b9736-120">Stream</span></span>      | <span data-ttu-id="b9736-121">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="b9736-121">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="b9736-122">如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。</span><span class="sxs-lookup"><span data-stu-id="b9736-122">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span> |
| [<span data-ttu-id="b9736-123">获取存储</span><span class="sxs-lookup"><span data-stu-id="b9736-123">Get storage</span></span>](../api/reportroot-getsharepointsiteusagestorage.md) | <span data-ttu-id="b9736-124">Stream</span><span class="sxs-lookup"><span data-stu-id="b9736-124">Stream</span></span>      | <span data-ttu-id="b9736-125">获取报表周期内分配和使用的存储趋势。</span><span class="sxs-lookup"><span data-stu-id="b9736-125">Get the trend of storage allocated and consumed during the reporting period.</span></span> |
| [<span data-ttu-id="b9736-126">获取页面数</span><span class="sxs-lookup"><span data-stu-id="b9736-126">Get pages</span></span>](../api/reportroot-getsharepointsiteusagepages.md) | <span data-ttu-id="b9736-127">Stream</span><span class="sxs-lookup"><span data-stu-id="b9736-127">Stream</span></span>      | <span data-ttu-id="b9736-128">获取跨所有网站浏览的页面数。</span><span class="sxs-lookup"><span data-stu-id="b9736-128">Get the number of pages viewed across all sites.</span></span> |
