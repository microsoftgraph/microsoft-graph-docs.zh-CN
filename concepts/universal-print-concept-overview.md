---
title: 通用打印云打印 API 概述
description: 通用打印是一种新式打印解决方案，组织可以使用它通过 Microsoft 云服务来管理自己的打印基础设施。
author: braedenp-msft
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: d3df3a36ac9994b3ce4560b995a52288dd197e34
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44215652"
---
# <a name="universal-print-cloud-printing-api-overview"></a><span data-ttu-id="60a84-103">通用打印云打印 API 概述</span><span class="sxs-lookup"><span data-stu-id="60a84-103">Universal Print cloud printing API overview</span></span>

<span data-ttu-id="60a84-104">通用打印是一种新式打印解决方案，组织可以使用它通过 Microsoft 云服务来管理自己的打印基础设施。</span><span class="sxs-lookup"><span data-stu-id="60a84-104">Universal Print is a modern print solution that organizations can use to manage their print infrastructure through cloud services from Microsoft.</span></span>

![通用打印 Azure 门户主页的屏幕截图](images/universal-print-portal-homepage.png)

## <a name="why-use-universal-print"></a><span data-ttu-id="60a84-106">为什么要使用通用打印？</span><span class="sxs-lookup"><span data-stu-id="60a84-106">Why use Universal Print?</span></span>

<span data-ttu-id="60a84-107">通用打印将关键的 Windows Server 打印功能迁移到 Microsoft 365 云中，这样组织就不再需要本地打印服务器，也不需要在设备上安装打印机驱动程序。</span><span class="sxs-lookup"><span data-stu-id="60a84-107">Universal Print moves key Windows Server print functionality to the Microsoft 365 cloud, so organizations no longer need on-premises print servers and do not need to install printer drivers on devices.</span></span> <span data-ttu-id="60a84-108">此外，通用打印还带来了一些关键功能，如用于授予打印机访问权限的安全组、基于位置的打印机发现和丰富的管理员体验。</span><span class="sxs-lookup"><span data-stu-id="60a84-108">In addition, Universal Print adds key functionality like security groups for printer access, location-based printer discovery, and a rich administrator experience.</span></span>

<span data-ttu-id="60a84-109">随着组织采用通用打印，组织和独立软件供应商 (ISV) 可使用 Microsoft Graph 中的通用打印 API 来生成和扩展应用程序，从而支持新方案。</span><span class="sxs-lookup"><span data-stu-id="60a84-109">As organizations adopt Universal Print, organizations and independent software vendors (ISVs) can use the Universal Print API in Microsoft Graph to build and extend applications to support new scenarios.</span></span>

### <a name="print-documents-from-web-and-mobile-applications"></a><span data-ttu-id="60a84-110">从 Web 和移动应用打印文档</span><span class="sxs-lookup"><span data-stu-id="60a84-110">Print documents from web and mobile applications</span></span>

<span data-ttu-id="60a84-111">将打印基础设施迁移到云中，可直接从 Web 和移动应用打印文档。</span><span class="sxs-lookup"><span data-stu-id="60a84-111">Moving print infrastructure to the cloud enables printing documents directly from web and mobile applications.</span></span>

<span data-ttu-id="60a84-112">若要开始使用通用打印 API，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="60a84-112">To get started with the Universal Print API:</span></span>

1. <span data-ttu-id="60a84-113">[创建打印作业](/graph/api/printer-post-jobs?view=graph-rest-beta)，并存储生成的文档 ID。</span><span class="sxs-lookup"><span data-stu-id="60a84-113">[Create a print job](/graph/api/printer-post-jobs?view=graph-rest-beta) and store the resulting document ID.</span></span>
2. <span data-ttu-id="60a84-114">[将文档数据上传](/graph/api/printdocument-uploaddata?view=graph-rest-beta)到文档。</span><span class="sxs-lookup"><span data-stu-id="60a84-114">[Upload document data](/graph/api/printdocument-uploaddata?view=graph-rest-beta) to the document.</span></span>
3. <span data-ttu-id="60a84-115">[启动打印作业](/graph/api/printjob-startprintjob?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="60a84-115">[Start the print job](/graph/api/printjob-startprintjob?view=graph-rest-beta).</span></span>

### <a name="manage-printers"></a><span data-ttu-id="60a84-116">管理打印机</span><span class="sxs-lookup"><span data-stu-id="60a84-116">Manage printers</span></span>

<span data-ttu-id="60a84-117">跟踪组织的打印机、打印机配置和打印机使用情况是一项很复杂的任务。</span><span class="sxs-lookup"><span data-stu-id="60a84-117">Keeping track of an organization's printers, printer configurations, and printer usage is a complex task.</span></span> <span data-ttu-id="60a84-118">通用打印 API 可以在所有三个方面实现集成。</span><span class="sxs-lookup"><span data-stu-id="60a84-118">The Universal Print API enables integration in all three areas.</span></span>

* <span data-ttu-id="60a84-119">使用[列出打印机](/graph/api/print-list-printers?view=graph-rest-beta)和 [printerStatus](/graph/api/resources/printerstatus?view=graph-rest-beta)，**监视打印机状态、配置和可用性**。</span><span class="sxs-lookup"><span data-stu-id="60a84-119">**Keep an eye on printer status, configurations, and availability** by using [List printers](/graph/api/print-list-printers?view=graph-rest-beta) and [printerStatus](/graph/api/resources/printerstatus?view=graph-rest-beta).</span></span>

* <span data-ttu-id="60a84-120">使用报告 API，**了解谁在使用打印机以及打印进度**：</span><span class="sxs-lookup"><span data-stu-id="60a84-120">**See who's using your printers and how much they're printing** by using the reporting APIs:</span></span>
  * [<span data-ttu-id="60a84-121">列出 dailyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="60a84-121">List dailyPrintUsageSummariesByUser</span></span>](/graph/api/reportroot-list-dailyprintusagesummariesbyuser?view=graph-rest-beta)
  * [<span data-ttu-id="60a84-122">列出 monthlyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="60a84-122">List monthlyPrintUsageSummariesByUser</span></span>](/graph/api/reportroot-list-monthlyprintusagesummariesbyuser?view=graph-rest-beta)
  * [<span data-ttu-id="60a84-123">列出 dailyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="60a84-123">List dailyPrintUsageSummariesByPrinter</span></span>](/graph/api/reportroot-list-dailyprintusagesummariesbyprinter?view=graph-rest-beta)
  * [<span data-ttu-id="60a84-124">列出 monthlyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="60a84-124">List monthlyPrintUsageSummariesByPrinter</span></span>](/graph/api/reportroot-list-monthlyprintusagesummariesbyprinter?view=graph-rest-beta)

* <span data-ttu-id="60a84-125">通过修改打印机上的用户和组成员资格，**配置用户权限**：</span><span class="sxs-lookup"><span data-stu-id="60a84-125">**Configure user permissions** by modifying user and group membership on printers:</span></span>
  * [<span data-ttu-id="60a84-126">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="60a84-126">List allowedUsers</span></span>](/graph/api/printer-list-allowedusers?view=graph-rest-beta)
  * [<span data-ttu-id="60a84-127">添加 allowedUser</span><span class="sxs-lookup"><span data-stu-id="60a84-127">Add allowedUser</span></span>](/graph/api/printer-post-allowedusers?view=graph-rest-beta)
  * [<span data-ttu-id="60a84-128">删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="60a84-128">Remove allowedUser</span></span>](/graph/api/printer-delete-alloweduser?view=graph-rest-beta)
  * [<span data-ttu-id="60a84-129">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="60a84-129">List allowedGroups</span></span>](/graph/api/printer-list-allowedgroups?view=graph-rest-beta)
  * [<span data-ttu-id="60a84-130">添加 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="60a84-130">Add allowedGroup</span></span>](/graph/api/printer-post-allowedgroups?view=graph-rest-beta)
  * [<span data-ttu-id="60a84-131">删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="60a84-131">Remove allowedGroup</span></span>](/graph/api/printer-delete-allowedgroup?view=graph-rest-beta)

### <a name="seamlessly-replace-or-update-printer-hardware"></a><span data-ttu-id="60a84-132">无缝更换或更新打印机硬件</span><span class="sxs-lookup"><span data-stu-id="60a84-132">Seamlessly replace or update printer hardware</span></span>

<span data-ttu-id="60a84-133">用户只能看到[共享](/graph/api/print-post-shares?view=graph-rest-beta)的打印机，这样管理员可以精细地控制哪个打印机硬件在给定时间可用。</span><span class="sxs-lookup"><span data-stu-id="60a84-133">Printers are not visible to users until they are [shared](/graph/api/print-post-shares?view=graph-rest-beta), providing administrators fine-grained control over which printer hardware is available at a given time.</span></span>

<span data-ttu-id="60a84-134">共享打印机会创建 [printerShare](/graph/api/resources/printershare?view=graph-rest-beta) 资源，它可随时更新为指向其他打印机，这样就能轻松更换损坏的打印机硬件，或让打印机脱机接受维护。</span><span class="sxs-lookup"><span data-stu-id="60a84-134">Sharing a printer creates a [printerShare](/graph/api/resources/printershare?view=graph-rest-beta) resource that can be updated at any time to point to a different printer, making it easy to replace broken printer hardware or take printers offline for maintenance.</span></span>

<span data-ttu-id="60a84-135">若要在应用程序中使用此功能，请使用[更新 printerShare](/graph/api/printershare-update?view=graph-rest-beta) 来更新 printerShare 的 `printer` 引用。</span><span class="sxs-lookup"><span data-stu-id="60a84-135">To use this in your application, use [Update printerShare](/graph/api/printershare-update?view=graph-rest-beta) to update the printerShare's `printer` reference.</span></span>

## <a name="api-reference"></a><span data-ttu-id="60a84-136">API 参考</span><span class="sxs-lookup"><span data-stu-id="60a84-136">API reference</span></span>
<span data-ttu-id="60a84-137">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="60a84-137">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="60a84-138">Microsoft Graph Beta 中的通用打印 API</span><span class="sxs-lookup"><span data-stu-id="60a84-138">Universal Print API in Microsoft Graph beta</span></span>](/graph/api/resources/print?view=graph-rest-beta)

## <a name="see-also"></a><span data-ttu-id="60a84-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="60a84-139">See also</span></span>

- [<span data-ttu-id="60a84-140">什么是通用打印</span><span class="sxs-lookup"><span data-stu-id="60a84-140">What is Universal Print</span></span>](https://docs.microsoft.com/universal-print/fundamentals/universal-print-whatis)
- <span data-ttu-id="60a84-141">欢迎在 [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 上提供有关通用打印 API 的反馈！</span><span class="sxs-lookup"><span data-stu-id="60a84-141">We'd love to hear your feedback about the Universal Print APIs over at [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)!</span></span>
