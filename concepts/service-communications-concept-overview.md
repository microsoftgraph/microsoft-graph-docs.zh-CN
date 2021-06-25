---
title: 通过 Microsoft Graph 访问服务运行状况和通信的概述
description: 使用 Microsoft Graph 中的服务通信 API 访问有关 Microsoft 云服务的运行状况和消息中心帖子。
author: payiAzure
localization_priority: Priority
ms.prod: service-communications
ms.custom: scenarios:getting-started
ms.openlocfilehash: f10aabbdbdb7028af3f16058a6137bd9da8615d6
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108961"
---
# <a name="overview-for-accessing-service-health-and-communications-in-microsoft-graph"></a><span data-ttu-id="337d2-103">在 Microsoft Graph 中访问服务运行状况和通信的概述</span><span class="sxs-lookup"><span data-stu-id="337d2-103">Overview for accessing service health and communications in Microsoft Graph</span></span>
<span data-ttu-id="337d2-104">可以使用 Microsoft Graph 中的服务通信 API 访问有关 Microsoft 云服务的运行状况和消息中心帖子。</span><span class="sxs-lookup"><span data-stu-id="337d2-104">You can use the service communications API in Microsoft Graph to access the health status and message center posts about Microsoft cloud services.</span></span> <span data-ttu-id="337d2-105">实际运行状况和帖子对应于 API 所支持且由租户订阅的 Microsoft 365 和 Dynamics 365 服务。</span><span class="sxs-lookup"><span data-stu-id="337d2-105">The actual health status and posts correspond to the Microsoft 365 and Dynamics 365 services that are supported by the API and subscribed by the tenant.</span></span>

## <a name="why-integrate-with-service-health-and-communications-data"></a><span data-ttu-id="337d2-106">为何与服务运行状况和通信数据集成？</span><span class="sxs-lookup"><span data-stu-id="337d2-106">Why integrate with service health and communications data?</span></span>

### <a name="get-service-health-and-message-center-posts-for-a-tenant"></a><span data-ttu-id="337d2-107">获取租户的服务运行状况和消息中心帖子</span><span class="sxs-lookup"><span data-stu-id="337d2-107">Get service health and message center posts for a tenant</span></span>
<span data-ttu-id="337d2-108">客户可以获取受支持 Microsoft 服务的当前或历史运行状况数据。</span><span class="sxs-lookup"><span data-stu-id="337d2-108">Customers can get current or historical health data of supported Microsoft services.</span></span> <span data-ttu-id="337d2-109">当遇到 Microsoft 服务问题时，客户可以检查其运行状况，以验证是否已通过正在进行的解决方法识别问题，然后再请求支持或花费时间进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="337d2-109">When experiencing problems with a Microsoft service, they can check its health status to verify if an issue has been identified with a resolution in progress, before calling for support or spending time troubleshooting.</span></span> 

<span data-ttu-id="337d2-110">客户可以定期查看消息中心帖子，以跟踪即将发布的新功能和更新以及其他重要公告。</span><span class="sxs-lookup"><span data-stu-id="337d2-110">Customers can regularly review message center posts to keep track of upcoming new features and updates, and other important announcements.</span></span> <span data-ttu-id="337d2-111">然后，他们可以预测这些更改对用户有何影响，并制定相应的计划。</span><span class="sxs-lookup"><span data-stu-id="337d2-111">They can then anticipate how these changes may affect users and plan accordingly.</span></span>

### <a name="integrate-service-communications-data-into-custom-workflows"></a><span data-ttu-id="337d2-112">将服务通信数据集成到自定义工作流中</span><span class="sxs-lookup"><span data-stu-id="337d2-112">Integrate service communications data into custom workflows</span></span>
<span data-ttu-id="337d2-113">应用开发人员可以将活动服务运行状况问题直接集成到自定义应用程序中，从而允许管理员进行会审并与受影响的访问群体共享状态信息。</span><span class="sxs-lookup"><span data-stu-id="337d2-113">App developers can integrate active service health issues directly into custom applications, allowing administrators to triage and share status information with impacted audiences.</span></span>

<span data-ttu-id="337d2-114">应用可以启用自定义工作流，以便管理员从消息中心查看、分配和会审更改通信。</span><span class="sxs-lookup"><span data-stu-id="337d2-114">Apps can enable custom workflows for administrators to review, assign, and triage change communications from the message center.</span></span>

### <a name="build-customer-facing-dashboards"></a><span data-ttu-id="337d2-115">构建面向客户的仪表板</span><span class="sxs-lookup"><span data-stu-id="337d2-115">Build customer-facing dashboards</span></span>

<span data-ttu-id="337d2-116">使用面向客户的仪表板创建应用程序，以显示Microsoft 服务的运行状况，并允许客户跟踪即将发生的更改以及有关服务的其他重要公告。</span><span class="sxs-lookup"><span data-stu-id="337d2-116">Create applications with customer-facing dashboards to show the health of Microsoft services, and let customers keep track of upcoming changes and other important announcements about the services.</span></span>


## <a name="dashboards-examples-in-microsoft-365-admin-center"></a><span data-ttu-id="337d2-117">Microsoft 365 管理中心中的仪表板示例</span><span class="sxs-lookup"><span data-stu-id="337d2-117">Dashboards examples in Microsoft 365 admin center</span></span>
<span data-ttu-id="337d2-118">本部分演示 [Microsoft 365 管理中心](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/homepage) 中使用服务通信 API 生成各自运行状况仪表板的示例。</span><span class="sxs-lookup"><span data-stu-id="337d2-118">This section shows examples in the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/homepage) that uses the service communications API to build respective health dashboards.</span></span> <span data-ttu-id="337d2-119">使用管理员帐户登录管理中心，然后单击“**运行状况**”以查看以下仪表板：</span><span class="sxs-lookup"><span data-stu-id="337d2-119">Sign in to the admin center with an admin account, then click **Health** to see the following dashboards:</span></span>
- [<span data-ttu-id="337d2-120">服务运行状况</span><span class="sxs-lookup"><span data-stu-id="337d2-120">Service health</span></span>](#service-health-dashboard)
- [<span data-ttu-id="337d2-121">Windows 版本运行状况</span><span class="sxs-lookup"><span data-stu-id="337d2-121">Windows release health</span></span>](#windows-release-health-dashboard)
- [<span data-ttu-id="337d2-122">消息中心</span><span class="sxs-lookup"><span data-stu-id="337d2-122">Message center</span></span>](#message-center-dashboard)

### <a name="service-health-dashboard"></a><span data-ttu-id="337d2-123">服务运行状况仪表板</span><span class="sxs-lookup"><span data-stu-id="337d2-123">Service health dashboard</span></span>

<span data-ttu-id="337d2-124">在 **服务运行状况** 仪表板中，可以查看订阅的Microsoft 服务的运行状况，其中可以包括 Office 网页版、Yammer、Microsoft Dynamics CRM 和移动设备管理云服务。</span><span class="sxs-lookup"><span data-stu-id="337d2-124">From the **Service health** dashboad, you can view the health of your subscribed Microsoft services, which can include Office on the web, Yammer, Microsoft Dynamics CRM, and mobile device management cloud services.</span></span> <span data-ttu-id="337d2-125">请参阅图 1 中所述的示例。</span><span class="sxs-lookup"><span data-stu-id="337d2-125">See examples as demarcated in figure 1.</span></span>

<span data-ttu-id="337d2-126">**图 1. Microsoft 365 管理中心中的服务运行状况仪表板**</span><span class="sxs-lookup"><span data-stu-id="337d2-126">**Figure 1. Service health dashboard in Microsoft 365 admin center**</span></span>

![用户 Microsoft 365 管理中心服务运行状况仪表板的屏幕截图](images/service-communications-concept-overview-admin-center-serviceHealth2.png)

### <a name="windows-release-health-dashboard"></a><span data-ttu-id="337d2-128">Windows 版本运行状况仪表板</span><span class="sxs-lookup"><span data-stu-id="337d2-128">Windows release health dashboard</span></span>

<span data-ttu-id="337d2-129">从 **Windows 版本运行状况** 仪表板，可以查看有关每月质量和功能更新的重要信息，以及 Windows 的最新功能和增强功能。</span><span class="sxs-lookup"><span data-stu-id="337d2-129">From the **Windows release health** dashboad, you can view essential information about monthly quality and feature updates, and the latest features and enhancements for Windows.</span></span> <span data-ttu-id="337d2-130">请参阅图 2 中所述的示例。</span><span class="sxs-lookup"><span data-stu-id="337d2-130">See an example as demarcated in figure 2.</span></span>

<span data-ttu-id="337d2-131">**图 2. Microsoft 365 管理中心中的 Windows 版本运行状况仪表板**</span><span class="sxs-lookup"><span data-stu-id="337d2-131">**Figure 2. Windows release health dashboard in Microsoft 365 admin center**</span></span>

![用户 Microsoft 365 管理中心 Windows 版本运行状况仪表板的屏幕截图](images/service-communications-concept-overview-admin-center-windowshealth2.png)


### <a name="message-center-dashboard"></a><span data-ttu-id="337d2-133">消息中心仪表板</span><span class="sxs-lookup"><span data-stu-id="337d2-133">Message center dashboard</span></span>
<span data-ttu-id="337d2-134">从 **消息中心** 仪表板，可以查看即将发生的更改，包括新增和已更改的功能、计划内维护和其他重要公告。</span><span class="sxs-lookup"><span data-stu-id="337d2-134">From the **Message center** dashboad, you can view upcoming changes, including new and changed features, planned maintenance, and other important announcements.</span></span> <span data-ttu-id="337d2-135">请参阅图 3 中所述的示例。</span><span class="sxs-lookup"><span data-stu-id="337d2-135">See examples as demarcated in figure 3.</span></span>

<span data-ttu-id="337d2-136">**图 3. Microsoft 365 管理中心中的消息中心仪表板**</span><span class="sxs-lookup"><span data-stu-id="337d2-136">**Figure 3. Message center dashboard in Microsoft 365 admin center**</span></span>

![用户 Microsoft 365 管理中心消息中心仪表板的屏幕截图](images/service-communications-concept-overview-admin-center-messagecenter2.png)



## <a name="next-steps"></a><span data-ttu-id="337d2-138">后续步骤</span><span class="sxs-lookup"><span data-stu-id="337d2-138">Next steps</span></span>

- <span data-ttu-id="337d2-139">在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/?request=admin%2FserviceAnnouncement%2FhealthOverviews&version=beta) 中试用服务通信示例查询。</span><span class="sxs-lookup"><span data-stu-id="337d2-139">Try service communications sample queries in [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=admin%2FserviceAnnouncement%2FhealthOverviews&version=beta).</span></span>

- <span data-ttu-id="337d2-140">详细了解 [服务通信 API](/graph/api/resources/service-communications-api-overview?view=graph-rest-beta&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="337d2-140">Learn more about the [service communications API](/graph/api/resources/service-communications-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>