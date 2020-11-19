---
title: 应用迁移规划清单
description: 将应用程序从 Azure AD Graph 迁移到 Microsoft Graph 的清单
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: d6a5fc83717c2facbbb016cbbc621d6d1bb36dc0
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352401"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="82f69-103">应用迁移规划清单</span><span class="sxs-lookup"><span data-stu-id="82f69-103">App migration planning checklist</span></span>

> [!Important]
> <span data-ttu-id="82f69-104">Azure AD Graph API 现已弃用。</span><span class="sxs-lookup"><span data-stu-id="82f69-104">Azure AD Graph API is now deprecated.</span></span> <span data-ttu-id="82f69-105">我们将继续提供技术支持和安全更新，但不会再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="82f69-105">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
> <span data-ttu-id="82f69-106">从2022年6月30日起，我们将结束对 Azure AD Graph 的支持，将不再提供技术支持或安全更新。</span><span class="sxs-lookup"><span data-stu-id="82f69-106">Starting June 30th, 2022, we will end support for Azure AD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="82f69-107">此后使用 Azure AD Graph 的应用程序将不再接收来自 Azure AD Graph 终结点的响应。</span><span class="sxs-lookup"><span data-stu-id="82f69-107">Apps using Azure AD Graph after this time will no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="82f69-108">使用以下检查表来规划迁移。</span><span class="sxs-lookup"><span data-stu-id="82f69-108">Use the following checklist to plan your migration.</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="82f69-109">步骤1：查看 Api 之间的差异</span><span class="sxs-lookup"><span data-stu-id="82f69-109">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="82f69-110">在许多方面，Microsoft Graph 类似于早期的 Azure AD Graph。</span><span class="sxs-lookup"><span data-stu-id="82f69-110">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="82f69-111">在很多情况下，只需更改代码中的终结点服务名称和版本，一切都应继续有效。</span><span class="sxs-lookup"><span data-stu-id="82f69-111">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="82f69-112">尽管如此，也存在差异。</span><span class="sxs-lookup"><span data-stu-id="82f69-112">Nonetheless, there are differences.</span></span> <span data-ttu-id="82f69-113">某些资源、属性、方法和核心功能已更改。</span><span class="sxs-lookup"><span data-stu-id="82f69-113">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="82f69-114">具体来说，请查找以下领域中的差异：</span><span class="sxs-lookup"><span data-stu-id="82f69-114">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="82f69-115">在两个服务之间[请求调用语法](migrate-azure-ad-graph-request-differences.md)</span><span class="sxs-lookup"><span data-stu-id="82f69-115">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="82f69-116">[功能差异](migrate-azure-ad-graph-feature-differences.md)，如目录扩展、批处理、差异查询等</span><span class="sxs-lookup"><span data-stu-id="82f69-116">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="82f69-117">[实体资源名称](migrate-azure-ad-graph-resource-differences.md) 及其类型</span><span class="sxs-lookup"><span data-stu-id="82f69-117">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="82f69-118">请求和响应对象的[属性](migrate-azure-ad-graph-property-differences.md)</span><span class="sxs-lookup"><span data-stu-id="82f69-118">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="82f69-119">[方法](migrate-azure-ad-graph-method-differences.md)（包括参数和类型）</span><span class="sxs-lookup"><span data-stu-id="82f69-119">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="82f69-120">步骤2：检查 API 使用情况</span><span class="sxs-lookup"><span data-stu-id="82f69-120">Step 2: Examine API use</span></span>

<span data-ttu-id="82f69-121">检查您的应用程序使用[的 api](migrate-azure-ad-graph-audit-api-use.md) 、所需的权限，并与已知差异的列表进行比较。</span><span class="sxs-lookup"><span data-stu-id="82f69-121">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="82f69-122">验证应用程序所需的 Api 在 Microsoft Graph v1.0 中通常可用，并且这些 Api 的工作方式相同。</span><span class="sxs-lookup"><span data-stu-id="82f69-122">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="82f69-123">在某些情况下，新功能和功能旨在取代早期的方法。</span><span class="sxs-lookup"><span data-stu-id="82f69-123">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="82f69-124">使用 [Graph 浏览器](https://aka.ms/ge) 体验新的呼叫并开发新的方法。</span><span class="sxs-lookup"><span data-stu-id="82f69-124">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="82f69-125">为获得最佳结果，请使用测试租户中的测试用户的凭据登录，以便您可以看到 API 对重要数据集执行的操作。</span><span class="sxs-lookup"><span data-stu-id="82f69-125">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="82f69-126">步骤3：查看应用程序详细信息</span><span class="sxs-lookup"><span data-stu-id="82f69-126">Step 3: Review app details</span></span>

- <span data-ttu-id="82f69-127">[应用注册](migrate-azure-ad-graph-app-registration.md) 和许可更改 () 不应为 "无"。</span><span class="sxs-lookup"><span data-stu-id="82f69-127">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="82f69-128">令牌获取和 [身份验证库](migrate-azure-ad-graph-authentication-library.md)。</span><span class="sxs-lookup"><span data-stu-id="82f69-128">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="82f69-129">对于 .NET 应用程序，使用 [客户端库](migrate-azure-ad-graph-client-libraries.md)。</span><span class="sxs-lookup"><span data-stu-id="82f69-129">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="82f69-130">步骤4：部署、测试和扩展应用程序</span><span class="sxs-lookup"><span data-stu-id="82f69-130">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="82f69-131">在更新您的应用程序以供每个人更新之前，请确保全面测试并向客户访问群体转移您的部署。</span><span class="sxs-lookup"><span data-stu-id="82f69-131">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="82f69-132">现在，您已将切换到 Microsoft Graph，对现在可以轻松解锁的更多数据集和功能的方法也变得更加轻松了。</span><span class="sxs-lookup"><span data-stu-id="82f69-132">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="82f69-133">你可以通过查看 [Microsoft Graph 中的一些主要服务和功能](/graph/overview-major-services)来了解可能会有什么。</span><span class="sxs-lookup"><span data-stu-id="82f69-133">You can get a taste of what's possible by looking at some of the [Major services and features in Microsoft Graph](/graph/overview-major-services).</span></span>

<span data-ttu-id="82f69-134">如果你当前使用的是 [AD 身份验证库](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL) ，请考虑切换到 [Microsoft 身份验证库](/azure/active-directory/develop/reference-v2-libraries) (MSAL) 。</span><span class="sxs-lookup"><span data-stu-id="82f69-134">If you're currently using the [AD authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), consider switching to the [Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span></span>

## <a name="next-steps"></a><span data-ttu-id="82f69-135">后续步骤</span><span class="sxs-lookup"><span data-stu-id="82f69-135">Next Steps</span></span>

- <span data-ttu-id="82f69-136">了解开始步骤1：检查 API 差异的 [请求调用语法](migrate-azure-ad-graph-request-differences.md) 。</span><span class="sxs-lookup"><span data-stu-id="82f69-136">Learn about [request call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>