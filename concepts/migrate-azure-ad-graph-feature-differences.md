---
title: Azure AD Graph 和 Microsoft Graph 之间的功能差异
description: 介绍 Azure Active Directory (Azure AD) API 和 Microsoft Graph API 之间的功能差异，以帮助你快速轻松地迁移应用。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: a404c69370c7b6aaeee07e20df1165c43a98a243
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760677"
---
# <a name="feature-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="d0966-103">Azure AD Graph 和 Microsoft Graph 之间的功能差异</span><span class="sxs-lookup"><span data-stu-id="d0966-103">Feature differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="d0966-104">本文是步骤 *1：查看迁移应用的* 过程的 API [差异的一部分](migrate-azure-ad-graph-planning-checklist.md)。</span><span class="sxs-lookup"><span data-stu-id="d0966-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="d0966-105">Microsoft Graph 中的许多功能与 Azure AD Graph 对应的功能类似。</span><span class="sxs-lookup"><span data-stu-id="d0966-105">Many features in Microsoft Graph work similarly to their Azure AD Graph counterparts.</span></span> <span data-ttu-id="d0966-106">但是，一些已更改和/或改进。</span><span class="sxs-lookup"><span data-stu-id="d0966-106">However, a few have been changed and/or improved.</span></span> <span data-ttu-id="d0966-107">在这里，你将了解如何调整应用以充分利用这些差异。</span><span class="sxs-lookup"><span data-stu-id="d0966-107">Here, you'll learn how to adapt your apps to take advantage of these differences.</span></span>  <span data-ttu-id="d0966-108">更改通常很小，但值得付出努力。</span><span class="sxs-lookup"><span data-stu-id="d0966-108">Frequently, the changes are minor, but well worth the effort.</span></span>

<span data-ttu-id="d0966-109">本文介绍了 Microsoft Graph 如何处理：</span><span class="sxs-lookup"><span data-stu-id="d0966-109">This article explores how Microsoft Graph handles:</span></span>

- <span data-ttu-id="d0966-110">目录架构扩展</span><span class="sxs-lookup"><span data-stu-id="d0966-110">Directory schema extensions</span></span>
- <span data-ttu-id="d0966-111">差异查询</span><span class="sxs-lookup"><span data-stu-id="d0966-111">Differential queries</span></span>
- <span data-ttu-id="d0966-112">批处理</span><span class="sxs-lookup"><span data-stu-id="d0966-112">Batching</span></span>

## <a name="directory-schema-extensions"></a><span data-ttu-id="d0966-113">目录架构扩展</span><span class="sxs-lookup"><span data-stu-id="d0966-113">Directory schema extensions</span></span>

<span data-ttu-id="d0966-114">如果你的应用使用 Azure AD Graph 目录扩展，你可以继续使用与 Microsoft Graph (URL 相同的基本 API，) ：</span><span class="sxs-lookup"><span data-stu-id="d0966-114">If your app uses Azure AD Graph directory extensions, you can continue to use the same basic APIs (with Microsoft Graph request URLs) to:</span></span>

- <span data-ttu-id="d0966-115">使用 [application][/graph/api/resources/application？view=graph-rest-v1.0 资源上的 **extensionProperties** 属性) 定义。</span><span class="sxs-lookup"><span data-stu-id="d0966-115">Manage extension property definitions using the **extensionProperties** property on the [application][/graph/api/resources/application?view=graph-rest-v1.0) resource.</span></span>
- <span data-ttu-id="d0966-116">使用 [getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-v1.0) 操作获取可用的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d0966-116">Get available extension properties using the [getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-v1.0) action.</span></span>
- <span data-ttu-id="d0966-117">使用 GET 和 读取扩展值 `$select`</span><span class="sxs-lookup"><span data-stu-id="d0966-117">Read extension values using GET and `$select`</span></span>
- <span data-ttu-id="d0966-118">使用 GET 和 搜索扩展值 `$filter`</span><span class="sxs-lookup"><span data-stu-id="d0966-118">Search on extension values using GET and `$filter`</span></span>
- <span data-ttu-id="d0966-119">使用 PATCH 更新扩展值</span><span class="sxs-lookup"><span data-stu-id="d0966-119">Update extension values using PATCH</span></span>
- <span data-ttu-id="d0966-120">使用 PATCH 删除扩展 (设置为 null **)**</span><span class="sxs-lookup"><span data-stu-id="d0966-120">Remove extension values using PATCH (set to **null**)</span></span>

<span data-ttu-id="d0966-121">Microsoft Graph 提供了增强的架构扩展开发人员体验，现在体验与 Azure AD Graph 目录扩展不兼容。</span><span class="sxs-lookup"><span data-stu-id="d0966-121">Microsoft Graph provides an enhanced schema extensions developer experience, which today is not backwards compatible with Azure AD Graph directory extensions.</span></span> <span data-ttu-id="d0966-122">若要了解更多信息，请参阅 [添加自定义数据 中的架构扩展](./extensibility-overview.md#schema-extensions)。</span><span class="sxs-lookup"><span data-stu-id="d0966-122">To learn more, see [schema extensions in add custom data](./extensibility-overview.md#schema-extensions).</span></span>

### <a name="recommended-migration-approach"></a><span data-ttu-id="d0966-123">建议的迁移方法</span><span class="sxs-lookup"><span data-stu-id="d0966-123">Recommended migration approach</span></span>

<span data-ttu-id="d0966-124">如果你的 Azure AD Graph 应用使用目录扩展，请采用增量方法将应用迁移到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="d0966-124">If your Azure AD Graph app uses directory extensions, take an incremental approach to migrate the app to Microsoft Graph.</span></span>

<span data-ttu-id="d0966-125">首先，将应用切换到使用 Microsoft Graph API 调用，但允许应用继续利用 Azure AD Graph 目录扩展。</span><span class="sxs-lookup"><span data-stu-id="d0966-125">First, switch your app to using Microsoft Graph API calls, but let the app continue to leverage Azure AD Graph directory extensions.</span></span>

<span data-ttu-id="d0966-126">然后，你可以切换到使用 Microsoft Graph 架构扩展。</span><span class="sxs-lookup"><span data-stu-id="d0966-126">Then, you can switch to using Microsoft Graph schema extensions.</span></span> <span data-ttu-id="d0966-127">在某些情况下，切换将不适合。</span><span class="sxs-lookup"><span data-stu-id="d0966-127">In some cases, switching will not be appropriate.</span></span> <span data-ttu-id="d0966-128">如果：</span><span class="sxs-lookup"><span data-stu-id="d0966-128">Do not switch if:</span></span>

- <span data-ttu-id="d0966-129">你的应用使用通过 AD Connect 创建的目录扩展</span><span class="sxs-lookup"><span data-stu-id="d0966-129">Your app uses directory extensions created through AD Connect</span></span>
- <span data-ttu-id="d0966-130">你的应用设置其他应用在令牌声明中使用的目录扩展值</span><span class="sxs-lookup"><span data-stu-id="d0966-130">Your app sets directory extension values that are used in token claims by other apps</span></span>
- <span data-ttu-id="d0966-131">你的应用设置动态成员资格规则中使用的目录扩展值</span><span class="sxs-lookup"><span data-stu-id="d0966-131">Your app sets directory extension values that are used in dynamic membership rules</span></span> 

><span data-ttu-id="d0966-132">**注意**：尚不支持将 Microsoft Graph 架构扩展属性用作令牌中的声明（使用可选声明或在动态成员资格规则中）。</span><span class="sxs-lookup"><span data-stu-id="d0966-132">**NOTE**: Using Microsoft Graph schema extension properties as claims in a token using optional claims or in a dynamic membership rule is not yet supported.</span></span>

<span data-ttu-id="d0966-133">若要切换到较新的 Microsoft Graph 架构扩展模型，你需要：</span><span class="sxs-lookup"><span data-stu-id="d0966-133">To switch to the newer Microsoft Graph schema extension model, you'll need to:</span></span>

- <span data-ttu-id="d0966-134">使用 Microsoft Graph 定义新的架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="d0966-134">Define new schema extension definitions using Microsoft Graph.</span></span>
- <span data-ttu-id="d0966-135">更新应用以支持新的架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="d0966-135">Update the app to support the new schema extension definitions.</span></span>
- <span data-ttu-id="d0966-136">将数据从 Azure AD 架构扩展属性迁移到新的 Microsoft Graph 架构扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d0966-136">Migrate the data from the Azure AD schema extension properties to the new Microsoft Graph schema extension properties.</span></span>  <span data-ttu-id="d0966-137">不支持自动迁移数据。</span><span class="sxs-lookup"><span data-stu-id="d0966-137">Automatic migration of data is not supported.</span></span>

## <a name="differential-queries"></a><span data-ttu-id="d0966-138">差异查询</span><span class="sxs-lookup"><span data-stu-id="d0966-138">Differential queries</span></span>

<span data-ttu-id="d0966-139">Azure AD Graph 和 Microsoft Graph 让你可以使用查询跟踪更改。</span><span class="sxs-lookup"><span data-stu-id="d0966-139">Azure AD Graph and Microsoft Graph let you track changes using queries.</span></span>  <span data-ttu-id="d0966-140">高级方法在两个 API 之间相似，但语法不同。</span><span class="sxs-lookup"><span data-stu-id="d0966-140">The high-level approach is similar between the two APIs, but the syntax is different.</span></span>

<span data-ttu-id="d0966-141">Azure AD Graph 调用这些差异查询。</span><span class="sxs-lookup"><span data-stu-id="d0966-141">Azure AD Graph calls these differential queries.</span></span>  <span data-ttu-id="d0966-142">在 Microsoft Graph 中，它们是 [delta 查询](./delta-query-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="d0966-142">In Microsoft Graph, they're [delta queries](./delta-query-overview.md).</span></span>

<span data-ttu-id="d0966-143">下表重点介绍了主要相似之处和区别：</span><span class="sxs-lookup"><span data-stu-id="d0966-143">The following table highlights key similarities and differences:</span></span>

|<span data-ttu-id="d0966-144">Delta 请求</span><span class="sxs-lookup"><span data-stu-id="d0966-144">Delta request</span></span> |<span data-ttu-id="d0966-145">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="d0966-145">Azure AD Graph</span></span> | <span data-ttu-id="d0966-146">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d0966-146">Microsoft Graph</span></span> |
|----|----|----|
| <span data-ttu-id="d0966-147">_初始数据请求_</span><span class="sxs-lookup"><span data-stu-id="d0966-147">_Initial data request_</span></span> | <span data-ttu-id="d0966-148">使用查询参数：</span><span class="sxs-lookup"><span data-stu-id="d0966-148">Uses a query parameter:</span></span><br>`GET /groups?deltaLink=` | <span data-ttu-id="d0966-149">使用 函数：</span><span class="sxs-lookup"><span data-stu-id="d0966-149">Uses a function:</span></span> <br> `GET /groups/delta` |
| <span data-ttu-id="d0966-150">_获取新更改_</span><span class="sxs-lookup"><span data-stu-id="d0966-150">_Get new changes_</span></span> | `GET /groups?deltaLink={deltaToken}` | `GET /groups/delta?$deltaToken={deltaToken}` |
| <span data-ttu-id="d0966-151">_从现在开始同步_</span><span class="sxs-lookup"><span data-stu-id="d0966-151">_Sync from now_</span></span> |<span data-ttu-id="d0966-152">使用自定义 HTTP 标头：</span><span class="sxs-lookup"><span data-stu-id="d0966-152">Uses a custom HTTP header:</span></span><br> `ocp-aad-dq-include-only-delta-token: true` | <span data-ttu-id="d0966-153">使用查询参数：</span><span class="sxs-lookup"><span data-stu-id="d0966-153">Uses a query parameter:</span></span> <br> `GET /groups/delta?$deltaToken=latest` |
| <span data-ttu-id="d0966-154">_跟踪 directoryObjects 的更改_</span><span class="sxs-lookup"><span data-stu-id="d0966-154">_Track changes for directoryObjects_</span></span> | <span data-ttu-id="d0966-155">在同一操作中 (多个资源组) 组更改：&nbsp;&nbsp;</span><span class="sxs-lookup"><span data-stu-id="d0966-155">Gets changes for multiple resource (user and group) in the same operation:&nbsp;&nbsp;</span></span><br> `GET /directoryObject?$filter=isof('User') or isof('Group')&deltaLink=` | <span data-ttu-id="d0966-156">对 Microsoft Graph 使用单独的查询，每个资源使用一个查询。</span><span class="sxs-lookup"><span data-stu-id="d0966-156">Uses separate queries with Microsoft Graph, one for each resource.</span></span> |
| <span data-ttu-id="d0966-157">_获取资源和关系更改_</span><span class="sxs-lookup"><span data-stu-id="d0966-157">_Get resource and relationship changes_</span></span> | <span data-ttu-id="d0966-158">如果资源具有关系，则所有请求都返回资源和关系更改。</span><span class="sxs-lookup"><span data-stu-id="d0966-158">All requests return resource and relationship changes, if the resource has relationships.</span></span> | `GET /groups/delta?$expand=members` |
| <span data-ttu-id="d0966-159">_指示新项和已更改项的响应_</span><span class="sxs-lookup"><span data-stu-id="d0966-159">_Response indicating new and changed items_</span></span> | <ul><li><p><span data-ttu-id="d0966-160">表示使用其标准表示形式新建的实例。</span><span class="sxs-lookup"><span data-stu-id="d0966-160">Represents newly created instances using their standard representation.</span></span></p></li><li><p><span data-ttu-id="d0966-161">更新的实例用其 ID 表示，其中 *至少* 具有已更新的属性。</span><span class="sxs-lookup"><span data-stu-id="d0966-161">Updated instances are represented by their id with *at least* the properties that have been updated.</span></span> <span data-ttu-id="d0966-162">也可以包括其他属性。</span><span class="sxs-lookup"><span data-stu-id="d0966-162">Other properties may be included.</span></span></p></li><li><p><span data-ttu-id="d0966-163">关系表示为 `directoryLinkChange` 类型。</span><span class="sxs-lookup"><span data-stu-id="d0966-163">Relationships are represented as the `directoryLinkChange` type.</span></span></p></li></ul>|<ul><li><p><span data-ttu-id="d0966-164">表示使用其标准表示形式新建的实例。</span><span class="sxs-lookup"><span data-stu-id="d0966-164">Represents newly created instances using their standard representation.</span></span></p></li><li><p><span data-ttu-id="d0966-165">更新的实例用其 ID 表示，其中 *至少* 具有已更新的属性。</span><span class="sxs-lookup"><span data-stu-id="d0966-165">Updated instances are represented by their id with *at least* the properties that have been updated.</span></span> <span data-ttu-id="d0966-166">也可以包括其他属性。</span><span class="sxs-lookup"><span data-stu-id="d0966-166">Other properties may be included.</span></span></p></li><li><p><span data-ttu-id="d0966-167">关系表示为对标准资源表示法的注释。</span><span class="sxs-lookup"><span data-stu-id="d0966-167">Relationships are represented as annotations on the standard resource representation.</span></span> <span data-ttu-id="d0966-168">这些批注使用 格式 `propertyName@delta` ，例如 `members@delta` ，用于更改组的成员身份。</span><span class="sxs-lookup"><span data-stu-id="d0966-168">These annotations use the format `propertyName@delta`, for example `members@delta` for a group's membership changes.</span></span></p></li></ul> |
| <span data-ttu-id="d0966-169">_指示已删除项目的响应_</span><span class="sxs-lookup"><span data-stu-id="d0966-169">_Response indicating  deleted items_</span></span>| <span data-ttu-id="d0966-170">指示已删除的项目，其中 *aad.isDeleted* 的其他属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="d0966-170">Indicates a deleted item with an additional property of *aad.isDeleted* set to true.</span></span> | <span data-ttu-id="d0966-171">指示具有已删除批注的 \@ 已删除项目。</span><span class="sxs-lookup"><span data-stu-id="d0966-171">Indicates a deleted item with the \@removed annotation.</span></span> <span data-ttu-id="d0966-172">它还可能包含原因代码，该代码指示项目是否被删除，但可以还原或永久删除。</span><span class="sxs-lookup"><span data-stu-id="d0966-172">It may also contain a reason code, which indicates if the item is deleted, but can be restored, or is permanently deleted.</span></span> |

<span data-ttu-id="d0966-173">如果你的应用已存储状态数据，请考虑使用前面显示的"立即同步"来帮助管理到增量查询的过渡。</span><span class="sxs-lookup"><span data-stu-id="d0966-173">If your app is already storing state data, consider using the "sync from now" shown earlier to help manage the transition to delta queries.</span></span>

## <a name="batching"></a><span data-ttu-id="d0966-174">批处理</span><span class="sxs-lookup"><span data-stu-id="d0966-174">Batching</span></span>

<span data-ttu-id="d0966-175">Azure AD Graph 使用名为多部分 MIME 邮件的系统来管理批处理。</span><span class="sxs-lookup"><span data-stu-id="d0966-175">Azure AD Graph used a system called multi-part MIME messages to manage batching.</span></span>  <span data-ttu-id="d0966-176">Microsoft Graph [使用 JSON 批处理](json-batching.md) 在一个批处理操作中允许最多 20 个请求。</span><span class="sxs-lookup"><span data-stu-id="d0966-176">Microsoft Graph uses [JSON batching](json-batching.md) to permit up to 20 requests in a single batch operation.</span></span> <span data-ttu-id="d0966-177">JSON 批处理机制使用起来要简单许多，尤其是与 JSON 分析库一起使用。</span><span class="sxs-lookup"><span data-stu-id="d0966-177">The JSON batching mechanism is significantly simpler to use, especially together with JSON parsing libraries.</span></span>  <span data-ttu-id="d0966-178">它还允许排序批处理操作。</span><span class="sxs-lookup"><span data-stu-id="d0966-178">It also allows for sequencing batch operations.</span></span>  <span data-ttu-id="d0966-179">但是，它与 Azure AD Graph 批处理方法不兼容。</span><span class="sxs-lookup"><span data-stu-id="d0966-179">However, it is not backwards compatible with the Azure AD Graph batching approach.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d0966-180">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d0966-180">Next Steps</span></span>

- <span data-ttu-id="d0966-181">了解 Azure AD Graph [和](migrate-azure-ad-graph-resource-differences.md) Microsoft Graph 之间的资源差异。</span><span class="sxs-lookup"><span data-stu-id="d0966-181">Learn about [resource differences](migrate-azure-ad-graph-resource-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="d0966-182">再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。</span><span class="sxs-lookup"><span data-stu-id="d0966-182">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /concepts/migrate-azure-ad-graph-feature-changes.md:
      Failed to parse any rows out of table with headers: |Task|Azure AD Graph|Microsoft Graph|"
  ],
}
-->