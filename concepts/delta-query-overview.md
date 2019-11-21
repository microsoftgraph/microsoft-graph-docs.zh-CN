---
title: 使用增量查询跟踪 Microsoft Graph 数据更改
description: Delta 查询使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。Microsoft Graph 应用程序可以使用 delta 查询和本地数据存储高效地同步更改。
author: piotrci
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 224ef601bf089ed24eac39a7061f0453c8fd6e3e
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748494"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a><span data-ttu-id="15fa2-104">使用 delta 查询跟踪 Microsoft Graph 数据变更</span><span class="sxs-lookup"><span data-stu-id="15fa2-104">Use delta query to track changes in Microsoft Graph data</span></span>

<span data-ttu-id="15fa2-p102">Delta 查询使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。Microsoft Graph 应用程序可以使用 delta 查询和本地数据存储高效地同步更改。</span><span class="sxs-lookup"><span data-stu-id="15fa2-p102">Delta query enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. Microsoft Graph applications can use delta query to efficiently synchronize changes with a local data store.</span></span>

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a><span data-ttu-id="15fa2-107">使用 delta 查询来跟踪资源集合的更改</span><span class="sxs-lookup"><span data-stu-id="15fa2-107">Use delta query to track changes in a resource collection</span></span>

<span data-ttu-id="15fa2-108">通常的调用模式如下：</span><span class="sxs-lookup"><span data-stu-id="15fa2-108">The typical call pattern is as follows:</span></span>

1. <span data-ttu-id="15fa2-109">应用程序首先对所需资源运行 delta 函数以调用 GET 请求。</span><span class="sxs-lookup"><span data-stu-id="15fa2-109">The application begins by calling a GET request with the delta function on the desired resource.</span></span>
2. <span data-ttu-id="15fa2-110">Microsoft Graph 发送一个包含已请求资源和[状态令牌](#state-tokens)的响应。</span><span class="sxs-lookup"><span data-stu-id="15fa2-110">Microsoft Graph sends a response containing the requested resource and a [state token](#state-tokens).</span></span>

     <span data-ttu-id="15fa2-p103">a.如果返回了 `nextLink` URL，则会话中可能存在要检索的其他数据页面。应用程序继续使用 `nextLink` URL 发出请求以检索所有页面中的数据，直到响应中返回 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="15fa2-p103">a.  If a `nextLink` URL is returned, there may be additional pages of data to be retrieved in the session. The application continues making requests using the `nextLink` URL to retrieve all pages of data until a `deltaLink` URL is returned in the response.</span></span>

     <span data-ttu-id="15fa2-p104">b.如果返回了 `deltaLink` URL，则未返回关于资源现有状态的更多数据。为了执行以后的请求，应用程序使用 `deltaLink` URL 了解资源更改。</span><span class="sxs-lookup"><span data-stu-id="15fa2-p104">b.  If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the `deltaLink` URL to learn about changes to the resource.</span></span>

3. <span data-ttu-id="15fa2-p105">当应用程序需要了解资源更改时，会使用步骤 2 中收到的 `deltaLink` URL 发出新请求。*可能*在完成步骤 2 或应用程序检查更改时立即发出此请求。</span><span class="sxs-lookup"><span data-stu-id="15fa2-p105">When the application needs to learn about changes to the resource, it makes a new request using the `deltaLink` URL received in step 2. This request *may* be made immediately after completing step 2 or when the application checks for changes.</span></span>
4. <span data-ttu-id="15fa2-119">Microsoft Graph 返回响应（`nextLink` URL 或 `deltaLink` URL），其中描述了自上一个请求以来的资源变更。</span><span class="sxs-lookup"><span data-stu-id="15fa2-119">Microsoft Graph returns a response describing changes to the resource since the previous request, and either a `nextLink` URL or a `deltaLink` URL.</span></span>

><span data-ttu-id="15fa2-120">**注意：** Azure Active Directory 中存储的资源（如用户和组）支持“从现在开始同步”方案。</span><span class="sxs-lookup"><span data-stu-id="15fa2-120">**Note:** Resources stored in Azure Active Directory (such as users and groups) support "sync from now" scenarios.</span></span> <span data-ttu-id="15fa2-121">这样一来，便可以跳过上面的第 1 步和第 2 步（如果不想检索资源完整状态的话），并改为请求获取最新 `deltaLink`。</span><span class="sxs-lookup"><span data-stu-id="15fa2-121">This allows you to skip steps 1 and 2 above (if you are not interested in retrieving the full state of the resource) and ask for the latest `deltaLink` instead.</span></span> <span data-ttu-id="15fa2-122">将 `$deltaToken=latest` 追加到 `delta` 函数中，这样响应就会包含 `deltaLink`，而不包含资源数据。</span><span class="sxs-lookup"><span data-stu-id="15fa2-122">Append `$deltaToken=latest` to the `delta` function and the response will contain a `deltaLink` and no resource data.</span></span>

### <a name="state-tokens"></a><span data-ttu-id="15fa2-123">状态令牌</span><span class="sxs-lookup"><span data-stu-id="15fa2-123">State tokens</span></span>

<span data-ttu-id="15fa2-p107">增量查询 GET 响应中始终返回 `nextLink` 或 `deltaLink` 响应头中指定的 URL。`nextLink` URL 包含的是 _skipToken_，`deltaLink` URL 包含的是 _deltaToken_。</span><span class="sxs-lookup"><span data-stu-id="15fa2-p107">A delta query GET response always includes a URL specified in a `nextLink` or `deltaLink` response header. The `nextLink` URL includes a _skipToken_, and a `deltaLink` URL includes a _deltaToken_.</span></span>

<span data-ttu-id="15fa2-p108">这些令牌对客户端不透明。以下是需要了解的详细信息：</span><span class="sxs-lookup"><span data-stu-id="15fa2-p108">These tokens are opaque to the client. The following details are what you need to know about them:</span></span>

- <span data-ttu-id="15fa2-128">每个令牌都反映状态，并表示一轮更改跟踪中的响应快照。</span><span class="sxs-lookup"><span data-stu-id="15fa2-128">Each token reflects the state and represents a snapshot of the resource in that round of change tracking.</span></span>

- <span data-ttu-id="15fa2-p109">状态令牌还会进行编码，并包括初始 delta 查询请求中指定的其他查询参数（如 `$select`）。因此，不需要在后续 delta 查询请求中重复这些操作。</span><span class="sxs-lookup"><span data-stu-id="15fa2-p109">The state tokens also encode and include other query parameters (such as `$select`) specified in the initial delta query request. Therefore, it's not required to repeat them in subsequent delta query requests.</span></span>

- <span data-ttu-id="15fa2-131">执行增量查询时，可以将 `nextLink` 或 `deltaLink` URL 复制并应用到下一个 **delta** 函数调用，无需检查 URL 的内容（包括其状态令牌）。</span><span class="sxs-lookup"><span data-stu-id="15fa2-131">When carrying out delta query, you can copy and apply the `nextLink` or `deltaLink` URL to the next **delta** function call without having to inspect the contents of the URL, including its state token.</span></span>

### <a name="optional-query-parameters"></a><span data-ttu-id="15fa2-132">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="15fa2-132">Optional query parameters</span></span>

<span data-ttu-id="15fa2-p110">如果客户使用查询参数，则它必须在初始请求中指定。Microsoft Graph 自动将指定参数编码为响应中提供的 `nextLink` 或 `deltaLink`。调用应用程序只需预先指定查询参数一次。Microsoft Graph 将为所有后续请求自动添加指定参数。</span><span class="sxs-lookup"><span data-stu-id="15fa2-p110">If a client uses a query parameter, it must be specified in the initial request. Microsoft Graph automatically encodes the specified parameter into the `nextLink` or `deltaLink` provided in the response. The calling application only needs to specify the query parameters once upfront. Microsoft Graph adds the specified parameters automatically for all subsequent requests.</span></span>

<span data-ttu-id="15fa2-137">请注意以下相关可选查询参数：</span><span class="sxs-lookup"><span data-stu-id="15fa2-137">Note the following regarding optional query parameters:</span></span>

- <span data-ttu-id="15fa2-138">`$orderby` 不可用于增量查询。</span><span class="sxs-lookup"><span data-stu-id="15fa2-138">`$orderby` is not a supported for delta queries.</span></span>
     - <span data-ttu-id="15fa2-139">不要假设增量查询返回特定响应顺序。</span><span class="sxs-lookup"><span data-stu-id="15fa2-139">Do not assume a specific sequence of the responses returned from a delta query.</span></span> <span data-ttu-id="15fa2-140">假设同一项目可以显示在 `nextLink` 序列的任意位置，并以合并逻辑进行处理。</span><span class="sxs-lookup"><span data-stu-id="15fa2-140">Assume that the same item can show up anywhere in the `nextLink` sequence and handle that in your merge logic.</span></span>
- <span data-ttu-id="15fa2-141">`$top` 不可用于增量查询，而且每页中的对象数量可能因资源类型和资源更改类型而异。</span><span class="sxs-lookup"><span data-stu-id="15fa2-141">`$top` is not supported for delta queries, and the number of objects in each page can vary depending on the resource type and the type of changes made to the resource.</span></span>

<span data-ttu-id="15fa2-142">对于用户和组，下列限制适用于使用一些查询参数的 using：</span><span class="sxs-lookup"><span data-stu-id="15fa2-142">For users and groups, the following restrictions apply to using using some query parameters:</span></span>

<span data-ttu-id="15fa2-143">对于用户和组，在使用某些查询参数时受到限制：</span><span class="sxs-lookup"><span data-stu-id="15fa2-143">For users and groups, there are restrictions on using some query parameters:</span></span>

- <span data-ttu-id="15fa2-p112">如果使用的是 `$select` 查询参数，则该参数表示客户倾向于仅跟踪 `$select` 语句中指定的属性或关系的更改。如果未选中的属性发生更改，则属性已更改的资源将不会出现在后续请求之后的 delta 响应中。</span><span class="sxs-lookup"><span data-stu-id="15fa2-p112">If a `$select` query parameter is used, the parameter indicates that the client prefers to only track changes on the properties or relationships specified in the `$select` statement. If a change occurs to a property that is not selected, the resource for which that property changed does not appear in the delta response after a subsequent request.</span></span>
- <span data-ttu-id="15fa2-146">`$select` 还支持用户和组的 `manager` 和 `members` 导航属性。</span><span class="sxs-lookup"><span data-stu-id="15fa2-146">`$select` is only supported for the `manager` and `members` navigational property for users and groups respectively.</span></span> <span data-ttu-id="15fa2-147">选择这些属性可以跟踪对用户管理器和组成员身份的更改。</span><span class="sxs-lookup"><span data-stu-id="15fa2-147">Selecting those properties allows tracking of changes to user's manager and group memberships.</span></span>

- <span data-ttu-id="15fa2-148">借助范围筛选器，可按对象 ID 跟踪一个或多个特定用户或组的更改。</span><span class="sxs-lookup"><span data-stu-id="15fa2-148">Scoping filters allow you to track changes to one or more specific users or groups by object ID.</span></span> <span data-ttu-id="15fa2-149">例如，以下请求会返回与查询筛选器中指定的 ID 相匹配的组的更改。</span><span class="sxs-lookup"><span data-stu-id="15fa2-149">For example, the following request returns changes for the groups matching the IDs specified in the query filter.</span></span> 

<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
https://graph.microsoft.com/beta/groups/delta/?$filter=id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' or id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e' 
```

## <a name="resource-representation-in-the-delta-query-response"></a><span data-ttu-id="15fa2-150">delta 查询响应中的资源表示形式</span><span class="sxs-lookup"><span data-stu-id="15fa2-150">Resource representation in the delta query response</span></span>

- <span data-ttu-id="15fa2-151">在 delta 查询响应中，使用标准表示形式表示受支持资源的新建实例。</span><span class="sxs-lookup"><span data-stu-id="15fa2-151">Newly created instances of a supported resource are represented in the delta query response using their standard representation.</span></span>

- <span data-ttu-id="15fa2-152">更新实例由它们的 **id** 表示，*至少*具有已更新的属性，但可能也包含其他属性。</span><span class="sxs-lookup"><span data-stu-id="15fa2-152">Updated instances are represented by their **id** with *at least* the properties that have been updated, but additional properties may be included.</span></span>

- <span data-ttu-id="15fa2-p115">用户和组的关系表示为对标准资源表示形式的注释。这些注释使用格式 `propertyName@delta`。注释包含在初始 delta 查询请求的响应内。</span><span class="sxs-lookup"><span data-stu-id="15fa2-p115">Relationships on users and groups are represented as annotations on the standard resource representation. These annotations use the format `propertyName@delta`. The annotations are included in the response of the initial delta query request.</span></span>

<span data-ttu-id="15fa2-156">删除的实例使用其 **id** 和 `@removed` 对象表示。</span><span class="sxs-lookup"><span data-stu-id="15fa2-156">Removed instances are represented by their **id** and an `@removed` object.</span></span> <span data-ttu-id="15fa2-157">`@removed` 对象可能包含有关为何删除该实例的其他信息。</span><span class="sxs-lookup"><span data-stu-id="15fa2-157">The `@removed` node may include additional information about why the instance was removed.</span></span> <span data-ttu-id="15fa2-158">例如，"@removed": {"reason": "changed"}。</span><span class="sxs-lookup"><span data-stu-id="15fa2-158">For example,  "@removed": {"reason": "changed"}.</span></span>

<span data-ttu-id="15fa2-159">可能的 @removed 原因可以是*已更改*或*已删除*。</span><span class="sxs-lookup"><span data-stu-id="15fa2-159">Possible @removed reasons can be *changed* or *deleted*.</span></span>

- <span data-ttu-id="15fa2-160">*已更改*表示该项已被删除，可以从 [deletedItems](/graph/api/resources/directory?view=graph-rest-beta) 恢复。</span><span class="sxs-lookup"><span data-stu-id="15fa2-160">*Changed* indicates the item was deleted and can be restored from [deletedItems](/graph/api/resources/directory?view=graph-rest-beta).</span></span>

- <span data-ttu-id="15fa2-161">*已删除*表示该项已被删除，无法恢复。</span><span class="sxs-lookup"><span data-stu-id="15fa2-161">*Deleted* indicates the item is deleted and cannot be restored.</span></span>

<span data-ttu-id="15fa2-p117">`@removed` 对象可以在初始 delta 查询响应和跟踪的 (deltaLink) 响应中返回。使用 delta 查询请求的客户端应能够处理响应中的这些对象。</span><span class="sxs-lookup"><span data-stu-id="15fa2-p117">The `@removed` object can be returned in the initial delta query response and in tracked (deltaLink) responses. Clients using delta query requests should be designed to handle these objects in the responses.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="15fa2-164">支持的资源</span><span class="sxs-lookup"><span data-stu-id="15fa2-164">Supported resources</span></span>

<span data-ttu-id="15fa2-165">目前，以下资源支持 delta 查询。</span><span class="sxs-lookup"><span data-stu-id="15fa2-165">Delta query is currently supported for the following resources.</span></span>

| <span data-ttu-id="15fa2-166">**资源集合**</span><span class="sxs-lookup"><span data-stu-id="15fa2-166">**Resource collection**</span></span>                                        | <span data-ttu-id="15fa2-167">**API**</span><span class="sxs-lookup"><span data-stu-id="15fa2-167">**API**</span></span>                                                                                                                                                                                |
| :------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="15fa2-168">应用（预览版）</span><span class="sxs-lookup"><span data-stu-id="15fa2-168">Applications (preview)</span></span>                                         | <span data-ttu-id="15fa2-169">[application](/graph/api/resources/application?view=graph-rest-beta) 资源（预览版）的 [delta](/graph/api/application-delta?view=graph-rest-beta) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-169">[delta](/graph/api/application-delta?view=graph-rest-beta) function of the [application](/graph/api/resources/application?view=graph-rest-beta) resource (preview)</span></span>                     |
| <span data-ttu-id="15fa2-170">Classes（预览版）</span><span class="sxs-lookup"><span data-stu-id="15fa2-170">Classes (preview)</span></span>                                              | <span data-ttu-id="15fa2-171">[Class](/graph/api/resources/educationclass?view=graph-rest-beta) 资源（预览版）的 [delta](/graph/api/educationclass-delta?view=graph-rest-beta) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-171">[delta](/graph/api/educationclass-delta?view=graph-rest-beta) function of the [Class](/graph/api/resources/educationclass?view=graph-rest-beta) resource (preview)</span></span>                     |
| <span data-ttu-id="15fa2-172">目录对象 （预览版）。</span><span class="sxs-lookup"><span data-stu-id="15fa2-172">Directory objects (preview)</span></span>                                    | <span data-ttu-id="15fa2-173">[directoryObjects](/graph/api/resources/directoryobject?view=graph-rest-beta) 资源（预览版）的 [delta](/graph/api/directoryobject-delta?view=graph-rest-beta) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-173">[delta](/graph/api/directoryobject-delta?view=graph-rest-beta) function of the [directoryObjects](/graph/api/resources/directoryobject?view=graph-rest-beta) resource (preview)</span></span>        |
| <span data-ttu-id="15fa2-174">目录角色</span><span class="sxs-lookup"><span data-stu-id="15fa2-174">Directory roles</span></span>                                                | <span data-ttu-id="15fa2-175">[directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0) 资源的 [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-175">[delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) function of the [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0) resource</span></span>                           |
| <span data-ttu-id="15fa2-176">驱动器项目\*</span><span class="sxs-lookup"><span data-stu-id="15fa2-176">Drive items\*</span></span>                                                  | <span data-ttu-id="15fa2-177">[driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) 资源的 [delta](/graph/api/driveitem-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-177">[delta](/graph/api/driveitem-delta?view=graph-rest-1.0) function of the [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) resource</span></span>                                       |
| <span data-ttu-id="15fa2-178">教育用户（预览版）</span><span class="sxs-lookup"><span data-stu-id="15fa2-178">Education users (preview)</span></span>                                      | <span data-ttu-id="15fa2-179">[教育用户](/graph/api/resources/educationuser?view=graph-rest-beta) 资源（预览版）的 [delta](/graph/api/educationuser-delta?view=graph-rest-beta) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-179">[delta](/graph/api/educationuser-delta?view=graph-rest-beta) function of the [Education user](/graph/api/resources/educationuser?view=graph-rest-beta) resource (preview)</span></span>             |
| <span data-ttu-id="15fa2-180">主日历的日历视图（日期范围）中的事件</span><span class="sxs-lookup"><span data-stu-id="15fa2-180">Events in a calendar view (date range) of the primary calendar</span></span> | <span data-ttu-id="15fa2-181">[事件](/graph/api/resources/event?view=graph-rest-1.0)资源的 [delta](/graph/api/event-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-181">[delta](/graph/api/event-delta?view=graph-rest-1.0) function of the [event](/graph/api/resources/event?view=graph-rest-1.0) resource</span></span>                                                   |
| <span data-ttu-id="15fa2-182">组</span><span class="sxs-lookup"><span data-stu-id="15fa2-182">Groups</span></span>                                                         | <span data-ttu-id="15fa2-183">[组](/graph/api/resources/group?view=graph-rest-1.0)资源的 [delta](/graph/api/group-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-183">[delta](/graph/api/group-delta?view=graph-rest-1.0) function of the [group](/graph/api/resources/group?view=graph-rest-1.0) resource</span></span>                                                   |
| <span data-ttu-id="15fa2-184">邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="15fa2-184">Mail folders</span></span>                                                   | <span data-ttu-id="15fa2-185">[邮件文件夹](/graph/api/resources/mailfolder?view=graph-rest-1.0)资源的 [delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-185">[delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) function of the [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) resource</span></span>                                    |
| <span data-ttu-id="15fa2-186">文件夹中的邮件</span><span class="sxs-lookup"><span data-stu-id="15fa2-186">Messages in a folder</span></span>                                           | <span data-ttu-id="15fa2-187">[邮件](/graph/api/resources/message?view=graph-rest-1.0)资源的 [delta](/graph/api/message-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-187">[delta](/graph/api/message-delta?view=graph-rest-1.0) function of the [message](/graph/api/resources/message?view=graph-rest-1.0) resource</span></span>                                             |
| <span data-ttu-id="15fa2-188">私人联系人文件夹</span><span class="sxs-lookup"><span data-stu-id="15fa2-188">Personal contact folders</span></span>                                       | <span data-ttu-id="15fa2-189">[联系人文件夹](/graph/api/resources/contactfolder?view=graph-rest-1.0)资源的 [delta](/graph/api/contactfolder-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-189">[delta](/graph/api/contactfolder-delta?view=graph-rest-1.0) function of the [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) resource</span></span>                           |
| <span data-ttu-id="15fa2-190">文件夹中的私人联系人</span><span class="sxs-lookup"><span data-stu-id="15fa2-190">Personal contacts in a folder</span></span>                                  | <span data-ttu-id="15fa2-191">[contact](/graph/api/resources/contact?view=graph-rest-1.0) 资源的 [delta](/graph/api/contact-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-191">[delta](/graph/api/contact-delta?view=graph-rest-1.0) function of the [contact](/graph/api/resources/contact?view=graph-rest-1.0) resource</span></span>                                             |
| <span data-ttu-id="15fa2-192">学校（预览版）</span><span class="sxs-lookup"><span data-stu-id="15fa2-192">Schools (preview)</span></span>                                              | <span data-ttu-id="15fa2-193">[学校](/graph/api/resources/educationschool?view=graph-rest-beta) 资源（预览版）的 [delta](/graph/api/educationschool-delta?view=graph-rest-beta) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-193">[delta](/graph/api/educationschool-delta?view=graph-rest-beta) function of the [School](/graph/api/resources/educationschool?view=graph-rest-beta) resource (preview)</span></span>                  |
| <span data-ttu-id="15fa2-194">服务主体（预览版）</span><span class="sxs-lookup"><span data-stu-id="15fa2-194">Service principals (preview)</span></span>                                   | <span data-ttu-id="15fa2-195">[servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) 资源（预览版）的 [delta](/graph/api/serviceprincipal-delta?view=graph-rest-beta) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-195">[delta](/graph/api/serviceprincipal-delta?view=graph-rest-beta) function of the [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) resource (preview)</span></span>      |
| <span data-ttu-id="15fa2-196">用户</span><span class="sxs-lookup"><span data-stu-id="15fa2-196">Users</span></span>                                                          | <span data-ttu-id="15fa2-197">[用户](/graph/api/resources/user?view=graph-rest-1.0)资源的 [delta](/graph/api/user-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-197">[delta](/graph/api/user-delta?view=graph-rest-1.0) function of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource</span></span> |
| <span data-ttu-id="15fa2-198">Planner 项目\*\*（预览版）</span><span class="sxs-lookup"><span data-stu-id="15fa2-198">Planner items\*\* (preview)</span></span>                                    | <span data-ttu-id="15fa2-199">[plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta) 资源所有段的 [delta](/graph/api/planneruser-list-delta?view=graph-rest-beta) 函数（预览版）</span><span class="sxs-lookup"><span data-stu-id="15fa2-199">[delta](/graph/api/planneruser-list-delta?view=graph-rest-beta) function of the all segment of [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta) resource (preview)</span></span>|
| <span data-ttu-id="15fa2-200">频道中的 chatMessages（预览版）</span><span class="sxs-lookup"><span data-stu-id="15fa2-200">chatMessages in a channel (preview)</span></span>                            | <span data-ttu-id="15fa2-201">[chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) 的 [delta](/graph/api/chatmessage-delta?view=graph-rest-beta) 函数</span><span class="sxs-lookup"><span data-stu-id="15fa2-201">[delta](/graph/api/chatmessage-delta?view=graph-rest-beta) function of the [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta)</span></span> |

> <span data-ttu-id="15fa2-202">\* OneDrive 资源的使用模式与其他支持资源类似，仅存在一些小的语法差异。</span><span class="sxs-lookup"><span data-stu-id="15fa2-202">\* The usage pattern for OneDrive resources is similar to the other supported resources with some minor syntax differences.</span></span> <span data-ttu-id="15fa2-203">为了与其他资源类型保持一致，适用于驱动器的 delta 查询今后将进行更新。</span><span class="sxs-lookup"><span data-stu-id="15fa2-203">Delta query for drives will be updated in the future to be consistent with other resource types.</span></span> <span data-ttu-id="15fa2-204">若要详细了解现行语法，请参阅[跟踪驱动器更改](/graph/api/driveitem-delta?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="15fa2-204">For more detail about the current syntax, see [Track changes for a drive](/graph/api/driveitem-delta?view=graph-rest-1.0).</span></span>

> <span data-ttu-id="15fa2-205">\*\* Planner 资源的使用模式与其他支持资源类似，仅存在些许差异。</span><span class="sxs-lookup"><span data-stu-id="15fa2-205">\*\* The usage pattern for Planner resources is similar to other supported resources with a few differences.</span></span>  <span data-ttu-id="15fa2-206">有关详细信息，请参阅[跟踪 Planner 更改](/graph/api/planneruser-list-delta?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="15fa2-206">For details, see [Track changes for Planner](/graph/api/planneruser-list-delta?view=graph-rest-beta).</span></span>

### <a name="limitations"></a><span data-ttu-id="15fa2-207">限制</span><span class="sxs-lookup"><span data-stu-id="15fa2-207">Limitations</span></span>

#### <a name="properties-stored-outside-of-the-main-data-store"></a><span data-ttu-id="15fa2-208">在主数据存储外部存储的属性</span><span class="sxs-lookup"><span data-stu-id="15fa2-208">Properties stored outside of the main data store</span></span>

<span data-ttu-id="15fa2-209">某些资源包含一些存储在资源主数据存储外部的属性（例如，用户资源大部分存储在 Azure AD 系统中，而 **skills** 之类的一些属性存储在 SharePoint Online 中）。</span><span class="sxs-lookup"><span data-stu-id="15fa2-209">Some resources contain properties that are stored outside of the main data store for the resource (for example, the user resource is mostly stored in the Azure AD system, while some properties, like **skills**, are stored in SharePoint Online).</span></span> <span data-ttu-id="15fa2-210">目前，在更改跟踪中不支持这些属性；对其中一个属性所做的更改不会导致在增量查询响应中显示对象。</span><span class="sxs-lookup"><span data-stu-id="15fa2-210">Currently, those properties are not supported as part of change tracking; a change to one of those properties will not result in an object showing up in the delta query response.</span></span> <span data-ttu-id="15fa2-211">目前，仅在主数据存储中存储的属性会触发增量查询中的更改。</span><span class="sxs-lookup"><span data-stu-id="15fa2-211">Currently, only the properties stored in the main data store trigger changes in the delta query.</span></span>

<span data-ttu-id="15fa2-212">若要验证属性是否可在增量查询中使用，请尝试对资源集合执行常规 `GET` 操作，然后选择感兴趣的属性。</span><span class="sxs-lookup"><span data-stu-id="15fa2-212">To verify that a property can be used in delta query, try to perform a regular `GET` operation on the resource collection, and select the property you're interested in.</span></span> <span data-ttu-id="15fa2-213">例如，可尝试对用户集合使用 **skills** 属性。</span><span class="sxs-lookup"><span data-stu-id="15fa2-213">For example, you can try the **skills** property on the users collection.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/?$select=skills
```

<span data-ttu-id="15fa2-214">由于 **skills** 属性存储在 Azure AD 外部，因此响应如下。</span><span class="sxs-lookup"><span data-stu-id="15fa2-214">Because the **skills** property is stored outside of Azure AD, the following is the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 501 Not Implemented
Content-type: application/json

{
    "error": {
        "code": "NotImplemented",
        "message": "This operation target is not yet supported.",
        "innerError": {
            "request-id": "...",
            "date": "2019-09-20T21:47:50"
        }
    }
}
```

<span data-ttu-id="15fa2-215">据此可得知，**user** 资源的增量查询不支持 **skills** 属性。</span><span class="sxs-lookup"><span data-stu-id="15fa2-215">This tells you that the **skills** property is not supported for delta query on the **user** resource.</span></span>

#### <a name="navigation-properties"></a><span data-ttu-id="15fa2-216">导航属性</span><span class="sxs-lookup"><span data-stu-id="15fa2-216">Navigation properties</span></span>

<span data-ttu-id="15fa2-217">不支持导航属性。</span><span class="sxs-lookup"><span data-stu-id="15fa2-217">Navigation properties are not supported.</span></span> <span data-ttu-id="15fa2-218">例如，不能跟踪对用户集合所做的更改，这些更改将包含对用户 **photo** 属性所做的更改；**photo** 是一个存储在用户实体之外的导航属性，且对其进行的更改不会导致增量响应中包含用户对象。</span><span class="sxs-lookup"><span data-stu-id="15fa2-218">For example, you cannot track changes to the users collection that would include changes to their **photo** property; **photo** is a navigation property stored outside of the user entity, and changes to it do not cause the user object to be included in the delta response.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15fa2-219">先决条件</span><span class="sxs-lookup"><span data-stu-id="15fa2-219">Prerequisites</span></span>

<span data-ttu-id="15fa2-220">在对某个特定资源执行 delta 查询时也需要读取该资源所需的相同[权限](./permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="15fa2-220">The same [permissions](./permissions-reference.md) that are required to read a specific resource are also required to perform delta query on that resource.</span></span>

## <a name="delta-query-request-examples"></a><span data-ttu-id="15fa2-221">delta 查询请求示例</span><span class="sxs-lookup"><span data-stu-id="15fa2-221">Delta query request examples</span></span>

- [<span data-ttu-id="15fa2-222">获取日历视图中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="15fa2-222">Get incremental changes to events in a calendar view</span></span>](delta-query-events.md)
- [<span data-ttu-id="15fa2-223">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="15fa2-223">Get incremental changes to messages in a folder</span></span>](./delta-query-messages.md)
- [<span data-ttu-id="15fa2-224">获取组的增量更改</span><span class="sxs-lookup"><span data-stu-id="15fa2-224">Get incremental changes to groups</span></span>](./delta-query-groups.md)
- [<span data-ttu-id="15fa2-225">获取用户的增量更改</span><span class="sxs-lookup"><span data-stu-id="15fa2-225">Get incremental changes to users</span></span>](./delta-query-users.md)
