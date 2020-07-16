---
title: 使用增量查询跟踪 Microsoft Graph 数据更改
description: Delta 查询使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。Microsoft Graph 应用程序可以使用 delta 查询和本地数据存储高效地同步更改。
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 7e969858b7537ea36189d24c449803d2a00b125e
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990036"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a><span data-ttu-id="a124d-104">使用 delta 查询跟踪 Microsoft Graph 数据变更</span><span class="sxs-lookup"><span data-stu-id="a124d-104">Use delta query to track changes in Microsoft Graph data</span></span>

<span data-ttu-id="a124d-p102">Delta 查询使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。Microsoft Graph 应用程序可以使用 delta 查询和本地数据存储高效地同步更改。</span><span class="sxs-lookup"><span data-stu-id="a124d-p102">Delta query enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. Microsoft Graph applications can use delta query to efficiently synchronize changes with a local data store.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="a124d-107">教程：使用更改通知和跟踪 Microsoft Graph 中的更改</span><span class="sxs-lookup"><span data-stu-id="a124d-107">Tutorial: Use Change Notifications and Track Changes with Microsoft Graph</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a><span data-ttu-id="a124d-108">使用 delta 查询来跟踪资源集合的更改</span><span class="sxs-lookup"><span data-stu-id="a124d-108">Use delta query to track changes in a resource collection</span></span>

<span data-ttu-id="a124d-109">通常的调用模式如下：</span><span class="sxs-lookup"><span data-stu-id="a124d-109">The typical call pattern is as follows:</span></span>

1. <span data-ttu-id="a124d-110">应用程序首先对所需资源运行 delta 函数以调用 GET 请求。</span><span class="sxs-lookup"><span data-stu-id="a124d-110">The application begins by calling a GET request with the delta function on the desired resource.</span></span>
2. <span data-ttu-id="a124d-111">Microsoft Graph 发送一个包含已请求资源和[状态令牌](#state-tokens)的响应。</span><span class="sxs-lookup"><span data-stu-id="a124d-111">Microsoft Graph sends a response containing the requested resource and a [state token](#state-tokens).</span></span>

     <span data-ttu-id="a124d-p103">a.如果返回了 `nextLink` URL，则会话中可能存在要检索的其他数据页面。应用程序继续使用 `nextLink` URL 发出请求以检索所有页面中的数据，直到响应中返回 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="a124d-p103">a.  If a `nextLink` URL is returned, there may be additional pages of data to be retrieved in the session. The application continues making requests using the `nextLink` URL to retrieve all pages of data until a `deltaLink` URL is returned in the response.</span></span>

     <span data-ttu-id="a124d-p104">b.如果返回了 `deltaLink` URL，则未返回关于资源现有状态的更多数据。为了执行以后的请求，应用程序使用 `deltaLink` URL 了解资源更改。</span><span class="sxs-lookup"><span data-stu-id="a124d-p104">b.  If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the `deltaLink` URL to learn about changes to the resource.</span></span>

3. <span data-ttu-id="a124d-p105">当应用程序需要了解资源更改时，会使用步骤 2 中收到的 `deltaLink` URL 发出新请求。*可能*在完成步骤 2 或应用程序检查更改时立即发出此请求。</span><span class="sxs-lookup"><span data-stu-id="a124d-p105">When the application needs to learn about changes to the resource, it makes a new request using the `deltaLink` URL received in step 2. This request *may* be made immediately after completing step 2 or when the application checks for changes.</span></span>
4. <span data-ttu-id="a124d-120">Microsoft Graph 返回响应（`nextLink` URL 或 `deltaLink` URL），其中描述了自上一个请求以来的资源变更。</span><span class="sxs-lookup"><span data-stu-id="a124d-120">Microsoft Graph returns a response describing changes to the resource since the previous request, and either a `nextLink` URL or a `deltaLink` URL.</span></span>

><span data-ttu-id="a124d-121">**注意：** Azure Active Directory 中存储的资源（如用户和组）支持“从现在开始同步”方案。</span><span class="sxs-lookup"><span data-stu-id="a124d-121">**Note:** Resources stored in Azure Active Directory (such as users and groups) support "sync from now" scenarios.</span></span> <span data-ttu-id="a124d-122">这样一来，便可以跳过第 1 步和第 2 步（如果不想检索资源完整状态的话），并改为请求获取最新 `deltaLink`。</span><span class="sxs-lookup"><span data-stu-id="a124d-122">This allows you to skip steps 1 and 2 (if you're not interested in retrieving the full state of the resource) and ask for the latest `deltaLink` instead.</span></span> <span data-ttu-id="a124d-123">将 `$deltaToken=latest` 追加到 `delta` 函数中，这样响应就会包含 `deltaLink`，而不包含资源数据。</span><span class="sxs-lookup"><span data-stu-id="a124d-123">Append `$deltaToken=latest` to the `delta` function and the response will contain a `deltaLink` and no resource data.</span></span>

><span data-ttu-id="a124d-124">**注意：** 引用增量查询函数的方式通常是将 `/delta` 附加到资源名称。</span><span class="sxs-lookup"><span data-stu-id="a124d-124">**Note:** The delta query function is generally referred to by appending `/delta` to the resource name.</span></span> <span data-ttu-id="a124d-125">但是，`/delta` 是在 Microsoft Graph SDK 生成的请求中显示的完全限定名称 `/microsoft.graph.delta` 的快捷方式。</span><span class="sxs-lookup"><span data-stu-id="a124d-125">However, `/delta` is a shortcut for the fully qualified name `/microsoft.graph.delta` that you see in requests generated by the Microsoft Graph SDKs.</span></span>

><span data-ttu-id="a124d-126">**注意：** 对 delta 查询函数的初始请求（无 delta 或 skip 标记）将返回当前存在于集合中的资源。</span><span class="sxs-lookup"><span data-stu-id="a124d-126">**Note:** The initial request to the delta query function (no delta or skip token) will return the resources that currently exist in the collection.</span></span> <span data-ttu-id="a124d-127">在初始 delta 查询之前创建和删除的资源不会返回。</span><span class="sxs-lookup"><span data-stu-id="a124d-127">Resources that have been created and deleted prior to the initial delta query won't be returned.</span></span> <span data-ttu-id="a124d-128">在初始请求之前所做的更新将在返回的资源上汇总为其最新状态。</span><span class="sxs-lookup"><span data-stu-id="a124d-128">Updates made before the initial request are summarized on the resource returned as its latest state.</span></span>

### <a name="state-tokens"></a><span data-ttu-id="a124d-129">状态令牌</span><span class="sxs-lookup"><span data-stu-id="a124d-129">State tokens</span></span>

<span data-ttu-id="a124d-p109">增量查询 GET 响应中始终返回 `nextLink` 或 `deltaLink` 响应头中指定的 URL。`nextLink` URL 包含的是 _skipToken_，`deltaLink` URL 包含的是 _deltaToken_。</span><span class="sxs-lookup"><span data-stu-id="a124d-p109">A delta query GET response always includes a URL specified in a `nextLink` or `deltaLink` response header. The `nextLink` URL includes a _skipToken_, and a `deltaLink` URL includes a _deltaToken_.</span></span>

<span data-ttu-id="a124d-p110">这些令牌对客户端不透明。以下是需要了解的详细信息：</span><span class="sxs-lookup"><span data-stu-id="a124d-p110">These tokens are opaque to the client. The following details are what you need to know about them:</span></span>

- <span data-ttu-id="a124d-134">每个令牌都反映状态，并表示一轮更改跟踪中的响应快照。</span><span class="sxs-lookup"><span data-stu-id="a124d-134">Each token reflects the state and represents a snapshot of the resource in that round of change tracking.</span></span>

- <span data-ttu-id="a124d-p111">状态令牌还会进行编码，并包括初始 delta 查询请求中指定的其他查询参数（如 `$select`）。因此，不需要在后续 delta 查询请求中重复这些操作。</span><span class="sxs-lookup"><span data-stu-id="a124d-p111">The state tokens also encode and include other query parameters (such as `$select`) specified in the initial delta query request. Therefore, it's not required to repeat them in subsequent delta query requests.</span></span>

- <span data-ttu-id="a124d-137">执行增量查询时，可以将 `nextLink` 或 `deltaLink` URL 复制并应用到下一个 **delta** 函数调用，无需检查 URL 的内容（包括其状态令牌）。</span><span class="sxs-lookup"><span data-stu-id="a124d-137">When carrying out delta query, you can copy and apply the `nextLink` or `deltaLink` URL to the next **delta** function call without having to inspect the contents of the URL, including its state token.</span></span>

### <a name="optional-query-parameters"></a><span data-ttu-id="a124d-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a124d-138">Optional query parameters</span></span>

<span data-ttu-id="a124d-p112">如果客户使用查询参数，则它必须在初始请求中指定。Microsoft Graph 自动将指定参数编码为响应中提供的 `nextLink` 或 `deltaLink`。调用应用程序只需预先指定查询参数一次。Microsoft Graph 将为所有后续请求自动添加指定参数。</span><span class="sxs-lookup"><span data-stu-id="a124d-p112">If a client uses a query parameter, it must be specified in the initial request. Microsoft Graph automatically encodes the specified parameter into the `nextLink` or `deltaLink` provided in the response. The calling application only needs to specify the query parameters once upfront. Microsoft Graph adds the specified parameters automatically for all subsequent requests.</span></span>

<span data-ttu-id="a124d-143">请注意以下可选查询参数的常规有限支持：</span><span class="sxs-lookup"><span data-stu-id="a124d-143">Note the general limited support of the following optional query parameters:</span></span>

- `$orderby`

    <span data-ttu-id="a124d-144">不要假设增量查询返回特定响应顺序。</span><span class="sxs-lookup"><span data-stu-id="a124d-144">Do not assume a specific sequence of the responses returned from a delta query.</span></span> <span data-ttu-id="a124d-145">假设同一项目可以显示在 `nextLink` 序列的任意位置，并以合并逻辑进行处理。</span><span class="sxs-lookup"><span data-stu-id="a124d-145">Assume that the same item can show up anywhere in the `nextLink` sequence and handle that in your merge logic.</span></span>
- `$top`

    <span data-ttu-id="a124d-146">每页中的对象数量可能因资源类型和资源更改类型而异。</span><span class="sxs-lookup"><span data-stu-id="a124d-146">The number of objects in each page can vary depending on the resource type and the type of changes made to the resource.</span></span>

<span data-ttu-id="a124d-147">对于[消息](/graph/api/resources/message?view=graph-rest-1.0)资源，请参阅[增量查询中的查询参数支持](delta-query-messages.md#use-query-parameters-in-a-delta-query-for-messages)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a124d-147">For the [message](/graph/api/resources/message?view=graph-rest-1.0) resource, see details for [query parameters support in a delta query](delta-query-messages.md#use-query-parameters-in-a-delta-query-for-messages).</span></span>

<span data-ttu-id="a124d-148">对于[用户](/graph/api/resources/user?view=graph-rest-1.0)和[组](/graph/api/resources/group?view=graph-rest-1.0)资源，在使用某些查询参数时受到限制：</span><span class="sxs-lookup"><span data-stu-id="a124d-148">For the [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0) resources, there are restrictions on using some query parameters:</span></span>

- <span data-ttu-id="a124d-149">不支持 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="a124d-149">`$expand` is not supported.</span></span>
- <span data-ttu-id="a124d-150">不支持 `$top`。</span><span class="sxs-lookup"><span data-stu-id="a124d-150">`$top` is not supported.</span></span>
- <span data-ttu-id="a124d-151">不支持 `$orderby`。</span><span class="sxs-lookup"><span data-stu-id="a124d-151">`$orderby` is not supported.</span></span>
- <span data-ttu-id="a124d-p114">如果使用的是 `$select` 查询参数，则该参数表示客户倾向于仅跟踪 `$select` 语句中指定的属性或关系的更改。如果未选中的属性发生更改，则属性已更改的资源将不会出现在后续请求之后的 delta 响应中。</span><span class="sxs-lookup"><span data-stu-id="a124d-p114">If a `$select` query parameter is used, the parameter indicates that the client prefers to only track changes on the properties or relationships specified in the `$select` statement. If a change occurs to a property that is not selected, the resource for which that property changed does not appear in the delta response after a subsequent request.</span></span>
- <span data-ttu-id="a124d-154">`$select` 还支持用户和组的 `manager` 和 `members` 导航属性。</span><span class="sxs-lookup"><span data-stu-id="a124d-154">`$select` also supports `manager` and `members` navigational property for users and groups respectively.</span></span> <span data-ttu-id="a124d-155">选择这些属性可以跟踪对用户管理器和组成员身份的更改。</span><span class="sxs-lookup"><span data-stu-id="a124d-155">Selecting those properties allows tracking of changes to user's manager and group memberships.</span></span>

- <span data-ttu-id="a124d-156">借助范围筛选器，可按对象 ID 跟踪一个或多个特定用户或组的更改。</span><span class="sxs-lookup"><span data-stu-id="a124d-156">Scoping filters allow you to track changes to one or more specific users or groups by object ID.</span></span> <span data-ttu-id="a124d-157">例如，以下请求会返回与查询筛选器中指定的 ID 相匹配的组的更改。</span><span class="sxs-lookup"><span data-stu-id="a124d-157">For example, the following request returns changes for the groups matching the IDs specified in the query filter.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
https://graph.microsoft.com/beta/groups/delta/?$filter=id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' or id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e'
```

## <a name="resource-representation-in-the-delta-query-response"></a><span data-ttu-id="a124d-158">delta 查询响应中的资源表示形式</span><span class="sxs-lookup"><span data-stu-id="a124d-158">Resource representation in the delta query response</span></span>

- <span data-ttu-id="a124d-159">在 delta 查询响应中，使用标准表示形式表示受支持资源的新建实例。</span><span class="sxs-lookup"><span data-stu-id="a124d-159">Newly created instances of a supported resource are represented in the delta query response using their standard representation.</span></span>

- <span data-ttu-id="a124d-160">更新实例由它们的 **id** 表示，*至少*具有已更新的属性，但可能也包含其他属性。</span><span class="sxs-lookup"><span data-stu-id="a124d-160">Updated instances are represented by their **id** with *at least* the properties that have been updated, but additional properties may be included.</span></span>

- <span data-ttu-id="a124d-p117">用户和组的关系表示为对标准资源表示形式的注释。这些注释使用格式 `propertyName@delta`。注释包含在初始 delta 查询请求的响应内。</span><span class="sxs-lookup"><span data-stu-id="a124d-p117">Relationships on users and groups are represented as annotations on the standard resource representation. These annotations use the format `propertyName@delta`. The annotations are included in the response of the initial delta query request.</span></span>

<span data-ttu-id="a124d-164">删除的实例使用其 **id** 和 `@removed` 对象表示。</span><span class="sxs-lookup"><span data-stu-id="a124d-164">Removed instances are represented by their **id** and an `@removed` object.</span></span> <span data-ttu-id="a124d-165">`@removed` 对象可能包含有关为何删除该实例的其他信息。</span><span class="sxs-lookup"><span data-stu-id="a124d-165">The `@removed` object may include additional information about why the instance was removed.</span></span> <span data-ttu-id="a124d-166">例如，"@removed": {"reason": "changed"}。</span><span class="sxs-lookup"><span data-stu-id="a124d-166">For example,  "@removed": {"reason": "changed"}.</span></span>

<span data-ttu-id="a124d-167">可能的 @removed 原因可以是*已更改*或*已删除*。</span><span class="sxs-lookup"><span data-stu-id="a124d-167">Possible @removed reasons can be *changed* or *deleted*.</span></span>

- <span data-ttu-id="a124d-168">*已更改*表示该项已被删除，可以从 [deletedItems](/graph/api/resources/directory) 恢复。</span><span class="sxs-lookup"><span data-stu-id="a124d-168">*Changed* indicates the item was deleted and can be restored from [deletedItems](/graph/api/resources/directory).</span></span>

- <span data-ttu-id="a124d-169">*已删除*表示该项已被删除，无法恢复。</span><span class="sxs-lookup"><span data-stu-id="a124d-169">*Deleted* indicates the item is deleted and cannot be restored.</span></span>

<span data-ttu-id="a124d-p119">`@removed` 对象可以在初始 delta 查询响应和跟踪的 (deltaLink) 响应中返回。使用 delta 查询请求的客户端应能够处理响应中的这些对象。</span><span class="sxs-lookup"><span data-stu-id="a124d-p119">The `@removed` object can be returned in the initial delta query response and in tracked (deltaLink) responses. Clients using delta query requests should be designed to handle these objects in the responses.</span></span>

><span data-ttu-id="a124d-172">**注意：** 在响应中可能会多次包含一个实体，前提是多次在特定情况下更改了该实体。</span><span class="sxs-lookup"><span data-stu-id="a124d-172">**Note:** It's possible that a single entity will be contained multiple times in the response, if that entity was changed multiple times and under certain conditions.</span></span> <span data-ttu-id="a124d-173">增量查询可以使应用程序列出所有更改，但不能确保实体在单个响应中是统一的。</span><span class="sxs-lookup"><span data-stu-id="a124d-173">Delta queries enable your application to list all the changes, but can't ensure that entities are unified in a single response.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="a124d-174">支持的资源</span><span class="sxs-lookup"><span data-stu-id="a124d-174">Supported resources</span></span>

<span data-ttu-id="a124d-175">目前，以下资源支持 delta 查询。</span><span class="sxs-lookup"><span data-stu-id="a124d-175">Delta query is currently supported for the following resources.</span></span>

| <span data-ttu-id="a124d-176">**资源集合**</span><span class="sxs-lookup"><span data-stu-id="a124d-176">**Resource collection**</span></span>                                        | <span data-ttu-id="a124d-177">**API**</span><span class="sxs-lookup"><span data-stu-id="a124d-177">**API**</span></span>                                                                                                                                                                                          |
|:---------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a124d-178">应用程序</span><span class="sxs-lookup"><span data-stu-id="a124d-178">Applications</span></span>                                                   | <span data-ttu-id="a124d-179">[application](/graph/api/resources/application) 资源的 [delta](/graph/api/application-delta) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-179">[delta](/graph/api/application-delta) function of the [application](/graph/api/resources/application) resource</span></span>                                                                                   |
| <span data-ttu-id="a124d-180">管理单元（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-180">Administrative units (preview)</span></span>                                 | <span data-ttu-id="a124d-181">[administrativeUnit](/graph/api/resources/administrativeunit) 资源的 [delta](/graph/api/administrativeunit-delta) 函数（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-181">[delta](/graph/api/administrativeunit-delta) function of the [administrativeUnit](/graph/api/resources/administrativeunit) resource (preview)</span></span>                                                    |
| <span data-ttu-id="a124d-182">频道中的聊天消息（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-182">Chat messages in a channel (preview)</span></span>                           | <span data-ttu-id="a124d-183">[chatMessage](/graph/api/resources/chatmessage) 的 [delta](/graph/api/chatmessage-delta) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-183">[delta](/graph/api/chatmessage-delta) function of the [chatMessage](/graph/api/resources/chatmessage)</span></span>                                                                                            |
| <span data-ttu-id="a124d-184">类（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-184">Classes (preview)</span></span>                                              | <span data-ttu-id="a124d-185">[educationClass](/graph/api/resources/educationclass) 资源的 [delta](/graph/api/educationclass-delta) 函数（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-185">[delta](/graph/api/educationclass-delta) function of the [educationClass](/graph/api/resources/educationclass) resource (preview)</span></span>                                                                |
| <span data-ttu-id="a124d-186">目录对象（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-186">Directory objects (preview)</span></span>                                    | <span data-ttu-id="a124d-187">[directoryObject](/graph/api/resources/directoryobject) 资源的 [delta](/graph/api/directoryobject-delta) 函数（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-187">[delta](/graph/api/directoryobject-delta) function of the [directoryObject](/graph/api/resources/directoryobject) resource (preview)</span></span>                                                             |
| <span data-ttu-id="a124d-188">目录角色</span><span class="sxs-lookup"><span data-stu-id="a124d-188">Directory roles</span></span>                                                | <span data-ttu-id="a124d-189">[directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0) 资源的 [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-189">[delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) function of the [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0) resource</span></span>                                     |
| <span data-ttu-id="a124d-190">驱动器项目\*</span><span class="sxs-lookup"><span data-stu-id="a124d-190">Drive items\*</span></span>                                                  | <span data-ttu-id="a124d-191">[driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) 资源的 [delta](/graph/api/driveitem-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-191">[delta](/graph/api/driveitem-delta?view=graph-rest-1.0) function of the [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) resource</span></span>                                                 |
| <span data-ttu-id="a124d-192">教育用户（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-192">Education users (preview)</span></span>                                      | <span data-ttu-id="a124d-193">[educationUser](/graph/api/resources/educationuser) 资源的 [delta](/graph/api/educationuser-delta) 函数（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-193">[delta](/graph/api/educationuser-delta) function of the [educationUser](/graph/api/resources/educationuser) resource (preview)</span></span>                                                                   |
| <span data-ttu-id="a124d-194">主日历的日历视图（日期范围）中的事件</span><span class="sxs-lookup"><span data-stu-id="a124d-194">Events in a calendar view (date range) of the primary calendar</span></span> | <span data-ttu-id="a124d-195">[事件](/graph/api/resources/event?view=graph-rest-1.0)资源的 [delta](/graph/api/event-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-195">[delta](/graph/api/event-delta?view=graph-rest-1.0) function of the [event](/graph/api/resources/event?view=graph-rest-1.0) resource</span></span>                                                             |
| <span data-ttu-id="a124d-196">组</span><span class="sxs-lookup"><span data-stu-id="a124d-196">Groups</span></span>                                                         | <span data-ttu-id="a124d-197">[组](/graph/api/resources/group?view=graph-rest-1.0)资源的 [delta](/graph/api/group-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-197">[delta](/graph/api/group-delta?view=graph-rest-1.0) function of the [group](/graph/api/resources/group?view=graph-rest-1.0) resource</span></span>                                                             |
| <span data-ttu-id="a124d-198">邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="a124d-198">Mail folders</span></span>                                                   | <span data-ttu-id="a124d-199">[邮件文件夹](/graph/api/resources/mailfolder?view=graph-rest-1.0)资源的 [delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-199">[delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) function of the [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) resource</span></span>                                              |
| <span data-ttu-id="a124d-200">文件夹中的邮件</span><span class="sxs-lookup"><span data-stu-id="a124d-200">Messages in a folder</span></span>                                           | <span data-ttu-id="a124d-201">[邮件](/graph/api/resources/message?view=graph-rest-1.0)资源的 [delta](/graph/api/message-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-201">[delta](/graph/api/message-delta?view=graph-rest-1.0) function of the [message](/graph/api/resources/message?view=graph-rest-1.0) resource</span></span>                                                       |
| <span data-ttu-id="a124d-202">组织联系人</span><span class="sxs-lookup"><span data-stu-id="a124d-202">Organizational contacts</span></span>                                        | <span data-ttu-id="a124d-203">[orgContact](/graph/api/resources/orgcontact?view=graph-rest-1.0) 资源的 [delta](/graph/api/orgcontact-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-203">[delta](/graph/api/orgcontact-delta?view=graph-rest-1.0) function of the [orgContact](/graph/api/resources/orgcontact?view=graph-rest-1.0) resource</span></span>                                              |
| <span data-ttu-id="a124d-204">OAuth2PermissionGrants（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-204">OAuth2PermissionGrants (preview)</span></span>                               | <span data-ttu-id="a124d-205">[oauth2permissiongrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta) 资源的 [delta](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta) 函数（预览）</span><span class="sxs-lookup"><span data-stu-id="a124d-205">[delta](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta) function of the [oauth2permissiongrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta) resource (preview)</span></span> |
| <span data-ttu-id="a124d-206">私人联系人文件夹</span><span class="sxs-lookup"><span data-stu-id="a124d-206">Personal contact folders</span></span>                                       | <span data-ttu-id="a124d-207">[联系人文件夹](/graph/api/resources/contactfolder?view=graph-rest-1.0)资源的 [delta](/graph/api/contactfolder-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-207">[delta](/graph/api/contactfolder-delta?view=graph-rest-1.0) function of the [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) resource</span></span>                                     |
| <span data-ttu-id="a124d-208">文件夹中的私人联系人</span><span class="sxs-lookup"><span data-stu-id="a124d-208">Personal contacts in a folder</span></span>                                  | <span data-ttu-id="a124d-209">[contact](/graph/api/resources/contact?view=graph-rest-1.0) 资源的 [delta](/graph/api/contact-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-209">[delta](/graph/api/contact-delta?view=graph-rest-1.0) function of the [contact](/graph/api/resources/contact?view=graph-rest-1.0) resource</span></span>                                                       |
| <span data-ttu-id="a124d-210">Planner 项目\*\*（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-210">Planner items\*\* (preview)</span></span>                                    | <span data-ttu-id="a124d-211">[plannerUser](/graph/api/resources/planneruser) 资源所有段的 [delta](/graph/api/planneruser-list-delta) 函数（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-211">[delta](/graph/api/planneruser-list-delta) function of the all segment of [plannerUser](/graph/api/resources/planneruser) resource (preview)</span></span>                                                     |
| <span data-ttu-id="a124d-212">学校（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-212">Schools (preview)</span></span>                                              | <span data-ttu-id="a124d-213">[educationSchool](/graph/api/resources/educationschool) 资源的 [delta](/graph/api/educationschool-delta) 函数（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-213">[delta](/graph/api/educationschool-delta) function of the [educationSchool](/graph/api/resources/educationschool) resource (preview)</span></span>                                                             |
| <span data-ttu-id="a124d-214">服务主体（预览版）</span><span class="sxs-lookup"><span data-stu-id="a124d-214">Service principals (preview)</span></span>                                   | <span data-ttu-id="a124d-215">[servicePrincipal](/graph/api/resources/serviceprincipal) 资源（预览版）的 [delta](/graph/api/serviceprincipal-delta) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-215">[delta](/graph/api/serviceprincipal-delta) function of the [servicePrincipal](/graph/api/resources/serviceprincipal) resource (preview)</span></span>                                                          |
| <span data-ttu-id="a124d-216">用户</span><span class="sxs-lookup"><span data-stu-id="a124d-216">Users</span></span>                                                          | <span data-ttu-id="a124d-217">[用户](/graph/api/resources/user?view=graph-rest-1.0)资源的 [delta](/graph/api/user-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="a124d-217">[delta](/graph/api/user-delta?view=graph-rest-1.0) function of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource</span></span>                                                                |


> <span data-ttu-id="a124d-218">\* OneDrive 资源的使用模式与其他支持资源类似，仅存在一些小的语法差异。</span><span class="sxs-lookup"><span data-stu-id="a124d-218">\* The usage pattern for OneDrive resources is similar to the other supported resources with some minor syntax differences.</span></span> <span data-ttu-id="a124d-219">为了与其他资源类型保持一致，适用于驱动器的 delta 查询今后将进行更新。</span><span class="sxs-lookup"><span data-stu-id="a124d-219">Delta query for drives will be updated in the future to be consistent with other resource types.</span></span> <span data-ttu-id="a124d-220">若要详细了解现行语法，请参阅[跟踪驱动器更改](/graph/api/driveitem-delta?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="a124d-220">For more detail about the current syntax, see [Track changes for a drive](/graph/api/driveitem-delta?view=graph-rest-1.0).</span></span>

> <span data-ttu-id="a124d-221">\*\* Planner 资源的使用模式与其他支持资源类似，仅存在些许差异。</span><span class="sxs-lookup"><span data-stu-id="a124d-221">\*\* The usage pattern for Planner resources is similar to other supported resources with a few differences.</span></span>  <span data-ttu-id="a124d-222">有关详细信息，请参阅[跟踪 Planner 更改](/graph/api/planneruser-list-delta)。</span><span class="sxs-lookup"><span data-stu-id="a124d-222">For details, see [Track changes for Planner](/graph/api/planneruser-list-delta).</span></span>

## <a name="limitations"></a><span data-ttu-id="a124d-223">限制</span><span class="sxs-lookup"><span data-stu-id="a124d-223">Limitations</span></span>

### <a name="properties-stored-outside-of-the-main-data-store"></a><span data-ttu-id="a124d-224">在主数据存储外部存储的属性</span><span class="sxs-lookup"><span data-stu-id="a124d-224">Properties stored outside of the main data store</span></span>

<span data-ttu-id="a124d-225">某些资源包含一些存储在资源主数据存储外部的属性（例如，用户资源大部分存储在 Azure AD 系统中，而 **skills** 之类的一些属性存储在 SharePoint Online 中）。</span><span class="sxs-lookup"><span data-stu-id="a124d-225">Some resources contain properties that are stored outside of the main data store for the resource (for example, the user resource is mostly stored in the Azure AD system, while some properties, like **skills**, are stored in SharePoint Online).</span></span> <span data-ttu-id="a124d-226">目前，在更改跟踪中不支持这些属性；对其中一个属性所做的更改不会导致在增量查询响应中显示对象。</span><span class="sxs-lookup"><span data-stu-id="a124d-226">Currently, those properties are not supported as part of change tracking; a change to one of those properties will not result in an object showing up in the delta query response.</span></span> <span data-ttu-id="a124d-227">目前，仅在主数据存储中存储的属性会触发增量查询中的更改。</span><span class="sxs-lookup"><span data-stu-id="a124d-227">Currently, only the properties stored in the main data store trigger changes in the delta query.</span></span>

<span data-ttu-id="a124d-228">若要验证属性是否可在增量查询中使用，请尝试对资源集合执行常规 `GET` 操作，然后选择感兴趣的属性。</span><span class="sxs-lookup"><span data-stu-id="a124d-228">To verify that a property can be used in delta query, try to perform a regular `GET` operation on the resource collection, and select the property you're interested in.</span></span> <span data-ttu-id="a124d-229">例如，可尝试对用户集合使用 **skills** 属性。</span><span class="sxs-lookup"><span data-stu-id="a124d-229">For example, you can try the **skills** property on the users collection.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/?$select=skills
```

<span data-ttu-id="a124d-230">由于 **skills** 属性存储在 Azure AD 外部，因此响应如下。</span><span class="sxs-lookup"><span data-stu-id="a124d-230">Because the **skills** property is stored outside of Azure AD, the following is the response.</span></span>

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

<span data-ttu-id="a124d-231">据此可得知，**user** 资源的增量查询不支持 **skills** 属性。</span><span class="sxs-lookup"><span data-stu-id="a124d-231">This tells you that the **skills** property is not supported for delta query on the **user** resource.</span></span>

### <a name="navigation-properties"></a><span data-ttu-id="a124d-232">导航属性</span><span class="sxs-lookup"><span data-stu-id="a124d-232">Navigation properties</span></span>

<span data-ttu-id="a124d-233">不支持导航属性。</span><span class="sxs-lookup"><span data-stu-id="a124d-233">Navigation properties are not supported.</span></span> <span data-ttu-id="a124d-234">例如，不能跟踪对用户集合所做的更改，这些更改将包含对用户 **photo** 属性所做的更改；**photo** 是一个存储在用户实体之外的导航属性，且对其进行的更改不会导致增量响应中包含用户对象。</span><span class="sxs-lookup"><span data-stu-id="a124d-234">For example, you cannot track changes to the users collection that would include changes to their **photo** property; **photo** is a navigation property stored outside of the user entity, and changes to it do not cause the user object to be included in the delta response.</span></span>

### <a name="processing-delays"></a><span data-ttu-id="a124d-235">处理延迟</span><span class="sxs-lookup"><span data-stu-id="a124d-235">Processing delays</span></span>

<span data-ttu-id="a124d-236">对资源实例进行更改（可通过应用界面或 API 进行）的时间与所做的更改反映在增量查询响应中的时间之间可能会出现不同的延迟。</span><span class="sxs-lookup"><span data-stu-id="a124d-236">Expect varying delays between the time a change is made to a resource instance, which can be through an app interface or API, and the time the tracked change is reflected in a delta query response.</span></span>

### <a name="national-clouds"></a><span data-ttu-id="a124d-237">国家云</span><span class="sxs-lookup"><span data-stu-id="a124d-237">National clouds</span></span>

<span data-ttu-id="a124d-238">增量查询仅适用于公共云和由世纪互联运营的 Microsoft Graph（中国）托管的客户。</span><span class="sxs-lookup"><span data-stu-id="a124d-238">Delta queries are available for customers hosted on the public cloud and Microsoft Graph China operated by 21Vianet only.</span></span>

### <a name="token-duration"></a><span data-ttu-id="a124d-239">令牌持续时间</span><span class="sxs-lookup"><span data-stu-id="a124d-239">Token duration</span></span>

<span data-ttu-id="a124d-240">增量令牌仅在客户端应用程序需要再次运行完整同步前的特定时间段内有效。</span><span class="sxs-lookup"><span data-stu-id="a124d-240">Delta tokens are only valid for a specific period before the client application needs to run a full synchronization again.</span></span> <span data-ttu-id="a124d-241">对于目录对象（**application**、 **administrativeUnit**、 **directoryObject**、 **directoryRole**、 **group**、 **orgContact**、 **oauth2permissiongrant**、 **servicePrincipal**和**user**），限制为7天。</span><span class="sxs-lookup"><span data-stu-id="a124d-241">For directory objects (**application**, **administrativeUnit**, **directoryObject**, **directoryRole**, **group**, **orgContact**, **oauth2permissiongrant**, **servicePrincipal**, and **user**), the limit is 7 days.</span></span> <span data-ttu-id="a124d-242">对于教育对象（**educationSchool**、 **educationUser**和**educationClass**），限制为7天。</span><span class="sxs-lookup"><span data-stu-id="a124d-242">For education objects (**educationSchool**, **educationUser**, and **educationClass**), the limit is 7 days.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a124d-243">先决条件</span><span class="sxs-lookup"><span data-stu-id="a124d-243">Prerequisites</span></span>

<span data-ttu-id="a124d-244">在对某个特定资源执行 delta 查询时也需要读取该资源所需的相同[权限](./permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a124d-244">The same [permissions](./permissions-reference.md) that are required to read a specific resource are also required to perform delta query on that resource.</span></span>

## <a name="delta-query-request-examples"></a><span data-ttu-id="a124d-245">delta 查询请求示例</span><span class="sxs-lookup"><span data-stu-id="a124d-245">Delta query request examples</span></span>

- [<span data-ttu-id="a124d-246">获取日历视图中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="a124d-246">Get incremental changes to events in a calendar view</span></span>](delta-query-events.md)
- [<span data-ttu-id="a124d-247">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="a124d-247">Get incremental changes to messages in a folder</span></span>](./delta-query-messages.md)
- [<span data-ttu-id="a124d-248">获取组的增量更改</span><span class="sxs-lookup"><span data-stu-id="a124d-248">Get incremental changes to groups</span></span>](./delta-query-groups.md)
- [<span data-ttu-id="a124d-249">获取用户的增量更改</span><span class="sxs-lookup"><span data-stu-id="a124d-249">Get incremental changes to users</span></span>](./delta-query-users.md)
