---
title: 使用增量查询跟踪 Microsoft Graph 数据更改
description: Delta 查询使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。Microsoft Graph 应用程序可以使用 delta 查询和本地数据存储高效地同步更改。
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: cceab6a803b403560c6a72831584c99202d65618
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231988"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a><span data-ttu-id="4076c-104">使用 delta 查询跟踪 Microsoft Graph 数据变更</span><span class="sxs-lookup"><span data-stu-id="4076c-104">Use delta query to track changes in Microsoft Graph data</span></span>

<span data-ttu-id="4076c-p102">Delta 查询使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。Microsoft Graph 应用程序可以使用 delta 查询和本地数据存储高效地同步更改。</span><span class="sxs-lookup"><span data-stu-id="4076c-p102">Delta query enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. Microsoft Graph applications can use delta query to efficiently synchronize changes with a local data store.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="4076c-107">教程：在 Microsoft Graph 上使用“更改通知”和“跟踪更改”</span><span class="sxs-lookup"><span data-stu-id="4076c-107">Tutorial: Use Change Notifications and Track Changes with Microsoft Graph</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a><span data-ttu-id="4076c-108">使用 delta 查询来跟踪资源集合的更改</span><span class="sxs-lookup"><span data-stu-id="4076c-108">Use delta query to track changes in a resource collection</span></span>

<span data-ttu-id="4076c-109">通常的调用模式如下：</span><span class="sxs-lookup"><span data-stu-id="4076c-109">The typical call pattern is as follows:</span></span>

1. <span data-ttu-id="4076c-110">应用程序首先对所需资源运行 delta 函数以调用 GET 请求。</span><span class="sxs-lookup"><span data-stu-id="4076c-110">The application begins by calling a GET request with the delta function on the desired resource.</span></span>
2. <span data-ttu-id="4076c-111">Microsoft Graph 发送一个包含已请求资源和[状态令牌](#state-tokens)的响应。</span><span class="sxs-lookup"><span data-stu-id="4076c-111">Microsoft Graph sends a response containing the requested resource and a [state token](#state-tokens).</span></span>

     <span data-ttu-id="4076c-p103">a.如果返回了 `nextLink` URL，则会话中可能存在要检索的其他数据页面。应用程序继续使用 `nextLink` URL 发出请求以检索所有页面中的数据，直到响应中返回 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="4076c-p103">a.  If a `nextLink` URL is returned, there may be additional pages of data to be retrieved in the session. The application continues making requests using the `nextLink` URL to retrieve all pages of data until a `deltaLink` URL is returned in the response.</span></span>

     <span data-ttu-id="4076c-p104">b.如果返回了 `deltaLink` URL，则未返回关于资源现有状态的更多数据。为了执行以后的请求，应用程序使用 `deltaLink` URL 了解资源更改。</span><span class="sxs-lookup"><span data-stu-id="4076c-p104">b.  If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the `deltaLink` URL to learn about changes to the resource.</span></span>

3. <span data-ttu-id="4076c-p105">当应用程序需要了解资源更改时，会使用步骤 2 中收到的 `deltaLink` URL 发出新请求。*可能* 在完成步骤 2 或应用程序检查更改时立即发出此请求。</span><span class="sxs-lookup"><span data-stu-id="4076c-p105">When the application needs to learn about changes to the resource, it makes a new request using the `deltaLink` URL received in step 2. This request *may* be made immediately after completing step 2 or when the application checks for changes.</span></span>
4. <span data-ttu-id="4076c-120">Microsoft Graph 返回响应（`nextLink` URL 或 `deltaLink` URL），其中描述了自上一个请求以来的资源变更。</span><span class="sxs-lookup"><span data-stu-id="4076c-120">Microsoft Graph returns a response describing changes to the resource since the previous request, and either a `nextLink` URL or a `deltaLink` URL.</span></span>

><span data-ttu-id="4076c-121">**注意：** Azure Active Directory 中存储的资源（如用户和组）支持“从现在开始同步”方案。</span><span class="sxs-lookup"><span data-stu-id="4076c-121">**Note:** Resources stored in Azure Active Directory (such as users and groups) support "sync from now" scenarios.</span></span> <span data-ttu-id="4076c-122">这样一来，便可以跳过第 1 步和第 2 步（如果不想检索资源完整状态的话），并改为请求获取最新 `deltaLink`。</span><span class="sxs-lookup"><span data-stu-id="4076c-122">This allows you to skip steps 1 and 2 (if you're not interested in retrieving the full state of the resource) and ask for the latest `deltaLink` instead.</span></span> <span data-ttu-id="4076c-123">将 `$deltaToken=latest` 追加到 `delta` 函数中，这样响应就会包含 `deltaLink`，而不包含资源数据。</span><span class="sxs-lookup"><span data-stu-id="4076c-123">Append `$deltaToken=latest` to the `delta` function and the response will contain a `deltaLink` and no resource data.</span></span> <span data-ttu-id="4076c-124">OneDrive 和 SharePoint 中的资源也支持此功能。</span><span class="sxs-lookup"><span data-stu-id="4076c-124">Resources in OneDrive and SharePoint also support this feature.</span></span> <span data-ttu-id="4076c-125">有关 OneDrive 和 SharePoint 中的资源，请改为附加 `token=latest` 。</span><span class="sxs-lookup"><span data-stu-id="4076c-125">For resources in OneDrive and SharePoint, append `token=latest` instead.</span></span>

><span data-ttu-id="4076c-126">**注意：** 引用增量查询函数的方式通常是将 `/delta` 附加到资源名称。</span><span class="sxs-lookup"><span data-stu-id="4076c-126">**Note:** The delta query function is generally referred to by appending `/delta` to the resource name.</span></span> <span data-ttu-id="4076c-127">但是，`/delta` 是在 Microsoft Graph SDK 生成的请求中显示的完全限定名称 `/microsoft.graph.delta` 的快捷方式。</span><span class="sxs-lookup"><span data-stu-id="4076c-127">However, `/delta` is a shortcut for the fully qualified name `/microsoft.graph.delta` that you see in requests generated by the Microsoft Graph SDKs.</span></span>

><span data-ttu-id="4076c-128">**注意** 初始请求发到 delta 查询函数后（无 delta 或跳过标记），会返回集合中现有的资源。</span><span class="sxs-lookup"><span data-stu-id="4076c-128">**Note:** The initial request to the delta query function (no delta or skip token) will return the resources that currently exist in the collection.</span></span> <span data-ttu-id="4076c-129">初始 delta 查询之前创建并已删除的资源不会返回。</span><span class="sxs-lookup"><span data-stu-id="4076c-129">Resources that have been created and deleted prior to the initial delta query won't be returned.</span></span> <span data-ttu-id="4076c-130">初始请求前进行的更新在返回的资源上按其最新状态进行汇总。</span><span class="sxs-lookup"><span data-stu-id="4076c-130">Updates made before the initial request are summarized on the resource returned as its latest state.</span></span>

### <a name="state-tokens"></a><span data-ttu-id="4076c-131">状态令牌</span><span class="sxs-lookup"><span data-stu-id="4076c-131">State tokens</span></span>

<span data-ttu-id="4076c-p109">增量查询 GET 响应中始终返回 `nextLink` 或 `deltaLink` 响应头中指定的 URL。`nextLink` URL 包含的是 _skipToken_，`deltaLink` URL 包含的是 _deltaToken_。</span><span class="sxs-lookup"><span data-stu-id="4076c-p109">A delta query GET response always includes a URL specified in a `nextLink` or `deltaLink` response header. The `nextLink` URL includes a _skipToken_, and a `deltaLink` URL includes a _deltaToken_.</span></span>

<span data-ttu-id="4076c-p110">这些令牌对客户端不透明。以下是需要了解的详细信息：</span><span class="sxs-lookup"><span data-stu-id="4076c-p110">These tokens are opaque to the client. The following details are what you need to know about them:</span></span>

- <span data-ttu-id="4076c-136">每个令牌都反映状态，并表示一轮更改跟踪中的响应快照。</span><span class="sxs-lookup"><span data-stu-id="4076c-136">Each token reflects the state and represents a snapshot of the resource in that round of change tracking.</span></span>

- <span data-ttu-id="4076c-p111">状态令牌还会进行编码，并包括初始 delta 查询请求中指定的其他查询参数（如 `$select`）。因此，不需要在后续 delta 查询请求中重复这些操作。</span><span class="sxs-lookup"><span data-stu-id="4076c-p111">The state tokens also encode and include other query parameters (such as `$select`) specified in the initial delta query request. Therefore, it's not required to repeat them in subsequent delta query requests.</span></span>

- <span data-ttu-id="4076c-139">执行增量查询时，可以将 `nextLink` 或 `deltaLink` URL 复制并应用到下一个 **delta** 函数调用，无需检查 URL 的内容（包括其状态令牌）。</span><span class="sxs-lookup"><span data-stu-id="4076c-139">When carrying out delta query, you can copy and apply the `nextLink` or `deltaLink` URL to the next **delta** function call without having to inspect the contents of the URL, including its state token.</span></span>

### <a name="optional-query-parameters"></a><span data-ttu-id="4076c-140">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4076c-140">Optional query parameters</span></span>

<span data-ttu-id="4076c-p112">如果客户使用查询参数，则它必须在初始请求中指定。Microsoft Graph 自动将指定参数编码为响应中提供的 `nextLink` 或 `deltaLink`。调用应用程序只需预先指定查询参数一次。Microsoft Graph 将为所有后续请求自动添加指定参数。</span><span class="sxs-lookup"><span data-stu-id="4076c-p112">If a client uses a query parameter, it must be specified in the initial request. Microsoft Graph automatically encodes the specified parameter into the `nextLink` or `deltaLink` provided in the response. The calling application only needs to specify the query parameters once upfront. Microsoft Graph adds the specified parameters automatically for all subsequent requests.</span></span>

<span data-ttu-id="4076c-145">请注意以下可选查询参数的常规有限支持：</span><span class="sxs-lookup"><span data-stu-id="4076c-145">Note the general limited support of the following optional query parameters:</span></span>

- `$orderby`

    <span data-ttu-id="4076c-146">不要假设增量查询返回特定响应顺序。</span><span class="sxs-lookup"><span data-stu-id="4076c-146">Do not assume a specific sequence of the responses returned from a delta query.</span></span> <span data-ttu-id="4076c-147">假设同一项目可以显示在 `nextLink` 序列的任意位置，并以合并逻辑进行处理。</span><span class="sxs-lookup"><span data-stu-id="4076c-147">Assume that the same item can show up anywhere in the `nextLink` sequence and handle that in your merge logic.</span></span>
- `$top`

    <span data-ttu-id="4076c-148">每页中的对象数量可能因资源类型和资源更改类型而异。</span><span class="sxs-lookup"><span data-stu-id="4076c-148">The number of objects in each page can vary depending on the resource type and the type of changes made to the resource.</span></span>

<span data-ttu-id="4076c-149">对于[消息](/graph/api/resources/message?view=graph-rest-1.0)资源，请参阅[增量查询中的查询参数支持](delta-query-messages.md#use-query-parameters-in-a-delta-query-for-messages)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4076c-149">For the [message](/graph/api/resources/message?view=graph-rest-1.0) resource, see details for [query parameters support in a delta query](delta-query-messages.md#use-query-parameters-in-a-delta-query-for-messages).</span></span>

<span data-ttu-id="4076c-150">对于[用户](/graph/api/resources/user?view=graph-rest-1.0)和[组](/graph/api/resources/group?view=graph-rest-1.0)资源，在使用某些查询参数时受到限制：</span><span class="sxs-lookup"><span data-stu-id="4076c-150">For the [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0) resources, there are restrictions on using some query parameters:</span></span>

- <span data-ttu-id="4076c-151">不支持 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="4076c-151">`$expand` is not supported.</span></span>
- <span data-ttu-id="4076c-152">不支持 `$top`。</span><span class="sxs-lookup"><span data-stu-id="4076c-152">`$top` is not supported.</span></span>
- <span data-ttu-id="4076c-153">不支持 `$orderby`。</span><span class="sxs-lookup"><span data-stu-id="4076c-153">`$orderby` is not supported.</span></span>
- <span data-ttu-id="4076c-p114">如果使用的是 `$select` 查询参数，则该参数表示客户倾向于仅跟踪 `$select` 语句中指定的属性或关系的更改。如果未选中的属性发生更改，则属性已更改的资源将不会出现在后续请求之后的 delta 响应中。</span><span class="sxs-lookup"><span data-stu-id="4076c-p114">If a `$select` query parameter is used, the parameter indicates that the client prefers to only track changes on the properties or relationships specified in the `$select` statement. If a change occurs to a property that is not selected, the resource for which that property changed does not appear in the delta response after a subsequent request.</span></span>
- <span data-ttu-id="4076c-156">`$select` 还支持用户和组的 `manager` 和 `members` 导航属性。</span><span class="sxs-lookup"><span data-stu-id="4076c-156">`$select` also supports `manager` and `members` navigational property for users and groups respectively.</span></span> <span data-ttu-id="4076c-157">选择这些属性可以跟踪对用户管理器和组成员身份的更改。</span><span class="sxs-lookup"><span data-stu-id="4076c-157">Selecting those properties allows tracking of changes to user's manager and group memberships.</span></span>

- <span data-ttu-id="4076c-p116">使用范围筛选器可以按对象 ID 跟踪对一个或多个特定用户或组所做的更改。例如，以下请求返回与查询筛选器中指定的 ID 匹配的组所做的更改。</span><span class="sxs-lookup"><span data-stu-id="4076c-p116">Scoping filters allow you to track changes to one or more specific users or groups by object ID. For example, the following request returns changes for the groups matching the IDs specified in the query filter.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
https://graph.microsoft.com/beta/groups/delta/?$filter=id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' or id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e'
```

## <a name="resource-representation-in-the-delta-query-response"></a><span data-ttu-id="4076c-160">delta 查询响应中的资源表示形式</span><span class="sxs-lookup"><span data-stu-id="4076c-160">Resource representation in the delta query response</span></span>

- <span data-ttu-id="4076c-161">在 delta 查询响应中，使用标准表示形式表示受支持资源的新建实例。</span><span class="sxs-lookup"><span data-stu-id="4076c-161">Newly created instances of a supported resource are represented in the delta query response using their standard representation.</span></span>

- <span data-ttu-id="4076c-162">更新实例由它们的 **id** 表示，*至少* 具有已更新的属性，但可能也包含其他属性。</span><span class="sxs-lookup"><span data-stu-id="4076c-162">Updated instances are represented by their **id** with *at least* the properties that have been updated, but additional properties may be included.</span></span>

- <span data-ttu-id="4076c-p117">用户和组的关系表示为对标准资源表示形式的注释。这些注释使用格式 `propertyName@delta`。注释包含在初始 delta 查询请求的响应内。</span><span class="sxs-lookup"><span data-stu-id="4076c-p117">Relationships on users and groups are represented as annotations on the standard resource representation. These annotations use the format `propertyName@delta`. The annotations are included in the response of the initial delta query request.</span></span>

<span data-ttu-id="4076c-p118">删除的实例使用其 **id** 和 `@removed` 对象表示。`@removed` 对象可能包含有关为何删除该实例的其他信息。例如，"@removed": {"reason": “changed”}。</span><span class="sxs-lookup"><span data-stu-id="4076c-p118">Removed instances are represented by their **id** and an `@removed` object. The `@removed` object may include additional information about why the instance was removed. For example,  "@removed": {"reason": "changed"}.</span></span>

<span data-ttu-id="4076c-169">可能的 @removed 原因可以是 *已更改* 或 *已删除*。</span><span class="sxs-lookup"><span data-stu-id="4076c-169">Possible @removed reasons can be *changed* or *deleted*.</span></span>

- <span data-ttu-id="4076c-170">*已更改* 表示该项已被删除，可以从 [deletedItems](/graph/api/resources/directory) 恢复。</span><span class="sxs-lookup"><span data-stu-id="4076c-170">*Changed* indicates the item was deleted and can be restored from [deletedItems](/graph/api/resources/directory).</span></span>

- <span data-ttu-id="4076c-171">*已删除* 表示该项已被删除，无法恢复。</span><span class="sxs-lookup"><span data-stu-id="4076c-171">*Deleted* indicates the item is deleted and cannot be restored.</span></span>

<span data-ttu-id="4076c-p119">`@removed` 对象可以在初始 delta 查询响应和跟踪的 (deltaLink) 响应中返回。使用 delta 查询请求的客户端应能够处理响应中的这些对象。</span><span class="sxs-lookup"><span data-stu-id="4076c-p119">The `@removed` object can be returned in the initial delta query response and in tracked (deltaLink) responses. Clients using delta query requests should be designed to handle these objects in the responses.</span></span>

><span data-ttu-id="4076c-174">**注意：** 在响应中可能会多次包含一个实体，前提是多次在特定情况下更改了该实体。</span><span class="sxs-lookup"><span data-stu-id="4076c-174">**Note:** It's possible that a single entity will be contained multiple times in the response, if that entity was changed multiple times and under certain conditions.</span></span> <span data-ttu-id="4076c-175">增量查询可以使应用程序列出所有更改，但不能确保实体在单个响应中是统一的。</span><span class="sxs-lookup"><span data-stu-id="4076c-175">Delta queries enable your application to list all the changes, but can't ensure that entities are unified in a single response.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="4076c-176">支持的资源</span><span class="sxs-lookup"><span data-stu-id="4076c-176">Supported resources</span></span>

<span data-ttu-id="4076c-177">目前，以下资源支持 delta 查询。</span><span class="sxs-lookup"><span data-stu-id="4076c-177">Delta query is currently supported for the following resources.</span></span> <span data-ttu-id="4076c-178">请注意，v1.0 中可用的某些资源的相应 **delta** 函数仍处于预览状态，如下所示。</span><span class="sxs-lookup"><span data-stu-id="4076c-178">Note that some resources which are available in v1.0 have their corresponding **delta** functions still in preview status, as indicated.</span></span>

| <span data-ttu-id="4076c-179">**资源集合**</span><span class="sxs-lookup"><span data-stu-id="4076c-179">**Resource collection**</span></span>                                        | <span data-ttu-id="4076c-180">**API**</span><span class="sxs-lookup"><span data-stu-id="4076c-180">**API**</span></span>                                                                                                                                                      |
| :------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4076c-181">应用程序</span><span class="sxs-lookup"><span data-stu-id="4076c-181">Applications</span></span>                                                   | <span data-ttu-id="4076c-182">[application](/graph/api/resources/application) 资源的 [delta](/graph/api/application-delta) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-182">[delta](/graph/api/application-delta) function of the [application](/graph/api/resources/application) resource</span></span>                                               |
| <span data-ttu-id="4076c-183">管理单元（预览版）</span><span class="sxs-lookup"><span data-stu-id="4076c-183">Administrative units (preview)</span></span>                                 | <span data-ttu-id="4076c-184">[administrativeUnit](/graph/api/resources/administrativeunit) 资源的 [delta](/graph/api/administrativeunit-delta) 函数（预览版）</span><span class="sxs-lookup"><span data-stu-id="4076c-184">[delta](/graph/api/administrativeunit-delta) function (preview) of the [administrativeUnit](/graph/api/resources/administrativeunit) resource</span></span>                |
| <span data-ttu-id="4076c-185">频道中的聊天消息</span><span class="sxs-lookup"><span data-stu-id="4076c-185">Chat messages in a channel</span></span>                                     | <span data-ttu-id="4076c-186">[chatMessage](/graph/api/resources/chatmessage) 的 [delta](/graph/api/chatmessage-delta) 函数（预览版）</span><span class="sxs-lookup"><span data-stu-id="4076c-186">[delta](/graph/api/chatmessage-delta) function (preview) of the [chatMessage](/graph/api/resources/chatmessage)</span></span>                                              |
| <span data-ttu-id="4076c-187">目录对象</span><span class="sxs-lookup"><span data-stu-id="4076c-187">Directory objects</span></span>                                              | <span data-ttu-id="4076c-188">[directoryObject](/graph/api/resources/directoryobject) 资源的 [delta](/graph/api/directoryobject-delta) 函数（预览版）</span><span class="sxs-lookup"><span data-stu-id="4076c-188">[delta](/graph/api/directoryobject-delta) function (preview) of the [directoryObject](/graph/api/resources/directoryobject) resource</span></span>                         |
| <span data-ttu-id="4076c-189">目录角色</span><span class="sxs-lookup"><span data-stu-id="4076c-189">Directory roles</span></span>                                                | <span data-ttu-id="4076c-190">[directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0) 资源的 [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-190">[delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) function of the [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0) resource</span></span> |
| <span data-ttu-id="4076c-191">驱动器项目\*</span><span class="sxs-lookup"><span data-stu-id="4076c-191">Drive items\*</span></span>                                                  | <span data-ttu-id="4076c-192">[driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) 资源的 [delta](/graph/api/driveitem-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-192">[delta](/graph/api/driveitem-delta?view=graph-rest-1.0) function of the [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) resource</span></span>             |
| <span data-ttu-id="4076c-193">教育课堂</span><span class="sxs-lookup"><span data-stu-id="4076c-193">Education Classes</span></span>                                              | <span data-ttu-id="4076c-194">[educationClass](/graph/api/resources/educationclass) 资源的 [delta](/graph/api/educationclass-delta) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-194">[delta](/graph/api/educationclass-delta) function of the [educationClass](/graph/api/resources/educationclass) resource</span></span>                                      |
| <span data-ttu-id="4076c-195">教育用户</span><span class="sxs-lookup"><span data-stu-id="4076c-195">Education Users</span></span>                                                | <span data-ttu-id="4076c-196">[educationUser](/graph/api/resources/educationuser) 资源的 [delta](/graph/api/educationuser-delta) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-196">[delta](/graph/api/educationuser-delta) function of the [educationUser](/graph/api/resources/educationuser) resource</span></span>                                         |
| <span data-ttu-id="4076c-197">教育学校</span><span class="sxs-lookup"><span data-stu-id="4076c-197">Education Schools</span></span>                                              | <span data-ttu-id="4076c-198">[educationSchool](/graph/api/resources/educationschool) 资源的 [delta](/graph/api/educationschool-delta) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-198">[delta](/graph/api/educationschool-delta) function of the [educationSchool](/graph/api/resources/educationschool) resource</span></span>                                   |
| <span data-ttu-id="4076c-199">主日历的日历视图（日期范围）中的事件</span><span class="sxs-lookup"><span data-stu-id="4076c-199">Events in a calendar view (date range) of the primary calendar</span></span> | <span data-ttu-id="4076c-200">[事件](/graph/api/resources/event?view=graph-rest-1.0)资源的 [delta](/graph/api/event-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-200">[delta](/graph/api/event-delta?view=graph-rest-1.0) function of the [event](/graph/api/resources/event?view=graph-rest-1.0) resource</span></span>                         |
| <span data-ttu-id="4076c-201">组</span><span class="sxs-lookup"><span data-stu-id="4076c-201">Groups</span></span>                                                         | <span data-ttu-id="4076c-202">[组](/graph/api/resources/group?view=graph-rest-1.0)资源的 [delta](/graph/api/group-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-202">[delta](/graph/api/group-delta?view=graph-rest-1.0) function of the [group](/graph/api/resources/group?view=graph-rest-1.0) resource</span></span>                         |
| <span data-ttu-id="4076c-203">邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="4076c-203">Mail folders</span></span>                                                   | <span data-ttu-id="4076c-204">[邮件文件夹](/graph/api/resources/mailfolder?view=graph-rest-1.0)资源的 [delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-204">[delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) function of the [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) resource</span></span>          |
| <span data-ttu-id="4076c-205">文件夹中的邮件</span><span class="sxs-lookup"><span data-stu-id="4076c-205">Messages in a folder</span></span>                                           | <span data-ttu-id="4076c-206">[邮件](/graph/api/resources/message?view=graph-rest-1.0)资源的 [delta](/graph/api/message-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-206">[delta](/graph/api/message-delta?view=graph-rest-1.0) function of the [message](/graph/api/resources/message?view=graph-rest-1.0) resource</span></span>                   |
| <span data-ttu-id="4076c-207">组织联系人</span><span class="sxs-lookup"><span data-stu-id="4076c-207">Organizational contacts</span></span>                                        | <span data-ttu-id="4076c-208">[orgContact](/graph/api/resources/orgcontact?view=graph-rest-1.0) 资源的 [delta](/graph/api/orgcontact-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-208">[delta](/graph/api/orgcontact-delta?view=graph-rest-1.0) function of the [orgContact](/graph/api/resources/orgcontact?view=graph-rest-1.0) resource</span></span>          |
| <span data-ttu-id="4076c-209">OAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="4076c-209">OAuth2PermissionGrants</span></span>                                         | <span data-ttu-id="4076c-210">[oauth2permissiongrant](/graph/api/resources/oauth2permissiongrant) 资源的 [delta](/graph/api/oauth2permissiongrant-delta) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-210">[delta](/graph/api/oauth2permissiongrant-delta) function of the [oauth2permissiongrant](/graph/api/resources/oauth2permissiongrant) resource</span></span>                 |
| <span data-ttu-id="4076c-211">私人联系人文件夹</span><span class="sxs-lookup"><span data-stu-id="4076c-211">Personal contact folders</span></span>                                       | <span data-ttu-id="4076c-212">[联系人文件夹](/graph/api/resources/contactfolder?view=graph-rest-1.0)资源的 [delta](/graph/api/contactfolder-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-212">[delta](/graph/api/contactfolder-delta?view=graph-rest-1.0) function of the [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) resource</span></span> |
| <span data-ttu-id="4076c-213">文件夹中的私人联系人</span><span class="sxs-lookup"><span data-stu-id="4076c-213">Personal contacts in a folder</span></span>                                  | <span data-ttu-id="4076c-214">[contact](/graph/api/resources/contact?view=graph-rest-1.0) 资源的 [delta](/graph/api/contact-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-214">[delta](/graph/api/contact-delta?view=graph-rest-1.0) function of the [contact](/graph/api/resources/contact?view=graph-rest-1.0) resource</span></span>                   |
| <span data-ttu-id="4076c-215">Planner 项目\*\*（预览版）</span><span class="sxs-lookup"><span data-stu-id="4076c-215">Planner items\*\* (preview)</span></span>                                    | <span data-ttu-id="4076c-216">[plannerUser](/graph/api/resources/planneruser) 资源所有段的 [delta](/graph/api/planneruser-list-delta) 函数（预览版）</span><span class="sxs-lookup"><span data-stu-id="4076c-216">[delta](/graph/api/planneruser-list-delta) function (preview) of the all segment of [plannerUser](/graph/api/resources/planneruser) resource</span></span>                 |
| <span data-ttu-id="4076c-217">服务主体</span><span class="sxs-lookup"><span data-stu-id="4076c-217">Service principals</span></span>                                             | <span data-ttu-id="4076c-218">[servicePrincipal](/graph/api/resources/serviceprincipal) 资源的 [delta](/graph/api/serviceprincipal-delta) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-218">[delta](/graph/api/serviceprincipal-delta) function of the [servicePrincipal](/graph/api/resources/serviceprincipal) resource</span></span>                                |
| <span data-ttu-id="4076c-219">任务列表中的任务</span><span class="sxs-lookup"><span data-stu-id="4076c-219">Tasks in a task list</span></span>                                           | <span data-ttu-id="4076c-220">[todoTask](/graph/api/resources/todotask) 资源的 [delta](/graph/api/todotask-delta) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-220">[delta](/graph/api/todotask-delta) function of the [todoTask](/graph/api/resources/todotask) resource</span></span>                                                        |
| <span data-ttu-id="4076c-221">任务列表</span><span class="sxs-lookup"><span data-stu-id="4076c-221">Task lists</span></span>                                                     | <span data-ttu-id="4076c-222">[todoTaskList](/graph/api/resources/todotasklist) 资源的 [delta](/graph/api/todotasklist-delta) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-222">[delta](/graph/api/todotasklist-delta) function of the [todoTaskList](/graph/api/resources/todotasklist) resource</span></span>                                            |
| <span data-ttu-id="4076c-223">用户</span><span class="sxs-lookup"><span data-stu-id="4076c-223">Users</span></span>                                                          | <span data-ttu-id="4076c-224">[用户](/graph/api/resources/user?view=graph-rest-1.0)资源的 [delta](/graph/api/user-delta?view=graph-rest-1.0) 函数</span><span class="sxs-lookup"><span data-stu-id="4076c-224">[delta](/graph/api/user-delta?view=graph-rest-1.0) function of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource</span></span>                            |


> <span data-ttu-id="4076c-p122">\* OneDrive 资源的使用模式与其他支持资源类似，仅存在一些小的语法差异。为了与其他资源类型保持一致，适用于驱动器的 delta 查询今后将进行更新。若要详细了解现行语法，请参阅[跟踪驱动器更改](/graph/api/driveitem-delta?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="4076c-p122">\* The usage pattern for OneDrive resources is similar to the other supported resources with some minor syntax differences. Delta query for drives will be updated in the future to be consistent with other resource types. For more detail about the current syntax, see [Track changes for a drive](/graph/api/driveitem-delta?view=graph-rest-1.0).</span></span>

> <span data-ttu-id="4076c-228">\*\* Planner 资源的使用模式与其他支持资源类似，仅存在些许差异。</span><span class="sxs-lookup"><span data-stu-id="4076c-228">\*\* The usage pattern for Planner resources is similar to other supported resources with a few differences.</span></span>  <span data-ttu-id="4076c-229">有关详细信息，请参阅[跟踪 Planner 更改](/graph/api/planneruser-list-delta)。</span><span class="sxs-lookup"><span data-stu-id="4076c-229">For details, see [Track changes for Planner](/graph/api/planneruser-list-delta).</span></span>

## <a name="limitations"></a><span data-ttu-id="4076c-230">限制</span><span class="sxs-lookup"><span data-stu-id="4076c-230">Limitations</span></span>

### <a name="properties-stored-outside-of-the-main-data-store"></a><span data-ttu-id="4076c-231">在主数据存储外部存储的属性</span><span class="sxs-lookup"><span data-stu-id="4076c-231">Properties stored outside of the main data store</span></span>

<span data-ttu-id="4076c-232">某些资源包含一些存储在资源主数据存储外部的属性（例如，用户资源大部分存储在 Azure AD 系统中，而 **skills** 之类的一些属性存储在 SharePoint Online 中）。</span><span class="sxs-lookup"><span data-stu-id="4076c-232">Some resources contain properties that are stored outside of the main data store for the resource (for example, the user resource is mostly stored in the Azure AD system, while some properties, like **skills**, are stored in SharePoint Online).</span></span> <span data-ttu-id="4076c-233">目前，在更改跟踪中不支持这些属性；对其中一个属性所做的更改不会导致在增量查询响应中显示对象。</span><span class="sxs-lookup"><span data-stu-id="4076c-233">Currently, those properties are not supported as part of change tracking; a change to one of those properties will not result in an object showing up in the delta query response.</span></span> <span data-ttu-id="4076c-234">目前，仅在主数据存储中存储的属性会触发增量查询中的更改。</span><span class="sxs-lookup"><span data-stu-id="4076c-234">Currently, only the properties stored in the main data store trigger changes in the delta query.</span></span>

<span data-ttu-id="4076c-235">若要验证属性是否可在增量查询中使用，请尝试对资源集合执行常规 `GET` 操作，然后选择感兴趣的属性。</span><span class="sxs-lookup"><span data-stu-id="4076c-235">To verify that a property can be used in delta query, try to perform a regular `GET` operation on the resource collection, and select the property you're interested in.</span></span> <span data-ttu-id="4076c-236">例如，可尝试对用户集合使用 **skills** 属性。</span><span class="sxs-lookup"><span data-stu-id="4076c-236">For example, you can try the **skills** property on the users collection.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/?$select=skills
```

<span data-ttu-id="4076c-237">由于 **skills** 属性存储在 Azure AD 外部，因此响应如下。</span><span class="sxs-lookup"><span data-stu-id="4076c-237">Because the **skills** property is stored outside of Azure AD, the following is the response.</span></span>

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

<span data-ttu-id="4076c-238">据此可得知，**user** 资源的增量查询不支持 **skills** 属性。</span><span class="sxs-lookup"><span data-stu-id="4076c-238">This tells you that the **skills** property is not supported for delta query on the **user** resource.</span></span>

### <a name="navigation-properties"></a><span data-ttu-id="4076c-239">导航属性</span><span class="sxs-lookup"><span data-stu-id="4076c-239">Navigation properties</span></span>

<span data-ttu-id="4076c-240">不支持导航属性。</span><span class="sxs-lookup"><span data-stu-id="4076c-240">Navigation properties are not supported.</span></span> <span data-ttu-id="4076c-241">例如，不能跟踪对用户集合所做的更改，这些更改将包含对用户 **photo** 属性所做的更改；**photo** 是一个存储在用户实体之外的导航属性，且对其进行的更改不会导致增量响应中包含用户对象。</span><span class="sxs-lookup"><span data-stu-id="4076c-241">For example, you cannot track changes to the users collection that would include changes to their **photo** property; **photo** is a navigation property stored outside of the user entity, and changes to it do not cause the user object to be included in the delta response.</span></span>

### <a name="processing-delays"></a><span data-ttu-id="4076c-242">处理延迟</span><span class="sxs-lookup"><span data-stu-id="4076c-242">Processing delays</span></span>

<span data-ttu-id="4076c-243">对资源实例进行更改（可通过应用界面或 API 进行）的时间与所做的更改反映在增量查询响应中的时间之间可能会出现不同的延迟。</span><span class="sxs-lookup"><span data-stu-id="4076c-243">Expect varying delays between the time a change is made to a resource instance, which can be through an app interface or API, and the time the tracked change is reflected in a delta query response.</span></span>

### <a name="national-clouds"></a><span data-ttu-id="4076c-244">国家云</span><span class="sxs-lookup"><span data-stu-id="4076c-244">National clouds</span></span>

<span data-ttu-id="4076c-245">增量查询仅适用于公共云和由世纪互联运营的 Microsoft Graph（中国）托管的客户。</span><span class="sxs-lookup"><span data-stu-id="4076c-245">Delta queries are available for customers hosted on the public cloud and Microsoft Graph China operated by 21Vianet only.</span></span>

### <a name="replays"></a><span data-ttu-id="4076c-246">重新发送</span><span class="sxs-lookup"><span data-stu-id="4076c-246">Replays</span></span>

<span data-ttu-id="4076c-247">应用程序必须为重播做好准备，重新发送是在后续响应中出现相同更改时发生的。</span><span class="sxs-lookup"><span data-stu-id="4076c-247">Your application must be prepared for replays, which occur when the same change appears in subsequent responses.</span></span> <span data-ttu-id="4076c-248">虽然 delta 查询会尽力减少重新发送，但这种情况还是有可能发生。</span><span class="sxs-lookup"><span data-stu-id="4076c-248">While delta query makes a best effort to reduce replays, they are still possible.</span></span>

### <a name="synchronization-reset"></a><span data-ttu-id="4076c-249">同步重置</span><span class="sxs-lookup"><span data-stu-id="4076c-249">Synchronization reset</span></span>

<span data-ttu-id="4076c-250">delta 查询可以返回 `410 (gone)` 响应代码和一个 **Location** 标头，其中包含带空增量标记（与初始查询相同）的请求 URL。</span><span class="sxs-lookup"><span data-stu-id="4076c-250">Delta query can return a response code of `410 (gone)` and a **Location** header containing a request URL with an empty delta token (same as the initial query).</span></span> <span data-ttu-id="4076c-251">这表示应用程序必须在目标租户的完全同步的情况下重启。</span><span class="sxs-lookup"><span data-stu-id="4076c-251">This is an indication that the application must restart with a full synchronization of the target tenant.</span></span> <span data-ttu-id="4076c-252">发生这种情况的原因通常是由于目标租户的内部维护或迁移导致数据不一致。</span><span class="sxs-lookup"><span data-stu-id="4076c-252">This usually happens to prevent data inconsistency due to internal maintenance or migration of the target tenant.</span></span>

### <a name="token-duration"></a><span data-ttu-id="4076c-253">令牌持续时间</span><span class="sxs-lookup"><span data-stu-id="4076c-253">Token duration</span></span>

<span data-ttu-id="4076c-254">增量令牌仅在客户端应用程序需要再次运行完整同步前的特定时间段内有效。</span><span class="sxs-lookup"><span data-stu-id="4076c-254">Delta tokens are only valid for a specific period before the client application needs to run a full synchronization again.</span></span> <span data-ttu-id="4076c-255">目录对象（**应用程序**、**administrativeUnit**、**directoryObject**、**directoryRole**、**组**、**orgContact**、**oauth2permissiongrant**、**servicePrincipal** 和 **用户**）的时限为 7 天。</span><span class="sxs-lookup"><span data-stu-id="4076c-255">For directory objects (**application**, **administrativeUnit**, **directoryObject**, **directoryRole**, **group**, **orgContact**, **oauth2permissiongrant**, **servicePrincipal**, and **user**), the limit is 7 days.</span></span> <span data-ttu-id="4076c-256">教育对象（**educationSchool**、**educationUser** 和 **educationClass**）的时限为 7 天内。</span><span class="sxs-lookup"><span data-stu-id="4076c-256">For education objects (**educationSchool**, **educationUser**, and **educationClass**), the limit is 7 days.</span></span> <span data-ttu-id="4076c-257">Outlook 实体（**邮件**、**邮件文件夹**、**事件**、**联系人**、**联系人文件夹**、**待办事项** 和 **待办事项列表**）没有固定时间上限，取决于内部 delta 令牌缓存的大小。</span><span class="sxs-lookup"><span data-stu-id="4076c-257">For Outlook entities (**message**, **mailFolder**, **event**, **contact**, **contactFolder**, **todoTask**, and **todoTaskList**), the upper limit is not fixed; it's dependent on the size of the internal delta token cache.</span></span> <span data-ttu-id="4076c-258">因为缓存中不断添加新 delta 令牌，因此超过缓存容量后，旧 delta 令牌将被删除。</span><span class="sxs-lookup"><span data-stu-id="4076c-258">While new delta tokens are continuously added in the cache, after the cache capacity is exceeded, the older delta tokens are deleted.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4076c-259">必备条件</span><span class="sxs-lookup"><span data-stu-id="4076c-259">Prerequisites</span></span>

<span data-ttu-id="4076c-260">在对某个特定资源执行 delta 查询时也需要读取该资源所需的相同[权限](./permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4076c-260">The same [permissions](./permissions-reference.md) that are required to read a specific resource are also required to perform delta query on that resource.</span></span>

## <a name="delta-query-request-examples"></a><span data-ttu-id="4076c-261">delta 查询请求示例</span><span class="sxs-lookup"><span data-stu-id="4076c-261">Delta query request examples</span></span>

- [<span data-ttu-id="4076c-262">获取日历视图中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="4076c-262">Get incremental changes to events in a calendar view</span></span>](delta-query-events.md)
- [<span data-ttu-id="4076c-263">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="4076c-263">Get incremental changes to messages in a folder</span></span>](./delta-query-messages.md)
- [<span data-ttu-id="4076c-264">获取组的增量更改</span><span class="sxs-lookup"><span data-stu-id="4076c-264">Get incremental changes to groups</span></span>](./delta-query-groups.md)
- [<span data-ttu-id="4076c-265">获取用户的增量更改</span><span class="sxs-lookup"><span data-stu-id="4076c-265">Get incremental changes to users</span></span>](./delta-query-users.md)
