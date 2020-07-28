---
title: 'Microsoft Graph 的版本控制、支持和重大更改策略 '
description: 本文介绍了 Microsoft Graph 的支持和重大更改策略，以及当前可用的 Microsoft Graph API 版本。
localization_priority: Priority
ms.openlocfilehash: 0c23ec2e358547a7824a9417e167e3c057c52b43
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427380"
---
# <a name="versioning-support-and-breaking-change-policies-for-microsoft-graph"></a><span data-ttu-id="da9ff-103">Microsoft Graph 的版本控制、支持和中断性变更策略</span><span class="sxs-lookup"><span data-stu-id="da9ff-103">Versioning, support, and breaking change policies for Microsoft Graph</span></span>

<span data-ttu-id="da9ff-104">本文介绍了 Microsoft Graph 的支持和重大更改策略，以及当前可用的 Microsoft Graph API 版本。</span><span class="sxs-lookup"><span data-stu-id="da9ff-104">This article describes the support and breaking change policies for Microsoft Graph and the versions of the Microsoft Graph API that are currently available.</span></span>

## <a name="support-policy-and-deprecation-information"></a><span data-ttu-id="da9ff-105">支持策略和弃用信息</span><span class="sxs-lookup"><span data-stu-id="da9ff-105">Support policy and deprecation information</span></span>

<span data-ttu-id="da9ff-106">Microsoft Graph 遵循 [Microsoft 生命周期策略](https://support.microsoft.com/lifecycle)。</span><span class="sxs-lookup"><span data-stu-id="da9ff-106">Microsoft Graph follows the [Microsoft Lifecycle Policy](https://support.microsoft.com/lifecycle).</span></span>

<span data-ttu-id="da9ff-p101">由于已发布新版本的 Microsoft Graph REST API 和 Microsoft Graph SDK，之前的版本将停用。Microsoft 将在停用 API 或 SDK 之前至少 24 个月声明弃用的版本。</span><span class="sxs-lookup"><span data-stu-id="da9ff-p101">As new versions of the Microsoft Graph REST APIs and Microsoft Graph SDKs are released, earlier versions will be retired. Microsoft will declare a version as deprecated at least 24 months in advance of retiring an API or an SDK.</span></span>

<span data-ttu-id="da9ff-109">递增 API 的主要版本（例如，从 v1.0 到 v2.0）时，我们将通知立即弃用当前版本（在此示例中为 v1.0），在通知 24 个月后，我们将不再支持该版本。</span><span class="sxs-lookup"><span data-stu-id="da9ff-109">When we increment the major version of the API (for example, from v1.0 to v2.0), we are announcing that the current version (in this example, v1.0) is immediately deprecated and we will no longer support it 24 months after the announcement.</span></span> <span data-ttu-id="da9ff-110">出于服务安全或运行状况可靠性问题的考虑，我们可能会对此策略作例外处理。</span><span class="sxs-lookup"><span data-stu-id="da9ff-110">We might make exceptions to this policy for service security or health reliability issues.</span></span>

<span data-ttu-id="da9ff-111">当 API 被标记为已弃用时，我们强烈建议你尽快迁移到最新版本。</span><span class="sxs-lookup"><span data-stu-id="da9ff-111">When an API is marked as deprecated, we strongly recommend that you migrate to the latest version as soon as possible.</span></span> <span data-ttu-id="da9ff-112">某些情况下，我们将公布新应用程序必须在原始 API 弃用后不久开始使用新的 API。</span><span class="sxs-lookup"><span data-stu-id="da9ff-112">In some cases, we will announce that new applications will have to start using the new APIs a short time after the original APIs are deprecated.</span></span> <span data-ttu-id="da9ff-113">在这些情况下，仅当前使用已弃用 API 的活动应用程序能够继续使用它们。</span><span class="sxs-lookup"><span data-stu-id="da9ff-113">In those cases, only active applications that currently use the deprecated APIs can continue to use them.</span></span>

### <a name="api-contract-and-non-backward-compatible-changes"></a><span data-ttu-id="da9ff-114">API 协定和非后向兼容更改</span><span class="sxs-lookup"><span data-stu-id="da9ff-114">API contract and non-backward compatible changes</span></span>

<span data-ttu-id="da9ff-p104">Microsoft Graph 在版本中进行了许多更改。这些更改已在 [Microsoft Graph 更改日志](changelog.md)中列出。随着向 Microsoft Graph 中添加新功能和数据，我们将递增 API 版本号，以对 API 进行任意不向后兼容更改。</span><span class="sxs-lookup"><span data-stu-id="da9ff-p104">Microsoft Graph has a log of changes across versions. These changes are listed in the [Microsoft Graph Changelog](changelog.md). As new functionality and data is added to Microsoft Graph, we will increment the API version number for any non-backward compatible changes to the API.</span></span>

<span data-ttu-id="da9ff-118">非后向兼容更改的示例如下：</span><span class="sxs-lookup"><span data-stu-id="da9ff-118">The following are examples of non-backward compatible changes:</span></span>

- <span data-ttu-id="da9ff-119">对与资源关联的 URL 或基本请求/响应进行更改</span><span class="sxs-lookup"><span data-stu-id="da9ff-119">Changes to the URL or fundamental request/response associated with a resource</span></span>
- <span data-ttu-id="da9ff-120">删除、重命名或更改声明的属性的类型</span><span class="sxs-lookup"><span data-stu-id="da9ff-120">Removal, rename, or change to the type of a declared property</span></span>
- <span data-ttu-id="da9ff-121">删除或重命名 API 或 API 参数</span><span class="sxs-lookup"><span data-stu-id="da9ff-121">Removal or rename of APIs or API parameters</span></span>
- <span data-ttu-id="da9ff-122">添加所需的请求标头</span><span class="sxs-lookup"><span data-stu-id="da9ff-122">Addition of a required request header</span></span>

<span data-ttu-id="da9ff-123">向后兼容的更改示例如下：</span><span class="sxs-lookup"><span data-stu-id="da9ff-123">The following are examples of backward compatible changes:</span></span>

- <span data-ttu-id="da9ff-124">添加可为 Null 或具有默认值的属性</span><span class="sxs-lookup"><span data-stu-id="da9ff-124">Addition of properties that are nullable or have a default value</span></span>
- <span data-ttu-id="da9ff-125">向枚举添加成员</span><span class="sxs-lookup"><span data-stu-id="da9ff-125">Addition of a member to an enumeration</span></span>
- <span data-ttu-id="da9ff-126">删除、重命名或更改开放扩展的类型</span><span class="sxs-lookup"><span data-stu-id="da9ff-126">Removal, rename, or change to the type of an open extension</span></span>
- <span data-ttu-id="da9ff-127">删除、重命名或更改注释的类型</span><span class="sxs-lookup"><span data-stu-id="da9ff-127">Removal, rename, or change to the type of an annotation</span></span>
- <span data-ttu-id="da9ff-128">向现有集合引入分页</span><span class="sxs-lookup"><span data-stu-id="da9ff-128">Introduction of paging to existing collections</span></span>
- <span data-ttu-id="da9ff-129">更改错误代码</span><span class="sxs-lookup"><span data-stu-id="da9ff-129">Changes to error codes</span></span>
- <span data-ttu-id="da9ff-130">更改属性的顺序</span><span class="sxs-lookup"><span data-stu-id="da9ff-130">Changes to the order of properties</span></span>
- <span data-ttu-id="da9ff-131">更改不透明字符串（如资源 ID）的长度或格式</span><span class="sxs-lookup"><span data-stu-id="da9ff-131">Changes to the length or format of opaque strings, such as resource IDs</span></span>

><span data-ttu-id="da9ff-p105">**注意：** 随着时间的推移，我们将更新向后兼容更改的列表。如果你生成了自己的客户端代理（如 WCF 客户端），我们的建议是，客户端应用程序应准备接收之前未由 Microsoft Graph API 服务定义的属性和派生类型。Microsoft Graph API 遵循 [Microsoft REST API 准则](https://github.com/microsoft/api-guidelines/)的[模型版本控制](https://github.com/microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning)部分中描述的指导。</span><span class="sxs-lookup"><span data-stu-id="da9ff-p105">**Note:** Over time, we will update the list of backward compatible changes. If you generate your own client proxies (like WCF clients), our guidance is that your client applications should be prepared to receive properties and derived types not previously defined by the Microsoft Graph API service. Microsoft Graph API follows the guidance described in the [Model Versioning](https://github.com/microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning) section in the [Microsoft REST API guidelines](https://github.com/microsoft/api-guidelines/).</span></span>

## <a name="versions"></a><span data-ttu-id="da9ff-135">版本</span><span class="sxs-lookup"><span data-stu-id="da9ff-135">Versions</span></span>

<span data-ttu-id="da9ff-136">以下版本的 Microsoft Graph API 目前可用。</span><span class="sxs-lookup"><span data-stu-id="da9ff-136">The following versions of the Microsoft Graph API are currently available.</span></span>

### <a name="beta-version"></a><span data-ttu-id="da9ff-137">Beta 版</span><span class="sxs-lookup"><span data-stu-id="da9ff-137">Beta version</span></span>
<span data-ttu-id="da9ff-138">通常，API在 beta 版本中首次亮相，并且可以在 `https://graph.microsoft.com/beta` 终结点中访问。</span><span class="sxs-lookup"><span data-stu-id="da9ff-138">In general, APIs debut in the beta version and are accessible in the `https://graph.microsoft.com/beta` endpoint.</span></span> <span data-ttu-id="da9ff-139">如需了解 beta API 文档，请参阅 [Microsoft Graph beta 终结点参考](/graph/api/overview?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="da9ff-139">For beta API documentation, see [Microsoft Graph beta endpoint reference](/graph/api/overview?view=graph-rest-beta).</span></span> <span data-ttu-id="da9ff-140">预计将不时地对 beta 版本进行重大更改。</span><span class="sxs-lookup"><span data-stu-id="da9ff-140">Expect breaking changes to the beta version from time to time.</span></span> <span data-ttu-id="da9ff-141">请勿对 /beta API 产生生产依赖性。</span><span class="sxs-lookup"><span data-stu-id="da9ff-141">Do not take a production dependency on /beta APIs.</span></span>

<span data-ttu-id="da9ff-p107">我们无法保证将测试功能升级至当前版本。当 Microsoft Graph API 团队认为测试功能可正式发布 (GA) 时，我们将把该功能添加到最新的当前版本中。如果功能升级将导致当前版本出现重大更改，则版本号将递增，而新版本将成为当前版本。我们的开发者社区可以在 [UserVoice](https://officespdev.uservoice.com/) 上发布功能请求，包括对新功能的请求以及将现有的测试 API 升级到当前版本的请求。</span><span class="sxs-lookup"><span data-stu-id="da9ff-p107">We make no guarantees that a beta feature will be promoted to the current version. When the Microsoft Graph API team believes that a beta feature is ready for general availability (GA), we will add that feature to the latest current version. If the promotion of the feature would result in a breaking change to the current version, the version number will be incremented, with the new version becoming the current version. Our developer community can post feature request on [UserVoice](https://officespdev.uservoice.com/), including requests for new features as well as requests to promote existing beta APIs to the current version.</span></span>

### <a name="current-version"></a><span data-ttu-id="da9ff-146">当前版本</span><span class="sxs-lookup"><span data-stu-id="da9ff-146">Current version</span></span>

<span data-ttu-id="da9ff-p108">Microsoft Graph 的当前版本为 v1.0。Microsoft Graph API /v1.0 版本在 `https://graph.microsoft.com/v1.0` 中公开，包含可正式发布和可用于生产的功能。可以浏览 [v1.0 API 文档](/graph/api/overview?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="da9ff-p108">The current version of Microsoft Graph is v1.0. Exposed under `https://graph.microsoft.com/v1.0`, the Microsoft Graph API /v1.0 version contains features that are generally available and ready for production use. Browse the [documentation for the v1.0 APIs](/graph/api/overview?view=graph-rest-1.0).</span></span>

## <a name="preview-status"></a><span data-ttu-id="da9ff-150">预览状态</span><span class="sxs-lookup"><span data-stu-id="da9ff-150">Preview status</span></span>
<span data-ttu-id="da9ff-151">功能或 API 标记为“（预览）”，以表示其行为在 beta 终结点中为_唯一_。</span><span class="sxs-lookup"><span data-stu-id="da9ff-151">A feature or API is labelled as "(preview)" to indicate its behavior is _unique_ in the beta endpoint.</span></span> 

<span data-ttu-id="da9ff-152">v1.0 版本中大多数功能和 API 行为与 Beta 版本相同。</span><span class="sxs-lookup"><span data-stu-id="da9ff-152">The behavior of most features and APIs in the v1.0 version is in parity with the beta version.</span></span> <span data-ttu-id="da9ff-153">在以下两种情况之一中，“预览”限定了少数功能和 API：</span><span class="sxs-lookup"><span data-stu-id="da9ff-153">"preview" qualifies a minority of features and APIs in one of the following two cases:</span></span> 
- <span data-ttu-id="da9ff-154">仅可在 Beta 中使用</span><span class="sxs-lookup"><span data-stu-id="da9ff-154">Available in only beta</span></span>
- <span data-ttu-id="da9ff-155">Beta 版中的提供的内容与 v1 不同</span><span class="sxs-lookup"><span data-stu-id="da9ff-155">Available in beta differently than in v1</span></span>

<span data-ttu-id="da9ff-156">与 Beta 终结点中的任何其他 API 一样，在文档中标记为“（预览）”的 API 可能会遇到重大更改，恕不另行通知。</span><span class="sxs-lookup"><span data-stu-id="da9ff-156">Like any other API in the beta endpoint, APIs marked in the documentation as "(preview)" may experience breaking changes without notice.</span></span> <span data-ttu-id="da9ff-157">请勿从生产应用程序中的 beta 终结点访问 API。</span><span class="sxs-lookup"><span data-stu-id="da9ff-157">Do not access APIs from the beta endpoint in production apps.</span></span>


### <a name="deprecated-and-unsupported-versions"></a><span data-ttu-id="da9ff-158">已弃用和不支持的版本</span><span class="sxs-lookup"><span data-stu-id="da9ff-158">Deprecated and unsupported versions</span></span>

<span data-ttu-id="da9ff-159">目前没有弃用的 Microsoft Graph 版本。</span><span class="sxs-lookup"><span data-stu-id="da9ff-159">There are currently no deprecated versions of Microsoft Graph.</span></span>

## <a name="terms-of-use"></a><span data-ttu-id="da9ff-160">使用条款</span><span class="sxs-lookup"><span data-stu-id="da9ff-160">Terms of use</span></span>

<span data-ttu-id="da9ff-161">使用 Microsoft Graph API 即表示你同意 [Microsoft API 使用条款](/legal/microsoft-apis/terms-of-use?context=/graph/context)。</span><span class="sxs-lookup"><span data-stu-id="da9ff-161">By using the Microsoft Graph APIs, you agree to the [Microsoft APIs Terms of Use](/legal/microsoft-apis/terms-of-use?context=/graph/context).</span></span>

<span data-ttu-id="da9ff-162">你的反馈对我们非常重要。</span><span class="sxs-lookup"><span data-stu-id="da9ff-162">Your feedback is important to us.</span></span> <span data-ttu-id="da9ff-163">请在 [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest) 上与我们联系。</span><span class="sxs-lookup"><span data-stu-id="da9ff-163">Connect with us on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest).</span></span> <span data-ttu-id="da9ff-164">使用 [microsoft-graph] 标记安全。</span><span class="sxs-lookup"><span data-stu-id="da9ff-164">Tag your questions with [microsoft-graph].</span></span>
