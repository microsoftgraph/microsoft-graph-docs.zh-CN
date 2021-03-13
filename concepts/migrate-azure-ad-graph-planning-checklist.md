---
title: 应用迁移规划清单
description: 将应用从 Azure AD Graph 迁移到 Microsoft Graph 的清单
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: a61e5180194246bbea5cc32e42666beab83882fa
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761281"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="8827a-103">应用迁移规划清单</span><span class="sxs-lookup"><span data-stu-id="8827a-103">App migration planning checklist</span></span>

> [!Important]
> <span data-ttu-id="8827a-104">Azure AD Graph API 现已弃用。</span><span class="sxs-lookup"><span data-stu-id="8827a-104">Azure AD Graph API is now deprecated.</span></span> <span data-ttu-id="8827a-105">我们将继续提供技术支持和安全更新，但不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="8827a-105">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
> <span data-ttu-id="8827a-106">从 2022 年 6 月 30 日开始，我们将停止对 Azure AD Graph 的支持，并且将不再提供技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="8827a-106">Starting June 30th, 2022, we will end support for Azure AD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="8827a-107">在此时间之后，使用 Azure AD Graph 的应用将不再收到来自 Azure AD Graph 终结点的响应。</span><span class="sxs-lookup"><span data-stu-id="8827a-107">Apps using Azure AD Graph after this time will no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="8827a-108">使用以下清单规划迁移。</span><span class="sxs-lookup"><span data-stu-id="8827a-108">Use the following checklist to plan your migration.</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="8827a-109">步骤 1：查看 API 之间的差异</span><span class="sxs-lookup"><span data-stu-id="8827a-109">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="8827a-110">在很多方面，Microsoft Graph 与早期的 Azure AD Graph 类似。</span><span class="sxs-lookup"><span data-stu-id="8827a-110">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="8827a-111">在许多情况下，只需在代码中更改终结点服务名称和版本，所有内容都应继续工作。</span><span class="sxs-lookup"><span data-stu-id="8827a-111">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="8827a-112">尽管如此，仍有一些差异。</span><span class="sxs-lookup"><span data-stu-id="8827a-112">Nonetheless, there are differences.</span></span> <span data-ttu-id="8827a-113">某些资源、属性、方法和核心功能已更改。</span><span class="sxs-lookup"><span data-stu-id="8827a-113">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="8827a-114">具体而言，请查找以下方面的差异：</span><span class="sxs-lookup"><span data-stu-id="8827a-114">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="8827a-115">[两个服务](migrate-azure-ad-graph-request-differences.md) 之间的请求调用语法</span><span class="sxs-lookup"><span data-stu-id="8827a-115">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="8827a-116">[功能](migrate-azure-ad-graph-feature-differences.md)差异，如目录扩展、批处理、差异查询等</span><span class="sxs-lookup"><span data-stu-id="8827a-116">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="8827a-117">[实体资源名称](migrate-azure-ad-graph-resource-differences.md) 及其类型</span><span class="sxs-lookup"><span data-stu-id="8827a-117">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="8827a-118">[请求](migrate-azure-ad-graph-property-differences.md) 和响应对象的属性</span><span class="sxs-lookup"><span data-stu-id="8827a-118">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="8827a-119">[方法](migrate-azure-ad-graph-method-differences.md)，包括参数和类型</span><span class="sxs-lookup"><span data-stu-id="8827a-119">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="8827a-120">步骤 2：检查 API 使用</span><span class="sxs-lookup"><span data-stu-id="8827a-120">Step 2: Examine API use</span></span>

<span data-ttu-id="8827a-121">[检查你的应用使用的](migrate-azure-ad-graph-audit-api-use.md) API、它们所需的权限，并与已知差异列表进行比较。</span><span class="sxs-lookup"><span data-stu-id="8827a-121">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="8827a-122">验证你的应用所需的 API 在 Microsoft Graph v1.0 中是否通常可用，以及这些 API 是否以相同方式工作。</span><span class="sxs-lookup"><span data-stu-id="8827a-122">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="8827a-123">在某些情况下，新功能和特性旨在取代早期方法。</span><span class="sxs-lookup"><span data-stu-id="8827a-123">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="8827a-124">使用 [Graph 浏览器](https://aka.ms/ge) 试验新调用并开发新方法。</span><span class="sxs-lookup"><span data-stu-id="8827a-124">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="8827a-125">为了获得最佳结果，使用测试租户中的测试用户的凭据登录，以便查看 API 对重要数据集执行哪些操作。</span><span class="sxs-lookup"><span data-stu-id="8827a-125">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="8827a-126">步骤 3：查看应用详细信息</span><span class="sxs-lookup"><span data-stu-id="8827a-126">Step 3: Review app details</span></span>

- <span data-ttu-id="8827a-127">[应用注册](migrate-azure-ad-graph-app-registration.md) 和同意 (更改，这些更改不应) 。</span><span class="sxs-lookup"><span data-stu-id="8827a-127">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="8827a-128">令牌获取 [和身份验证库](migrate-azure-ad-graph-authentication-library.md)。</span><span class="sxs-lookup"><span data-stu-id="8827a-128">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="8827a-129">对于 .NET 应用程序，请使用 [客户端库](migrate-azure-ad-graph-client-libraries.md)。</span><span class="sxs-lookup"><span data-stu-id="8827a-129">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="8827a-130">步骤 4：部署、测试和扩展应用</span><span class="sxs-lookup"><span data-stu-id="8827a-130">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="8827a-131">在为所有人更新应用之前，请确保全面测试并推广到客户受众。</span><span class="sxs-lookup"><span data-stu-id="8827a-131">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="8827a-132">现在，你已切换到 Microsoft Graph，因此解锁现在触手可及的更多数据集和功能从未如此简单。</span><span class="sxs-lookup"><span data-stu-id="8827a-132">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="8827a-133">通过查看 Microsoft Graph 中的一些主要服务和功能，你可以尝试一下 [可能的功能](./overview-major-services.md)。</span><span class="sxs-lookup"><span data-stu-id="8827a-133">You can get a taste of what's possible by looking at some of the [Major services and features in Microsoft Graph](./overview-major-services.md).</span></span>

<span data-ttu-id="8827a-134">如果当前使用的是 ADAL ([AD](/azure/active-directory/develop/active-directory-authentication-libraries)) ，请考虑切换到 [MSAL](/azure/active-directory/develop/reference-v2-libraries) (Microsoft 身份验证) 。</span><span class="sxs-lookup"><span data-stu-id="8827a-134">If you're currently using the [AD authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), consider switching to the [Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span></span>

## <a name="next-steps"></a><span data-ttu-id="8827a-135">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8827a-135">Next Steps</span></span>

- <span data-ttu-id="8827a-136">了解开始 [步骤](migrate-azure-ad-graph-request-differences.md) 1：查看 API 差异的请求调用语法。</span><span class="sxs-lookup"><span data-stu-id="8827a-136">Learn about [request call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>