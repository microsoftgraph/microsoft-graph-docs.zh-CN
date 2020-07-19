---
title: 通用打印云打印 API 概述
description: 通用打印是一种新式打印解决方案，组织可以使用它通过 Microsoft 云服务来管理自己的打印基础设施。
author: braedenp-msft
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: 3ae838f408b6c0452a10379080895e5fdc64b6b1
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091527"
---
# <a name="universal-print-cloud-printing-api-overview"></a><span data-ttu-id="deb76-103">通用打印云打印 API 概述</span><span class="sxs-lookup"><span data-stu-id="deb76-103">Universal Print cloud printing API overview</span></span>

<span data-ttu-id="deb76-104">通用打印是一种新式打印解决方案，组织可以使用它通过 Microsoft 云服务来管理自己的打印基础设施。</span><span class="sxs-lookup"><span data-stu-id="deb76-104">Universal Print is a modern print solution that organizations can use to manage their print infrastructure through cloud services from Microsoft.</span></span>

![通用打印 Azure 门户主页的屏幕截图](images/universal-print-portal-homepage.png)

## <a name="why-use-universal-print"></a><span data-ttu-id="deb76-106">为什么要使用通用打印？</span><span class="sxs-lookup"><span data-stu-id="deb76-106">Why use Universal Print?</span></span>

<span data-ttu-id="deb76-107">通用打印将关键的 Windows Server 打印功能迁移到 Microsoft 365 云中，这样组织就不再需要本地打印服务器，也不需要在设备上安装打印机驱动程序。</span><span class="sxs-lookup"><span data-stu-id="deb76-107">Universal Print moves key Windows Server print functionality to the Microsoft 365 cloud, so organizations no longer need on-premises print servers and do not need to install printer drivers on devices.</span></span> <span data-ttu-id="deb76-108">此外，通用打印还带来了一些关键功能，如用于授予打印机访问权限的安全组、基于位置的打印机发现和丰富的管理员体验。</span><span class="sxs-lookup"><span data-stu-id="deb76-108">In addition, Universal Print adds key functionality like security groups for printer access, location-based printer discovery, and a rich administrator experience.</span></span>

<span data-ttu-id="deb76-109">随着组织采用通用打印，组织和独立软件供应商 (ISV) 可使用 Microsoft Graph 中的通用打印 API 来生成和扩展应用程序，从而支持新方案。</span><span class="sxs-lookup"><span data-stu-id="deb76-109">As organizations adopt Universal Print, organizations and independent software vendors (ISVs) can use the Universal Print API in Microsoft Graph to build and extend applications to support new scenarios.</span></span>

### <a name="print-documents-from-web-and-mobile-applications"></a><span data-ttu-id="deb76-110">从 Web 和移动应用打印文档</span><span class="sxs-lookup"><span data-stu-id="deb76-110">Print documents from web and mobile applications</span></span>

<span data-ttu-id="deb76-111">将打印基础设施迁移到云中，可直接从 Web 和移动应用打印文档。</span><span class="sxs-lookup"><span data-stu-id="deb76-111">Moving print infrastructure to the cloud enables printing documents directly from web and mobile applications.</span></span>

<span data-ttu-id="deb76-112">若要开始使用通用打印 API，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="deb76-112">To get started with the Universal Print API:</span></span>

1. <span data-ttu-id="deb76-113">[创建打印作业](/graph/api/printer-post-jobs?view=graph-rest-beta)，并存储生成的文档 ID。</span><span class="sxs-lookup"><span data-stu-id="deb76-113">[Create a print job](/graph/api/printer-post-jobs?view=graph-rest-beta) and store the resulting document ID.</span></span>
2. <span data-ttu-id="deb76-114">[将文档数据上传](/graph/api/printdocument-uploaddata?view=graph-rest-beta)到文档。</span><span class="sxs-lookup"><span data-stu-id="deb76-114">[Upload document data](/graph/api/printdocument-uploaddata?view=graph-rest-beta) to the document.</span></span>
3. <span data-ttu-id="deb76-115">[启动打印作业](/graph/api/printjob-startprintjob?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="deb76-115">[Start the print job](/graph/api/printjob-startprintjob?view=graph-rest-beta).</span></span>

### <a name="manage-printers"></a><span data-ttu-id="deb76-116">管理打印机</span><span class="sxs-lookup"><span data-stu-id="deb76-116">Manage printers</span></span>

<span data-ttu-id="deb76-117">跟踪组织的打印机、打印机配置和打印机使用情况是一项很复杂的任务。</span><span class="sxs-lookup"><span data-stu-id="deb76-117">Keeping track of an organization's printers, printer configurations, and printer usage is a complex task.</span></span> <span data-ttu-id="deb76-118">通用打印 API 可以在所有三个方面实现集成。</span><span class="sxs-lookup"><span data-stu-id="deb76-118">The Universal Print API enables integration in all three areas.</span></span>

* <span data-ttu-id="deb76-119">使用[列出打印机](/graph/api/print-list-printers?view=graph-rest-beta)和 [printerStatus](/graph/api/resources/printerstatus?view=graph-rest-beta)，**监视打印机状态、配置和可用性**。</span><span class="sxs-lookup"><span data-stu-id="deb76-119">**Keep an eye on printer status, configurations, and availability** by using [List printers](/graph/api/print-list-printers?view=graph-rest-beta) and [printerStatus](/graph/api/resources/printerstatus?view=graph-rest-beta).</span></span>

* <span data-ttu-id="deb76-120">使用报告 API，**了解谁在使用打印机以及打印进度**：</span><span class="sxs-lookup"><span data-stu-id="deb76-120">**See who's using your printers and how much they're printing** by using the reporting APIs:</span></span>
  * [<span data-ttu-id="deb76-121">列出 dailyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="deb76-121">List dailyPrintUsageSummariesByUser</span></span>](/graph/api/reportroot-list-dailyprintusagesummariesbyuser?view=graph-rest-beta)
  * [<span data-ttu-id="deb76-122">列出 monthlyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="deb76-122">List monthlyPrintUsageSummariesByUser</span></span>](/graph/api/reportroot-list-monthlyprintusagesummariesbyuser?view=graph-rest-beta)
  * [<span data-ttu-id="deb76-123">列出 dailyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="deb76-123">List dailyPrintUsageSummariesByPrinter</span></span>](/graph/api/reportroot-list-dailyprintusagesummariesbyprinter?view=graph-rest-beta)
  * [<span data-ttu-id="deb76-124">列出 monthlyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="deb76-124">List monthlyPrintUsageSummariesByPrinter</span></span>](/graph/api/reportroot-list-monthlyprintusagesummariesbyprinter?view=graph-rest-beta)

* <span data-ttu-id="deb76-125">通过修改打印机上的用户和组成员资格，**配置用户权限**：</span><span class="sxs-lookup"><span data-stu-id="deb76-125">**Configure user permissions** by modifying user and group membership on printers:</span></span>
  * [<span data-ttu-id="deb76-126">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="deb76-126">List allowedUsers</span></span>](/graph/api/printer-list-allowedusers?view=graph-rest-beta)
  * [<span data-ttu-id="deb76-127">添加 allowedUser</span><span class="sxs-lookup"><span data-stu-id="deb76-127">Add allowedUser</span></span>](/graph/api/printer-post-allowedusers?view=graph-rest-beta)
  * [<span data-ttu-id="deb76-128">删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="deb76-128">Remove allowedUser</span></span>](/graph/api/printer-delete-alloweduser?view=graph-rest-beta)
  * [<span data-ttu-id="deb76-129">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="deb76-129">List allowedGroups</span></span>](/graph/api/printer-list-allowedgroups?view=graph-rest-beta)
  * [<span data-ttu-id="deb76-130">添加 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="deb76-130">Add allowedGroup</span></span>](/graph/api/printer-post-allowedgroups?view=graph-rest-beta)
  * [<span data-ttu-id="deb76-131">删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="deb76-131">Remove allowedGroup</span></span>](/graph/api/printer-delete-allowedgroup?view=graph-rest-beta)

### <a name="seamlessly-replace-or-update-printer-hardware"></a><span data-ttu-id="deb76-132">无缝更换或更新打印机硬件</span><span class="sxs-lookup"><span data-stu-id="deb76-132">Seamlessly replace or update printer hardware</span></span>

<span data-ttu-id="deb76-133">用户只能看到[共享](/graph/api/print-post-shares?view=graph-rest-beta)的打印机，这样管理员可以精细地控制哪个打印机硬件在给定时间可用。</span><span class="sxs-lookup"><span data-stu-id="deb76-133">Printers are not visible to users until they are [shared](/graph/api/print-post-shares?view=graph-rest-beta), providing administrators fine-grained control over which printer hardware is available at a given time.</span></span>

<span data-ttu-id="deb76-134">共享打印机会创建 [printerShare](/graph/api/resources/printershare?view=graph-rest-beta) 资源，它可随时更新为指向其他打印机，这样就能轻松更换损坏的打印机硬件，或让打印机脱机接受维护。</span><span class="sxs-lookup"><span data-stu-id="deb76-134">Sharing a printer creates a [printerShare](/graph/api/resources/printershare?view=graph-rest-beta) resource that can be updated at any time to point to a different printer, making it easy to replace broken printer hardware or take printers offline for maintenance.</span></span>

<span data-ttu-id="deb76-135">若要在应用程序中使用此功能，请使用[更新 printerShare](/graph/api/printershare-update?view=graph-rest-beta) 来更新 printerShare 的 `printer` 引用。</span><span class="sxs-lookup"><span data-stu-id="deb76-135">To use this in your application, use [Update printerShare](/graph/api/printershare-update?view=graph-rest-beta) to update the printerShare's `printer` reference.</span></span>

### <a name="extending-universal-print-to-support-pull-printing"></a><span data-ttu-id="deb76-136">扩展通用打印以支持拉取打印</span><span class="sxs-lookup"><span data-stu-id="deb76-136">Extending Universal Print to support pull printing</span></span>

<span data-ttu-id="deb76-137">Microsoft Graph 通用打印 API 可让你的应用程序支持拉取打印。</span><span class="sxs-lookup"><span data-stu-id="deb76-137">The Microsoft Graph Universal Print API enables your application to support pull printing.</span></span> <span data-ttu-id="deb76-138">若要设置拉取打印，你需要注册触发器，以便在发生某些打印事件（例如正在启动打印作业）时通知应用程序（通过服务到服务通信）。</span><span class="sxs-lookup"><span data-stu-id="deb76-138">To set up pull printing, you will register triggers that notify your application (via service-to-service communication) when certain print events happen, such as a print job being started.</span></span>

<span data-ttu-id="deb76-139">这些触发器可使应用程序中断打印工作流，以执行将作业重定向到其他打印机和修改文档负载等操作。</span><span class="sxs-lookup"><span data-stu-id="deb76-139">These triggers enable your application to interrupt the print workflow to do things such as redirecting jobs to different printers and modifying the document payload.</span></span>

<span data-ttu-id="deb76-140">按以下步骤启用拉取打印：</span><span class="sxs-lookup"><span data-stu-id="deb76-140">Follow these steps to enable pull printing:</span></span>

1. <span data-ttu-id="deb76-141">使用应用程序权限[创建 printTaskDefinition](/graph/api/print-post-taskdefinitions?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="deb76-141">[Create a printTaskDefinition](/graph/api/print-post-taskdefinitions?view=graph-rest-beta) using application permissions.</span></span> <span data-ttu-id="deb76-142">此抽象任务定义将用于创建为应用程序保留作业的任务。</span><span class="sxs-lookup"><span data-stu-id="deb76-142">This abstract task definition will be used to create task that will hold the job for your application.</span></span> <span data-ttu-id="deb76-143">你需要为每个租户定义至少一个任务定义，可使用任务触发器将其与租户中任意数量的打印机关联（参阅步骤 4）。</span><span class="sxs-lookup"><span data-stu-id="deb76-143">You need to define at least one task definition per tenant, which can be associated with any number of printers in the tenant using task triggers (see step 4).</span></span>

2. <span data-ttu-id="deb76-144">使用管理员身份验证令牌和 `null` **physicalDeviceId** [注册一个或多个虚拟打印机](/graph/api/printer-create?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="deb76-144">[Register one or more virtual printers](/graph/api/printer-create?view=graph-rest-beta) using an administrator authentication token and a `null` **physicalDeviceId**.</span></span> <span data-ttu-id="deb76-145">“虚拟打印机”只是通用打印中没有连接物理设备的打印机对象。</span><span class="sxs-lookup"><span data-stu-id="deb76-145">A "virtual printer" is just a printer object in Universal Print without a physical device attached.</span></span> <span data-ttu-id="deb76-146">通常，用户将打印到虚拟打印机，然后在物理打印设备上执行打印作业。</span><span class="sxs-lookup"><span data-stu-id="deb76-146">Usually, users will print to virtual printers and later pick up their print jobs at a physical print device.</span></span> <span data-ttu-id="deb76-147">请参阅步骤 6。</span><span class="sxs-lookup"><span data-stu-id="deb76-147">See step 6.</span></span>

3. <span data-ttu-id="deb76-148">使用应用程序权限和 `application/ipp` 介质类型[更新虚拟打印机的属性](/graph/api/printer-update?view=graph-rest-beta)（参阅示例）。</span><span class="sxs-lookup"><span data-stu-id="deb76-148">[Update the attributes of your virtual printer](/graph/api/printer-update?view=graph-rest-beta) by using application permissions and an `application/ipp` media type (see examples).</span></span>

4. <span data-ttu-id="deb76-149">使用将任务定义与虚拟打印机相关联的管理员身份验证令牌来[为虚拟打印机创建任务触发器](/graph/api/printer-post-tasktriggers?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="deb76-149">[Create a task trigger for your virtual printer](/graph/api/printer-post-tasktriggers?view=graph-rest-beta) using an administrator authentication token that will associate your task definition with virtual printer.</span></span>

5. <span data-ttu-id="deb76-150">将打印作业提交到虚拟打印机后，由于 [printTaskTrigger](/graph/api/resources/printtasktrigger?view=graph-rest-beta)，它将暂停。</span><span class="sxs-lookup"><span data-stu-id="deb76-150">When a print job is submitted to the virtual printer, it will be paused due to the [printTaskTrigger](/graph/api/resources/printtasktrigger?view=graph-rest-beta).</span></span> <span data-ttu-id="deb76-151">将根据关联的 [printTaskDefinition](/graph/api/resources/printtaskdefinition?view=graph-rest-beta) 创建状态为 `processing` 的 [printTask](/graph/api/resources/printtask?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="deb76-151">A [printTask](/graph/api/resources/printtask?view=graph-rest-beta) with `processing` state will be created based on the associated [printTaskDefinition](/graph/api/resources/printtaskdefinition?view=graph-rest-beta).</span></span>

6. <span data-ttu-id="deb76-152">当用户在物理打印机设备上刷卡时，打印机将通知你的应用程序。</span><span class="sxs-lookup"><span data-stu-id="deb76-152">When the user swipes a badge at a physical printer device, the printer will notify your application.</span></span> <span data-ttu-id="deb76-153">此时，应用程序可以[获取关联虚拟打印机的作业](/graph/api/printer-list-jobs?view=graph-rest-beta)，并将列表筛选为当前用户创建的作业。</span><span class="sxs-lookup"><span data-stu-id="deb76-153">At that time, your application can [fetch the jobs of the associated virtual printer](/graph/api/printer-list-jobs?view=graph-rest-beta) and filter the list to jobs created by the current user.</span></span>

7. <span data-ttu-id="deb76-154">当用户选择要打印的一个或多个作业时，应用程序可以[将打印作业重定向到物理打印机](/graph/api/printjob-redirect?view=graph-rest-beta)，作业将开始打印！</span><span class="sxs-lookup"><span data-stu-id="deb76-154">When the user selects one or more jobs to print, your application can [redirect the print job(s)](/graph/api/printjob-redirect?view=graph-rest-beta) to the physical printer and the job will start printing!</span></span> <span data-ttu-id="deb76-155">仅当关联打印机上有一个 [printTask](/graph/api/resources/printtask?view=graph-rest-beta) 处于 `processing` 状态时，重定向调用才会成功，该打印机是由此应用在步骤 4 中创建的触发器启动的。</span><span class="sxs-lookup"><span data-stu-id="deb76-155">The redirect call will only succeed if there is a [printTask](/graph/api/resources/printtask?view=graph-rest-beta) in `processing` state on the associated printer started by a trigger that this app created in step 4.</span></span> <span data-ttu-id="deb76-156">重定向任务后，该任务将自动设置为 `completed` 状态。</span><span class="sxs-lookup"><span data-stu-id="deb76-156">The task will automatically be set to `completed` state after redirecting it.</span></span>

## <a name="api-reference"></a><span data-ttu-id="deb76-157">API 参考</span><span class="sxs-lookup"><span data-stu-id="deb76-157">API reference</span></span>
<span data-ttu-id="deb76-158">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="deb76-158">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="deb76-159">Microsoft Graph Beta 中的通用打印 API</span><span class="sxs-lookup"><span data-stu-id="deb76-159">Universal Print API in Microsoft Graph beta</span></span>](/graph/api/resources/print?view=graph-rest-beta)

## <a name="see-also"></a><span data-ttu-id="deb76-160">另请参阅</span><span class="sxs-lookup"><span data-stu-id="deb76-160">See also</span></span>

- [<span data-ttu-id="deb76-161">什么是通用打印</span><span class="sxs-lookup"><span data-stu-id="deb76-161">What is Universal Print</span></span>](https://docs.microsoft.com/universal-print/fundamentals/universal-print-whatis)
- <span data-ttu-id="deb76-162">欢迎在 [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 上提供有关通用打印 API 的反馈！</span><span class="sxs-lookup"><span data-stu-id="deb76-162">We'd love to hear your feedback about the Universal Print APIs over at [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)!</span></span>
