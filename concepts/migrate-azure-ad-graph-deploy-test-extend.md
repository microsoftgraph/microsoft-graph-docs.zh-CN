---
title: 部署、测试和扩展迁移的应用程序
description: 介绍如何将 Azure Active Directory (Azure AD) 应用程序迁移到使用 Microsoft Graph API (REST) ;这讨论了步骤3：部署、测试和扩展。
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 57ee22b7c1f04e9f8fd4a6a1f3ec0d32f75d51be
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872941"
---
# <a name="deploy-test-and-extend"></a><span data-ttu-id="ecb51-103">部署、测试和扩展</span><span class="sxs-lookup"><span data-stu-id="ecb51-103">Deploy, test, and extend</span></span>

<span data-ttu-id="ecb51-104">这是 [迁移应用程序过程](migrate-azure-ad-graph-planning-checklist.md)的第4步。</span><span class="sxs-lookup"><span data-stu-id="ecb51-104">This is step 4 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

1.  <span data-ttu-id="ecb51-105">**测试 throughly**</span><span class="sxs-lookup"><span data-stu-id="ecb51-105">**Test throughly**</span></span>

    <span data-ttu-id="ecb51-106">更新应用后，请对其进行全面测试，以验证它是否按预期运行，并且未引入任何回归。</span><span class="sxs-lookup"><span data-stu-id="ecb51-106">Once you've updated your app, test it thoroughly to verify that it works as expected and that you haven't introduced any regressions.</span></span>  

    <span data-ttu-id="ecb51-107">请务必使用多个环境、数据集和最终用户角色，例如具有不同角色、权利和责任的凭据。</span><span class="sxs-lookup"><span data-stu-id="ecb51-107">Be sure to use multiple environments, data sets, and end-user personas, e.g. credentials with different roles, rights, and responsibilities.</span></span> <span data-ttu-id="ecb51-108">在整个生命周期中，让新的测试用户首次获取应用程序，以及现有用户 (已) 尝试再次使用应用程序的现有用户。</span><span class="sxs-lookup"><span data-stu-id="ecb51-108">Go through the entire lifecycle, by having a new test user acquire the app for the first time, as well as an existing user (who already consented) trying to use the app again.</span></span>

2.  <span data-ttu-id="ecb51-109">**部署暂存更新**</span><span class="sxs-lookup"><span data-stu-id="ecb51-109">**Deploy staged updates**</span></span>

    <span data-ttu-id="ecb51-110">请考虑分阶段部署更新。</span><span class="sxs-lookup"><span data-stu-id="ecb51-110">Consider deploying your updates in stages.</span></span>  <span data-ttu-id="ecb51-111">仅向一小部分友好用户进行有限的滚动，可帮助确定故障和其他可能 embarrassing 的问题。</span><span class="sxs-lookup"><span data-stu-id="ecb51-111">A limited roll-out to a small set of friendly users can help identify glitches and other potentially-embarrassing issues.</span></span>  <span data-ttu-id="ecb51-112">这还为您提供了监视初始接收和反馈的机会。</span><span class="sxs-lookup"><span data-stu-id="ecb51-112">This also gives you a chance to monitor initial reception and feedback.</span></span>

    <span data-ttu-id="ecb51-113">如果初始滚动很好，请在部署到更大的访问群体时监视进度。</span><span class="sxs-lookup"><span data-stu-id="ecb51-113">If the initial roll-out goes well, monitor progress as you deploy to larger audiences.</span></span>

3.  <span data-ttu-id="ecb51-114">**浏览新值**</span><span class="sxs-lookup"><span data-stu-id="ecb51-114">**Explore new value**</span></span>

    <span data-ttu-id="ecb51-115">现在，您已将切换到 Microsoft Graph，对现在可以轻松解锁的更多数据集和功能的方法也变得更加轻松了。</span><span class="sxs-lookup"><span data-stu-id="ecb51-115">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> 
    <span data-ttu-id="ecb51-116">Microsoft Graph 支持 Azure AD Graph 中不可用的许多新的 Azure AD 数据集和功能，包括：</span><span class="sxs-lookup"><span data-stu-id="ecb51-116">Microsoft Graph supports many new Azure AD datasets and features that are not available in Azure AD Graph, including:</span></span> 

    - [<span data-ttu-id="ecb51-117">Microsoft 365 组管理</span><span class="sxs-lookup"><span data-stu-id="ecb51-117">Microsoft 365 group management</span></span>](/graph/office365-groups-concept-overview)
    - [<span data-ttu-id="ecb51-118">外部用户邀请</span><span class="sxs-lookup"><span data-stu-id="ecb51-118">External user invitations</span></span>](/graph/api/resources/invitation?view=graph-rest-1.0)
    - <span data-ttu-id="ecb51-119">能够在删除 [用户和 Microsoft 365 组](/graph/api/resources/directory?view=graph-rest-1.0) 之后对其进行还原</span><span class="sxs-lookup"><span data-stu-id="ecb51-119">The ability to [restore users and Microsoft 365 groups](/graph/api/resources/directory?view=graph-rest-1.0) after they've been deleted</span></span>
    - [<span data-ttu-id="ecb51-120">用户和组上的 Webhook 通知</span><span class="sxs-lookup"><span data-stu-id="ecb51-120">Webhook notifications on users and groups</span></span>](/graph/webhooks?toc=./ref/toc.json&view=graph-rest-1.0)
    - <span data-ttu-id="ecb51-121">身份管理功能，如：</span><span class="sxs-lookup"><span data-stu-id="ecb51-121">Identity governance features such as:</span></span>
      - <span data-ttu-id="ecb51-122">[特权身份管理](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) 仅在需要时和在有限的时间段内将用户提升到特权角色</span><span class="sxs-lookup"><span data-stu-id="ecb51-122">[Privileged identity management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) to elevate users to privileged roles only when needed and for a limited time period</span></span>
      - <span data-ttu-id="ecb51-123">[对用户](/graph/api/resources/accessreviews-root?view=graph-rest-beta) 访问权限证明的一次性或定期访问审核</span><span class="sxs-lookup"><span data-stu-id="ecb51-123">[Access reviews](/graph/api/resources/accessreviews-root?view=graph-rest-beta) for one-time or recurring access reviews for attestation of user's access rights</span></span>
      - <span data-ttu-id="ecb51-124">帮助组织提供有关法律或合规性要求的信息（如免责声明通知）[的使用条款](/graph/api/resources/accessreviews-root?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="ecb51-124">[Terms-of-use](/graph/api/resources/accessreviews-root?view=graph-rest-beta) to enable organizations to present information for legal or compliance requirements, like disclaimer notices</span></span>
    - <span data-ttu-id="ecb51-125">安全功能，如：</span><span class="sxs-lookup"><span data-stu-id="ecb51-125">Security features such as:</span></span>
      - [<span data-ttu-id="ecb51-126">身份风险事件</span><span class="sxs-lookup"><span data-stu-id="ecb51-126">Identity risk events</span></span>](/graph/api/resources/identityriskevent?view=graph-rest-1.0)
      - [<span data-ttu-id="ecb51-127">风险用户</span><span class="sxs-lookup"><span data-stu-id="ecb51-127">Risky users</span></span>](/graph/api/resources/riskyuser?view=graph-rest-1.0)
    - <span data-ttu-id="ecb51-128">可在更多平台和语言中使用的[客户端库和示例](/graph/)。</span><span class="sxs-lookup"><span data-stu-id="ecb51-128">[Client libraries and samples](/graph/) available on many more platforms and languages.</span></span> <span data-ttu-id="ecb51-129">Microsoft Graph Sdk 提供了一个可发现接口，可在透明地处理令牌获取、重试处理（由于错误和限制、安全重定向处理以及模型序列化和反序列化）而轻松访问数据。</span><span class="sxs-lookup"><span data-stu-id="ecb51-129">The Microsoft Graph SDKs provide a discoverable interface to easily access your data while transparently handling token acquisition, retry handling due to errors and throttling, secure redirect handling and model serialization and deserialization.</span></span>

    <span data-ttu-id="ecb51-130">与 Azure Active Directory 相比，Microsoft Graph 提供了更多的服务访问权限。</span><span class="sxs-lookup"><span data-stu-id="ecb51-130">Microsoft Graph offers access to many more services than just Azure Active Directory.</span></span> <span data-ttu-id="ecb51-131">这也是 [Microsoft 365 服务的 API 网关](/graph/)。</span><span class="sxs-lookup"><span data-stu-id="ecb51-131">It's the [API gateway to Microsoft 365 services too](/graph/).</span></span>
    <span data-ttu-id="ecb51-132">定期检查新的数据集和功能。</span><span class="sxs-lookup"><span data-stu-id="ecb51-132">Check for new datasets and capabilities regularly.</span></span>  

    - <span data-ttu-id="ecb51-133">请参阅 [使用 Microsoft Graph 可以执行的操作](/graph/examples)</span><span class="sxs-lookup"><span data-stu-id="ecb51-133">Take a look at [what you can do with Microsoft Graph](/graph/examples)</span></span>
    - <span data-ttu-id="ecb51-134">浏览 [Microsoft graph 博客](/graph/blogs) ，了解有关 Microsoft Graph 的最新新闻和一些出色的学习系列。</span><span class="sxs-lookup"><span data-stu-id="ecb51-134">Explore the [Microsoft Graph blog](/graph/blogs) for the latest news about Microsoft Graph and some great learning series.</span></span>
    - <span data-ttu-id="ecb51-135">[更改日志](/greaph/changelog)汇总了服务和文档更新。</span><span class="sxs-lookup"><span data-stu-id="ecb51-135">The [changelog](/greaph/changelog) summarizes service and document updates.</span></span> <span data-ttu-id="ecb51-136">按照这些更新，将帮助您跟踪引入到/beta (preview) 的新 Api，以及升级到 (GA) 的新 Api。</span><span class="sxs-lookup"><span data-stu-id="ecb51-136">Following these updates will help you track new APIs introduced to /beta (preview) and those promoted to v1.0 (GA).</span></span>  <span data-ttu-id="ecb51-137">这些新 Api 可为你提供新的方法，以向你的应用添加更多价值和新体验。</span><span class="sxs-lookup"><span data-stu-id="ecb51-137">These new APIs can provide new ways for you to add more value and new experiences to your apps.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ecb51-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ecb51-138">See also</span></span>

<span data-ttu-id="ecb51-139">如果在迁移过程中遇到问题或需要帮助，可以执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="ecb51-139">If you run into problems or need help during the migration process, you can:</span></span>

- <span data-ttu-id="ecb51-140">再次查看[检查表](migrate-azure-ad-graph-planning-checklist.md)</span><span class="sxs-lookup"><span data-stu-id="ecb51-140">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again</span></span>
- <span data-ttu-id="ecb51-141">将问题发布到 [StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)</span><span class="sxs-lookup"><span data-stu-id="ecb51-141">Post questions to [StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)</span></span>
- <span data-ttu-id="ecb51-142">查看 Microsoft Graph 示例以对比现有应用程序代码并与之进行比较：</span><span class="sxs-lookup"><span data-stu-id="ecb51-142">Review Microsoft Graph samples to contrast and compare with your existing application code:</span></span>
  - <span data-ttu-id="ecb51-143">**使用 REST API 的应用程序**：浏览 [快速入门和示例](https://developer.microsoft.com/graph/get-started)，选择您的选择平台，并在快速启动或搜索相应的示例中运行</span><span class="sxs-lookup"><span data-stu-id="ecb51-143">**Apps that use the REST API**: explore [quick starts and samples](https://developer.microsoft.com/graph/get-started), choosing your platform of choice and run through the quick start or search for an appropriate sample</span></span>
  - <span data-ttu-id="ecb51-144">**使用 .net 客户端库的应用程序**：查看 [控制台-csharp-示例](https://github.com/microsoftgraph/console-csharp-snippets-sample) 和/或 [dotnetcore-示例](https://github.com/microsoftgraph/dotnetcore-console-sample)</span><span class="sxs-lookup"><span data-stu-id="ecb51-144">**App that use the .NET client library**: review [console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) and/or [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)</span></span>

## <a name="next-steps"></a><span data-ttu-id="ecb51-145">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ecb51-145">Next Steps</span></span>

- <span data-ttu-id="ecb51-146">使用 [快速入门和示例](/graph/get-started) 快速提高速度。</span><span class="sxs-lookup"><span data-stu-id="ecb51-146">Use [quick starts and samples](/graph/get-started) to come up to speed quickly.</span></span>
- <span data-ttu-id="ecb51-147">利用 [客户端库和 sdk](https://developer.microsoft.com/graph/get-started) 开发自定义应用程序</span><span class="sxs-lookup"><span data-stu-id="ecb51-147">Leverage [client libraries and SDKs](https://developer.microsoft.com/graph/get-started) to develop custom applications</span></span> 
- <span data-ttu-id="ecb51-148">浏览 [Microsoft Graph](/graph/overview) 概念和实践。</span><span class="sxs-lookup"><span data-stu-id="ecb51-148">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="ecb51-149">使用 [Graph 浏览器](https://aka.ms/ge) 试用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="ecb51-149">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
