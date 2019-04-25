---
title: Business Central API 概述
description: 概述为什么要将您的解决方案与业务中心 api 集成。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0602b02592bec5210f243f77654a52ba96e6746a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526151"
---
# <a name="dynamics-365-business-central-api-overview-preview"></a><span data-ttu-id="2d320-103">Dynamics 365 Business 中央 API 概述 (预览)</span><span class="sxs-lookup"><span data-stu-id="2d320-103">Dynamics 365 Business Central API overview (preview)</span></span>
<span data-ttu-id="2d320-104">Dynamics 365 business Central 是一个易于使用和调整的一体式业务管理解决方案, 可帮助您连接业务并做出更明智的决策。</span><span class="sxs-lookup"><span data-stu-id="2d320-104">Dynamics 365 Business Central is an all-in-one business management solution that is easy to use and adapt, helping you connect your business and make smarter decisions.</span></span> <span data-ttu-id="2d320-105">它提供了业务的端到端视图, 使您能够管理财务、自动化和保护供应链、更智能化地销售和改进客户服务、使项目按时完成并在预算范围之内, 并优化您的操作。</span><span class="sxs-lookup"><span data-stu-id="2d320-105">It provides an end-to-end view of your business, enabling you to manage your financials, automate and secure your supply chain, sell smarter and improve customer service, keep projects on time and under budget, and optimize your operations.</span></span>

## <a name="why-integrate-with-dynamics-365-business-central"></a><span data-ttu-id="2d320-106">为什么要与 Dynamics 365 业务中心集成？</span><span class="sxs-lookup"><span data-stu-id="2d320-106">Why integrate with Dynamics 365 Business Central?</span></span>
<span data-ttu-id="2d320-107">通过将应用与 Dynamics 365 业务中心集成, 可以创建满足业务需求的经验。</span><span class="sxs-lookup"><span data-stu-id="2d320-107">By integrating your apps with Dynamics 365 Business Central, you can create experiences that span your business needs.</span></span> <span data-ttu-id="2d320-108">您可以创建可让用户执行关键业务任务和功能的解决方案。</span><span class="sxs-lookup"><span data-stu-id="2d320-108">You can create solutions that empower your users to perform key business tasks and functions.</span></span> <span data-ttu-id="2d320-109">您可以使用 Microsoft Graph 访问和管理您的财务、与业务联系人合作、创建和发送销售和采购文档, 并从财务报表获取见解。</span><span class="sxs-lookup"><span data-stu-id="2d320-109">You can use Microsoft Graph to access and manage your financials, work with business contacts, create and send sales and purchasing documents, and gain insights from financial reports.</span></span> 

### <a name="synchronize-your-business-applications"></a><span data-ttu-id="2d320-110">同步业务应用程序</span><span class="sxs-lookup"><span data-stu-id="2d320-110">Synchronize your business applications</span></span>
<span data-ttu-id="2d320-111">许多公司使用不同的断开连接的业务应用程序来管理企业的各种功能。</span><span class="sxs-lookup"><span data-stu-id="2d320-111">Many companies use different, disconnected business applications to manage various functions of the business.</span></span> <span data-ttu-id="2d320-112">通过 Microsoft Graph, 可以连接数据以将这些应用程序一起引入。</span><span class="sxs-lookup"><span data-stu-id="2d320-112">Microsoft Graph enables you to connect the data to bring these applications together.</span></span> <span data-ttu-id="2d320-113">这使您可以轻松地将工资应用程序连接到员工记录, 将您的费用应用程序连接到供应商记录, 并让您的 CRM 应用程序保持您的客户记录保持最新。</span><span class="sxs-lookup"><span data-stu-id="2d320-113">This makes it easy to connect your payroll application to employee records, connect your expense application to vendor records, and have your CRM application keep your customer records up to date.</span></span> <span data-ttu-id="2d320-114">连接数据以保持应用程序同步。</span><span class="sxs-lookup"><span data-stu-id="2d320-114">Connect your data to keep your applications in sync.</span></span>

### <a name="create-custom-apps-to-manage-your-business-processes"></a><span data-ttu-id="2d320-115">创建用于管理业务流程的自定义应用程序</span><span class="sxs-lookup"><span data-stu-id="2d320-115">Create custom apps to manage your business processes</span></span>
<span data-ttu-id="2d320-116">每个企业都不同, 并且可以有专门的业务流程。</span><span class="sxs-lookup"><span data-stu-id="2d320-116">Every business is different and can have specialized business processes.</span></span> <span data-ttu-id="2d320-117">可以使用针对此过程量身定制的自定义应用程序简化这些过程。</span><span class="sxs-lookup"><span data-stu-id="2d320-117">These processes can be streamlined with custom apps tailored to the process.</span></span> <span data-ttu-id="2d320-118">使用 Microsoft Graph, 可以轻松地将这些应用与财务数据集成。</span><span class="sxs-lookup"><span data-stu-id="2d320-118">Microsoft Graph makes it easy to integrate these apps with your financial data.</span></span> <span data-ttu-id="2d320-119">建立 sales 或 field service 应用程序来创建销售文档、创建采购文档的费用应用程序或创建总帐日志的工资应用程序是可行的, 并将所有文档保留在财务系统中。</span><span class="sxs-lookup"><span data-stu-id="2d320-119">Building a sales or field service app that creates sales documents, an expense app that creates purchasing documents, or a payroll app that creates general ledger journals becomes possible, keeping all your documents in your financial system.</span></span>

### <a name="gain-insights-from-your-financial-data"></a><span data-ttu-id="2d320-120">深入了解你的财务数据</span><span class="sxs-lookup"><span data-stu-id="2d320-120">Gain insights from your financial data</span></span>
<span data-ttu-id="2d320-121">Microsoft Graph 提供了对财务报告的访问权限。</span><span class="sxs-lookup"><span data-stu-id="2d320-121">Microsoft Graph provides access to your financial reports.</span></span> <span data-ttu-id="2d320-122">将 BI 工具和应用程序连接到资产负债表、现金流量表、应付帐款和应收帐款帐龄报告和试用余额报告, 以创建 BI 仪表板, 并确保用户有权访问他们所需的信息。</span><span class="sxs-lookup"><span data-stu-id="2d320-122">Connect BI tools and apps to your balance sheet, cash flow statement, payables and receivables aging reports, and trial balance reports to create BI dashboards and ensure that users have access to the information they need.</span></span>

## <a name="authorization"></a><span data-ttu-id="2d320-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d320-123">Authorization</span></span>
<span data-ttu-id="2d320-124">使用 Azure AD v2.0 终结点对 Dynamics 365 Business Central api 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="2d320-124">Use the Azure AD v2.0 endpoint to authenticate Dynamics 365 Business Central APIs.</span></span> <span data-ttu-id="2d320-125">所有 api 都需要`Authorization: Bearer {access-token}`请求标头。</span><span class="sxs-lookup"><span data-stu-id="2d320-125">All APIs require the `Authorization: Bearer {access-token}` request header.</span></span> <span data-ttu-id="2d320-126">有关授权的详细信息, 请参阅[获取访问令牌以调用 Microsoft Graph](auth-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="2d320-126">For more information about authorization, see [Get access tokens to call Microsoft Graph](auth-overview.md).</span></span>

## <a name="api-reference"></a><span data-ttu-id="2d320-127">API 参考</span><span class="sxs-lookup"><span data-stu-id="2d320-127">API reference</span></span>
<span data-ttu-id="2d320-128">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="2d320-128">Looking for the API reference for this service?</span></span>

<span data-ttu-id="2d320-129">请参阅[Dynamics 365 Business Central API in Microsoft Graph beta 版](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="2d320-129">See [Dynamics 365 Business Central API in Microsoft Graph beta](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta).</span></span>


## <a name="next-steps"></a><span data-ttu-id="2d320-130">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2d320-130">Next steps</span></span>
<span data-ttu-id="2d320-131">了解有关 Microsoft Graph 中支持的[业务中心 API 和使用案例](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2d320-131">Find out more about the [Business Central API and use cases](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta) supported in Microsoft Graph.</span></span>
