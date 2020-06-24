---
title: Azure AD Graph 与 Microsoft Graph 之间的功能差异
description: 介绍了 Azure Active Directory （Azure AD） API 与 Microsoft Graph API 之间的功能差异，以帮助你快速轻松地迁移应用。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7bebb0437ac3f099d7518640ad4fbb0f9fd75990
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845776"
---
# <a name="feature-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="3b7b7-103">Azure AD Graph 与 Microsoft Graph 之间的功能差异</span><span class="sxs-lookup"><span data-stu-id="3b7b7-103">Feature differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="3b7b7-104">本文是*第1步：查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="3b7b7-105">Microsoft Graph 中的许多功能与 Azure AD Graph 对应的工作方式类似。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-105">Many features in Microsoft Graph work similarly to their Azure AD Graph counterparts.</span></span> <span data-ttu-id="3b7b7-106">不过，已经更改和/或改进了少数几个部分。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-106">However, a few have been changed and/or improved.</span></span> <span data-ttu-id="3b7b7-107">在这里，你将了解如何改编你的应用以利用这些差异。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-107">Here, you'll learn how to adapt your apps to take advantage of these differences.</span></span>  <span data-ttu-id="3b7b7-108">通常情况下，更改很小，但值得努力。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-108">Frequently, the changes are minor, but well worth the effort.</span></span>

<span data-ttu-id="3b7b7-109">本文探讨 Microsoft Graph 如何处理以下内容：</span><span class="sxs-lookup"><span data-stu-id="3b7b7-109">This article explores how Microsoft Graph handles:</span></span>

- <span data-ttu-id="3b7b7-110">目录架构扩展</span><span class="sxs-lookup"><span data-stu-id="3b7b7-110">Directory schema extensions</span></span>
- <span data-ttu-id="3b7b7-111">差异查询</span><span class="sxs-lookup"><span data-stu-id="3b7b7-111">Differential queries</span></span>
- <span data-ttu-id="3b7b7-112">批处理</span><span class="sxs-lookup"><span data-stu-id="3b7b7-112">Batching</span></span>

## <a name="directory-schema-extensions"></a><span data-ttu-id="3b7b7-113">目录架构扩展</span><span class="sxs-lookup"><span data-stu-id="3b7b7-113">Directory schema extensions</span></span>

<span data-ttu-id="3b7b7-114">如果您的应用程序使用 Azure AD Graph 目录架构扩展，则可以继续使用相同的基本 Api （使用 Microsoft Graph 请求 Url）执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="3b7b7-114">If your app uses Azure AD Graph directory schema extensions, you can continue to use the same basic APIs (with Microsoft Graph request URLs) to:</span></span>

- <span data-ttu-id="3b7b7-115">使用 [application] [/graph/api/resources/application？ view = graph-rest-extensionProperties 1.0）资源上的**extensionProperties**属性管理扩展属性定义。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-115">Manage extension property definitions using the **extensionProperties** property on the [application][/graph/api/resources/application?view=graph-rest-v1.0) resource.</span></span>
- <span data-ttu-id="3b7b7-116">使用 GET 和，读取扩展值`$select`</span><span class="sxs-lookup"><span data-stu-id="3b7b7-116">Read extension values using GET and `$select`</span></span>
- <span data-ttu-id="3b7b7-117">使用 GET 和，搜索扩展值`$filter`</span><span class="sxs-lookup"><span data-stu-id="3b7b7-117">Search on extension values using GET and `$filter`</span></span>
- <span data-ttu-id="3b7b7-118">使用修补程序更新扩展值</span><span class="sxs-lookup"><span data-stu-id="3b7b7-118">Update extension values using PATCH</span></span>
- <span data-ttu-id="3b7b7-119">使用修补程序删除扩展值（设置为**null**）</span><span class="sxs-lookup"><span data-stu-id="3b7b7-119">Remove extension values using PATCH (set to **null**)</span></span>

<span data-ttu-id="3b7b7-120">Microsoft Graph 提供了增强的架构扩展开发人员体验，这与 Azure AD Graph 目录架构 extentions 目前不是向后兼容。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-120">Microsoft Graph provides an enhanced schema extensions developer experience, which today is not backwards compatible with Azure AD Graph directory schema extentions.</span></span> <span data-ttu-id="3b7b7-121">若要了解详细信息，请参阅[添加自定义数据中的架构扩展](/graph/extensibility-overview#schema-extensions)。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-121">To learn more, see [schema extensions in add custom data](/graph/extensibility-overview#schema-extensions).</span></span>

### <a name="recommended-migration-approach"></a><span data-ttu-id="3b7b7-122">建议的迁移方法</span><span class="sxs-lookup"><span data-stu-id="3b7b7-122">Recommended migration approach</span></span>

<span data-ttu-id="3b7b7-123">如果你的 Azure AD Graph 应用使用目录架构扩展，请采用增量方法将应用迁移到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-123">If your Azure AD Graph app uses directory schema extensions, take an incremental approach to migrate the app to Microsoft Graph.</span></span>

<span data-ttu-id="3b7b7-124">首先，将您的应用程序切换为使用 Microsoft Graph API 调用，但让应用继续利用 Azure AD Graph 目录架构扩展。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-124">First, switch your app to using Microsoft Graph API calls, but let the app continue to leverage Azure AD Graph directory schema extensions.</span></span>

<span data-ttu-id="3b7b7-125">然后，您可以切换到使用 Microsoft Graph 架构扩展。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-125">Then, you can switch to using Microsoft Graph schema extensions.</span></span> <span data-ttu-id="3b7b7-126">在某些情况下，切换将不合适。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-126">In some cases, switching will not be appropriate.</span></span> <span data-ttu-id="3b7b7-127">请勿切换（如果有）：</span><span class="sxs-lookup"><span data-stu-id="3b7b7-127">Do not switch if:</span></span>

- <span data-ttu-id="3b7b7-128">您的应用程序使用通过 AD Connect 创建的目录架构扩展，或者</span><span class="sxs-lookup"><span data-stu-id="3b7b7-128">Your app uses directory schema extensions created through AD Connect, or</span></span>
- <span data-ttu-id="3b7b7-129">您的应用程序依赖于令牌声明中的目录架构扩展值。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-129">Your app relies on directory schema extension values in token claims.</span></span>

><span data-ttu-id="3b7b7-130">**注意**：尚不支持使用 Microsoft Graph 架构扩展属性作为令牌中使用可选声明或动态成员身份规则的声明。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-130">**NOTE**: Using Microsoft Graph schema extension properties as claims in a token using optional claims or in a dynamic membership rule is also not yet supported.</span></span>

<span data-ttu-id="3b7b7-131">若要切换到较新的 Microsoft Graph 架构扩展模型，需要执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="3b7b7-131">To switch to the newer Microsoft Graph schema extension model, you'll need to:</span></span>

- <span data-ttu-id="3b7b7-132">使用 Microsoft Graph 定义新的架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-132">Define new schema extension definitions using Microsoft Graph.</span></span>
- <span data-ttu-id="3b7b7-133">更新应用程序以支持新的架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-133">Update the app to support the new schema extension definitions.</span></span>
- <span data-ttu-id="3b7b7-134">将数据从 Azure AD 架构扩展属性迁移到新的 Microsoft Graph 架构扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-134">Migrate the data from the Azure AD schema extension properties to the new Microsoft Graph schema extension properties.</span></span>  <span data-ttu-id="3b7b7-135">不支持自动迁移数据。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-135">Automatic migration of data is not supported.</span></span>

## <a name="differential-queries"></a><span data-ttu-id="3b7b7-136">差异查询</span><span class="sxs-lookup"><span data-stu-id="3b7b7-136">Differential queries</span></span>

<span data-ttu-id="3b7b7-137">Azure AD Graph 和 Microsoft Graph 让你可以使用查询跟踪更改。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-137">Azure AD Graph and Microsoft Graph let you track changes using queries.</span></span>  <span data-ttu-id="3b7b7-138">这两个 Api 的高级别方法类似，但语法不同。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-138">The high-level approach is similar between the two APIs, but the syntax is different.</span></span>

<span data-ttu-id="3b7b7-139">Azure AD Graph 调用这些差异查询。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-139">Azure AD Graph calls these differential queries.</span></span>  <span data-ttu-id="3b7b7-140">在 Microsoft Graph 中，它们是[delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-140">In Microsoft Graph, they're [delta queries](/graph/delta-query-overview).</span></span>

<span data-ttu-id="3b7b7-141">下表重点介绍了主要的相似之处和差异：</span><span class="sxs-lookup"><span data-stu-id="3b7b7-141">The following table highlights key similarities and differences:</span></span>

|<span data-ttu-id="3b7b7-142">Delta 请求</span><span class="sxs-lookup"><span data-stu-id="3b7b7-142">Delta request</span></span> |<span data-ttu-id="3b7b7-143">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="3b7b7-143">Azure AD Graph</span></span> | <span data-ttu-id="3b7b7-144">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3b7b7-144">Microsoft Graph</span></span> |
|----|----|----|
| <span data-ttu-id="3b7b7-145">_初始数据请求_</span><span class="sxs-lookup"><span data-stu-id="3b7b7-145">_Initial data request_</span></span> | <span data-ttu-id="3b7b7-146">使用查询参数：</span><span class="sxs-lookup"><span data-stu-id="3b7b7-146">Uses a query parameter:</span></span><br>`GET /groups?deltaLink=` | <span data-ttu-id="3b7b7-147">使用函数：</span><span class="sxs-lookup"><span data-stu-id="3b7b7-147">Uses a function:</span></span> <br> `GET /groups/delta` |
| <span data-ttu-id="3b7b7-148">_获取新更改_</span><span class="sxs-lookup"><span data-stu-id="3b7b7-148">_Get new changes_</span></span> | `GET /groups?deltaLink={deltaToken}` | `GET /groups/delta?$deltaToken={deltaToken}` |
| <span data-ttu-id="3b7b7-149">_从现在开始同步_</span><span class="sxs-lookup"><span data-stu-id="3b7b7-149">_Sync from now_</span></span> |<span data-ttu-id="3b7b7-150">使用自定义 HTTP 标头：</span><span class="sxs-lookup"><span data-stu-id="3b7b7-150">Uses a custom HTTP header:</span></span><br> `ocp-aad-dq-include-only-delta-token: true` | <span data-ttu-id="3b7b7-151">使用查询参数：</span><span class="sxs-lookup"><span data-stu-id="3b7b7-151">Uses a query parameter:</span></span> <br> `GET /groups/delta?$deltaToken=latest` |
| <span data-ttu-id="3b7b7-152">_跟踪 directoryObjects 的更改_</span><span class="sxs-lookup"><span data-stu-id="3b7b7-152">_Track changes for directoryObjects_</span></span> | <span data-ttu-id="3b7b7-153">获取相同操作中的多个资源（用户和组）的更改：&nbsp;&nbsp;</span><span class="sxs-lookup"><span data-stu-id="3b7b7-153">Gets changes for multiple resource (user and group) in the same operation:&nbsp;&nbsp;</span></span><br> `GET /directoryObject?$filter=isof('User') or isof('Group')&deltaLink=` | <span data-ttu-id="3b7b7-154">将单独的查询与 Microsoft Graph 结合使用，每个资源对应一项。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-154">Uses separate queries with Microsoft Graph, one for each resource.</span></span> |
| <span data-ttu-id="3b7b7-155">_获取资源和关系更改_</span><span class="sxs-lookup"><span data-stu-id="3b7b7-155">_Get resource and relationship changes_</span></span> | <span data-ttu-id="3b7b7-156">如果资源有关系，所有请求都将返回资源和关系更改。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-156">All requests return resource and relationship changes, if the resource has relationships.</span></span> | `GET /groups/delta?$expand=members` |
| <span data-ttu-id="3b7b7-157">_指示新项目和已更改项目的响应_</span><span class="sxs-lookup"><span data-stu-id="3b7b7-157">_Response indicating new and changed items_</span></span> | <ul><li><p><span data-ttu-id="3b7b7-158">使用其标准表示形式表示新创建的实例。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-158">Represents newly created instances using their standard representation.</span></span></p></li><li><p><span data-ttu-id="3b7b7-159">更新后的实例由其 id 表示，*至少*具有已更新的属性。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-159">Updated instances are represented by their id with *at least* the properties that have been updated.</span></span> <span data-ttu-id="3b7b7-160">可以包含其他属性。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-160">Other properties may be included.</span></span></p></li><li><p><span data-ttu-id="3b7b7-161">关系表示为 `directoryLinkChange` 类型。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-161">Relationships are represented as the `directoryLinkChange` type.</span></span></p></li></ul>|<ul><li><p><span data-ttu-id="3b7b7-162">使用其标准表示形式表示新创建的实例。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-162">Represents newly created instances using their standard representation.</span></span></p></li><li><p><span data-ttu-id="3b7b7-163">更新后的实例由其 id 表示，*至少*具有已更新的属性。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-163">Updated instances are represented by their id with *at least* the properties that have been updated.</span></span> <span data-ttu-id="3b7b7-164">可以包含其他属性。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-164">Other properties may be included.</span></span></p></li><li><p><span data-ttu-id="3b7b7-165">关系表示为标准资源表示形式的批注。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-165">Relationships are represented as annotations on the standard resource representation.</span></span> <span data-ttu-id="3b7b7-166">这些批注使用格式 `propertyName@delta` ，例如， `members@delta` 组的成员资格更改。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-166">These annotations use the format `propertyName@delta`, for example `members@delta` for a group's membership changes.</span></span></p></li></ul> |
| <span data-ttu-id="3b7b7-167">_指示已删除项目的响应_</span><span class="sxs-lookup"><span data-stu-id="3b7b7-167">_Response indicating  deleted items_</span></span>| <span data-ttu-id="3b7b7-168">指示一个已删除的项，其附加属性为*isDeleted*设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-168">Indicates a deleted item with an additional property of *aad.isDeleted* set to true.</span></span> | <span data-ttu-id="3b7b7-169">指示已删除的项目和 \@ 已删除的注释。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-169">Indicates a deleted item with the \@removed annotation.</span></span> <span data-ttu-id="3b7b7-170">它还可能包含原因代码，以指示是否已删除项目，但可以还原或永久删除。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-170">It may also contain a reason code, which indicates if the item is deleted, but can be restored, or is permanently deleted.</span></span> |

<span data-ttu-id="3b7b7-171">如果您的应用程序已在存储状态数据，请考虑使用前面所示的 "从现在同步"，以帮助管理到增量查询的转换。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-171">If your app is already storing state data, consider using the "sync from now" shown earlier to help manage the transition to delta queries.</span></span>

## <a name="batching"></a><span data-ttu-id="3b7b7-172">批处理</span><span class="sxs-lookup"><span data-stu-id="3b7b7-172">Batching</span></span>

<span data-ttu-id="3b7b7-173">Azure AD Graph 使用称为多部分 MIME 邮件的系统来管理批处理。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-173">Azure AD Graph used a system called multi-part MIME messages to manage batching.</span></span>  <span data-ttu-id="3b7b7-174">Microsoft Graph 使用[JSON 批处理](json-batching.md)在单个批处理操作中允许最长20个请求。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-174">Microsoft Graph uses [JSON batching](json-batching.md) to permit up to 20 requests in a single batch operation.</span></span> <span data-ttu-id="3b7b7-175">JSON 批处理机制使用起来明显简单，尤其是 JSON 分析库。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-175">The JSON batching mechanism is significantly simpler to use, especially together with JSON parsing libraries.</span></span>  <span data-ttu-id="3b7b7-176">它还允许对批处理操作进行排序。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-176">It also allows for sequencing batch operations.</span></span>  <span data-ttu-id="3b7b7-177">但是，与 Azure AD Graph 批处理方法相比，它不是向后兼容。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-177">However, it is not backwards compatible with the Azure AD Graph batching approach.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3b7b7-178">后续步骤</span><span class="sxs-lookup"><span data-stu-id="3b7b7-178">Next Steps</span></span>

- <span data-ttu-id="3b7b7-179">了解 Azure AD Graph 与 Microsoft Graph 之间的[资源差异](migrate-azure-ad-graph-resource-differences.md)。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-179">Learn about [resource differences](migrate-azure-ad-graph-resource-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="3b7b7-180">探索[添加自定义数据](/graph/extensibility-overview)，以获取有关开放和架构扩展的信息。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-180">Explore [add custom data](/graph/extensibility-overview) for information about open and schema extensions.</span></span>
- <span data-ttu-id="3b7b7-181">浏览[delta 查询](/graph/delta-query-overview)以了解 Microsoft Graph 的差异查询版本。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-181">Explore [delta queries](/graph/delta-query-overview) to learn about Microsoft Graph's version of differential query.</span></span>
- <span data-ttu-id="3b7b7-182">浏览[JSON 批处理](json-batching.md)以了解批处理在 Microsoft Graph 中的工作方式。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-182">Explore [JSON batching](json-batching.md) to understand how batching works in Microsoft Graph.</span></span>
- <span data-ttu-id="3b7b7-183">使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-183">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /concepts/migrate-azure-ad-graph-feature-changes.md:
      Failed to parse any rows out of table with headers: |Task|Azure AD Graph|Microsoft Graph|"
  ],
}
-->
