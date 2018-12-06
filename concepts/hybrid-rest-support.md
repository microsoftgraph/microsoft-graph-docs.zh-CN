---
title: 使用 REST API 访问 Exchange 混合部署中的邮箱（预览）
description: 在属于 Office 365 的 Exchange Online 中，Microsoft Graph 始终提供对云中客户邮箱的访问权限。
ms.openlocfilehash: 78b324765c580e76f080e2e8023e52617b3851f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091760"
---
# <a name="use-rest-apis-to-access-mailboxes-in-exchange-hybrid-deployments-preview"></a><span data-ttu-id="5c77e-103">使用 REST API 访问 Exchange 混合部署中的邮箱（预览版）</span><span class="sxs-lookup"><span data-stu-id="5c77e-103">Use REST APIs to access mailboxes in Exchange hybrid deployments (preview)</span></span>

<span data-ttu-id="5c77e-104">在作为 Office 365 一部分的 Exchange Online 中，Microsoft Graph 始终提供对云中客户邮箱的访问权限。</span><span class="sxs-lookup"><span data-stu-id="5c77e-104">Microsoft Graph has always provided access to customer mailboxes in the cloud on Exchange Online as part of Office 365.</span></span>
<span data-ttu-id="5c77e-105">Exchange 本地服务器的 Exchange 2016 累积更新 3 (CU3) 于 2016 年 9 月发布，增加了对 REST API 与 Office 365 集成的支持。</span><span class="sxs-lookup"><span data-stu-id="5c77e-105">Exchange 2016 Cumulative Update 3 (CU3), released in September 2016 for Exchange on-premises servers, adds support for REST API integration with Office 365.</span></span> <span data-ttu-id="5c77e-106">如果你的应用使用 v1.0 的[邮件](/graph/api/resources/message?view=graph-rest-1.0)、[日历](/graph/api/resources/calendar?view=graph-rest-1.0)或[联系人](/graph/api/resources/contact?view=graph-rest-1.0) API，则只要部署满足特定的[要求](#requirements-for-the-rest-api-to-work-in-hybrid-deployments)，现在还可以在_混合_部署中找到无缝的身份验证和应用程序体验，而不论该邮箱是在本地还是在云中。</span><span class="sxs-lookup"><span data-stu-id="5c77e-106">If your app uses v1.0 of the [Mail](/graph/api/resources/message?view=graph-rest-1.0), [Calendar](/graph/api/resources/calendar?view=graph-rest-1.0), or [Contacts](/graph/api/resources/contact?view=graph-rest-1.0) API, you will now also find a seamless authentication and application experience in _hybrid_ deployments, regardless of whether the mailbox is on-premises or in the cloud, provided that the deployment meets specific [requirements](#requirements-for-the-rest-api-to-work-in-hybrid-deployments).</span></span> 


<span data-ttu-id="5c77e-p102">当 Microsoft Graph 在后台识别到一个 REST API 调用正在尝试访问混合部署中的本地邮箱时，它会将 REST 请求代理到本地 REST 终结点，然后处理此请求。此发现使得访问 REST API 成为可能。</span><span class="sxs-lookup"><span data-stu-id="5c77e-p102">Behind the scenes, when Microsoft Graph identifies that a REST API call is attempting to access an on-premises mailbox in a hybrid deployment, it proxies the REST request to an on-premises REST endpoint which then processes the request. This discovery makes accessing the REST API possible.</span></span>

><span data-ttu-id="5c77e-109">**注意：** 在混合部署中使用这些 REST API 的功能目前处于预览阶段。</span><span class="sxs-lookup"><span data-stu-id="5c77e-109">**Note:** The ability to use these REST APIs in hybrid deployments is currently in preview.</span></span>

><span data-ttu-id="5c77e-p103">只有 v1.0 的邮件、日历和联系人 API 可用于混合部署中的邮箱。其他 v1.0 API 集，如[组](/graph/api/resources/group?view=graph-rest-1.0) API，或者其他版本中的 API 都不能用于上述邮箱。如果尝试使用的 API 不是混合部署中受支持的 API 集，则会收到以下错误消息：</span><span class="sxs-lookup"><span data-stu-id="5c77e-p103">Only v1.0 of the Mail, Calendar and Contacts API are available for mailboxes in hybrid deployments. Other v1.0 API sets, such as the [Groups](/graph/api/resources/group?view=graph-rest-1.0) API, or APIs in other versions, are not. If you attempt to use an API that is not part of the supported set in a hybrid deployment, you will get the following error message:</span></span>

><span data-ttu-id="5c77e-113">“此邮箱的 REST API 当前处于预览阶段。</span><span class="sxs-lookup"><span data-stu-id="5c77e-113">"REST APIs for this mailbox are currently in preview.</span></span> <span data-ttu-id="5c77e-114">可以在 https://dev.outlook.com 中查找有关预览 REST API 的详细信息。”</span><span class="sxs-lookup"><span data-stu-id="5c77e-114">You can find more information about the preview REST APIs at https://dev.outlook.com."</span></span>

## <a name="requirements-for-the-rest-api-to-work-in-hybrid-deployments"></a><span data-ttu-id="5c77e-115">REST API 用于混合部署的要求</span><span class="sxs-lookup"><span data-stu-id="5c77e-115">Requirements for the REST API to work in hybrid deployments</span></span>

<span data-ttu-id="5c77e-116">Microsoft Graph 提供开放性（支持 JSON、OAUTH 和 ODATA 等开放标准，从大多数主流平台连接）和灵活性（用户数据的精确、范围严格的访问权限）。</span><span class="sxs-lookup"><span data-stu-id="5c77e-116">Microsoft Graph provides openness (open standards support like JSON, OAUTH and ODATA, connecting from most popular platforms) and flexibility (granular, tightly scoped permissions to access user data).</span></span> <span data-ttu-id="5c77e-117">如果贵组织有兴趣启用 Microsoft Graph 应用开发，并且正在使用或考虑混合部署，请注意以下部署要求：</span><span class="sxs-lookup"><span data-stu-id="5c77e-117">If your organization is interested in enabling Microsoft Graph app development and is currently in or considering a hybrid deployment, be aware of the following deployment requirements:</span></span>

- <span data-ttu-id="5c77e-118">邮箱要求</span><span class="sxs-lookup"><span data-stu-id="5c77e-118">Mailbox requirements</span></span>

  - <span data-ttu-id="5c77e-119">所有将使用 REST API 的本地邮箱必须位于处于 Exchange 2016 CU3 服务器的数据库中。</span><span class="sxs-lookup"><span data-stu-id="5c77e-119">All on-premises mailboxes that will use the REST APIs must be located on databases located on Exchange 2016 CU3 servers.</span></span> 

- <span data-ttu-id="5c77e-120">基础结构要求</span><span class="sxs-lookup"><span data-stu-id="5c77e-120">Infrastructure requirements</span></span>

  - <span data-ttu-id="5c77e-121">所有 Exchange 2016 服务器必须升级到 CU3 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="5c77e-121">All Exchange 2016 servers must be upgraded to CU3 or later.</span></span>  
  - <span data-ttu-id="5c77e-122">本地 Active Directory 必须与 Azure Active Directory 同步。</span><span class="sxs-lookup"><span data-stu-id="5c77e-122">On-premises Active Directory must synchronize with Azure Active Directory.</span></span>
  - <span data-ttu-id="5c77e-123">必须将同一负载平衡的数组上与 Exchange 2016 服务器共存的所有 Exchange 2013 服务器从数组中删除。</span><span class="sxs-lookup"><span data-stu-id="5c77e-123">Any Exchange 2013 servers coexisting in the same load-balanced array with Exchange 2016 servers must be removed from the array.</span></span>

- <span data-ttu-id="5c77e-124">网络要求</span><span class="sxs-lookup"><span data-stu-id="5c77e-124">Networking requirements</span></span>

  - <span data-ttu-id="5c77e-125">从 DNS 的角度看，自动发现命名空间和本地客户端命名空间必须具有 Internet DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="5c77e-125">From a DNS perspective, the Autodiscover namespace and on-premises client namespace must have Internet DNS records.</span></span> 
  - <span data-ttu-id="5c77e-126">如果具有检查和限制访问的防火墙或应用程序网关，请更新相应的设置，以允许进行发现和访问。</span><span class="sxs-lookup"><span data-stu-id="5c77e-126">If you have a firewall or application gateway that inspects and restricts access, update the appropriate settings to allow discovery and access.</span></span>


<span data-ttu-id="5c77e-127">IT 管理员可以在以下资源中找到详细信息：</span><span class="sxs-lookup"><span data-stu-id="5c77e-127">IT administrators can find more information in the following resources:</span></span>

- <span data-ttu-id="5c77e-128">
  [Exchange Server 混合部署](https://technet.microsoft.com/zh-CN/library/jj200581(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="5c77e-128">[Exchange Server Hybrid Deployments](https://technet.microsoft.com/en-us/library/jj200581(v=exchg.150).aspx)</span></span>
- [<span data-ttu-id="5c77e-129">2016 年 9 月累积更新版本</span><span class="sxs-lookup"><span data-stu-id="5c77e-129">September 2016 Cumulative Update Release</span></span>](https://blogs.technet.microsoft.com/exchange/2016/09/20/released-september-2016-quarterly-exchange-updates/) 
- [<span data-ttu-id="5c77e-130">针对 REST API 的本地体系结构要求</span><span class="sxs-lookup"><span data-stu-id="5c77e-130">On-Premises Architectural Requirements for the REST API</span></span>](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api/)
