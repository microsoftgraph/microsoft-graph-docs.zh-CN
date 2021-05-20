---
title: 应用迁移规划清单
description: 将应用从 Azure AD Graph迁移到 Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 84d486cd64d838a00998179a25dbba3ea35738eb
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546929"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="19e42-103">应用迁移规划清单</span><span class="sxs-lookup"><span data-stu-id="19e42-103">App migration planning checklist</span></span>

> [!Important]
> <span data-ttu-id="19e42-104">Azure AD Graph API 现已弃用。</span><span class="sxs-lookup"><span data-stu-id="19e42-104">Azure AD Graph API is now deprecated.</span></span> <span data-ttu-id="19e42-105">我们将继续提供技术支持和安全更新，但不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="19e42-105">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
> <span data-ttu-id="19e42-106">从 2022 年 6 月 30 开始，我们将停止对 Azure AD Graph将不再提供技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="19e42-106">Starting June 30th, 2022, we will end support for Azure AD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="19e42-107">在此时间Graph使用 Azure AD 应用的应用将不再收到来自 Azure AD Graph响应。</span><span class="sxs-lookup"><span data-stu-id="19e42-107">Apps using Azure AD Graph after this time will no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="19e42-108">使用以下清单规划迁移。</span><span class="sxs-lookup"><span data-stu-id="19e42-108">Use the following checklist to plan your migration.</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="19e42-109">步骤 1：查看 API 之间的差异</span><span class="sxs-lookup"><span data-stu-id="19e42-109">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="19e42-110">许多方面，Microsoft Graph类似于早期的 Azure AD Graph。</span><span class="sxs-lookup"><span data-stu-id="19e42-110">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="19e42-111">在许多情况下，只需在代码中更改终结点服务名称和版本，所有内容都应继续工作。</span><span class="sxs-lookup"><span data-stu-id="19e42-111">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="19e42-112">尽管如此，仍有一些差异。</span><span class="sxs-lookup"><span data-stu-id="19e42-112">Nonetheless, there are differences.</span></span> <span data-ttu-id="19e42-113">某些资源、属性、方法和核心功能已更改。</span><span class="sxs-lookup"><span data-stu-id="19e42-113">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="19e42-114">具体而言，请查找以下方面的差异：</span><span class="sxs-lookup"><span data-stu-id="19e42-114">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="19e42-115">[两个服务](migrate-azure-ad-graph-request-differences.md) 之间的请求调用语法</span><span class="sxs-lookup"><span data-stu-id="19e42-115">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="19e42-116">[功能](migrate-azure-ad-graph-feature-differences.md)差异，如目录扩展、批处理、差异查询等</span><span class="sxs-lookup"><span data-stu-id="19e42-116">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="19e42-117">[实体资源名称](migrate-azure-ad-graph-resource-differences.md) 及其类型</span><span class="sxs-lookup"><span data-stu-id="19e42-117">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="19e42-118">[请求](migrate-azure-ad-graph-property-differences.md) 和响应对象的属性</span><span class="sxs-lookup"><span data-stu-id="19e42-118">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="19e42-119">[方法](migrate-azure-ad-graph-method-differences.md)，包括参数和类型</span><span class="sxs-lookup"><span data-stu-id="19e42-119">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="19e42-120">步骤 2：检查 API 使用</span><span class="sxs-lookup"><span data-stu-id="19e42-120">Step 2: Examine API use</span></span>

<span data-ttu-id="19e42-121">[检查你的应用使用的](migrate-azure-ad-graph-audit-api-use.md) API、它们所需的权限，并与已知差异列表进行比较。</span><span class="sxs-lookup"><span data-stu-id="19e42-121">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="19e42-122">验证你的应用所需的 API 在 Microsoft Graph v1.0 中是否通常可用，以及这些 API 是否以相同方式工作。</span><span class="sxs-lookup"><span data-stu-id="19e42-122">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="19e42-123">在某些情况下，新功能和特性旨在取代早期方法。</span><span class="sxs-lookup"><span data-stu-id="19e42-123">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="19e42-124">使用[Graph 资源管理器](https://aka.ms/ge)试验新调用并开发新方法。</span><span class="sxs-lookup"><span data-stu-id="19e42-124">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="19e42-125">为了获得最佳结果，使用测试租户中的测试用户的凭据登录，以便查看 API 对重要数据集执行哪些操作。</span><span class="sxs-lookup"><span data-stu-id="19e42-125">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="19e42-126">步骤 3：查看应用详细信息</span><span class="sxs-lookup"><span data-stu-id="19e42-126">Step 3: Review app details</span></span>

- <span data-ttu-id="19e42-127">[应用注册](migrate-azure-ad-graph-app-registration.md) 和同意 (更改，这些更改不应) 。</span><span class="sxs-lookup"><span data-stu-id="19e42-127">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="19e42-128">令牌获取 [和身份验证库](migrate-azure-ad-graph-authentication-library.md)。</span><span class="sxs-lookup"><span data-stu-id="19e42-128">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="19e42-129">对于 .NET 应用程序，请使用 [客户端库](migrate-azure-ad-graph-client-libraries.md)。</span><span class="sxs-lookup"><span data-stu-id="19e42-129">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="19e42-130">步骤 4：部署、测试和扩展应用</span><span class="sxs-lookup"><span data-stu-id="19e42-130">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="19e42-131">在为所有人更新应用之前，请确保全面测试并推广到客户受众。</span><span class="sxs-lookup"><span data-stu-id="19e42-131">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="19e42-132">现在，你已切换到 Microsoft Graph，那么解锁现在触手可及的更多数据集和功能从未如此简单。</span><span class="sxs-lookup"><span data-stu-id="19e42-132">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="19e42-133">通过查看 Microsoft Graph 中的一些主要服务和功能，你可以尝试[一下Graph。](./overview-major-services.md)</span><span class="sxs-lookup"><span data-stu-id="19e42-133">You can get a taste of what's possible by looking at some of the [Major services and features in Microsoft Graph](./overview-major-services.md).</span></span>

<span data-ttu-id="19e42-134">[Microsoft 身份验证库](/azure/active-directory/develop/reference-v2-libraries) (MSAL) 现在是建议用于该身份验证库的Microsoft 标识平台。</span><span class="sxs-lookup"><span data-stu-id="19e42-134">[Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL) is now the recommended authentication library for use with the Microsoft identity platform.</span></span> <span data-ttu-id="19e42-135">如果当前正在使用 ADAL ([ADAL](/azure/active-directory/develop/active-directory-authentication-libraries)) ，请计划切换到 MSAL。</span><span class="sxs-lookup"><span data-stu-id="19e42-135">If you're currently using the [AD authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), plan to switch to MSAL.</span></span> <span data-ttu-id="19e42-136">请参阅将应用程序迁移到[MSAL (Microsoft 身份验证库) 。 ](/azure/active-directory/develop/msal-migration)</span><span class="sxs-lookup"><span data-stu-id="19e42-136">See further guidance to [migrate applications to the Microsoft Authentication Library (MSAL)](/azure/active-directory/develop/msal-migration).</span></span>

## <a name="next-steps"></a><span data-ttu-id="19e42-137">后续步骤</span><span class="sxs-lookup"><span data-stu-id="19e42-137">Next Steps</span></span>

- <span data-ttu-id="19e42-138">了解开始 [步骤](migrate-azure-ad-graph-request-differences.md) 1：查看 API 差异的请求调用语法。</span><span class="sxs-lookup"><span data-stu-id="19e42-138">Learn about [request call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>