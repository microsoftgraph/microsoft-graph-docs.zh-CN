---
title: Azure AD Graph 与 Microsoft Graph 之间的功能差异
description: 介绍了 Azure Active Directory (Azure AD) API 与 Microsoft Graph API 之间的功能差异, 以帮助你快速轻松地迁移应用。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e18bc286f4373c15da9d6a2360491e1b2f0371f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630242"
---
# <a name="feature-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="8d1cb-103">Azure AD Graph 与 Microsoft Graph 之间的功能差异</span><span class="sxs-lookup"><span data-stu-id="8d1cb-103">Feature differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="8d1cb-104">本文是*第1步: 查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="8d1cb-105">Microsoft Graph 中的许多功能与 Azure AD Graph 对应的工作方式类似。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-105">Many features in Microsoft Graph work similarly to their Azure AD Graph counterparts.</span></span> <span data-ttu-id="8d1cb-106">不过, 已经更改和/或改进了少数几个部分。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-106">However, a few have been changed and/or improved.</span></span> <span data-ttu-id="8d1cb-107">在这里, 你将了解如何改编你的应用以利用这些差异。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-107">Here, you'll learn how to adapt your apps to take advantage of these differences.</span></span>  <span data-ttu-id="8d1cb-108">通常情况下, 更改很小, 但值得努力。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-108">Frequently, the changes are minor, but well worth the effort.</span></span>

<span data-ttu-id="8d1cb-109">本文探讨 Microsoft Graph 如何处理以下内容:</span><span class="sxs-lookup"><span data-stu-id="8d1cb-109">This article explores how Microsoft Graph handles:</span></span>

- <span data-ttu-id="8d1cb-110">目录架构扩展</span><span class="sxs-lookup"><span data-stu-id="8d1cb-110">Directory schema extensions</span></span>
- <span data-ttu-id="8d1cb-111">差异查询</span><span class="sxs-lookup"><span data-stu-id="8d1cb-111">Differential queries</span></span>
- <span data-ttu-id="8d1cb-112">批处理</span><span class="sxs-lookup"><span data-stu-id="8d1cb-112">Batching</span></span>

## <a name="directory-schema-extensions"></a><span data-ttu-id="8d1cb-113">目录架构扩展</span><span class="sxs-lookup"><span data-stu-id="8d1cb-113">Directory schema extensions</span></span>

<span data-ttu-id="8d1cb-114">如果您的应用程序使用 Azure AD Graph 目录架构扩展, 则可以继续使用相同的基本 Api (使用 Microsoft Graph 请求 Url) 执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="8d1cb-114">If your app uses Azure AD Graph directory schema extensions, you can continue to use the same basic APIs (with Microsoft Graph request URLs) to:</span></span>

- <span data-ttu-id="8d1cb-115">使用 GET 和, 读取扩展值`$select`</span><span class="sxs-lookup"><span data-stu-id="8d1cb-115">Read extension values using GET and `$select`</span></span>
- <span data-ttu-id="8d1cb-116">使用 GET 和, 搜索扩展值`$filter`</span><span class="sxs-lookup"><span data-stu-id="8d1cb-116">Search on extension values using GET and `$filter`</span></span>
- <span data-ttu-id="8d1cb-117">使用修补程序更新扩展值</span><span class="sxs-lookup"><span data-stu-id="8d1cb-117">Update extension values using PATCH</span></span>
- <span data-ttu-id="8d1cb-118">使用修补程序删除扩展值 (设置为**null**)</span><span class="sxs-lookup"><span data-stu-id="8d1cb-118">Remove extension values using PATCH (set to **null**)</span></span>

<span data-ttu-id="8d1cb-119">但是, Microsoft Graph 不提供管理 Azure AD Graph 目录架构扩展定义或查看租户中可用的所有架构扩展定义的方法。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-119">However, Microsoft Graph doesn't provide a way to manage Azure AD Graph directory schema extension definitions or to view all schema extension definitions available in a tenant.</span></span>

<span data-ttu-id="8d1cb-120">相反, Microsoft Graph 提供了增强的架构扩展开发人员体验, 这与 Azure AD Graph 目录架构 extentions 目前不是向后兼容。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-120">Instead, Microsoft Graph provides an enhanced schema extensions developer experience, which today is not backwards compatible with Azure AD Graph directory schema extentions.</span></span> <span data-ttu-id="8d1cb-121">若要了解详细信息, 请参阅[添加自定义数据中的架构扩展](/graph/extensibility-overview#schema-extensions)。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-121">To learn more, see [schema extensions in add custom data](/graph/extensibility-overview#schema-extensions).</span></span>

### <a name="recommended-migration-approach"></a><span data-ttu-id="8d1cb-122">建议的迁移方法</span><span class="sxs-lookup"><span data-stu-id="8d1cb-122">Recommended migration approach</span></span>

<span data-ttu-id="8d1cb-123">如果你的 Azure AD Graph 应用使用目录架构扩展, 请采用增量方法将应用迁移到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-123">If your Azure AD Graph app uses directory schema extensions, take an incremental approach to migrate the app to Microsoft Graph.</span></span>

<span data-ttu-id="8d1cb-124">首先, 将您的应用程序切换为使用 Microsoft Graph API 调用, 但让应用继续利用 Azure AD Graph 目录架构扩展。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-124">First, switch your app to using Microsoft Graph API calls, but let the app continue to leverage Azure AD Graph directory schema extensions.</span></span>

<span data-ttu-id="8d1cb-125">然后, 您可以切换到使用 Microsoft Graph 架构扩展。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-125">Then, you can switch to using Microsoft Graph schema extensions.</span></span> <span data-ttu-id="8d1cb-126">在某些情况下, 切换将不合适。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-126">In some cases, switching will not be appropriate.</span></span> <span data-ttu-id="8d1cb-127">请勿切换 (如果有):</span><span class="sxs-lookup"><span data-stu-id="8d1cb-127">Do not switch if:</span></span>

- <span data-ttu-id="8d1cb-128">您的应用程序使用通过 AD Connect 创建的目录架构扩展, 或者</span><span class="sxs-lookup"><span data-stu-id="8d1cb-128">Your app uses directory schema extensions created through AD Connect, or</span></span>
- <span data-ttu-id="8d1cb-129">您的应用程序依赖于令牌声明中的目录架构扩展值。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-129">Your app relies on directory schema extension values in token claims.</span></span>

><span data-ttu-id="8d1cb-130">**注意**: 也尚不支持将 Microsoft Graph 架构扩展属性用作令牌中使用可选声明的声明。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-130">**NOTE**: Using Microsoft Graph schema extension properties as claims in a token using optional claims is also not yet supported.</span></span>

<span data-ttu-id="8d1cb-131">若要切换到较新的 Microsoft Graph 架构扩展模型, 需要执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="8d1cb-131">To switch to the newer Microsoft Graph schema extension model, you'll need to:</span></span>

- <span data-ttu-id="8d1cb-132">使用 Microsoft Graph 定义新的架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-132">Define new schema extension definitions using Microsoft Graph.</span></span>
- <span data-ttu-id="8d1cb-133">更新应用程序以支持新的架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-133">Update the app to support the new schema extension definitions.</span></span>
- <span data-ttu-id="8d1cb-134">将数据从 Azure AD 架构扩展属性迁移到新的 Microsoft Graph 架构扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-134">Migrate the data from the Azure AD schema extension properties to the new Microsoft Graph schema extension properties.</span></span>  <span data-ttu-id="8d1cb-135">不支持自动迁移数据。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-135">Automatic migration of data is not supported.</span></span>

## <a name="differential-queries"></a><span data-ttu-id="8d1cb-136">差异查询</span><span class="sxs-lookup"><span data-stu-id="8d1cb-136">Differential queries</span></span>

<span data-ttu-id="8d1cb-137">Azure AD Graph 和 Microsoft Graph 让你可以使用查询跟踪更改。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-137">Azure AD Graph and Microsoft Graph let you track changes using queries.</span></span>  <span data-ttu-id="8d1cb-138">这两个 Api 的高级别方法类似, 但语法不同。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-138">The high-level approach is similar between the two APIs, but the syntax is different.</span></span>  

<span data-ttu-id="8d1cb-139">Azure AD Graph 调用这些差异查询。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-139">Azure AD Graph calls these differential queries.</span></span>  <span data-ttu-id="8d1cb-140">在 Microsoft Graph 中, 它们是[delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-140">In Microsoft Graph, they're [delta queries](/graph/delta-query-overview).</span></span>

<span data-ttu-id="8d1cb-141">下表重点介绍了主要的相似之处和差异:</span><span class="sxs-lookup"><span data-stu-id="8d1cb-141">The following table highlights key similarities and differences:</span></span>

||<span data-ttu-id="8d1cb-142">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="8d1cb-142">Azure AD Graph</span></span> | <span data-ttu-id="8d1cb-143">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8d1cb-143">Microsoft Graph</span></span> |
|----|----|----|
| <span data-ttu-id="8d1cb-144">_初始数据请求_</span><span class="sxs-lookup"><span data-stu-id="8d1cb-144">_Initial data request_</span></span> | <span data-ttu-id="8d1cb-145">使用查询参数:</span><span class="sxs-lookup"><span data-stu-id="8d1cb-145">Uses a query parameter:</span></span><br>`GET /groups?deltaLink=` | <span data-ttu-id="8d1cb-146">使用函数:</span><span class="sxs-lookup"><span data-stu-id="8d1cb-146">Uses a function:</span></span> <br> `GET /groups/delta` |
| <span data-ttu-id="8d1cb-147">_获取新更改_</span><span class="sxs-lookup"><span data-stu-id="8d1cb-147">_Get new changes_</span></span> | `GET /groups?deltaLink={deltaToken}` | `GET /groups/delta?$deltaToken={deltaToken}` |
| <span data-ttu-id="8d1cb-148">_从现在开始同步_</span><span class="sxs-lookup"><span data-stu-id="8d1cb-148">_Sync from now_</span></span> |<span data-ttu-id="8d1cb-149">使用自定义 HTTP 标头:</span><span class="sxs-lookup"><span data-stu-id="8d1cb-149">Uses a custom HTTP header:</span></span><br> `ocp-aad-dq-include-only-delta-token: true` | <span data-ttu-id="8d1cb-150">使用查询参数:</span><span class="sxs-lookup"><span data-stu-id="8d1cb-150">Uses a query parameter:</span></span> <br> `GET /groups/delta?$deltaToken=latest` |
| <span data-ttu-id="8d1cb-151">_跟踪 directoryObjects 的更改_</span><span class="sxs-lookup"><span data-stu-id="8d1cb-151">_Track changes for directoryObjects_</span></span> | <span data-ttu-id="8d1cb-152">获取相同操作中的多个资源 (用户和组) 的更改:&nbsp;&nbsp;</span><span class="sxs-lookup"><span data-stu-id="8d1cb-152">Gets changes for multiple resource (user and group) in the same operation:&nbsp;&nbsp;</span></span><br> `GET /directoryObject?$filter=isof('User') or isof('Group')&deltaLink=` | <span data-ttu-id="8d1cb-153">将单独的查询与 Microsoft Graph 结合使用, 每个资源对应一项。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-153">Uses separate queries with Microsoft Graph, one for each resource.</span></span> |
| <span data-ttu-id="8d1cb-154">_获取资源和关系更改_</span><span class="sxs-lookup"><span data-stu-id="8d1cb-154">_Get resource and relationship changes_</span></span> | <span data-ttu-id="8d1cb-155">如果资源有关系, 所有请求都将返回资源和关系更改。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-155">All requests return resource and relationship changes, if the resource has relationships.</span></span> | `GET /groups/delta?$expand=members` |
| <span data-ttu-id="8d1cb-156">_指示新项目和已更改项目的响应_</span><span class="sxs-lookup"><span data-stu-id="8d1cb-156">_Response indicating new and changed items_</span></span> | <ul><li><p><span data-ttu-id="8d1cb-157">使用其标准表示形式表示新创建的实例。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-157">Represents newly created instances using their standard representation.</span></span></p></li><li><p><span data-ttu-id="8d1cb-158">更新后的实例由其 id 表示,*至少*具有已更新的属性。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-158">Updated instances are represented by their id with *at least* the properties that have been updated.</span></span> <span data-ttu-id="8d1cb-159">可以包含其他属性。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-159">Other properties may be included.</span></span></p></li><li><p><span data-ttu-id="8d1cb-160">关系表示为`directoryLinkChange`类型。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-160">Relationships are represented as the `directoryLinkChange` type.</span></span></p></li></ul>|<ul><li><p><span data-ttu-id="8d1cb-161">使用其标准表示形式表示新创建的实例。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-161">Represents newly created instances using their standard representation.</span></span></p></li><li><p><span data-ttu-id="8d1cb-162">更新后的实例由其 id 表示,*至少*具有已更新的属性。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-162">Updated instances are represented by their id with *at least* the properties that have been updated.</span></span> <span data-ttu-id="8d1cb-163">可以包含其他属性。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-163">Other properties may be included.</span></span></p></li><li><p><span data-ttu-id="8d1cb-164">关系表示为标准资源表示形式的批注。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-164">Relationships are represented as annotations on the standard resource representation.</span></span> <span data-ttu-id="8d1cb-165">这些批注使用格式`propertyName@delta`, 例如`members@delta` , 组的成员资格更改。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-165">These annotations use the format `propertyName@delta`, for example `members@delta` for a group's membership changes.</span></span></p></li></ul> |
| <span data-ttu-id="8d1cb-166">_指示已删除项目的响应_</span><span class="sxs-lookup"><span data-stu-id="8d1cb-166">_Response indicating  deleted items_</span></span>| <span data-ttu-id="8d1cb-167">指示一个已删除的项, 其附加属性为*isDeleted*设置为 true。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-167">Indicates a deleted item with an additional property of *aad.isDeleted* set to true.</span></span> | <span data-ttu-id="8d1cb-168">指示已删除的项目和\@已删除的注释。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-168">Indicates a deleted item with the \@removed annotation.</span></span> <span data-ttu-id="8d1cb-169">它还可能包含原因代码, 以指示是否已删除项目, 但可以还原或永久删除。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-169">It may also contain a reason code, which indicates if the item is deleted, but can be restored, or is permanently deleted.</span></span> |

<span data-ttu-id="8d1cb-170">如果您的应用程序已在存储状态数据, 请考虑使用前面所示的 "从现在同步", 以帮助管理到增量查询的转换。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-170">If your app is already storing state data, consider using the "sync from now" shown earlier to help manage the transition to delta queries.</span></span>

## <a name="batching"></a><span data-ttu-id="8d1cb-171">批处理</span><span class="sxs-lookup"><span data-stu-id="8d1cb-171">Batching</span></span>

<span data-ttu-id="8d1cb-172">Azure AD Graph 使用称为多部分 MIME 邮件的系统来管理批处理。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-172">Azure AD Graph used a system called multi-part MIME messages to manage batching.</span></span>  <span data-ttu-id="8d1cb-173">Microsoft Graph 使用[JSON 批处理](json-batching.md)在单个批处理操作中允许最长20个请求。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-173">Microsoft Graph uses [JSON batching](json-batching.md) to permit up to 20 requests in a single batch operation.</span></span> <span data-ttu-id="8d1cb-174">JSON 批处理机制使用起来明显简单, 尤其是 JSON 分析库。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-174">The JSON batching mechanism is significantly simpler to use, especially together with JSON parsing libraries.</span></span>  <span data-ttu-id="8d1cb-175">它还允许对批处理操作进行排序。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-175">It also allows for sequencing batch operations.</span></span>  <span data-ttu-id="8d1cb-176">但是, 与 Azure AD Graph 批处理方法相比, 它不是向后兼容。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-176">However, it is not backwards compatible with the Azure AD Graph batching approach.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8d1cb-177">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8d1cb-177">Next Steps</span></span>

- <span data-ttu-id="8d1cb-178">了解 Azure AD Graph 与 Microsoft Graph 之间的[资源差异](migrate-azure-ad-graph-resource-differences.md)。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-178">Learn about [resource differences](migrate-azure-ad-graph-resource-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="8d1cb-179">探索[添加自定义数据](/graph/extensibility-overview), 以获取有关开放和架构扩展的信息。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-179">Explore [add custom data](/graph/extensibility-overview) for information about open and schema extensions.</span></span>
- <span data-ttu-id="8d1cb-180">浏览[delta 查询](/graph/delta-query-overview)以了解 Microsoft Graph 的差异查询版本。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-180">Explore [delta queries](/graph/delta-query-overview) to learn about Microsoft Graph's version of differential query.</span></span>
- <span data-ttu-id="8d1cb-181">浏览[JSON 批处理](json-batching.md)以了解批处理在 Microsoft Graph 中的工作方式。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-181">Explore [JSON batching](json-batching.md) to understand how batching works in Microsoft Graph.</span></span>
- <span data-ttu-id="8d1cb-182">使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="8d1cb-182">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /concepts/migrate-azure-ad-graph-feature-changes.md:
      Failed to parse any rows out of table with headers: |Task|Azure AD Graph|Microsoft Graph|"
  ],
}
-->
