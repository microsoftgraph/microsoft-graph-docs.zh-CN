---
title: SharePoint 网站使用情况报表
description: SharePoint 网站使用情况报表可用于大致了解 SharePoint 带来的价值，具体是以用户在 SharePoint 网站中存储的文件总数、使用的活跃文件数以及跨所有这些网站使用的存储为依据。 然后，可以向下钻取这些报表，了解所有网站的趋势以及每网站级别详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 064501634afb819ab9b0d8d6c729d2bc9f8181d5
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980966"
---
# <a name="sharepoint-site-usage-reports"></a><span data-ttu-id="3a73f-104">SharePoint 网站使用情况报表</span><span class="sxs-lookup"><span data-stu-id="3a73f-104">SharePoint site usage reports</span></span>

<span data-ttu-id="3a73f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a73f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a73f-106">SharePoint 网站使用情况报表可用于大致了解 SharePoint 带来的价值，具体是以用户在 SharePoint 网站中存储的文件总数、使用的活跃文件数以及跨所有这些网站使用的存储为依据。</span><span class="sxs-lookup"><span data-stu-id="3a73f-106">You can use the SharePoint site usage reports to gain a high level view of the value you are getting from SharePoint in terms of the total number of files that users store in SharePoint sites, how many files are actively being used, and the storage consumed across all these sites.</span></span> <span data-ttu-id="3a73f-107">然后，可以向下钻取这些报表，了解所有网站的趋势以及每网站级别详细信息。</span><span class="sxs-lookup"><span data-stu-id="3a73f-107">Then, you can drill into these reports to understand the trends and per site level details for all sites.</span></span>

> <span data-ttu-id="3a73f-108">**注意：** 有关不同报告视图和名称的详细信息，请参阅 [Microsoft 365 报告 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="3a73f-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="reports"></a><span data-ttu-id="3a73f-109">报告</span><span class="sxs-lookup"><span data-stu-id="3a73f-109">Reports</span></span>

| <span data-ttu-id="3a73f-110">函数</span><span class="sxs-lookup"><span data-stu-id="3a73f-110">Function</span></span>                                 | <span data-ttu-id="3a73f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3a73f-111">Return Type</span></span> | <span data-ttu-id="3a73f-112">说明</span><span class="sxs-lookup"><span data-stu-id="3a73f-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="3a73f-113">获取网站详细信息</span><span class="sxs-lookup"><span data-stu-id="3a73f-113">Get site detail</span></span>](../api/reportroot-getsharepointsiteusagedetail.md) | <span data-ttu-id="3a73f-114">Stream</span><span class="sxs-lookup"><span data-stu-id="3a73f-114">Stream</span></span>      | <span data-ttu-id="3a73f-115">获取 SharePoint 网站使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3a73f-115">Get details about SharePoint site usage.</span></span> |
| [<span data-ttu-id="3a73f-116">获取文件数</span><span class="sxs-lookup"><span data-stu-id="3a73f-116">Get file counts</span></span>](../api/reportroot-getsharepointsiteusagefilecounts.md) | <span data-ttu-id="3a73f-117">Stream</span><span class="sxs-lookup"><span data-stu-id="3a73f-117">Stream</span></span>      | <span data-ttu-id="3a73f-118">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="3a73f-118">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="3a73f-119">如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。</span><span class="sxs-lookup"><span data-stu-id="3a73f-119">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span> |
| [<span data-ttu-id="3a73f-120">获取网站数</span><span class="sxs-lookup"><span data-stu-id="3a73f-120">Get site counts</span></span>](../api/reportroot-getsharepointsiteusagesitecounts.md) | <span data-ttu-id="3a73f-121">Stream</span><span class="sxs-lookup"><span data-stu-id="3a73f-121">Stream</span></span>      | <span data-ttu-id="3a73f-122">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="3a73f-122">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="3a73f-123">如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。</span><span class="sxs-lookup"><span data-stu-id="3a73f-123">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span> |
| [<span data-ttu-id="3a73f-124">获取存储</span><span class="sxs-lookup"><span data-stu-id="3a73f-124">Get storage</span></span>](../api/reportroot-getsharepointsiteusagestorage.md) | <span data-ttu-id="3a73f-125">Stream</span><span class="sxs-lookup"><span data-stu-id="3a73f-125">Stream</span></span>      | <span data-ttu-id="3a73f-126">获取报表周期内分配和使用的存储趋势。</span><span class="sxs-lookup"><span data-stu-id="3a73f-126">Get the trend of storage allocated and consumed during the reporting period.</span></span> |
| [<span data-ttu-id="3a73f-127">获取页面数</span><span class="sxs-lookup"><span data-stu-id="3a73f-127">Get pages</span></span>](../api/reportroot-getsharepointsiteusagepages.md) | <span data-ttu-id="3a73f-128">Stream</span><span class="sxs-lookup"><span data-stu-id="3a73f-128">Stream</span></span>      | <span data-ttu-id="3a73f-129">获取跨所有网站浏览的页面数。</span><span class="sxs-lookup"><span data-stu-id="3a73f-129">Get the number of pages viewed across all sites.</span></span> |

