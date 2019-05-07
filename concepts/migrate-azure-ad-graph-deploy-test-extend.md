---
title: 部署、测试和扩展迁移的应用程序
description: '介绍如何将 Azure Active Directory (Azure AD) 应用迁移为使用 Microsoft Graph API (REST);这讨论了步骤 3: 部署、测试和扩展。'
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8a63c14ef27648a1d586551ebe12e18a5f263a9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630249"
---
# <a name="deploy-test-and-extend"></a><span data-ttu-id="12d26-103">部署、测试和扩展</span><span class="sxs-lookup"><span data-stu-id="12d26-103">Deploy, test, and extend</span></span>

<span data-ttu-id="12d26-104">这是[迁移应用程序过程](migrate-azure-ad-graph-planning-checklist.md)的第4步。</span><span class="sxs-lookup"><span data-stu-id="12d26-104">This is step 4 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

1.  <span data-ttu-id="12d26-105">**测试 throughly**</span><span class="sxs-lookup"><span data-stu-id="12d26-105">**Test throughly**</span></span>

    <span data-ttu-id="12d26-106">更新应用后, 请对其进行全面测试, 以验证它是否按预期运行, 并且未引入任何回归。</span><span class="sxs-lookup"><span data-stu-id="12d26-106">Once you've updated your app, test it thoroughly to verify that it works as expected and that you haven't introduced any regressions.</span></span>  

    <span data-ttu-id="12d26-107">请务必使用多个环境、数据集和最终用户角色, 例如具有不同角色、权利和责任的凭据。</span><span class="sxs-lookup"><span data-stu-id="12d26-107">Be sure to use multiple environments, data sets, and end-user personas, e.g. credentials with different roles, rights, and responsibilities.</span></span> <span data-ttu-id="12d26-108">通过让新的测试用户首次获取应用程序以及尝试再次使用应用程序的现有用户 (已有权), 完成整个生命周期。</span><span class="sxs-lookup"><span data-stu-id="12d26-108">Go through the entire lifecycle, by having a new test user acquire the app for the first time, as well as an existing user (who already consented) trying to use the app again.</span></span>

2.  <span data-ttu-id="12d26-109">**部署暂存更新**</span><span class="sxs-lookup"><span data-stu-id="12d26-109">**Deploy staged updates**</span></span>

    <span data-ttu-id="12d26-110">请考虑分阶段部署更新。</span><span class="sxs-lookup"><span data-stu-id="12d26-110">Consider deploying your updates in stages.</span></span>  <span data-ttu-id="12d26-111">仅向一小部分友好用户进行有限的滚动, 可帮助确定故障和其他可能 embarrassing 的问题。</span><span class="sxs-lookup"><span data-stu-id="12d26-111">A limited roll-out to a small set of friendly users can help identify glitches and other potentially-embarrassing issues.</span></span>  <span data-ttu-id="12d26-112">这还为您提供了监视初始接收和反馈的机会。</span><span class="sxs-lookup"><span data-stu-id="12d26-112">This also gives you a chance to monitor initial reception and feedback.</span></span>

    <span data-ttu-id="12d26-113">如果初始滚动很好, 请在部署到更大的访问群体时监视进度。</span><span class="sxs-lookup"><span data-stu-id="12d26-113">If the initial roll-out goes well, monitor progress as you deploy to larger audiences.</span></span>

3.  <span data-ttu-id="12d26-114">**浏览新值**</span><span class="sxs-lookup"><span data-stu-id="12d26-114">**Explore new value**</span></span>

    <span data-ttu-id="12d26-115">现在, 您已将切换到 Microsoft Graph, 对现在可以轻松解锁的更多数据集和功能的方法也变得更加轻松了。</span><span class="sxs-lookup"><span data-stu-id="12d26-115">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="12d26-116">定期检查新的数据集和功能。</span><span class="sxs-lookup"><span data-stu-id="12d26-116">Check for new datasets and capabilities regularly.</span></span>  

    - <span data-ttu-id="12d26-117">请参阅[使用 Microsoft Graph 可以执行的操作](/graph/examples)</span><span class="sxs-lookup"><span data-stu-id="12d26-117">Take a look at [what you can do with Microsoft Graph](/graph/examples)</span></span>
    - <span data-ttu-id="12d26-118">浏览[Microsoft graph 博客](/graph/blogs), 了解有关 Microsoft Graph 的最新新闻和一些出色的学习系列。</span><span class="sxs-lookup"><span data-stu-id="12d26-118">Explore the [Microsoft Graph blog](/graph/blogs) for the latest news about Microsoft Graph and some great learning series.</span></span>
    - <span data-ttu-id="12d26-119">[更改日志](/greaph/changelog)汇总了服务和文档更新。</span><span class="sxs-lookup"><span data-stu-id="12d26-119">The [changelog](/greaph/changelog) summarizes service and document updates.</span></span> <span data-ttu-id="12d26-120">按照这些更新, 将帮助您跟踪引入到/beta (预览) 的新 Api 以及升级为 v1。0 (GA) 的新 Api。</span><span class="sxs-lookup"><span data-stu-id="12d26-120">Following these updates will help you track new APIs introduced to /beta (preview) and those promoted to v1.0 (GA).</span></span>  <span data-ttu-id="12d26-121">这些新 Api 可为你提供新的方法, 以向你的应用添加更多价值和新体验。</span><span class="sxs-lookup"><span data-stu-id="12d26-121">These new APIs can provide new ways for you to add more value and new experiences to your apps.</span></span>  

## <a name="see-also"></a><span data-ttu-id="12d26-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="12d26-122">See also</span></span>

<span data-ttu-id="12d26-123">如果在迁移过程中遇到问题或需要帮助, 可以执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="12d26-123">If you run into problems or need help during the migration process, you can:</span></span>

- <span data-ttu-id="12d26-124">再次查看[检查表](migrate-azure-ad-graph-overview.md)</span><span class="sxs-lookup"><span data-stu-id="12d26-124">Review the [checklist](migrate-azure-ad-graph-overview.md) again</span></span>
- <span data-ttu-id="12d26-125">将问题发布到[StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)</span><span class="sxs-lookup"><span data-stu-id="12d26-125">Post questions to [StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)</span></span>
- <span data-ttu-id="12d26-126">查看 Microsoft Graph 示例以对比现有应用程序代码并与之进行比较:</span><span class="sxs-lookup"><span data-stu-id="12d26-126">Review Microsoft Graph samples to contrast and compare with your existing application code:</span></span>
  - <span data-ttu-id="12d26-127">**使用 REST API 的应用程序**: 浏览[快速入门和示例](/graph/get-started), 选择您的选择平台, 并在快速启动或搜索相应的示例中运行</span><span class="sxs-lookup"><span data-stu-id="12d26-127">**Apps that use the REST API**: explore [quick starts and samples](/graph/get-started), choosing your platform of choice and run through the quick start or search for an appropriate sample</span></span>
  - <span data-ttu-id="12d26-128">**使用 .net 客户端库的应用程序**: 查看[控制台-csharp-示例](https://github.com/microsoftgraph/console-csharp-snippets-sample)和/或[dotnetcore-示例](https://github.com/microsoftgraph/dotnetcore-console-sample)</span><span class="sxs-lookup"><span data-stu-id="12d26-128">**App that use the .NET client library**: review [console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) and/or [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)</span></span>

## <a name="next-steps"></a><span data-ttu-id="12d26-129">后续步骤</span><span class="sxs-lookup"><span data-stu-id="12d26-129">Next Steps</span></span>

- <span data-ttu-id="12d26-130">使用[快速入门和示例](/graph/get-started)快速提高速度。</span><span class="sxs-lookup"><span data-stu-id="12d26-130">Use [quick starts and samples](/graph/get-started) to come up to speed quickly.</span></span>
- <span data-ttu-id="12d26-131">利用[客户端库和 sdk](https://developer.microsoft.com/graph/get-started)开发自定义应用程序</span><span class="sxs-lookup"><span data-stu-id="12d26-131">Leverage [client libraries and SDKs](https://developer.microsoft.com/graph/get-started) to develop custom applications</span></span> 
- <span data-ttu-id="12d26-132">浏览[Microsoft Graph](/graph/overview)概念和实践。</span><span class="sxs-lookup"><span data-stu-id="12d26-132">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="12d26-133">使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="12d26-133">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
