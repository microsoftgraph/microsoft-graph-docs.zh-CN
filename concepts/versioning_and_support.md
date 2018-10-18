# <a name="versioning-support-and-breaking-change-policies-for-microsoft-graph"></a><span data-ttu-id="6848c-101">Microsoft Graph 的版本控制、支持和重大更改策略</span><span class="sxs-lookup"><span data-stu-id="6848c-101">Versioning, support, and breaking change policies for Microsoft Graph</span></span> 

<span data-ttu-id="6848c-102">本文介绍了 Microsoft Graph 的支持和重大更改策略，以及当前可用的 Microsoft Graph API 版本。</span><span class="sxs-lookup"><span data-stu-id="6848c-102">This article describes the support and breaking change policies for Microsoft Graph and the versions of the Microsoft Graph API that are currently available.</span></span>

## <a name="support-policy-and-deprecation-information"></a><span data-ttu-id="6848c-103">支持策略和弃用信息</span><span class="sxs-lookup"><span data-stu-id="6848c-103">Support policy and deprecation information</span></span>

<span data-ttu-id="6848c-104">Microsoft Graph 遵循 [Microsoft 生命周期策略](https://support.microsoft.com/en-us/lifecycle)。</span><span class="sxs-lookup"><span data-stu-id="6848c-104">Microsoft Graph follows the [Microsoft Lifecycle Policy](https://support.microsoft.com/en-us/lifecycle).</span></span> 

<span data-ttu-id="6848c-p101">由于已发布新版本的 Microsoft Graph REST API 和 Microsoft Graph SDK，之前的版本将停用。Microsoft 将在停用 API 或 SDK 之前至少 24 个月声明弃用的版本。</span><span class="sxs-lookup"><span data-stu-id="6848c-p101">As new versions of the Microsoft Graph REST APIs and Microsoft Graph SDKs are released, earlier versions will be retired. Microsoft will declare a version as deprecated at least 24 months in advance of retiring an API or an SDK.</span></span> 

<span data-ttu-id="6848c-107">递增 API 的主要版本（例如，从 v1.0 到 v2.0）时，我们将通知立即弃用当前版本（在此示例中为 v1.0），在通知 24 个月后，我们将不再支持该版本。</span><span class="sxs-lookup"><span data-stu-id="6848c-107">When we increment the major version of the API (for example, from v1.0 to v2.0), we are announcing that the current version (in this example, v1.0) is immediately deprecated and we will no longer support it 24 months after the announcement.</span></span> <span data-ttu-id="6848c-108">出于服务安全或运行状况可靠性问题的考虑，我们可能会对此策略作例外处理。</span><span class="sxs-lookup"><span data-stu-id="6848c-108">We might make exceptions to this policy for service security or health reliability issues.</span></span>  

<span data-ttu-id="6848c-109">当 API 被标记为已弃用时，我们强烈建议你尽快迁移到最新版本。</span><span class="sxs-lookup"><span data-stu-id="6848c-109">When an API is marked as deprecated, we strongly recommend that you migrate to the latest version as soon as possible.</span></span> <span data-ttu-id="6848c-110">某些情况下，我们将公布新应用程序必须在原始 API 弃用后不久开始使用新的 API。</span><span class="sxs-lookup"><span data-stu-id="6848c-110">In some cases, we will announce that new applications will have to start using the new APIs a short time after the original APIs are deprecated.</span></span> <span data-ttu-id="6848c-111">在这些情况下，仅当前使用已弃用 API 的活动应用程序能够继续使用它们。</span><span class="sxs-lookup"><span data-stu-id="6848c-111">In those cases, only active applications that currently use the deprecated APIs can continue to use them.</span></span>   

### <a name="api-contract-and-non-backward-compatible-changes"></a><span data-ttu-id="6848c-112">API 协定和非后向兼容更改</span><span class="sxs-lookup"><span data-stu-id="6848c-112">API contract and non-backward compatible changes</span></span>

<span data-ttu-id="6848c-p104">Microsoft Graph 在版本中进行了许多更改。这些更改已在 [Microsoft Graph 更改日志](changelog.md)中列出。随着向 Microsoft Graph 中添加新功能和数据，我们将递增 API 版本号，以对 API 进行任意不向后兼容更改。</span><span class="sxs-lookup"><span data-stu-id="6848c-p104">Microsoft Graph has a log of changes across versions. These changes are listed in the [Microsoft Graph Changelog](changelog.md). As new functionality and data is added to Microsoft Graph, we will increment the API version number for any non-backward compatible changes to the API.</span></span> 

<span data-ttu-id="6848c-116">不向后兼容的更改的示例如下：</span><span class="sxs-lookup"><span data-stu-id="6848c-116">The following are examples of non-backward compatible changes:</span></span>

 - <span data-ttu-id="6848c-117">对与资源关联的 URL 或基本请求/响应进行更改</span><span class="sxs-lookup"><span data-stu-id="6848c-117">Changes to the URL or fundamental request/response associated with a resource</span></span>    
 - <span data-ttu-id="6848c-118">删除、重命名或更改声明的属性的类型</span><span class="sxs-lookup"><span data-stu-id="6848c-118">Removal, rename, or change to the type of a declared property</span></span>
 - <span data-ttu-id="6848c-119">删除或重命名 API 或 API 参数</span><span class="sxs-lookup"><span data-stu-id="6848c-119">Removal or rename of APIs or API parameters</span></span>
 - <span data-ttu-id="6848c-120">添加所需的请求标头</span><span class="sxs-lookup"><span data-stu-id="6848c-120">Addition of a required request header</span></span>

<span data-ttu-id="6848c-121">向后兼容的更改示例如下：</span><span class="sxs-lookup"><span data-stu-id="6848c-121">The following are examples of backward compatible changes:</span></span>

 - <span data-ttu-id="6848c-122">添加可为 Null 或具有默认值的属性</span><span class="sxs-lookup"><span data-stu-id="6848c-122">Addition of properties that are nullable or have a default value</span></span>
 - <span data-ttu-id="6848c-123">向枚举添加成员</span><span class="sxs-lookup"><span data-stu-id="6848c-123">Addition of a member to an enumeration</span></span>
 - <span data-ttu-id="6848c-124">删除、重命名或更改开放扩展的类型</span><span class="sxs-lookup"><span data-stu-id="6848c-124">Removal, rename, or change to the type of an open extension</span></span>
 - <span data-ttu-id="6848c-125">删除、重命名或更改注释的类型</span><span class="sxs-lookup"><span data-stu-id="6848c-125">Removal, rename, or change to the type of an annotation</span></span>
 - <span data-ttu-id="6848c-126">向现有集合引入分页</span><span class="sxs-lookup"><span data-stu-id="6848c-126">Introduction of paging to existing collections</span></span>
 - <span data-ttu-id="6848c-127">更改错误代码</span><span class="sxs-lookup"><span data-stu-id="6848c-127">Changes to error codes</span></span>
 - <span data-ttu-id="6848c-128">更改属性的顺序</span><span class="sxs-lookup"><span data-stu-id="6848c-128">Changes to the order of properties</span></span>
 - <span data-ttu-id="6848c-129">更改不透明字符串（例如资源 ID）的长度或格式</span><span class="sxs-lookup"><span data-stu-id="6848c-129">Changes to the length or format of opaque strings, such as resource IDs</span></span>

><span data-ttu-id="6848c-p105">**注意：** 随着时间的推移，我们将更新向后兼容更改的列表。如果你生成了自己的客户端代理（如 WCF 客户端），我们的建议是，客户端应用程序应准备接收之前未由 Microsoft Graph API 服务定义的属性和派生类型。Microsoft Graph API 遵循 [Microsoft REST API 准则](https://github.com/microsoft/api-guidelines/)的[模型版本控制](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning)部分中描述的指导。</span><span class="sxs-lookup"><span data-stu-id="6848c-p105">**Note:** Over time, we will update the list of backward compatible changes. If you generate your own client proxies (like WCF clients), our guidance is that your client applications should be prepared to receive properties and derived types not previously defined by the Microsoft Graph API service. Microsoft Graph API follows the guidance described in the [Model Versioning](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning) section in the [Microsoft REST API guidelines](https://github.com/microsoft/api-guidelines/).</span></span> 

## <a name="versions"></a><span data-ttu-id="6848c-133">版本</span><span class="sxs-lookup"><span data-stu-id="6848c-133">Versions</span></span>

<span data-ttu-id="6848c-134">以下版本的 Microsoft Graph API 目前可用。</span><span class="sxs-lookup"><span data-stu-id="6848c-134">The following versions of the Microsoft Graph API are currently available.</span></span>

### <a name="beta-version"></a><span data-ttu-id="6848c-135">Beta 版</span><span class="sxs-lookup"><span data-stu-id="6848c-135">Beta version</span></span>
<span data-ttu-id="6848c-136">Microsoft Graph API beta 版在 `https://graph.microsoft.com/beta` 中公开，包含当前_**处于预览状态**_ 的功能。</span><span class="sxs-lookup"><span data-stu-id="6848c-136">Exposed under `https://graph.microsoft.com/beta`, the Microsoft Graph API beta version contains features that are currently _**in preview**_.</span></span> <span data-ttu-id="6848c-137">如需了解 beta API 文档，请参阅 [Microsoft Graph beta 终结点参考](../api-reference/beta/beta-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="6848c-137">For beta API documentation, see [Microsoft Graph beta endpoint reference](../api-reference/beta/beta-overview.md).</span></span> <span data-ttu-id="6848c-138">预计将不时地对 beta 版本进行重大更改。</span><span class="sxs-lookup"><span data-stu-id="6848c-138">Expect breaking changes to the beta version from time to time.</span></span> <span data-ttu-id="6848c-139">请勿对 /beta API 产生生产依赖性。</span><span class="sxs-lookup"><span data-stu-id="6848c-139">Do not take a production dependency on /beta APIs.</span></span>

<span data-ttu-id="6848c-p107">我们无法保证将测试功能升级至当前版本。当 Microsoft Graph API 团队认为测试功能可正式发布 (GA) 时，我们将把该功能添加到最新的当前版本中。如果功能升级将导致当前版本出现重大更改，则版本号将递增，而新版本将成为当前版本。我们的开发者社区可以在 [UserVoice](https://officespdev.uservoice.com/) 上发布功能请求，包括对新功能的请求以及将现有的测试 API 升级到当前版本的请求。</span><span class="sxs-lookup"><span data-stu-id="6848c-p107">We make no guarantees that a beta feature will be promoted to the current version. When the Microsoft Graph API team believes that a beta feature is ready for general availability (GA), we will add that feature to the latest current version. If the promotion of the feature would result in a breaking change to the current version, the version number will be incremented, with the new version becoming the current version. Our developer community can post feature request on [UserVoice](https://officespdev.uservoice.com/), including requests for new features as well as requests to promote existing beta APIs to the current version.</span></span> 

### <a name="current-version"></a><span data-ttu-id="6848c-144">当前版本</span><span class="sxs-lookup"><span data-stu-id="6848c-144">Current version</span></span>

<span data-ttu-id="6848c-p108">Microsoft Graph 的当前版本为 v1.0。Microsoft Graph API /v1.0 版本在 `https://graph.microsoft.com/v1.0` 中公开，包含可正式发布和可用于生产的功能。你可以浏览目录中的 v1.0 API 文档。</span><span class="sxs-lookup"><span data-stu-id="6848c-p108">The current version of Microsoft Graph is v1.0. Exposed under `https://graph.microsoft.com/v1.0`, the Microsoft Graph API /v1.0 version contains features that are generally available and ready for production use. You can browse the documentation for the v1.0 APIs in the table of contents.</span></span>

### <a name="deprecated-and-unsupported-versions"></a><span data-ttu-id="6848c-148">已弃用和不支持的版本</span><span class="sxs-lookup"><span data-stu-id="6848c-148">Deprecated and unsupported versions</span></span>

<span data-ttu-id="6848c-149">目前没有弃用的 Microsoft Graph 版本。</span><span class="sxs-lookup"><span data-stu-id="6848c-149">There are currently no deprecated versions of Microsoft Graph.</span></span>

## <a name="terms-of-use"></a><span data-ttu-id="6848c-150">使用条款</span><span class="sxs-lookup"><span data-stu-id="6848c-150">Terms of use</span></span>

<span data-ttu-id="6848c-151">使用 Microsoft Graph API 即表示你同意[使用条款](https://developer.microsoft.com/en-us/graph/docs/misc/terms-of-use)。</span><span class="sxs-lookup"><span data-stu-id="6848c-151">By using the Microsoft Graph APIs, you agree to the [Terms of Use](https://developer.microsoft.com/en-us/graph/docs/misc/terms-of-use).</span></span> 

<span data-ttu-id="6848c-p109">我们非常重视你的反馈意见。请在 [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest) 上与我们联系。使用 [MicrosoftGraph] 标记你的问题。</span><span class="sxs-lookup"><span data-stu-id="6848c-p109">Your feedback is important to us. Connect with us on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Tag your questions with {MicrosoftGraph}.</span></span>
