---
title: 创建、更新和删除与 Microsoft 搜索服务的连接
description: 了解如何使用 Microsoft Graph 管理与 Microsoft 搜索服务的连接
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 99f0ab4591caa6c311f2771f1c6a0772a8f16087
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892798"
---
# <a name="create-update-and-delete-connections-to-the-microsoft-search-service"></a><span data-ttu-id="69896-103">创建、更新和删除与 Microsoft 搜索服务的连接</span><span class="sxs-lookup"><span data-stu-id="69896-103">Create, update, and delete connections to the Microsoft Search service</span></span>

<span data-ttu-id="69896-104">外部服务与 Microsoft 搜索服务的连接由 Microsoft Graph 中的 [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) 资源表示。</span><span class="sxs-lookup"><span data-stu-id="69896-104">Connections from external services to the Microsoft Search service are represented by the [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) resource in Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="69896-105">通过连接，你的应用程序可以为要编入索引的项目[定义架构](/graph/api/externalconnection-post-schema?view=graph-rest-beta)，并为服务提供终结点，以便[在索引中添加、更新或删除项目](search-index-manage-items.md)。</span><span class="sxs-lookup"><span data-stu-id="69896-105">A connection allows your application to [define a schema](/graph/api/externalconnection-post-schema?view=graph-rest-beta) for items that will be indexed, and provides an endpoint for your service to [add, update, or delete items from the index](search-index-manage-items.md).</span></span> <span data-ttu-id="69896-106">创建连接是应用程序将项目添加到搜索索引的第一步。</span><span class="sxs-lookup"><span data-stu-id="69896-106">Creating a connection is the first step for an application to add items to the search index.</span></span>

## <a name="create-a-connection"></a><span data-ttu-id="69896-107">创建连接</span><span class="sxs-lookup"><span data-stu-id="69896-107">Create a connection</span></span>

<span data-ttu-id="69896-108">应用程序必须先按照以下步骤创建并配置连接，才能将项目添加到搜索索引。</span><span class="sxs-lookup"><span data-stu-id="69896-108">Before an application can add items to the search index, it must create and configure a connection using the following steps.</span></span>

- <span data-ttu-id="69896-109">使用唯一 ID、显示名称和说明[创建连接](/graph/api/external-post-connections?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="69896-109">[Create a connection](/graph/api/external-post-connections?view=graph-rest-beta) with a unique ID, display name, and description.</span></span>
- <span data-ttu-id="69896-110">[注册架构](/graph/api/externalconnection-post-schema?view=graph-rest-beta)，以定义索引中将包含的字段。</span><span class="sxs-lookup"><span data-stu-id="69896-110">[Register a schema](/graph/api/externalconnection-post-schema?view=graph-rest-beta) to define the fields that will be included in the index.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="69896-111">架构注册后，不能为现有连接更改架构。</span><span class="sxs-lookup"><span data-stu-id="69896-111">Once a schema has been registered, it cannot be changed for an existing connection.</span></span>

## <a name="update-a-connection"></a><span data-ttu-id="69896-112">更新连接</span><span class="sxs-lookup"><span data-stu-id="69896-112">Update a connection</span></span>

<span data-ttu-id="69896-113">可通过[更新连接](/graph/api/externalconnection-update?view=graph-rest-beta)来更改现有连接的显示名称或说明。</span><span class="sxs-lookup"><span data-stu-id="69896-113">You can change the display name or description of an existing connection by [updating the connection](/graph/api/externalconnection-update?view=graph-rest-beta).</span></span>

## <a name="delete-a-connection"></a><span data-ttu-id="69896-114">删除连接</span><span class="sxs-lookup"><span data-stu-id="69896-114">Delete a connection</span></span>

<span data-ttu-id="69896-115">可[删除连接](/graph/api/externalconnection-delete?view=graph-rest-beta)，并删除通过该连接进行索引的所有项目。</span><span class="sxs-lookup"><span data-stu-id="69896-115">You can [delete a connection](/graph/api/externalconnection-delete?view=graph-rest-beta), and remove all items that were indexed via that connection.</span></span>

## <a name="next-steps"></a><span data-ttu-id="69896-116">后续步骤</span><span class="sxs-lookup"><span data-stu-id="69896-116">Next steps</span></span>

- [<span data-ttu-id="69896-117">为什么使用 Microsoft 搜索 API？</span><span class="sxs-lookup"><span data-stu-id="69896-117">Why use the Microsoft Search API?</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="69896-118">查看索引 API 参考</span><span class="sxs-lookup"><span data-stu-id="69896-118">Review the Indexing API reference</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="69896-119">Microsoft Graph 连接器概述</span><span class="sxs-lookup"><span data-stu-id="69896-119">Overview for Microsoft Graph Connectors</span></span>](/microsoftsearch/connectors-overview)
- <span data-ttu-id="69896-120">从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)</span><span class="sxs-lookup"><span data-stu-id="69896-120">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
