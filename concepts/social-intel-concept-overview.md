---
title: Microsoft Graph 中的人员和工作场所智能概述
description: Microsoft 365 云服务的亿万用户组成了 Microsoft Graph 的核心部分。 用户的数据通过 Microsoft Graph 提供的服务得到精心的管理、保护和适当的授权，以提升企业生产力和创造力。 因为在 Microsoft Graph 中有大量的用户数据，所以派生自用户社交交互的数据将尤为受到关注。
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.custom: scenarios:getting-started
ms.openlocfilehash: 8de176c72568929db81591abfd4280c22b3d0829
ms.sourcegitcommit: 3afb8123098a25ce30b16648ce2f31e8eaac388c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/30/2020
ms.locfileid: "48816196"
---
# <a name="overview-of-people-and-workplace-intelligence-in-microsoft-graph"></a><span data-ttu-id="959ad-105">Microsoft Graph 中的人员和工作场所智能概述</span><span class="sxs-lookup"><span data-stu-id="959ad-105">Overview of people and workplace intelligence in Microsoft Graph</span></span>

<span data-ttu-id="959ad-106">Microsoft 365 云服务的亿万用户组成了 Microsoft Graph 的核心部分。</span><span class="sxs-lookup"><span data-stu-id="959ad-106">The hundreds of millions of users of Microsoft 365 cloud services form part of the core of Microsoft Graph.</span></span> <span data-ttu-id="959ad-107">用户的数据通过 Microsoft Graph 提供的服务得到精心的管理、保护和适当的授权，以提升企业生产力和创造力。</span><span class="sxs-lookup"><span data-stu-id="959ad-107">The users' data is carefully managed, protected, and with proper authorization, made available by Microsoft Graph services to drive productivity and creativity in businesses.</span></span> 

<span data-ttu-id="959ad-108">通过配置文件API，您可以作为应用开发人员为 Microsoft 365 服务中的人员建模并代表他们，借助配置文件 API，管理员可以控制组织中用户个人资料卡上显示的信息。</span><span class="sxs-lookup"><span data-stu-id="959ad-108">The profile API lets you, as app developers, model and represent people in Microsoft 365 services, and the profile card API lets administrators control the information showing on users' profile cards in the organization.</span></span>

<span data-ttu-id="959ad-109">因为在 Microsoft Graph 中有大量的用户数据，所以派生自用户社交交互的数据将尤为受到关注。</span><span class="sxs-lookup"><span data-stu-id="959ad-109">As ubiquitous the user's data is in Microsoft Graph, data derived from the user's social interactions is particularly interesting.</span></span> <span data-ttu-id="959ad-110">它可以对回答类似以下问题提供智能见解：</span><span class="sxs-lookup"><span data-stu-id="959ad-110">It provides intelligent insights that can answer questions such as the following:</span></span>

- <span data-ttu-id="959ad-111">“搜索名称以‘J’开头的人”</span><span class="sxs-lookup"><span data-stu-id="959ad-111">"Search for People who’s name starts with ‘J’"</span></span>
- <span data-ttu-id="959ad-112">“此人最感兴趣的文档有哪些？”</span><span class="sxs-lookup"><span data-stu-id="959ad-112">"Which documents are most interesting to this person?"</span></span>

<span data-ttu-id="959ad-113">你可以在 Microsoft Graph 中使用人员 API 和见解 API 来构建更为智能的应用，分别访问与用户相关度高的人员和文档。</span><span class="sxs-lookup"><span data-stu-id="959ad-113">You can use the people API and insights API in Microsoft Graph to build smarter apps that can, respectively, access the relevant people and documents for a user.</span></span>

<span data-ttu-id="959ad-114">人员 API 基于用户的联系人、社交网络、组织目录以及电子邮件上的最近通信，返回按与该用户相关性排序的人员。</span><span class="sxs-lookup"><span data-stu-id="959ad-114">The people API returns people ordered by relevance to a user, based on that user's contacts, social networks, organization directory, and recent communications on email.</span></span> <span data-ttu-id="959ad-115">这对于选取人员的应用场景尤为有用。</span><span class="sxs-lookup"><span data-stu-id="959ad-115">This is particularly useful for people-picking scenarios.</span></span>

<span data-ttu-id="959ad-116">见解 API 使用高级分析和机器学习为用户提供他们在工作中所需的相关度最高的文件。</span><span class="sxs-lookup"><span data-stu-id="959ad-116">The insights API uses advanced analytics and machine learning to provide the most relevant files users need throughout their work day.</span></span> <span data-ttu-id="959ad-117">API 提升了我们所熟悉的 Microsoft 365 体验，其中包括 Office Delve、SharePoint Home、OneDrive for Business 中的发现视图以及 Outlook 网页版。</span><span class="sxs-lookup"><span data-stu-id="959ad-117">The API powers familiar Microsoft 365 experiences, including Office Delve, SharePoint Home, the Discover view in OneDrive for Business, and Outlook on the web.</span></span>

![人员和见解 API 为用户返回具有相关度的人员和文档](images/social-intel-concept-overview-data-update2020-1.png)

## <a name="why-integrate-with-people-data"></a><span data-ttu-id="959ad-119">为什么与人员数据集成？</span><span class="sxs-lookup"><span data-stu-id="959ad-119">Why integrate with people data?</span></span>

<span data-ttu-id="959ad-120">人员 API 可返回单个实体的数据[人员](/graph/api/resources/person?view=graph-rest-1.0)，其中包括当今商界中的个人典型数据。</span><span class="sxs-lookup"><span data-stu-id="959ad-120">The people API returns data of a single entity, [person](/graph/api/resources/person?view=graph-rest-1.0), which includes typical data of an individual in today's business world.</span></span> <span data-ttu-id="959ad-121"> “人员”数据的优势在于它相对于 Microsoft Graph 用户的  “相关性”。</span><span class="sxs-lookup"><span data-stu-id="959ad-121">What makes this **person** data especially useful is its _relevance_ with respect to a Microsoft Graph user.</span></span> <span data-ttu-id="959ad-122">相关性是基于用户的通信和协作模式以及业务关系来计算的，并且以每个人的相关性分数进行记录。</span><span class="sxs-lookup"><span data-stu-id="959ad-122">Relevance is noted in a relevance score of each person, calculated based on the user's communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="959ad-123">有 3 种主要类型的“相关性”  数据的应用程序。</span><span class="sxs-lookup"><span data-stu-id="959ad-123">There are 3 main types of application of this _relevance_ data.</span></span>

### <a name="browse-people-by-relevance"></a><span data-ttu-id="959ad-124">按相关性浏览人员</span><span class="sxs-lookup"><span data-stu-id="959ad-124">Browse people by relevance</span></span>

<span data-ttu-id="959ad-125">你可以浏览与登录用户相关的人员或与登录用户组织中某一些用户相关的人员，前提是你已获取相应的[授权](people-example.md#authorization)。</span><span class="sxs-lookup"><span data-stu-id="959ad-125">You can browse people who are related to the signed-in user or to some other user in the signed-in user's organization, provided you have got the appropriate [authorization](people-example.md#authorization).</span></span> <span data-ttu-id="959ad-126">获取按相关性排序的“人员”  对象的集合。</span><span class="sxs-lookup"><span data-stu-id="959ad-126">You get a collection of **person** objects that are ordered by relevance.</span></span> <span data-ttu-id="959ad-127">而且，通过指定查询参数 `top`、`skip`、`orderby`、`select` 和 `filter`，你还可以进一步  “人员”对象的集合。</span><span class="sxs-lookup"><span data-stu-id="959ad-127">You can further [customize](people-example.md#browse-people) the collection of **person** objects that is returned in the response by specifying the query parameters `top`, `skip`, `orderby`, `select`, and `filter`.</span></span>

### <a name="fuzzy-searches-based-on-people-criteria"></a><span data-ttu-id="959ad-128">基于人员条件的模糊搜索</span><span class="sxs-lookup"><span data-stu-id="959ad-128">Fuzzy searches based on people criteria</span></span>

<span data-ttu-id="959ad-129">人员 API 允许你搜索与登录用户相关的人员，前提是你的应用已获取该用户授予的权限。</span><span class="sxs-lookup"><span data-stu-id="959ad-129">The people API lets you search for people relevant to the signed-in user, provided that your app has got permissions by that user.</span></span> <span data-ttu-id="959ad-130">（详细了解[人员权限](permissions-reference.md#people-permissions)。）</span><span class="sxs-lookup"><span data-stu-id="959ad-130">(Read more on [people permissions](permissions-reference.md#people-permissions).)</span></span>

<span data-ttu-id="959ad-131">模糊搜索根据完全匹配以及搜索意图推断返回结果。</span><span class="sxs-lookup"><span data-stu-id="959ad-131">Fuzzy searches return results based on an exact match and also on inferences about the intent of the search.</span></span> <span data-ttu-id="959ad-132">为了说明这一点，请见以下示例：这将返回与登录用户相关的  、其名字或电子邮件地址  中包含以“j”开头的单词的人员对象。</span><span class="sxs-lookup"><span data-stu-id="959ad-132">To illustrate this, the following example returns **person** objects relevant to the signed-in user whose name, _or email address_ , contains a word that starts with 'j'.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/people/?$search=j
```

## <a name="why-integrate-with-the-profile-api-preview"></a><span data-ttu-id="959ad-133">为什么要与配置文件 API（预览版）集成？</span><span class="sxs-lookup"><span data-stu-id="959ad-133">Why integrate with the profile API (preview)?</span></span>

<span data-ttu-id="959ad-134">[配置文件](/graph/api/resources/profile) API 表示下一代建模并代表 Microsoft 365 服务中的人脉。</span><span class="sxs-lookup"><span data-stu-id="959ad-134">The [profile](/graph/api/resources/profile) API represents the next generation in modeling and representing people in Microsoft 365 services.</span></span> <span data-ttu-id="959ad-135">配置文件数据可与人脉数据一起使用，以基于 Microsoft Graph 生成自定义体验。</span><span class="sxs-lookup"><span data-stu-id="959ad-135">Profile data can be used together with people data to build customized experiences based on Microsoft Graph.</span></span>

## <a name="why-configure-profile-cards-in-your-organization-preview"></a><span data-ttu-id="959ad-136">为什么要在组织中配置个人资料卡片（预览版）？</span><span class="sxs-lookup"><span data-stu-id="959ad-136">Why configure profile cards in your organization (preview)?</span></span>

<span data-ttu-id="959ad-137">个人资料卡让组织中的用户可以查看其他人的信息，如姓名和联系信息。</span><span class="sxs-lookup"><span data-stu-id="959ad-137">Profile cards let users in an organization see information about one another, such as their names and contact information.</span></span> <span data-ttu-id="959ad-138">管理员可以使用[个人资料卡](/graph/api/resources/profilecardproperty) API来定制有关 Microsoft 365 人员体验内的组织外观。</span><span class="sxs-lookup"><span data-stu-id="959ad-138">Administrators can use the [profile card](/graph/api/resources/profilecardproperty) API to customize how information about their organization surfaces within Microsoft 365 people experiences.</span></span>

## <a name="why-integrate-with-document-based-insights"></a><span data-ttu-id="959ad-139">为什么与基于文档的见解集成？</span><span class="sxs-lookup"><span data-stu-id="959ad-139">Why integrate with document-based insights?</span></span>

### <a name="use-intelligence-to-improve-collaboration"></a><span data-ttu-id="959ad-140">使用智能来提升协作</span><span class="sxs-lookup"><span data-stu-id="959ad-140">Use intelligence to improve collaboration</span></span>

<span data-ttu-id="959ad-141">在平时的工作日中，用户通常会与存储在多个文档中的大量信息进行交互，并以多种不同的方式与其他用户协作。</span><span class="sxs-lookup"><span data-stu-id="959ad-141">During a typical work day, users often interact with large amounts of information stored across many documents and collaborate with other users in many different ways.</span></span> <span data-ttu-id="959ad-142">当他们需要任何信息时，即可随时找到所需的信息，这一点很重要。</span><span class="sxs-lookup"><span data-stu-id="959ad-142">It's important that they can always can find what they need, when they need it.</span></span>

<span data-ttu-id="959ad-143">你可以使用见解 API（其中包含[热门](/graph/api/resources/insights-trending?view=graph-rest-1.0)、[共享](/graph/api/resources/insights-shared?view=graph-rest-1.0)和[使用](/graph/api/resources/insights-used?view=graph-rest-1.0) API），根据用户的当前上下文和需求跨 Microsoft 365 处理文件，使用户工作更为高效并提升组织中的协作。</span><span class="sxs-lookup"><span data-stu-id="959ad-143">You can use the insights API, which includes the [trending](/graph/api/resources/insights-trending?view=graph-rest-1.0), [shared](/graph/api/resources/insights-shared?view=graph-rest-1.0), and [used](/graph/api/resources/insights-used?view=graph-rest-1.0) APIs, to surface files from across Microsoft 365 based on your users' current context and needs, making users more productive and improving collaboration in your organization.</span></span> <span data-ttu-id="959ad-144">组织可以为这些基于文档的见解[自定义隐私设置](insights-customize-item-insights-privacy.md)，并控制特定 Microsoft 365体验中这些见解的可用性。</span><span class="sxs-lookup"><span data-stu-id="959ad-144">Organizations can [customize privacy settings](insights-customize-item-insights-privacy.md) for these document-based insights, and control the availability of these insights in specific Microsoft 365 experiences.</span></span>

<span data-ttu-id="959ad-145">在应用中呈现见解 API 中的结果很简单。</span><span class="sxs-lookup"><span data-stu-id="959ad-145">It is easy to render the results from the insights API in your app.</span></span> <span data-ttu-id="959ad-146">每个结果都附带了一组常用可视化属性，例如，预览图像 URL 或预览文本。</span><span class="sxs-lookup"><span data-stu-id="959ad-146">Every result comes with a set of common visualization properties, like a preview image URL or preview text.</span></span>

### <a name="make-relevant-content-visible"></a><span data-ttu-id="959ad-147">使相关内容可见</span><span class="sxs-lookup"><span data-stu-id="959ad-147">Make relevant content visible</span></span>

<span data-ttu-id="959ad-148">在 Microsoft 365 中，Delve 使用 _热门_ 见解来帮助用户发现目前最令他们感兴趣的文档。</span><span class="sxs-lookup"><span data-stu-id="959ad-148">In Microsoft 365, Delve uses the _trending_ insight to help users discover the documents that are most interesting to them right now.</span></span> <span data-ttu-id="959ad-149">请参见图 1。</span><span class="sxs-lookup"><span data-stu-id="959ad-149">See figure 1.</span></span>

<span data-ttu-id="959ad-150">通过编程的方式，可以使用见解 API 中的[热门](/graph/api/resources/insights-trending?view=graph-rest-1.0)实体为应用客户提供类似体验。</span><span class="sxs-lookup"><span data-stu-id="959ad-150">Programmatically, you can use the [trending](/graph/api/resources/insights-trending?view=graph-rest-1.0) entity in the insights API to provide your app customers a similar experience.</span></span> <span data-ttu-id="959ad-151">使用  “热门”实体可连接到最近热门或与用户相关的文档。</span><span class="sxs-lookup"><span data-stu-id="959ad-151">Use the **trending** entity to connect to documents that are trending around and relevant to the user.</span></span> <span data-ttu-id="959ad-152">[列出热门文档](/graph/api/insights-list-trending?view=graph-rest-1.0)将返回存储在 OneDrive 或 SharePoint 团队网站上的文件，并参照这些文件的重要程度来对其排序。</span><span class="sxs-lookup"><span data-stu-id="959ad-152">[Listing trending documents](/graph/api/insights-list-trending?view=graph-rest-1.0) returns those files stored on OneDrive or SharePoint team sites, sorted by relevance with the most important ones first.</span></span> 

<span data-ttu-id="959ad-153">**图 1. Microsoft 365 中的 Delve 为用户显示热门文档**</span><span class="sxs-lookup"><span data-stu-id="959ad-153">**Figure 1. Delve in Microsoft 365 showing popular documents for a user**</span></span>

![Microsoft 365 中的 Delve 为用户显示热门文档的屏幕截图](images/delve-concept.png)

### <a name="allow-users-to-collaborate-and-get-back-to-work"></a><span data-ttu-id="959ad-155">允许用户进行协作和恢复工作</span><span class="sxs-lookup"><span data-stu-id="959ad-155">Allow users to collaborate and get back to work</span></span>

<span data-ttu-id="959ad-156">新的 Microsoft 365 人员卡片融入了“ _使用_ ”和“ _共享_ ”见解，以连接人员和知识单元之间的点。</span><span class="sxs-lookup"><span data-stu-id="959ad-156">The new Microsoft 365 people cards tap into the _used_ and _shared_ insights to connect the dots between people and units of knowledge.</span></span> <span data-ttu-id="959ad-157">人员卡片将标识和显示有关人员的相关文档。</span><span class="sxs-lookup"><span data-stu-id="959ad-157">The people card identifies and displays relevant documents about a person.</span></span> <span data-ttu-id="959ad-158">用户可以在整个套件内查看人员卡片（例如，在 Outlook 网页版中）。</span><span class="sxs-lookup"><span data-stu-id="959ad-158">Users can see people cards across the suite, for example, in Outlook on the web.</span></span> <span data-ttu-id="959ad-159">请参见图 2。</span><span class="sxs-lookup"><span data-stu-id="959ad-159">See figure 2.</span></span>

<span data-ttu-id="959ad-160">见解 API 提供与[使用](/graph/api/resources/insights-used?view=graph-rest-1.0)和[共享](/graph/api/resources/insights-shared?view=graph-rest-1.0)实体类似的功能。</span><span class="sxs-lookup"><span data-stu-id="959ad-160">The insights API provides a similar functionality with the [used](/graph/api/resources/insights-used?view=graph-rest-1.0) and [shared](/graph/api/resources/insights-shared?view=graph-rest-1.0) entities.</span></span> <span data-ttu-id="959ad-161">它们返回用户最近最常查看或使用的内容，或同事最近在 Microsoft 365 中与用户共享的内容。</span><span class="sxs-lookup"><span data-stu-id="959ad-161">They return what a user has been viewing or working on most recently, or what colleagues have shared with the user most recently in Microsoft 365.</span></span>

<span data-ttu-id="959ad-162">**图 2. Outlook 网页版显示用户的人员卡片**</span><span class="sxs-lookup"><span data-stu-id="959ad-162">**Figure 2. Outlook on the web showing a people card for a user**</span></span>

![Outlook 网页版中用户的人员卡片屏幕截图，显示最近使用的文件](images/peoplecard-concept.png)

## <a name="why-integrate-with-myanalytics-preview"></a><span data-ttu-id="959ad-164">为什么要与 MyAnalytics（预览版）集成？</span><span class="sxs-lookup"><span data-stu-id="959ad-164">Why integrate with MyAnalytics (preview)?</span></span>

<span data-ttu-id="959ad-165">[MyAnalytics](/workplace-analytics/myanalytics/index) 提供了有关用户如何花费自己时间，以及用户与谁一起花费时间的见解。</span><span class="sxs-lookup"><span data-stu-id="959ad-165">[MyAnalytics](/workplace-analytics/myanalytics/index) provides insight into how people spend their time and who they spend it with.</span></span> <span data-ttu-id="959ad-166">此类数据可以帮助用户计划一天的日程安排，深入了解自己的不同工作模式，并帮助用户平衡工作和生活。</span><span class="sxs-lookup"><span data-stu-id="959ad-166">This data can help people plan their day, gain insights into their different work patterns, and help them balance work and life.</span></span>

<span data-ttu-id="959ad-167">借助分析 API，可以同步或集成用户分析数据与自定义第三方应用，以支持各种有助于提升用户工作效率和协作的方案。</span><span class="sxs-lookup"><span data-stu-id="959ad-167">The analytics API enables you to synchronize or integrate user analytics data with a custom, third-party app to support a wide range of scenarios that can help improve user productivity and collaboration.</span></span> <span data-ttu-id="959ad-168">例如，可以将 MyAnalytics 数据与移动设备活动集成，以帮助用户在一个应用中跟踪自己的所有工作和社交活动，并计划一天的日程安排。</span><span class="sxs-lookup"><span data-stu-id="959ad-168">For example, you could integrate MyAnalytics data with mobile device activities to help users keep track of all their work and social activities and plan their day all within one app.</span></span>
 
## <a name="api-reference"></a><span data-ttu-id="959ad-169">API 参考</span><span class="sxs-lookup"><span data-stu-id="959ad-169">API reference</span></span>

<span data-ttu-id="959ad-170">在查找这些服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="959ad-170">Looking for the API reference for these services?</span></span>

- [<span data-ttu-id="959ad-171">使用 Microsoft Graph API 在应用中集成人员和工作区智能</span><span class="sxs-lookup"><span data-stu-id="959ad-171">Use the Microsoft Graph API to integrate people and workplace intelligence in an app</span></span>](/graph/api/resources/social-overview)
- <span data-ttu-id="959ad-172">人脉 API [人员](/graph/api/resources/person) 资源</span><span class="sxs-lookup"><span data-stu-id="959ad-172">The People API [person](/graph/api/resources/person) resource</span></span>
- <span data-ttu-id="959ad-173">[个人资料（预览版）](/graph/api/resources/profile) 资源</span><span class="sxs-lookup"><span data-stu-id="959ad-173">[Profile (preview)](/graph/api/resources/profile) resource</span></span>
- <span data-ttu-id="959ad-174">[个人资料卡片（预览版）](/graph/api/resources/profilecardproperty) 资源</span><span class="sxs-lookup"><span data-stu-id="959ad-174">[Profile card property (preview)](/graph/api/resources/profilecardproperty) resource</span></span>
- [<span data-ttu-id="959ad-175">见解 API</span><span class="sxs-lookup"><span data-stu-id="959ad-175">Insights API</span></span>](/graph/api/resources/officegraphinsights)
- [<span data-ttu-id="959ad-176">分析 API（预览版）</span><span class="sxs-lookup"><span data-stu-id="959ad-176">Analytics API (preview)</span></span>](/graph/api/resources/useranalytics)

## <a name="next-steps"></a><span data-ttu-id="959ad-177">后续步骤</span><span class="sxs-lookup"><span data-stu-id="959ad-177">Next steps</span></span>

* <span data-ttu-id="959ad-178">在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用你自己的文件试用人员、见解和分析 API。</span><span class="sxs-lookup"><span data-stu-id="959ad-178">Use the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out the people, insights, and analytics APIs with your own files.</span></span> <span data-ttu-id="959ad-179">登录并选择左侧列中的“显示更多示例”  。</span><span class="sxs-lookup"><span data-stu-id="959ad-179">Sign in, and choose **Show more samples** in the column on the left.</span></span> <span data-ttu-id="959ad-180">使用菜单打开“人员”  和“见解”  和“分析”  。</span><span class="sxs-lookup"><span data-stu-id="959ad-180">Use the menu to turn on **People** , **Insights** , and **Analytics** .</span></span>
* <span data-ttu-id="959ad-181">查找有关[人脉 API](people-example.md) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="959ad-181">Find more about the [people API](people-example.md).</span></span>
* <span data-ttu-id="959ad-182">请参阅如何 [自定义个人资料卡片](add-properties-profilecard.md)。</span><span class="sxs-lookup"><span data-stu-id="959ad-182">See how to [customize the profile card](add-properties-profilecard.md).</span></span>
* <span data-ttu-id="959ad-183">了解有关[自定义用户隐私](insights-customize-item-insights-privacy.md)和 [insights API](/api-reference/beta/resources/iteminsights.md) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="959ad-183">Find out more about [customizing user privacy](insights-customize-item-insights-privacy.md), and the [insights API](/api-reference/beta/resources/iteminsights.md).</span></span>
* <span data-ttu-id="959ad-184">查找有关[分析 API](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-balance-work-and-life) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="959ad-184">Find more about the [analytics API](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-balance-work-and-life).</span></span>
* <span data-ttu-id="959ad-185">查找有关[配置文件 API](/graph/api/resources/profile?view=graph-rest-beta) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="959ad-185">Find more about the [profile API](/graph/api/resources/profile?view=graph-rest-beta).</span></span>
