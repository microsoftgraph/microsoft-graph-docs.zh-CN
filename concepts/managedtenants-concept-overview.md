---
title: Microsoft 365 LighthouseAPI 概述
description: Microsoft 365 Lighthouse 是一个管理门户，可帮助托管服务提供商 (MSP) 为使用 Microsoft 365 商业高级版 的中小型商业 (SMB) 客户大规模保护和管理设备、数据和用户。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
ms.openlocfilehash: 177a2f03fe5ee0e2e7d90ade038dcef1f7d6c3db
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401887"
---
# <a name="overview-for-multi-tenant-management-using-the-microsoft-365-lighthouse-api"></a><span data-ttu-id="f8f3c-103">使用应用程序 API 进行多租户Microsoft 365 Lighthouse概述</span><span class="sxs-lookup"><span data-stu-id="f8f3c-103">Overview for multi-tenant management using the Microsoft 365 Lighthouse API</span></span>

<span data-ttu-id="f8f3c-104">Microsoft 365 Lighthouse是一个管理门户，它允许托管服务提供商 (MSP) 远程管理多个客户租户。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-104">Microsoft 365 Lighthouse is an admin portal that lets Managed Service Providers (MSPs) remotely manage multiple customer tenants.</span></span> <span data-ttu-id="f8f3c-105">它可帮助使用 SMB 的中小型商业 (SMB) 级 MSP 大规模保护和管理Microsoft 365 商业高级版。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-105">It helps MSPs secure and manage devices, data, and users at scale for small- and medium-sized business (SMB) customers who are using Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="f8f3c-106">Microsoft 365 Lighthouse可帮助 MSP 简化客户租户Microsoft 365 商业高级版的载入。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-106">Microsoft 365 Lighthouse helps MSPs simplify onboarding of Microsoft 365 Business Premium customer tenants.</span></span> <span data-ttu-id="f8f3c-107">它提供 MSP，方便跨所有客户租户环境查看多租户。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-107">It offers an MSP the convenience of multi-tenant views across all its customer tenant environments.</span></span> <span data-ttu-id="f8f3c-108">它可推荐为 MSP 的 SMB 客户定制的安全配置基线。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-108">It can recommend security configuration baselines tailored to the MSP's SMB customers.</span></span> <span data-ttu-id="f8f3c-109">借助 Microsoft 365 Lighthouse，MSP 可以扩展其客户租户的管理，重点关注最重要的内容，快速查找和调查风险，并采取措施帮助其客户租户进入健康、安全的状态。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-109">With Microsoft 365 Lighthouse, MSPs can scale the management of their customer tenants, focus on what's most important, quickly find and investigate risks, and take action to help get their customer tenants to a healthy and secure state.</span></span>

> [!NOTE]  
> <span data-ttu-id="f8f3c-110">本文档与 Microsoft Microsoft 365 Lighthouse 上提供的 Graph _API 有关_。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-110">This documentation is about the Microsoft 365 Lighthouse API available on _Microsoft Graph_.</span></span> <span data-ttu-id="f8f3c-111">类似产品 Azure Lighthouse 通过使用内置于 Azure 平台的全面而稳固的管理工具，帮助服务提供商为 _Azure_ 服务提供托管服务。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-111">A similar offering, Azure Lighthouse, helps service providers deliver managed services for Azure services by using comprehensive and robust management tooling built into the _Azure_ platform.</span></span> <span data-ttu-id="f8f3c-112">若要了解更多信息，请参阅[什么是 Azure Lighthouse。](/azure/lighthouse/overview)</span><span class="sxs-lookup"><span data-stu-id="f8f3c-112">To learn more, see [What is Azure Lighthouse](/azure/lighthouse/overview).</span></span>

## <a name="why-integrate-with-microsoft-365-lighthouse"></a><span data-ttu-id="f8f3c-113">为什么与Microsoft 365 Lighthouse？</span><span class="sxs-lookup"><span data-stu-id="f8f3c-113">Why integrate with Microsoft 365 Lighthouse?</span></span>

<span data-ttu-id="f8f3c-114">作为 MSP，您可以使用 Microsoft Graph 中的 Microsoft 365 Lighthouse API 深入了解已识别的风险，并采取措施帮助客户进入健康、安全的状态。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-114">As an MSP, you can use the Microsoft 365 Lighthouse API in Microsoft Graph to gain insights into identified risks and take action to help get your customers into a healthy and secure state.</span></span>

### <a name="devices"></a><span data-ttu-id="f8f3c-115">设备</span><span class="sxs-lookup"><span data-stu-id="f8f3c-115">Devices</span></span>

<span data-ttu-id="f8f3c-116">可以使用 Lighthouse API 执行以下设备任务：</span><span class="sxs-lookup"><span data-stu-id="f8f3c-116">You can use the Lighthouse API to perform the following device tasks:</span></span>

- <span data-ttu-id="f8f3c-117">分析 [设备合规性趋势](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true) ，以更好地了解设备合规性如何随着时间的推移而发展。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-117">Analyze [device compliance trends](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true) to better understand how device compliance is evolving over time for your customers.</span></span>
- <span data-ttu-id="f8f3c-118">了解 [已在整个客户](/graph/api/resources/managedtenants-manageddevicecompliance) 中创建哪些设备合规性策略以及策略的状态。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-118">Understand what [device compliance policies](/graph/api/resources/managedtenants-manageddevicecompliance) have been created across your customers and the status of the policies.</span></span>

### <a name="threat-management"></a><span data-ttu-id="f8f3c-119">威胁管理</span><span class="sxs-lookup"><span data-stu-id="f8f3c-119">Threat management</span></span>

<span data-ttu-id="f8f3c-120">可以使用 Lighthouse API 执行以下威胁管理任务：</span><span class="sxs-lookup"><span data-stu-id="f8f3c-120">You can use the Lighthouse API to perform the following threat management tasks:</span></span>

- <span data-ttu-id="f8f3c-121">深入了解客户注册用于管理的[](/graph/api/resources/managedtenants-windowsdevicemalwarestate)Windows 设备上存在恶意软件的状态。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-121">Gain insight to the state of [malware](/graph/api/resources/managedtenants-windowsdevicemalwarestate) that is present on the Windows devices registered for management across your customers.</span></span>
- <span data-ttu-id="f8f3c-122">查看[注册用于](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true)Windows客户管理的设备的保护状态，以确保使用这些Windows Defender的设备都运行正常。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-122">View the [protection state](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true) for Windows devices registered for management across your customers to ensure those using Windows Defender are in a healthy state.</span></span>

### <a name="users"></a><span data-ttu-id="f8f3c-123">用户</span><span class="sxs-lookup"><span data-stu-id="f8f3c-123">Users</span></span>

<span data-ttu-id="f8f3c-124">可以使用 Lighthouse API 执行以下用户任务：</span><span class="sxs-lookup"><span data-stu-id="f8f3c-124">You can use the Lighthouse API to perform the following user tasks:</span></span>

- <span data-ttu-id="f8f3c-125">在 [客户中发现](/graph/api/resources/managedtenants-riskyuser?view=graph-rest-beta&preserve-view=true) 有风险的用户。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-125">Discover [risky users](/graph/api/resources/managedtenants-riskyuser?view=graph-rest-beta&preserve-view=true) across your customers.</span></span>
- <span data-ttu-id="f8f3c-126">查看 [凭据用户注册摘要](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) ，了解你的客户中哪些用户注册了多重身份验证和自助服务密码重置。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-126">View [credential user registration summary](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) to understand what users across your customers have registered for multi-factor authentication and self-service password reset.</span></span>

## <a name="api-reference"></a><span data-ttu-id="f8f3c-127">API 参考</span><span class="sxs-lookup"><span data-stu-id="f8f3c-127">API reference</span></span>

<span data-ttu-id="f8f3c-128">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="f8f3c-128">Looking for the API reference for this service?</span></span>

<span data-ttu-id="f8f3c-129">请参阅[microsoft Microsoft 365 Lighthouse 预览版中的 Graph (API) 。 ](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="f8f3c-129">See [Microsoft 365 Lighthouse API in Microsoft Graph (preview)](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true).</span></span>

> [!NOTE]
> <span data-ttu-id="f8f3c-130">该Microsoft 365 Lighthouse API 在 OData 子名称空间中定义 `microsoft.graph.managedTenants` 。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-130">The Microsoft 365 Lighthouse API is defined in the OData subnamespace, `microsoft.graph.managedTenants`.</span></span>


## <a name="next-steps"></a><span data-ttu-id="f8f3c-131">后续步骤</span><span class="sxs-lookup"><span data-stu-id="f8f3c-131">Next steps</span></span>

- <span data-ttu-id="f8f3c-132">详细了解 Microsoft 365 Lighthouse[门户。](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="f8f3c-132">Learn more about the [Microsoft 365 Lighthouse](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true) portal.</span></span>
- <span data-ttu-id="f8f3c-133">了解 Lighthouse [](/graph/whats-new-overview) API 的最新新功能和更新。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-133">Find out about the [latest new features and updates](/graph/whats-new-overview) for the Lighthouse API.</span></span>
- <span data-ttu-id="f8f3c-134">浏览[示例](https://developer.microsoft.com/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。</span><span class="sxs-lookup"><span data-stu-id="f8f3c-134">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
