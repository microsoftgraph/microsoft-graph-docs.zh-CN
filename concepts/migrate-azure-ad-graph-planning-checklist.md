---
title: 应用迁移规划清单
description: 将应用程序从 Azure AD Graph 迁移到 Microsoft Graph 的清单
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 78b6ba30d84a2ca71ae8998df1321b2b8e0ba331
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630221"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="7cb9c-103">应用迁移规划清单</span><span class="sxs-lookup"><span data-stu-id="7cb9c-103">App migration planning checklist</span></span>

<span data-ttu-id="7cb9c-104">使用以下检查表来规划迁移:</span><span class="sxs-lookup"><span data-stu-id="7cb9c-104">Use the following checklist to plan your migration:</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="7cb9c-105">步骤 1: 查看 Api 之间的差异</span><span class="sxs-lookup"><span data-stu-id="7cb9c-105">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="7cb9c-106">在许多方面, Microsoft Graph 类似于早期的 Azure AD Graph。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-106">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="7cb9c-107">在很多情况下, 只需更改代码中的终结点服务名称和版本, 一切都应继续有效。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-107">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="7cb9c-108">尽管如此, 也存在差异。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-108">Nonetheless, there are differences.</span></span> <span data-ttu-id="7cb9c-109">某些资源、属性、方法和核心功能已更改。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-109">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="7cb9c-110">具体来说, 请查找以下领域中的差异:</span><span class="sxs-lookup"><span data-stu-id="7cb9c-110">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="7cb9c-111">在两个服务之间[请求调用语法](migrate-azure-ad-graph-request-differences.md)</span><span class="sxs-lookup"><span data-stu-id="7cb9c-111">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="7cb9c-112">[功能差异](migrate-azure-ad-graph-feature-differences.md), 如目录扩展、批处理、差异查询等</span><span class="sxs-lookup"><span data-stu-id="7cb9c-112">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="7cb9c-113">[实体资源名称](migrate-azure-ad-graph-resource-differences.md)及其类型</span><span class="sxs-lookup"><span data-stu-id="7cb9c-113">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="7cb9c-114">请求和响应对象的[属性](migrate-azure-ad-graph-property-differences.md)</span><span class="sxs-lookup"><span data-stu-id="7cb9c-114">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="7cb9c-115">[方法](migrate-azure-ad-graph-method-differences.md)(包括参数和类型)</span><span class="sxs-lookup"><span data-stu-id="7cb9c-115">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="7cb9c-116">步骤 2: 检查 API 使用情况</span><span class="sxs-lookup"><span data-stu-id="7cb9c-116">Step 2: Examine API use</span></span>

<span data-ttu-id="7cb9c-117">检查您的应用程序使用[的 api](migrate-azure-ad-graph-audit-api-use.md) 、所需的权限, 并与已知差异的列表进行比较。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-117">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="7cb9c-118">验证应用程序所需的 Api 在 Microsoft Graph v1。0中通常可用, 并且这些 Api 的工作方式相同。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-118">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="7cb9c-119">在某些情况下, 新功能和功能旨在取代早期的方法。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-119">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="7cb9c-120">使用[Graph 浏览器](https://aka.ms/ge)体验新的呼叫并开发新的方法。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-120">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="7cb9c-121">为获得最佳结果, 请使用测试租户中的测试用户的凭据登录, 以便您可以看到 API 对重要数据集执行的操作。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-121">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="7cb9c-122">步骤 3: 查看应用程序详细信息</span><span class="sxs-lookup"><span data-stu-id="7cb9c-122">Step 3: Review app details</span></span>

  - <span data-ttu-id="7cb9c-123">[应用注册](migrate-azure-ad-graph-app-registration.md)和同意更改 (应为 "无")。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-123">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
  - <span data-ttu-id="7cb9c-124">令牌获取和[身份验证库](migrate-azure-ad-graph-authentication-library.md)。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-124">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
  - <span data-ttu-id="7cb9c-125">对于 .NET 应用程序, 使用[客户端库](migrate-azure-ad-graph-client-libraries.md)。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-125">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="7cb9c-126">步骤 4: 部署、测试和扩展应用程序</span><span class="sxs-lookup"><span data-stu-id="7cb9c-126">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="7cb9c-127">在更新您的应用程序以供每个人更新之前, 请确保全面测试并向客户访问群体转移您的部署。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-127">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="7cb9c-128">现在, 您已将切换到 Microsoft Graph, 对现在可以轻松解锁的更多数据集和功能的方法也变得更加轻松了。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-128">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="7cb9c-129">您可以通过查看一些[示例](/graph/examples)来了解可能的情况。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-129">You can get a taste of what's possible by looking at some [examples](/graph/examples).</span></span>

<span data-ttu-id="7cb9c-130">如果你当前使用的是[AD 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)(ADAL), 请考虑切换到[Microsoft 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)(MSAL)。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-130">If you're currently using the [AD authentication library](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), consider switching to the [Microsoft authentication library](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span></span>

## <a name="next-steps"></a><span data-ttu-id="7cb9c-131">后续步骤</span><span class="sxs-lookup"><span data-stu-id="7cb9c-131">Next Steps</span></span>

- <span data-ttu-id="7cb9c-132">了解用于启动步骤 1: 审阅 API 差异的[resquest 调用语法](migrate-azure-ad-graph-request-differences.md)。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-132">Learn about [resquest call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>
- <span data-ttu-id="7cb9c-133">浏览[Microsoft Graph](/graph/overview)概念和实践。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-133">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="7cb9c-134">使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-134">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
- <span data-ttu-id="7cb9c-135">若要了解有关进度更新和时间线的详细信息, 请参阅 Office 开发人员中心中[的 Microsoft Graph 或 AZURE AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) 。</span><span class="sxs-lookup"><span data-stu-id="7cb9c-135">To learn more about progress updates and timelines, see [Microsoft Graph or the Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) in the Office Dev Center.</span></span>
