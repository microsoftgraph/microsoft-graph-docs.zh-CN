---
title: Excel 工作簿和图表 API 概述
description: Excel 是一个提高工作效率不可或缺的工具。 所有行业和工作职能的用户都将其视为用于存储、跟踪和操作各类数据的工具。 从简单的任务跟踪和数据管理，到复杂的计算和专业报告，Excel 可用于处理各种各样的任务。 你可以使用 Microsoft Graph 中的 Excel REST API 扩展数据、计算、报告和仪表板的价值。
localization_priority: Priority
author: lumine2008
ms.prod: excel
ms.custom: scenarios:getting-started
ms.openlocfilehash: 3d3d09635bbe69d787d684b346d460854df4413e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897230"
---
# <a name="excel-workbooks-and-charts-api-overview"></a><span data-ttu-id="11a1c-106">Excel 工作簿和图表 API 概述</span><span class="sxs-lookup"><span data-stu-id="11a1c-106">Excel workbooks and charts API overview</span></span>

<span data-ttu-id="11a1c-107">Excel 是一个提高工作效率不可或缺的工具。</span><span class="sxs-lookup"><span data-stu-id="11a1c-107">Excel is an indispensable productivity tool.</span></span> <span data-ttu-id="11a1c-108">所有行业和工作职能的用户都将其视为用于存储、跟踪和操作各类数据的工具。</span><span class="sxs-lookup"><span data-stu-id="11a1c-108">Users across all industries and job functions embrace it as a tool for storing, tracking, and manipulating all kinds of data.</span></span> <span data-ttu-id="11a1c-109">从简单的任务跟踪和数据管理，到复杂的计算和专业报告，Excel 可用于处理各种各样的任务。</span><span class="sxs-lookup"><span data-stu-id="11a1c-109">It's used for everything from simple task tracking and data management, to complex calculations and professional reporting.</span></span> <span data-ttu-id="11a1c-110">你可以使用 Microsoft Graph 中的 Excel REST API 扩展数据、计算、报告和仪表板的价值。</span><span class="sxs-lookup"><span data-stu-id="11a1c-110">You can use the Excel REST API in Microsoft Graph to extend the value of your data, calculations, reporting, and dashboards.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/I1rSkJww2Dk]

## <a name="why-integrate-with-excel"></a><span data-ttu-id="11a1c-111">为什么与 Excel 集成？</span><span class="sxs-lookup"><span data-stu-id="11a1c-111">Why integrate with Excel?</span></span>

<span data-ttu-id="11a1c-112">你可以使用 Microsoft Graph 来让 Web 和移动应用程序读取和修改存储在 OneDrive、SharePoint 或其他支持的存储平台中的 Excel 工作簿。</span><span class="sxs-lookup"><span data-stu-id="11a1c-112">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive, SharePoint, or other supported storage platforms.</span></span>

### <a name="perform-calculations"></a><span data-ttu-id="11a1c-113">执行计算</span><span class="sxs-lookup"><span data-stu-id="11a1c-113">Perform calculations</span></span>

<span data-ttu-id="11a1c-114">用户喜欢他们可以轻松地在 Excel 中执行深入而复杂的计算。</span><span class="sxs-lookup"><span data-stu-id="11a1c-114">Users love the ease with which they can perform deep and complex calculations within Excel.</span></span> <span data-ttu-id="11a1c-115">现在，你可以使用 Excel 强大的计算引擎，并且可以立即得到结果。</span><span class="sxs-lookup"><span data-stu-id="11a1c-115">You can now access Excel’s powerful calculation engine with instant results.</span></span> <span data-ttu-id="11a1c-116">例如，按揭贷款计算器通过简单的 API 调用（包括付款的本金、利率和付款次数）即可利用 Excel 中的 PMT 函数。</span><span class="sxs-lookup"><span data-stu-id="11a1c-116">For example, a mortgage calculator can take advantage of the PMT function from Excel by making a simple API call that includes principal, rate and number of payments.</span></span> <span data-ttu-id="11a1c-117">Excel 将进行所有的复杂计算，并立即返回每月付款。</span><span class="sxs-lookup"><span data-stu-id="11a1c-117">Excel does all the difficult work and returns the monthly payment instantly.</span></span> <span data-ttu-id="11a1c-118">当前提供有 300 多个 Excel 工作表函数，你可以完全访问 Excel 目前支持的各种公式。</span><span class="sxs-lookup"><span data-stu-id="11a1c-118">With more than 300 Excel worksheet functions currently available, you have full access to the breadth of formulas supported by Excel today.</span></span> <span data-ttu-id="11a1c-119">不需要反复重建复杂业务模型。</span><span class="sxs-lookup"><span data-stu-id="11a1c-119">Complex business models don’t need to be rebuilt repeatedly.</span></span> <span data-ttu-id="11a1c-120">开发者可以对 Excel 编程以立即执行这些计算，并使用简单 API 调用检索这些结果。</span><span class="sxs-lookup"><span data-stu-id="11a1c-120">Developers can program Excel to perform those calculations instantly and retrieve the results with simple API calls.</span></span>

### <a name="generate-reports-and-analyze-results"></a><span data-ttu-id="11a1c-121">生成报告并分析结果</span><span class="sxs-lookup"><span data-stu-id="11a1c-121">Generate reports and analyze results</span></span>

<span data-ttu-id="11a1c-122">Excel 是一款灵活的报告和分析工具，范围从简单的数据表到复杂的专业仪表板。</span><span class="sxs-lookup"><span data-stu-id="11a1c-122">Excel is a flexible reporting and analysis tool, from simple data tables to complex professional dashboards.</span></span> <span data-ttu-id="11a1c-123">现在，我们为你提供了访问 Excel 报告功能的完整权限，使 Excel 成为 Microsoft 365 中的一个在线报告服务。</span><span class="sxs-lookup"><span data-stu-id="11a1c-123">Today, we give you full access to all of Excel’s reporting features, making Excel an online reporting service within Microsoft 365.</span></span> <span data-ttu-id="11a1c-124">想象一下：用户目前创建和依赖的所有报告方案都拉入到一个自定义应用，以创建专业图表或智能分析大量数据，从而将 Excel 无缝融合到这些自定义的体验中。</span><span class="sxs-lookup"><span data-stu-id="11a1c-124">Imagine any of the reporting scenarios users create and rely on today pulled into a custom app to create professional charts or analyze large sets of data intelligently, seamlessly blending Excel into those customized experiences.</span></span>

### <a name="store-and-track-data"></a><span data-ttu-id="11a1c-125">存储和跟踪数据</span><span class="sxs-lookup"><span data-stu-id="11a1c-125">Store and track data</span></span>

<span data-ttu-id="11a1c-126">Excel 还是一款出色的存储和跟踪数据的工具。</span><span class="sxs-lookup"><span data-stu-id="11a1c-126">Excel is also a great tool to store and track data.</span></span> <span data-ttu-id="11a1c-127">如果信息存储在工作簿中，则与 Microsoft 365 集成的任何应用都可以访问该数据。</span><span class="sxs-lookup"><span data-stu-id="11a1c-127">If your information is stored in a workbook, that data is available to any app that integrates with Microsoft 365.</span></span> <span data-ttu-id="11a1c-128">可以从自定义解决方案读取其内容，并且这些解决方案可以使用 Excel 来存储数据。</span><span class="sxs-lookup"><span data-stu-id="11a1c-128">Its contents are available to read from custom solutions, and those solutions can use Excel for data storage.</span></span>

><span data-ttu-id="11a1c-129">**注意：** Excel REST API 仅支持 Office Open XML 文件格式的工作簿（扩展名为 `.xlsx` 的文件）。</span><span class="sxs-lookup"><span data-stu-id="11a1c-129">**Note:** The Excel REST API supports only Office Open XML file formatted workbooks (files with the`.xlsx` extension).</span></span> <span data-ttu-id="11a1c-130">不支持扩展名为 `.xls` 的工作簿。</span><span class="sxs-lookup"><span data-stu-id="11a1c-130">The `.xls` extension workbooks are not supported.</span></span> 

### <a name="using-the-excel-rest-api"></a><span data-ttu-id="11a1c-131">使用 Excel REST API</span><span class="sxs-lookup"><span data-stu-id="11a1c-131">Using the Excel REST API</span></span>
<span data-ttu-id="11a1c-132">你可以使用 Microsoft Graph 来让 Web 和移动应用程序读取和修改存储在 OneDrive、SharePoint 或其他支持的存储平台中的 Excel 工作簿。</span><span class="sxs-lookup"><span data-stu-id="11a1c-132">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive, SharePoint, or other supported storage platforms.</span></span> <span data-ttu-id="11a1c-133">`Workbook`（或 Excel 文件）资源通过关系包含所有其他 Excel 资源。</span><span class="sxs-lookup"><span data-stu-id="11a1c-133">The `Workbook` (or Excel file) resource contains all the other Excel resources through relationships.</span></span> <span data-ttu-id="11a1c-134">你可以通过标识文件在该 URL 中的位置，借助 Drive API 访问工作簿。</span><span class="sxs-lookup"><span data-stu-id="11a1c-134">You can access a workbook through the Drive API by identifying the location of the file in the URL.</span></span> <span data-ttu-id="11a1c-135">例如：</span><span class="sxs-lookup"><span data-stu-id="11a1c-135">For example:</span></span>

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`

`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/`

<span data-ttu-id="11a1c-136">可以通过使用标准 REST API 访问一组 Excel 对象（例如表、区域或图表），以便对工作簿执行创建、读取、更新和删除 (CRUD) 操作。</span><span class="sxs-lookup"><span data-stu-id="11a1c-136">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform create, read, update, and delete (CRUD) operations on the workbook.</span></span>

## <a name="api-reference"></a><span data-ttu-id="11a1c-137">API 参考</span><span class="sxs-lookup"><span data-stu-id="11a1c-137">API reference</span></span>
<span data-ttu-id="11a1c-138">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="11a1c-138">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="11a1c-139">Microsoft Graph v1.0 中的 Excel API</span><span class="sxs-lookup"><span data-stu-id="11a1c-139">Excel API in Microsoft Graph v1.0</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
- [<span data-ttu-id="11a1c-140">Microsoft Graph beta 中的 Excel API</span><span class="sxs-lookup"><span data-stu-id="11a1c-140">Excel API in Microsoft Graph beta</span></span>](/graph/api/resources/excel?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="11a1c-141">后续步骤</span><span class="sxs-lookup"><span data-stu-id="11a1c-141">Next steps</span></span>

* [<span data-ttu-id="11a1c-142">通过 Microsoft Graph 管理 Excel 会话</span><span class="sxs-lookup"><span data-stu-id="11a1c-142">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="11a1c-143">使用 Microsoft Graph 编写 Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="11a1c-143">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="11a1c-144">通过 Microsoft Graph 使用 Excel 工作簿函数</span><span class="sxs-lookup"><span data-stu-id="11a1c-144">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="11a1c-145">通过 Microsoft Graph 更新 Excel 区域的格式</span><span class="sxs-lookup"><span data-stu-id="11a1c-145">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="11a1c-146">通过 Microsoft Graph 显示 Excel 图表图像</span><span class="sxs-lookup"><span data-stu-id="11a1c-146">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="11a1c-147">使用 Excel REST API</span><span class="sxs-lookup"><span data-stu-id="11a1c-147">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
