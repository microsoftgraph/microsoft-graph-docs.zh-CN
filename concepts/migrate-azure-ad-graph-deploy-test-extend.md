---
title: 部署、测试和扩展迁移的应用
description: 介绍如何将 Azure Active Directory (Azure AD) 应用迁移到使用 Microsoft Graph API (REST) ;这将讨论步骤 3：部署、测试和扩展。
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 55bca2b1d8499ef7ad788555f55f5f92033d1818
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470611"
---
# <a name="deploy-test-and-extend"></a><span data-ttu-id="61b6f-103">部署、测试和扩展</span><span class="sxs-lookup"><span data-stu-id="61b6f-103">Deploy, test, and extend</span></span>

<span data-ttu-id="61b6f-104">这是迁移应用 [的过程的第](migrate-azure-ad-graph-planning-checklist.md)4 步。</span><span class="sxs-lookup"><span data-stu-id="61b6f-104">This is step 4 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

1.  <span data-ttu-id="61b6f-105">**通过测试**</span><span class="sxs-lookup"><span data-stu-id="61b6f-105">**Test throughly**</span></span>

    <span data-ttu-id="61b6f-106">更新应用后，请全面测试它，以验证它是否正常工作，以及你尚未引入任何回归。</span><span class="sxs-lookup"><span data-stu-id="61b6f-106">Once you've updated your app, test it thoroughly to verify that it works as expected and that you haven't introduced any regressions.</span></span>  

    <span data-ttu-id="61b6f-107">请确保使用多个环境、数据集和最终用户角色，例如具有不同的角色、权限和职责的凭据。</span><span class="sxs-lookup"><span data-stu-id="61b6f-107">Be sure to use multiple environments, data sets, and end-user personas, e.g. credentials with different roles, rights, and responsibilities.</span></span> <span data-ttu-id="61b6f-108">通过让新的测试用户首次获取应用，以及已同意再次使用应用的现有用户 (，) 整个生命周期。</span><span class="sxs-lookup"><span data-stu-id="61b6f-108">Go through the entire lifecycle, by having a new test user acquire the app for the first time, as well as an existing user (who already consented) trying to use the app again.</span></span>

2.  <span data-ttu-id="61b6f-109">**部署阶段更新**</span><span class="sxs-lookup"><span data-stu-id="61b6f-109">**Deploy staged updates**</span></span>

    <span data-ttu-id="61b6f-110">请考虑分步部署更新。</span><span class="sxs-lookup"><span data-stu-id="61b6f-110">Consider deploying your updates in stages.</span></span>  <span data-ttu-id="61b6f-111">向一小组友好用户进行有限推出可帮助识别故障和其他潜在的麻烦问题。</span><span class="sxs-lookup"><span data-stu-id="61b6f-111">A limited roll-out to a small set of friendly users can help identify glitches and other potentially-embarrassing issues.</span></span>  <span data-ttu-id="61b6f-112">这还让你有机会监视初始接收和反馈。</span><span class="sxs-lookup"><span data-stu-id="61b6f-112">This also gives you a chance to monitor initial reception and feedback.</span></span>

    <span data-ttu-id="61b6f-113">如果初始推出成功，在部署到更大受众时监视进度。</span><span class="sxs-lookup"><span data-stu-id="61b6f-113">If the initial roll-out goes well, monitor progress as you deploy to larger audiences.</span></span>

3.  <span data-ttu-id="61b6f-114">**探索新值**</span><span class="sxs-lookup"><span data-stu-id="61b6f-114">**Explore new value**</span></span>

    <span data-ttu-id="61b6f-115">现在，你已切换到 Microsoft Graph，解锁现在触手可及的更多数据集和功能从未如此简单。</span><span class="sxs-lookup"><span data-stu-id="61b6f-115">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> 
    <span data-ttu-id="61b6f-116">Microsoft Graph 支持 Azure AD Graph 中不可用的许多新的 Azure AD 数据集和功能，包括：</span><span class="sxs-lookup"><span data-stu-id="61b6f-116">Microsoft Graph supports many new Azure AD datasets and features that are not available in Azure AD Graph, including:</span></span> 

    - [<span data-ttu-id="61b6f-117">Microsoft 365 组管理</span><span class="sxs-lookup"><span data-stu-id="61b6f-117">Microsoft 365 group management</span></span>](./office365-groups-concept-overview.md)
    - [<span data-ttu-id="61b6f-118">外部用户邀请</span><span class="sxs-lookup"><span data-stu-id="61b6f-118">External user invitations</span></span>](/graph/api/resources/invitation?view=graph-rest-1.0)
    - <span data-ttu-id="61b6f-119">删除用户 [和 Microsoft 365](/graph/api/resources/directory?view=graph-rest-1.0) 组后还原它们的能力</span><span class="sxs-lookup"><span data-stu-id="61b6f-119">The ability to [restore users and Microsoft 365 groups](/graph/api/resources/directory?view=graph-rest-1.0) after they've been deleted</span></span>
    - [<span data-ttu-id="61b6f-120">有关用户和组的 Webhook 通知</span><span class="sxs-lookup"><span data-stu-id="61b6f-120">Webhook notifications on users and groups</span></span>](./webhooks.md?toc=.%252fref%252ftoc.json&view=graph-rest-1.0)
    - <span data-ttu-id="61b6f-121">标识治理功能，例如：</span><span class="sxs-lookup"><span data-stu-id="61b6f-121">Identity governance features such as:</span></span>
      - <span data-ttu-id="61b6f-122">[特权标识管理](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) 仅在需要时和在有限时段内将用户提升为特权角色</span><span class="sxs-lookup"><span data-stu-id="61b6f-122">[Privileged identity management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) to elevate users to privileged roles only when needed and for a limited time period</span></span>
      - <span data-ttu-id="61b6f-123">[有关用户](/graph/api/resources/accessreviews-root?view=graph-rest-beta) 访问权限证明的一次性或定期访问评审的访问评审</span><span class="sxs-lookup"><span data-stu-id="61b6f-123">[Access reviews](/graph/api/resources/accessreviews-root?view=graph-rest-beta) for one-time or recurring access reviews for attestation of user's access rights</span></span>
      - <span data-ttu-id="61b6f-124">[使组织能够](/graph/api/resources/accessreviews-root?view=graph-rest-beta) 显示法律或合规性要求的信息的使用条款，如免责声明通知</span><span class="sxs-lookup"><span data-stu-id="61b6f-124">[Terms-of-use](/graph/api/resources/accessreviews-root?view=graph-rest-beta) to enable organizations to present information for legal or compliance requirements, like disclaimer notices</span></span>
    - <span data-ttu-id="61b6f-125">安全功能，例如：</span><span class="sxs-lookup"><span data-stu-id="61b6f-125">Security features such as:</span></span>
      - [<span data-ttu-id="61b6f-126">身份风险事件</span><span class="sxs-lookup"><span data-stu-id="61b6f-126">Identity risk events</span></span>](/graph/api/resources/identityriskevent?view=graph-rest-1.0)
      - [<span data-ttu-id="61b6f-127">风险用户</span><span class="sxs-lookup"><span data-stu-id="61b6f-127">Risky users</span></span>](/graph/api/resources/riskyuser?view=graph-rest-1.0)
    - <span data-ttu-id="61b6f-128">[更多平台和语言](./index.yml) 中提供了客户端库和示例。</span><span class="sxs-lookup"><span data-stu-id="61b6f-128">[Client libraries and samples](./index.yml) available on many more platforms and languages.</span></span> <span data-ttu-id="61b6f-129">Microsoft Graph SDK 提供了一个可发现接口，在以透明方式处理令牌获取、由于错误和限制而重试处理、安全重定向处理以及模型序列化和反序列化时，可轻松访问你的数据。</span><span class="sxs-lookup"><span data-stu-id="61b6f-129">The Microsoft Graph SDKs provide a discoverable interface to easily access your data while transparently handling token acquisition, retry handling due to errors and throttling, secure redirect handling and model serialization and deserialization.</span></span>

    <span data-ttu-id="61b6f-130">Microsoft Graph 提供对更多服务的访问权限，而不只是 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="61b6f-130">Microsoft Graph offers access to many more services than just Azure Active Directory.</span></span> <span data-ttu-id="61b6f-131">这也是 Microsoft [365 服务的 API 网关](./index.yml)。</span><span class="sxs-lookup"><span data-stu-id="61b6f-131">It's the [API gateway to Microsoft 365 services too](./index.yml).</span></span>
    <span data-ttu-id="61b6f-132">定期检查新的数据集和功能。</span><span class="sxs-lookup"><span data-stu-id="61b6f-132">Check for new datasets and capabilities regularly.</span></span>  

    - <span data-ttu-id="61b6f-133">查看可以使用 [Microsoft Graph 执行哪些功能](/graph/examples)</span><span class="sxs-lookup"><span data-stu-id="61b6f-133">Take a look at [what you can do with Microsoft Graph](/graph/examples)</span></span>
    - <span data-ttu-id="61b6f-134">浏览 [Microsoft Graph 博客](/graph/blogs) ，了解有关 Microsoft Graph 的最新新闻和一些出色的学习系列。</span><span class="sxs-lookup"><span data-stu-id="61b6f-134">Explore the [Microsoft Graph blog](/graph/blogs) for the latest news about Microsoft Graph and some great learning series.</span></span>
    - <span data-ttu-id="61b6f-135">更改 [日志汇总](/greaph/changelog) 了服务和文档更新。</span><span class="sxs-lookup"><span data-stu-id="61b6f-135">The [changelog](/greaph/changelog) summarizes service and document updates.</span></span> <span data-ttu-id="61b6f-136">遵循这些更新将帮助您跟踪 /beta (预览版中引入的新 API) 以及已提升为 (GA) 。</span><span class="sxs-lookup"><span data-stu-id="61b6f-136">Following these updates will help you track new APIs introduced to /beta (preview) and those promoted to v1.0 (GA).</span></span>  <span data-ttu-id="61b6f-137">这些新 API 可以为你提供向应用添加更多价值和新体验的新的方法。</span><span class="sxs-lookup"><span data-stu-id="61b6f-137">These new APIs can provide new ways for you to add more value and new experiences to your apps.</span></span>  

## <a name="see-also"></a><span data-ttu-id="61b6f-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="61b6f-138">See also</span></span>

<span data-ttu-id="61b6f-139">如果在迁移过程中遇到问题或需要帮助，可以：</span><span class="sxs-lookup"><span data-stu-id="61b6f-139">If you run into problems or need help during the migration process, you can:</span></span>

- <span data-ttu-id="61b6f-140">再次 [查看检查](migrate-azure-ad-graph-planning-checklist.md) 表</span><span class="sxs-lookup"><span data-stu-id="61b6f-140">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again</span></span>
- <span data-ttu-id="61b6f-141">向 [Microsoft 问答&问题](https://docs.microsoft.com/answers/topics/microsoft-graph-applications.html)</span><span class="sxs-lookup"><span data-stu-id="61b6f-141">Post questions to [Microsoft Q&A](https://docs.microsoft.com/answers/topics/microsoft-graph-applications.html)</span></span> 
- <span data-ttu-id="61b6f-142">查看 Microsoft Graph 示例以对比和比较现有应用程序代码：</span><span class="sxs-lookup"><span data-stu-id="61b6f-142">Review Microsoft Graph samples to contrast and compare with your existing application code:</span></span>
  - <span data-ttu-id="61b6f-143">**使用 REST API** 的应用：浏览 [快速入门](https://developer.microsoft.com/graph/get-started)和示例、选择选择的平台并运行快速入门或搜索相应示例</span><span class="sxs-lookup"><span data-stu-id="61b6f-143">**Apps that use the REST API**: explore [quick starts and samples](https://developer.microsoft.com/graph/get-started), choosing your platform of choice and run through the quick start or search for an appropriate sample</span></span>
  - <span data-ttu-id="61b6f-144">**使用 .NET 客户端库的应用**：查看 [console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) 和/或 [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)</span><span class="sxs-lookup"><span data-stu-id="61b6f-144">**App that use the .NET client library**: review [console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) and/or [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)</span></span>

## <a name="next-steps"></a><span data-ttu-id="61b6f-145">后续步骤</span><span class="sxs-lookup"><span data-stu-id="61b6f-145">Next Steps</span></span>

- <span data-ttu-id="61b6f-146">使用 [快速入门和示例](/graph/get-started) 快速入门。</span><span class="sxs-lookup"><span data-stu-id="61b6f-146">Use [quick starts and samples](/graph/get-started) to come up to speed quickly.</span></span>
- <span data-ttu-id="61b6f-147">利用 [客户端库和 SDK](https://developer.microsoft.com/graph/get-started) 开发自定义应用程序</span><span class="sxs-lookup"><span data-stu-id="61b6f-147">Leverage [client libraries and SDKs](https://developer.microsoft.com/graph/get-started) to develop custom applications</span></span> 
- <span data-ttu-id="61b6f-148">探索 [Microsoft Graph](./overview.md) 的概念和做法。</span><span class="sxs-lookup"><span data-stu-id="61b6f-148">Explore [Microsoft Graph](./overview.md) concepts and practices.</span></span>
- <span data-ttu-id="61b6f-149">使用 [Graph 资源管理器](https://aka.ms/ge) 试验 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="61b6f-149">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>