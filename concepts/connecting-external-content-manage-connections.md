---
title: 创建、更新和删除 Microsoft Graph 中的连接
description: 了解如何使用 Microsoft Graph 创建和管理员连接
localization_priority: Priority
author: mecampos
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 5020a8b56e6746e7c154af229113029c3f7731c0
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645741"
---
<!---<author of this doc: rsamai>--->

# <a name="create-update-and-delete-connections-in-the-microsoft-graph"></a><span data-ttu-id="cbb52-103">创建、更新和删除 Microsoft Graph 中的连接</span><span class="sxs-lookup"><span data-stu-id="cbb52-103">Create, update, and delete connections in the Microsoft Graph</span></span>

<span data-ttu-id="cbb52-104">外部服务与 Microsoft 搜索服务的连接由 Microsoft Graph 中的 [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) 资源表示。</span><span class="sxs-lookup"><span data-stu-id="cbb52-104">Connections from external services to the Microsoft Search service are represented by the [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) resource in Microsoft Graph.</span></span>

<span data-ttu-id="cbb52-105">Microsoft Graph 连接器平台提供了一种简单的方法，可将外部数据添加到 Microsoft Graph 中。</span><span class="sxs-lookup"><span data-stu-id="cbb52-105">The Microsoft Graph connectors platform offers a simple way to add your external data into the Microsoft Graph.</span></span> <span data-ttu-id="cbb52-106">连接是外部数据的逻辑容器，管理员可将其作为一个单元进行管理。</span><span class="sxs-lookup"><span data-stu-id="cbb52-106">A connection is a logical container for your external data that an administrator can manage as a single unit.</span></span>

<span data-ttu-id="cbb52-107">创建连接后，你可以添加来自任何外部数据源（如本地内容源或外部 SaaS 服务）的内容。</span><span class="sxs-lookup"><span data-stu-id="cbb52-107">Once a connection has been created, you can add your content from any external data source such as an on-premises content source or an external SaaS service.</span></span> <span data-ttu-id="cbb52-108">你只能查看和管理你创建的连接，或者显式[已授权](/graph/api/external-post-connections?view=graph-rest-beta&preserve-view=true)进行管理的连接。</span><span class="sxs-lookup"><span data-stu-id="cbb52-108">You can only view and manage the connections you created or were explicitly [authorized](/graph/api/external-post-connections?view=graph-rest-beta&preserve-view=true) to manage.</span></span> <span data-ttu-id="cbb52-109">搜索管理员可以从现代管理中心查看和管理租户中的所有连接。</span><span class="sxs-lookup"><span data-stu-id="cbb52-109">A search admin can view and manage all the connections in the tenant from the Modern Admin Center.</span></span>

<!-- markdownlint-disable MD036 -->
<span data-ttu-id="cbb52-110">![自定义支持人员系统票证连接器结构示例](./images/connectors-images/connecting-external-content-manage-connections-connector-structure.png)</span><span class="sxs-lookup"><span data-stu-id="cbb52-110">![Sample custom helpdesk system Tickets Connector Structure](./images/connectors-images/connecting-external-content-manage-connections-connector-structure.png)</span></span>

<span data-ttu-id="cbb52-111">*自定义支持人员系统票证连接器结构示例*</span><span class="sxs-lookup"><span data-stu-id="cbb52-111">*Sample custom helpdesk system Tickets Connector Structure*</span></span>

![连接的管理员视图，包括自定义票证连接器](./images/connectors-images/connecting-external-content-manage-connections-admin-view.svg)

<span data-ttu-id="cbb52-113">*连接的管理员视图，包括自定义票证连接器*</span><span class="sxs-lookup"><span data-stu-id="cbb52-113">*Admin View of Connections including the custom Tickets Connector*</span></span>

<!-- markdownlint-enable MD036 -->

<span data-ttu-id="cbb52-114">可建立任意的连接模型，但为每个连接器实例创建一个连接是最常见的模型。</span><span class="sxs-lookup"><span data-stu-id="cbb52-114">You can model a connection anyway you want, but creating one connection for every instance of your connector is the most common model.</span></span> <span data-ttu-id="cbb52-115">例如，每次[设置 Microsoft Windows 文件共享连接器](/microsoftsearch/configure-connector)时，都会创建一个新的连接。</span><span class="sxs-lookup"><span data-stu-id="cbb52-115">For example, each time you [set up the Microsoft Windows file share connector](/microsoftsearch/configure-connector), a new connection is created.</span></span> <span data-ttu-id="cbb52-116">你还可以创建一个连接来添加数据源中的所有项目。</span><span class="sxs-lookup"><span data-stu-id="cbb52-116">You can also create a single connection to add all items from your data source.</span></span> <span data-ttu-id="cbb52-117">例如，创建单一连接，从支持人员系统中的多个团队中添加所有票证和事件。</span><span class="sxs-lookup"><span data-stu-id="cbb52-117">For example, creating a single connection to add all the tickets and incidents across multiple teams from your helpdesk system.</span></span>

## <a name="states-and-operations"></a><span data-ttu-id="cbb52-118">状态与操作</span><span class="sxs-lookup"><span data-stu-id="cbb52-118">States and operations</span></span>

<span data-ttu-id="cbb52-119">你的连接可以以下列一种状态存在。</span><span class="sxs-lookup"><span data-stu-id="cbb52-119">Your connection can exist in one of the following states.</span></span>

| <span data-ttu-id="cbb52-120">状态</span><span class="sxs-lookup"><span data-stu-id="cbb52-120">State</span></span>             | <span data-ttu-id="cbb52-121">说明</span><span class="sxs-lookup"><span data-stu-id="cbb52-121">Description</span></span>                                                                                                                                               |
|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cbb52-122">**Draft**</span><span class="sxs-lookup"><span data-stu-id="cbb52-122">**Draft**</span></span>         | <span data-ttu-id="cbb52-p104">已预配空连接。尚未配置数据源、架构或任何设置。</span><span class="sxs-lookup"><span data-stu-id="cbb52-p104">An empty connection is provisioned. The data source, schema, or any settings have not been configured yet.</span></span>                                                |
| <span data-ttu-id="cbb52-125">**Ready**</span><span class="sxs-lookup"><span data-stu-id="cbb52-125">**Ready**</span></span>         | <span data-ttu-id="cbb52-126">该连接配有已注册的架构并已准备好接收。</span><span class="sxs-lookup"><span data-stu-id="cbb52-126">The connection is provisioned with registered schema and is ready for ingestion.</span></span>                                                                          |
| <span data-ttu-id="cbb52-127">**Obsolete**</span><span class="sxs-lookup"><span data-stu-id="cbb52-127">**Obsolete**</span></span>      | <span data-ttu-id="cbb52-128">如果已弃用依赖功能（如 API），则会出现这种情况。</span><span class="sxs-lookup"><span data-stu-id="cbb52-128">This occurs when a dependent feature, such as an API, has been deprecated.</span></span> <span data-ttu-id="cbb52-129">删除连接是唯一有效的操作。</span><span class="sxs-lookup"><span data-stu-id="cbb52-129">Deleting the connection is the only valid operation.</span></span>                           |
| <span data-ttu-id="cbb52-130">**LimitExceeded**</span><span class="sxs-lookup"><span data-stu-id="cbb52-130">**LimitExceeded**</span></span> | <span data-ttu-id="cbb52-131">如果点击了单个连接的最大限制或所有连接的租户级别配额，则无法添加更多项目，直至退出该状态。</span><span class="sxs-lookup"><span data-stu-id="cbb52-131">If you hit the maximum limit of a single connection or the tenant level quota across all connections, you cannot add more items until you exit the state.</span></span> |

<span data-ttu-id="cbb52-132">下表指定每种状态中的可用操作。</span><span class="sxs-lookup"><span data-stu-id="cbb52-132">The following table specifies which operations are available in each state.</span></span>

| <span data-ttu-id="cbb52-133">Operation</span><span class="sxs-lookup"><span data-stu-id="cbb52-133">Operation</span></span>         | <span data-ttu-id="cbb52-134">Draft</span><span class="sxs-lookup"><span data-stu-id="cbb52-134">Draft</span></span>              | <span data-ttu-id="cbb52-135">Ready</span><span class="sxs-lookup"><span data-stu-id="cbb52-135">Ready</span></span>              | <span data-ttu-id="cbb52-136">Obsolete</span><span class="sxs-lookup"><span data-stu-id="cbb52-136">Obsolete</span></span>           | <span data-ttu-id="cbb52-137">LimitExceeded</span><span class="sxs-lookup"><span data-stu-id="cbb52-137">LimitExceeded</span></span>      |
|-------------------|--------------------|--------------------|--------------------|--------------------|
| <span data-ttu-id="cbb52-138">Create Connection</span><span class="sxs-lookup"><span data-stu-id="cbb52-138">Create connection</span></span> | :x:                | :heavy_check_mark: | :x:                | :heavy_check_mark: |
| <span data-ttu-id="cbb52-143">Read connection</span><span class="sxs-lookup"><span data-stu-id="cbb52-143">Read connection</span></span>   | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| <span data-ttu-id="cbb52-148">更新连接</span><span class="sxs-lookup"><span data-stu-id="cbb52-148">Update connection</span></span> | :heavy_check_mark: | :heavy_check_mark: | :x:                | :heavy_check_mark: |
| <span data-ttu-id="cbb52-153">删除连接</span><span class="sxs-lookup"><span data-stu-id="cbb52-153">Delete connection</span></span> | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| <span data-ttu-id="cbb52-158">创建架构</span><span class="sxs-lookup"><span data-stu-id="cbb52-158">Create schema</span></span>     | :heavy_check_mark: | :x:                | :x:                | :x:                |
| <span data-ttu-id="cbb52-163">读取架构</span><span class="sxs-lookup"><span data-stu-id="cbb52-163">Read schema</span></span>       | :x:                | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| <span data-ttu-id="cbb52-168">更新架构</span><span class="sxs-lookup"><span data-stu-id="cbb52-168">Update schema</span></span>     | :x:                | :x:                | :x:                | :x:                |
| <span data-ttu-id="cbb52-173">删除架构</span><span class="sxs-lookup"><span data-stu-id="cbb52-173">Delete schema</span></span>     | :x:                | :x:                | :x:                | :x:                |
| <span data-ttu-id="cbb52-178">创建项目</span><span class="sxs-lookup"><span data-stu-id="cbb52-178">Create item</span></span>       | :x:                | :heavy_check_mark: | :x:                | :x:                |
| <span data-ttu-id="cbb52-183">读取项目</span><span class="sxs-lookup"><span data-stu-id="cbb52-183">Read item</span></span>         | :x:                | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| <span data-ttu-id="cbb52-188">更新项目</span><span class="sxs-lookup"><span data-stu-id="cbb52-188">Update item</span></span>       | :x:                | :heavy_check_mark: | :x:                | :heavy_check_mark: |
| <span data-ttu-id="cbb52-193">删除项目</span><span class="sxs-lookup"><span data-stu-id="cbb52-193">Delete item</span></span>       | :x:                | :heavy_check_mark: | :x:                | :heavy_check_mark: |

<span data-ttu-id="cbb52-198">通过连接，你的应用程序可以为要编入索引的项目[定义架构](/graph/api/externalconnection-post-schema?view=graph-rest-beta&preserve-view=true)，并为服务提供终结点，以便在索引中添加、更新或删除项目。</span><span class="sxs-lookup"><span data-stu-id="cbb52-198">A connection allows your application to [define a schema](/graph/api/externalconnection-post-schema?view=graph-rest-beta&preserve-view=true) for items that will be indexed, and provides an endpoint for your service to add, update, or delete items from the index.</span></span> <span data-ttu-id="cbb52-199">[创建连接](#create-a-connection)是应用程序将项目添加到搜索索引的第一步。</span><span class="sxs-lookup"><span data-stu-id="cbb52-199">[Creating a connection](#create-a-connection) is the first step for an application to add items to the search index.</span></span>

## <a name="create-a-connection"></a><span data-ttu-id="cbb52-200">创建连接</span><span class="sxs-lookup"><span data-stu-id="cbb52-200">Create a connection</span></span>

<span data-ttu-id="cbb52-201">应用程序必须先按照以下步骤创建并配置连接，才能将项目添加到搜索索引。</span><span class="sxs-lookup"><span data-stu-id="cbb52-201">Before an application can add items to the search index, it must create and configure a connection using the following steps.</span></span>

- <span data-ttu-id="cbb52-202">使用唯一 ID、显示名称和说明[创建连接](/graph/api/external-post-connections?view=graph-rest-beta&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="cbb52-202">[Create a connection](/graph/api/external-post-connections?view=graph-rest-beta&preserve-view=true) with a unique ID, display name, and description.</span></span>
- <span data-ttu-id="cbb52-203">[注册架构](/graph/api/externalconnection-post-schema?view=graph-rest-beta&preserve-view=true)，以定义索引中将包含的字段。</span><span class="sxs-lookup"><span data-stu-id="cbb52-203">[Register a schema](/graph/api/externalconnection-post-schema?view=graph-rest-beta&preserve-view=true) to define the fields that will be included in the index.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cbb52-204">架构注册后，不能为现有连接更改架构。</span><span class="sxs-lookup"><span data-stu-id="cbb52-204">After a schema has been registered, it cannot be changed for an existing connection.</span></span>

## <a name="update-a-connection"></a><span data-ttu-id="cbb52-205">更新连接</span><span class="sxs-lookup"><span data-stu-id="cbb52-205">Update a connection</span></span>

<span data-ttu-id="cbb52-206">可通过[更新连接](/graph/api/externalconnection-update?view=graph-rest-beta&preserve-view=true)来更改现有连接的显示名称或说明。</span><span class="sxs-lookup"><span data-stu-id="cbb52-206">You can change the display name or description of an existing connection by [updating the connection](/graph/api/externalconnection-update?view=graph-rest-beta&preserve-view=true).</span></span>

## <a name="delete-a-connection"></a><span data-ttu-id="cbb52-207">删除连接</span><span class="sxs-lookup"><span data-stu-id="cbb52-207">Delete a connection</span></span>

<span data-ttu-id="cbb52-208">可[删除连接](/graph/api/externalconnection-delete?view=graph-rest-beta&preserve-view=true)，并删除通过该连接进行索引的所有项目。</span><span class="sxs-lookup"><span data-stu-id="cbb52-208">You can [delete a connection](/graph/api/externalconnection-delete?view=graph-rest-beta&preserve-view=true), and remove all items that were indexed via that connection.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cbb52-209">后续步骤</span><span class="sxs-lookup"><span data-stu-id="cbb52-209">Next steps</span></span>

- [<span data-ttu-id="cbb52-210">注册连接架构</span><span class="sxs-lookup"><span data-stu-id="cbb52-210">Register the connection schema</span></span>](./connecting-external-content-manage-schema.md)
- [<span data-ttu-id="cbb52-211">查看图形连接器 API 参考</span><span class="sxs-lookup"><span data-stu-id="cbb52-211">Review the Graph Connectors API reference</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="cbb52-212">Microsoft Graph 连接器概述</span><span class="sxs-lookup"><span data-stu-id="cbb52-212">Overview for Microsoft Graph Connectors</span></span>](/microsoftsearch/connectors-overview)
- <span data-ttu-id="cbb52-213">从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)</span><span class="sxs-lookup"><span data-stu-id="cbb52-213">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>