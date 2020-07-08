---
title: 应用程序 API 概述
description: 向 Azure AD 注册应用程序，以便为其创建可与 Azure AD 集成的标识配置。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: scenarios:getting-started
ms.openlocfilehash: ff38e14182d2e38fbc2203241da911dec07f9846
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081192"
---
# <a name="applications-api-overview"></a><span data-ttu-id="1c774-103">应用程序 API 概述</span><span class="sxs-lookup"><span data-stu-id="1c774-103">Applications API overview</span></span>

<span data-ttu-id="1c774-104">为了将 identity and access management 函数委派给 Azure AD，必须向 Azure AD 租户注册应用程序。</span><span class="sxs-lookup"><span data-stu-id="1c774-104">In order to delegate identity and access management functions to Azure AD, an application must be registered with an Azure AD tenant.</span></span> <span data-ttu-id="1c774-105">当您向 Azure AD 注册应用程序时，您正在为应用程序创建标识配置，使其能够与 Azure AD 集成。</span><span class="sxs-lookup"><span data-stu-id="1c774-105">When you register your application with Azure AD, you're creating an identity configuration for your application that allows it to integrate with Azure AD.</span></span>

## <a name="why-use-applications-and-associated-resources"></a><span data-ttu-id="1c774-106">为什么要使用应用程序和相关联的资源？</span><span class="sxs-lookup"><span data-stu-id="1c774-106">Why use applications and associated resources?</span></span>

<span data-ttu-id="1c774-107">使用 Microsoft Graph Api，您可以管理与 Azure Active Directory 中的应用程序相关的这些资源和操作：</span><span class="sxs-lookup"><span data-stu-id="1c774-107">The Microsoft Graph APIs enable you to manage these resources and actions related to applications in Azure Active Directory:</span></span>
- <span data-ttu-id="1c774-108">**应用程序管理**-Azure AD 必须配置为与应用程序集成。</span><span class="sxs-lookup"><span data-stu-id="1c774-108">**Application management** - Azure AD must be configured to integrate with an application.</span></span> <span data-ttu-id="1c774-109">换句话说，它需要知道哪些应用程序正在将其用作标识系统。</span><span class="sxs-lookup"><span data-stu-id="1c774-109">In other words, it needs to know what applications are using it as an identity system.</span></span> <span data-ttu-id="1c774-110">阻止 Azure AD 识别这些应用程序以及它如何处理它们的过程称为 "应用程序管理"。</span><span class="sxs-lookup"><span data-stu-id="1c774-110">The process of keeping Azure AD aware of these applications, and how it should handle them, is known as application management.</span></span>
- <span data-ttu-id="1c774-111">可将租户管理员安装的本地**发布**代理（或应用程序代理的连接器）配置为将请求路由到特定的已发布资源。</span><span class="sxs-lookup"><span data-stu-id="1c774-111">**On-premises publishing** - On-premises agents (or connectors for Application Proxy) installed by a tenant administrator can be configured to route requests to a particular published resource.</span></span>
- <span data-ttu-id="1c774-112">**服务主体管理**-单个租户或目录中全局应用程序对象的本地表示形式或应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="1c774-112">**Service principal management** - The local representation, or application instance, of a global application object in a single tenant or directory.</span></span> <span data-ttu-id="1c774-113">服务主体是从 application 对象创建的具体实例，并继承该 application 对象的某些属性。</span><span class="sxs-lookup"><span data-stu-id="1c774-113">A service principal is a concrete instance created from the application object and inherits certain properties from that application object.</span></span>
- <span data-ttu-id="1c774-114">**同步**-Azure Active Directory （azure AD）标识同步（也称为*设置*）允许您自动创建、维护和删除云中的标识。</span><span class="sxs-lookup"><span data-stu-id="1c774-114">**Synchronization** - Azure Active Directory (Azure AD) identity synchronization (also called *provisioning*) allows you to automate the creation, maintenance, and removal of identities in the cloud.</span></span>

## <a name="application-management"></a><span data-ttu-id="1c774-115">应用管理</span><span class="sxs-lookup"><span data-stu-id="1c774-115">Application management</span></span>

<span data-ttu-id="1c774-116">应用程序注册涉及告知 Azure AD 有关应用程序的信息，包括其所在的 URL、身份验证后发送回复的 URL、标识应用程序的 URI 等。</span><span class="sxs-lookup"><span data-stu-id="1c774-116">Application registration involves telling Azure AD about your application, including the URL where it's located, the URL to send replies after authentication, the URI to identify your application, and more.</span></span> <span data-ttu-id="1c774-117">您可以使用 Microsoft Graph 中的[应用程序 api](/graph/api/resources/application?view=graph-rest-1.0)以编程方式管理应用程序。</span><span class="sxs-lookup"><span data-stu-id="1c774-117">You can use the [application APIs](/graph/api/resources/application?view=graph-rest-1.0) in Microsoft Graph to manage applications programmatically.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/93j0MmRruFo]

<span data-ttu-id="1c774-118">有关应用程序的详细信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="1c774-118">For more information about applications, see the following articles:</span></span>
- [<span data-ttu-id="1c774-119">应用程序模型</span><span class="sxs-lookup"><span data-stu-id="1c774-119">Application model</span></span>](https://docs.microsoft.com/azure/active-directory/develop/application-model)
- [<span data-ttu-id="1c774-120">Azure Active Directory 中的应用程序和服务主体对象</span><span class="sxs-lookup"><span data-stu-id="1c774-120">Application and service principal objects in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
- [<span data-ttu-id="1c774-121">Microsoft identity platform 的应用程序类型</span><span class="sxs-lookup"><span data-stu-id="1c774-121">Application types for Microsoft identity platform</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-app-types)

<span data-ttu-id="1c774-122">有关应用程序管理的详细信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="1c774-122">For more information about application management, see the following articles:</span></span>
- [<span data-ttu-id="1c774-123">什么是应用程序管理？</span><span class="sxs-lookup"><span data-stu-id="1c774-123">What is application management?</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-application-management)
- [<span data-ttu-id="1c774-124">身份验证流和应用程序方案</span><span class="sxs-lookup"><span data-stu-id="1c774-124">Authentication flows and application scenarios</span></span>](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios)

## <a name="on-premises-publishing-preview"></a><span data-ttu-id="1c774-125">本地发布（预览）</span><span class="sxs-lookup"><span data-stu-id="1c774-125">On-premises publishing (preview)</span></span>

<span data-ttu-id="1c774-126">创建和管理本地发布配置文件，其中包括创建本地代理和代理组。</span><span class="sxs-lookup"><span data-stu-id="1c774-126">Create and manage on-premises publishing profiles, which includes the creation of on-premises agents and agent groups.</span></span> <span data-ttu-id="1c774-127">您可以使用 Microsoft Graph 中的[本地发布 api](/graph/api/resources/onpremisespublishingprofile-root)以编程方式管理本地发布配置文件。</span><span class="sxs-lookup"><span data-stu-id="1c774-127">You can use the [on-premises publishing APIs](/graph/api/resources/onpremisespublishingprofile-root) in Microsoft Graph to manage on-premises publishing profiles programmatically.</span></span>

<span data-ttu-id="1c774-128">有关本地发布的详细信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="1c774-128">For more information about on-premises publishing, see the following articles:</span></span>
- [<span data-ttu-id="1c774-129">通过 Azure Active Directory 的应用程序代理远程访问本地应用程序</span><span class="sxs-lookup"><span data-stu-id="1c774-129">Remote access to on-premises applications through Azure Active Directory's Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy)
- [<span data-ttu-id="1c774-130">使用 Azure AD 应用程序代理为远程用户发布内部部署应用程序</span><span class="sxs-lookup"><span data-stu-id="1c774-130">Using Azure AD Application Proxy to publish on-premises apps for remote users</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-application-proxy)

<span data-ttu-id="1c774-131">若要了解如何使用内部部署发布 Api，请参阅以下教程及其关联的 Api：</span><span class="sxs-lookup"><span data-stu-id="1c774-131">To learn about using the on-premises publishing APIs, see the following tutorial and its associated APIs:</span></span>
- [<span data-ttu-id="1c774-132">使用 Microsoft Graph API 自动配置应用程序代理</span><span class="sxs-lookup"><span data-stu-id="1c774-132">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>](https://docs.microsoft.com/graph/application-proxy-configure-api)
    - [<span data-ttu-id="1c774-133">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="1c774-133">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [<span data-ttu-id="1c774-134">application</span><span class="sxs-lookup"><span data-stu-id="1c774-134">application</span></span>](/graph/api/resources/application?view=graph-rest-1.0)
    - [<span data-ttu-id="1c774-135">onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="1c774-135">onPremisesPublishing</span></span>](/graph/api/resources/onpremisespublishingprofile-root)
    - [<span data-ttu-id="1c774-136">连接器</span><span class="sxs-lookup"><span data-stu-id="1c774-136">connector</span></span>](/graph/api/resources/connector)
    - [<span data-ttu-id="1c774-137">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1c774-137">connectorGroup</span></span>](/graph/api/resources/connectorgroup)
    - [<span data-ttu-id="1c774-138">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="1c774-138">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="service-principal-management"></a><span data-ttu-id="1c774-139">服务主体管理</span><span class="sxs-lookup"><span data-stu-id="1c774-139">Service principal management</span></span>

<span data-ttu-id="1c774-140">若要访问受 Azure AD 租户保护的资源，需要访问的实体必须由安全主体表示。</span><span class="sxs-lookup"><span data-stu-id="1c774-140">To access resources that are secured by an Azure AD tenant, the entity that requires access must be represented by a security principal.</span></span> <span data-ttu-id="1c774-141">您可以使用 Microsoft Graph 中的[服务主体 api](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)以编程方式管理服务主体。</span><span class="sxs-lookup"><span data-stu-id="1c774-141">You can use the [service principal APIs](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) in Microsoft Graph to manage service principals programmatically.</span></span>

<span data-ttu-id="1c774-142">有关服务主体的详细信息，请参阅[Azure Active Directory 中的应用程序和服务主体对象](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)。</span><span class="sxs-lookup"><span data-stu-id="1c774-142">For more information about service principals, see [Application and service principal objects in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).</span></span>

## <a name="synchronization"></a><span data-ttu-id="1c774-143">同步</span><span class="sxs-lookup"><span data-stu-id="1c774-143">Synchronization</span></span>

<span data-ttu-id="1c774-144">您可以使用 Microsoft Graph 中的[同步 api](/graph/api/resources/synchronization-overview)以编程方式管理标识同步，包括：</span><span class="sxs-lookup"><span data-stu-id="1c774-144">You can use the [synchronization APIs](/graph/api/resources/synchronization-overview) in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>
- <span data-ttu-id="1c774-145">创建、启动和停止同步作业</span><span class="sxs-lookup"><span data-stu-id="1c774-145">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="1c774-146">对作业的同步架构进行更改</span><span class="sxs-lookup"><span data-stu-id="1c774-146">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="1c774-147">验证当前同步状态</span><span class="sxs-lookup"><span data-stu-id="1c774-147">Verify the current synchronization status</span></span>

<span data-ttu-id="1c774-148">有关同步的详细信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="1c774-148">For more information about synchronization, see the following articles:</span></span>
- [<span data-ttu-id="1c774-149">使用 Azure AD 自动化用户预配和预配到应用程序</span><span class="sxs-lookup"><span data-stu-id="1c774-149">Automate user provisioning and deprovisioning to applications with Azure AD</span></span>](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)
- [<span data-ttu-id="1c774-150">预配的工作原理</span><span class="sxs-lookup"><span data-stu-id="1c774-150">How provisioning works</span></span>](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works)

<span data-ttu-id="1c774-151">若要了解如何使用同步 Api，请参阅以下教程及其关联的 Api：</span><span class="sxs-lookup"><span data-stu-id="1c774-151">To learn about using the synchronization APIs, see the following tutorials and their associated APIs:</span></span>
- [<span data-ttu-id="1c774-152">使用 Microsoft Graph Api 配置设置</span><span class="sxs-lookup"><span data-stu-id="1c774-152">Configure provisioning using Microsoft Graph APIs</span></span>](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api)
    - [<span data-ttu-id="1c774-153">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="1c774-153">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [<span data-ttu-id="1c774-154">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="1c774-154">synchronizationTemplate</span></span>](/graph/api/resources/synchronization-synchronizationtemplate)
    - [<span data-ttu-id="1c774-155">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="1c774-155">synchronizationJob</span></span>](/graph/api/resources/synchronization-synchronizationjob)
- [<span data-ttu-id="1c774-156">使用 Microsoft Graph API 自动执行基于 SAML 的 SSO 应用配置</span><span class="sxs-lookup"><span data-stu-id="1c774-156">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api)
    - [<span data-ttu-id="1c774-157">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="1c774-157">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [<span data-ttu-id="1c774-158">application</span><span class="sxs-lookup"><span data-stu-id="1c774-158">application</span></span>](/graph/api/resources/application?view=graph-rest-1.0)
    - [<span data-ttu-id="1c774-159">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1c774-159">claimsMappingPolicy</span></span>](/graph/api/resources/claimsmappingpolicy)
    - [<span data-ttu-id="1c774-160">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="1c774-160">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="next-steps"></a><span data-ttu-id="1c774-161">后续步骤</span><span class="sxs-lookup"><span data-stu-id="1c774-161">Next steps</span></span>
- <span data-ttu-id="1c774-162">在[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中试用 MICROSOFT Graph API。</span><span class="sxs-lookup"><span data-stu-id="1c774-162">Try the Microsoft Graph API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="1c774-163">了解如何使用[这些示例](https://docs.microsoft.com/azure/active-directory/develop/sample-v2-code)向 web 应用程序和 web api 添加身份验证和授权。</span><span class="sxs-lookup"><span data-stu-id="1c774-163">Learn about how to add authentication and authorization to your web applications and web APIs using [these samples](https://docs.microsoft.com/azure/active-directory/develop/sample-v2-code).</span></span>
