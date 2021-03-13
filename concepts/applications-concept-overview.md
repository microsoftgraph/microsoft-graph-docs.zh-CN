---
title: 应用程序 API 概述
description: 向 Azure AD 注册应用程序，以为其创建标识配置，允许其与 Azure AD 集成。
author: davidmu1
localization_priority: Priority
ms.prod: applications
ms.custom: scenarios:getting-started
ms.openlocfilehash: d99f20d5bbf748030576e1cdc28fabb5f666bee0
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760824"
---
# <a name="applications-api-overview"></a><span data-ttu-id="14797-103">应用程序 API 概述</span><span class="sxs-lookup"><span data-stu-id="14797-103">Applications API overview</span></span>

<span data-ttu-id="14797-104">为将标识和访问管理功能委派给 Azure AD，必须向 Azure AD 租户注册应用程序。</span><span class="sxs-lookup"><span data-stu-id="14797-104">In order to delegate identity and access management functions to Azure AD, an application must be registered with an Azure AD tenant.</span></span> <span data-ttu-id="14797-105">向 Azure AD 注册应用程序时，将为应用程序创建标识配置，允许其与 Azure AD 集成。</span><span class="sxs-lookup"><span data-stu-id="14797-105">When you register your application with Azure AD, you're creating an identity configuration for your application that allows it to integrate with Azure AD.</span></span>

## <a name="why-use-applications-and-associated-resources"></a><span data-ttu-id="14797-106">为什么要使用应用程序和相关的资源？</span><span class="sxs-lookup"><span data-stu-id="14797-106">Why use applications and associated resources?</span></span>

<span data-ttu-id="14797-107">Microsoft Graph API 使你能够管理与 Azure Active Directory 中的应用程序相关的这些资源和操作：</span><span class="sxs-lookup"><span data-stu-id="14797-107">The Microsoft Graph APIs enable you to manage these resources and actions related to applications in Azure Active Directory:</span></span>
- <span data-ttu-id="14797-108">**应用程序管理** - Azure AD 必须配置为与应用程序集成。</span><span class="sxs-lookup"><span data-stu-id="14797-108">**Application management** - Azure AD must be configured to integrate with an application.</span></span> <span data-ttu-id="14797-109">换言之，需要了解哪些应用程序将其用作标识系统。</span><span class="sxs-lookup"><span data-stu-id="14797-109">In other words, it needs to know what applications are using it as an identity system.</span></span> <span data-ttu-id="14797-110">让 Azure AD 了解这些应用程序，以及应该如何处理这些应用程序的过程称为应用程序管理。</span><span class="sxs-lookup"><span data-stu-id="14797-110">The process of keeping Azure AD aware of these applications, and how it should handle them, is known as application management.</span></span>
- <span data-ttu-id="14797-111">**本地发布** - 可将租户管理员安装的本地代理（或应用程序代理的连接器）配置为请求转接到特定的已发布资源。</span><span class="sxs-lookup"><span data-stu-id="14797-111">**On-premises publishing** - On-premises agents (or connectors for Application Proxy) installed by a tenant administrator can be configured to route requests to a particular published resource.</span></span>
- <span data-ttu-id="14797-112">**服务主体管理** - 单个租户或目录中的全局应用程序对象的本地表示或应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="14797-112">**Service principal management** - The local representation, or application instance, of a global application object in a single tenant or directory.</span></span> <span data-ttu-id="14797-113">服务主体是通过应用程序对象创建的具体实例，并从该应用程序对象继承某些属性。</span><span class="sxs-lookup"><span data-stu-id="14797-113">A service principal is a concrete instance created from the application object and inherits certain properties from that application object.</span></span>
- <span data-ttu-id="14797-114">**同步** - Azure Active Directory (Azure AD) 标识同步（也称为 *预配*）使你能够自动化云中的标识的创建、维护和删除。</span><span class="sxs-lookup"><span data-stu-id="14797-114">**Synchronization** - Azure Active Directory (Azure AD) identity synchronization (also called *provisioning*) allows you to automate the creation, maintenance, and removal of identities in the cloud.</span></span>

## <a name="application-management"></a><span data-ttu-id="14797-115">应用管理</span><span class="sxs-lookup"><span data-stu-id="14797-115">Application management</span></span>

<span data-ttu-id="14797-116">应用程序注册涉及告知 Azure AD 有关应用程序的信息，包括其所在的 URL、身份验证后发送回复的 URL、标识应用程序的 URI 等。</span><span class="sxs-lookup"><span data-stu-id="14797-116">Application registration involves telling Azure AD about your application, including the URL where it's located, the URL to send replies after authentication, the URI to identify your application, and more.</span></span> <span data-ttu-id="14797-117">可使用 Microsoft Graph 中的[应用程序 API](/graph/api/resources/application?view=graph-rest-1.0) 以编程方式管理应用程序。</span><span class="sxs-lookup"><span data-stu-id="14797-117">You can use the [application APIs](/graph/api/resources/application?view=graph-rest-1.0) in Microsoft Graph to manage applications programmatically.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/93j0MmRruFo]

<span data-ttu-id="14797-118">有关应用程序的更多信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="14797-118">For more information about applications, see the following articles:</span></span>
- [<span data-ttu-id="14797-119">应用程序模型</span><span class="sxs-lookup"><span data-stu-id="14797-119">Application model</span></span>](/azure/active-directory/develop/application-model)
- [<span data-ttu-id="14797-120">Azure Active Directory 中的应用程序和服务主体对象</span><span class="sxs-lookup"><span data-stu-id="14797-120">Application and service principal objects in Azure Active Directory</span></span>](/azure/active-directory/develop/app-objects-and-service-principals)
- [<span data-ttu-id="14797-121">Microsoft 标识平台的应用程序类型</span><span class="sxs-lookup"><span data-stu-id="14797-121">Application types for Microsoft identity platform</span></span>](/azure/active-directory/develop/v2-app-types)

<span data-ttu-id="14797-122">有关应用程序管理的更多信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="14797-122">For more information about application management, see the following articles:</span></span>
- [<span data-ttu-id="14797-123">什么是应用程序管理？</span><span class="sxs-lookup"><span data-stu-id="14797-123">What is application management?</span></span>](/azure/active-directory/manage-apps/what-is-application-management)
- [<span data-ttu-id="14797-124">身份验证流程和应用程序方案</span><span class="sxs-lookup"><span data-stu-id="14797-124">Authentication flows and application scenarios</span></span>](/azure/active-directory/develop/authentication-flows-app-scenarios)

## <a name="on-premises-publishing-preview"></a><span data-ttu-id="14797-125">本地发布（预览版）</span><span class="sxs-lookup"><span data-stu-id="14797-125">On-premises publishing (preview)</span></span>

<span data-ttu-id="14797-126">创建和管理本地发布配置文件，其中包括创建本地代理和代理组。</span><span class="sxs-lookup"><span data-stu-id="14797-126">Create and manage on-premises publishing profiles, which includes the creation of on-premises agents and agent groups.</span></span> <span data-ttu-id="14797-127">可使用 Microsoft Graph 中的[本地发布 API](/graph/api/resources/onpremisespublishingprofile-root) 以编程方式管理本地发布配置文件。</span><span class="sxs-lookup"><span data-stu-id="14797-127">You can use the [on-premises publishing APIs](/graph/api/resources/onpremisespublishingprofile-root) in Microsoft Graph to manage on-premises publishing profiles programmatically.</span></span>

<span data-ttu-id="14797-128">有关本地发布的详细信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="14797-128">For more information about on-premises publishing, see the following articles:</span></span>
- [<span data-ttu-id="14797-129">通过 Azure Active Directory 的应用程序代理对本地应用程序进行远程访问</span><span class="sxs-lookup"><span data-stu-id="14797-129">Remote access to on-premises applications through Azure Active Directory's Application Proxy</span></span>](/azure/active-directory/manage-apps/application-proxy)
- [<span data-ttu-id="14797-130">使用 Azure AD 应用程序代理为远程用户发布本地应用</span><span class="sxs-lookup"><span data-stu-id="14797-130">Using Azure AD Application Proxy to publish on-premises apps for remote users</span></span>](/azure/active-directory/manage-apps/what-is-application-proxy)

<span data-ttu-id="14797-131">若要了解如何使用本地发布 API，请参阅以下教程及其相关的 API：</span><span class="sxs-lookup"><span data-stu-id="14797-131">To learn about using the on-premises publishing APIs, see the following tutorial and its associated APIs:</span></span>
- [<span data-ttu-id="14797-132">使用 Microsoft Graph API 自动化应用程序代理的配置</span><span class="sxs-lookup"><span data-stu-id="14797-132">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>](./application-proxy-configure-api.md)
    - [<span data-ttu-id="14797-133">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="14797-133">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [<span data-ttu-id="14797-134">application</span><span class="sxs-lookup"><span data-stu-id="14797-134">application</span></span>](/graph/api/resources/application?view=graph-rest-1.0)
    - [<span data-ttu-id="14797-135">onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="14797-135">onPremisesPublishing</span></span>](/graph/api/resources/onpremisespublishingprofile-root)
    - [<span data-ttu-id="14797-136">connector</span><span class="sxs-lookup"><span data-stu-id="14797-136">connector</span></span>](/graph/api/resources/connector)
    - [<span data-ttu-id="14797-137">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="14797-137">connectorGroup</span></span>](/graph/api/resources/connectorgroup)
    - [<span data-ttu-id="14797-138">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="14797-138">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="service-principal-management"></a><span data-ttu-id="14797-139">服务主体管理</span><span class="sxs-lookup"><span data-stu-id="14797-139">Service principal management</span></span>

<span data-ttu-id="14797-140">若要访问受 Azure AD 租户保护的资源，需要访问的实体必须由安全主体表示。</span><span class="sxs-lookup"><span data-stu-id="14797-140">To access resources that are secured by an Azure AD tenant, the entity that requires access must be represented by a security principal.</span></span> <span data-ttu-id="14797-141">可使用 Microsoft Graph 中的[服务主体 API](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) 以编程方式管理服务主体。</span><span class="sxs-lookup"><span data-stu-id="14797-141">You can use the [service principal APIs](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) in Microsoft Graph to manage service principals programmatically.</span></span>

<span data-ttu-id="14797-142">有关服务主体的详细信息，请参阅 [Azure Active Directory 中的应用程序和服务主体对象](/azure/active-directory/develop/app-objects-and-service-principals)。</span><span class="sxs-lookup"><span data-stu-id="14797-142">For more information about service principals, see [Application and service principal objects in Azure Active Directory](/azure/active-directory/develop/app-objects-and-service-principals).</span></span>

## <a name="synchronization"></a><span data-ttu-id="14797-143">同步</span><span class="sxs-lookup"><span data-stu-id="14797-143">Synchronization</span></span>

<span data-ttu-id="14797-144">可使用 Microsoft Graph 中的[同步 API](/graph/api/resources/synchronization-overview) 以编程方式管理标识同步，包括：</span><span class="sxs-lookup"><span data-stu-id="14797-144">You can use the [synchronization APIs](/graph/api/resources/synchronization-overview) in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>
- <span data-ttu-id="14797-145">创建、启动和停止同步作业</span><span class="sxs-lookup"><span data-stu-id="14797-145">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="14797-146">对作业的同步架构进行更改</span><span class="sxs-lookup"><span data-stu-id="14797-146">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="14797-147">验证当前同步状态</span><span class="sxs-lookup"><span data-stu-id="14797-147">Verify the current synchronization status</span></span>

<span data-ttu-id="14797-148">有关同步的详细信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="14797-148">For more information about synchronization, see the following articles:</span></span>
- [<span data-ttu-id="14797-149">使用 Azure AD 为应用程序自动预配和取消用户</span><span class="sxs-lookup"><span data-stu-id="14797-149">Automate user provisioning and deprovisioning to applications with Azure AD</span></span>](/azure/active-directory/app-provisioning/user-provisioning)
- [<span data-ttu-id="14797-150">预配的工作原理</span><span class="sxs-lookup"><span data-stu-id="14797-150">How provisioning works</span></span>](/azure/active-directory/app-provisioning/how-provisioning-works)

<span data-ttu-id="14797-151">若要了解有关使用同步 API 的信息，请参阅以下教程及其相关联的 API：</span><span class="sxs-lookup"><span data-stu-id="14797-151">To learn about using the synchronization APIs, see the following tutorials and their associated APIs:</span></span>
- [<span data-ttu-id="14797-152">使用 Microsoft Graph Api 配置预配</span><span class="sxs-lookup"><span data-stu-id="14797-152">Configure provisioning using Microsoft Graph APIs</span></span>](/azure/active-directory/app-provisioning/application-provisioning-configure-api)
    - [<span data-ttu-id="14797-153">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="14797-153">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [<span data-ttu-id="14797-154">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="14797-154">synchronizationTemplate</span></span>](/graph/api/resources/synchronization-synchronizationtemplate)
    - [<span data-ttu-id="14797-155">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="14797-155">synchronizationJob</span></span>](/graph/api/resources/synchronization-synchronizationjob)
- [<span data-ttu-id="14797-156">使用 Microsoft Graph API 自动化基于 SAML 的 SSO 应用配置</span><span class="sxs-lookup"><span data-stu-id="14797-156">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](/azure/active-directory/manage-apps/application-saml-sso-configure-api)
    - [<span data-ttu-id="14797-157">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="14797-157">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [<span data-ttu-id="14797-158">application</span><span class="sxs-lookup"><span data-stu-id="14797-158">application</span></span>](/graph/api/resources/application?view=graph-rest-1.0)
    - [<span data-ttu-id="14797-159">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="14797-159">claimsMappingPolicy</span></span>](/graph/api/resources/claimsmappingpolicy)
    - [<span data-ttu-id="14797-160">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="14797-160">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="next-steps"></a><span data-ttu-id="14797-161">后续步骤</span><span class="sxs-lookup"><span data-stu-id="14797-161">Next steps</span></span>
- <span data-ttu-id="14797-162">在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="14797-162">Try the Microsoft Graph API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="14797-163">了解如何使用[这些示例](/azure/active-directory/develop/sample-v2-code)将身份验证和授权添加到 web 应用程序和 web API。</span><span class="sxs-lookup"><span data-stu-id="14797-163">Learn about how to add authentication and authorization to your web applications and web APIs using [these samples](/azure/active-directory/develop/sample-v2-code).</span></span>