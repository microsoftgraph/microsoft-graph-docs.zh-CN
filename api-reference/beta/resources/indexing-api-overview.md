---
title: 使用 Microsoft 搜索 API 为数据编制索引
description: 使用 Microsoft Graph 为 Microsoft 搜索服务中的自定义项编制索引。
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 69a1c99af429b93d7fbddbea4e76523b281541d7
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366961"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a><span data-ttu-id="32101-103">使用 Microsoft 搜索 API 为数据编制索引</span><span class="sxs-lookup"><span data-stu-id="32101-103">Use the Microsoft Search API to index data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32101-104">可使用 Microsoft Graph 将自定义项添加到 [Microsoft 搜索](/microsoftsearch/overview-microsoft-search)体验的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="32101-104">You can use Microsoft Graph to add custom items to search results in the [Microsoft Search](/microsoftsearch/overview-microsoft-search) experience.</span></span>

<span data-ttu-id="32101-105">在无已登录用户的情况下，以应用程序的身份请求为数据编制索引，并使用[包含应用程序权限的访问令牌](/graph/auth-v2-service)进行标识。</span><span class="sxs-lookup"><span data-stu-id="32101-105">Requests to index data are performed on behalf of an application without the presence of a signed-in user, identified using an [access token with application permission](/graph/auth-v2-service).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="32101-106">常见用例</span><span class="sxs-lookup"><span data-stu-id="32101-106">Common use cases</span></span>

<span data-ttu-id="32101-107">此部分中的 API 用例涉及到构建 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview)，其中包括以下主要步骤：</span><span class="sxs-lookup"><span data-stu-id="32101-107">The use cases for the APIs in this section involve building [Microsoft Graph connectors](/microsoftsearch/connectors-overview), which involves the following primary steps:</span></span>

1. <span data-ttu-id="32101-108">与外部数据源[建立连接](../api/external-post-connections.md)。</span><span class="sxs-lookup"><span data-stu-id="32101-108">[Create a connection](../api/external-post-connections.md) to an external data source.</span></span>
2. <span data-ttu-id="32101-109">[创建并注册架构](../api/externalconnection-post-schema.md)，以描述类型及外部数据的索引编制方式。</span><span class="sxs-lookup"><span data-stu-id="32101-109">[Create and register a schema](../api/externalconnection-post-schema.md) that describes the type and how to index the external data.</span></span>
3. <span data-ttu-id="32101-110">将数据作为外部项[编制索引](../api/externalconnection-put-items.md)。</span><span class="sxs-lookup"><span data-stu-id="32101-110">[Index the data](../api/externalconnection-put-items.md) as an external item.</span></span>

| <span data-ttu-id="32101-111">用例</span><span class="sxs-lookup"><span data-stu-id="32101-111">Use cases</span></span>                                        | <span data-ttu-id="32101-112">REST 资源</span><span class="sxs-lookup"><span data-stu-id="32101-112">REST resources</span></span>                              | <span data-ttu-id="32101-113">另请参阅</span><span class="sxs-lookup"><span data-stu-id="32101-113">See also</span></span> |
|:-------------------------------------------------|:--------------------------------------------|:--|
| <span data-ttu-id="32101-114">**配置操作**</span><span class="sxs-lookup"><span data-stu-id="32101-114">**Configuration actions**</span></span>                        |                                             |   |
| <span data-ttu-id="32101-115">建立、更新或删除连接</span><span class="sxs-lookup"><span data-stu-id="32101-115">Create, update, or delete a connection</span></span>           | [<span data-ttu-id="32101-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="32101-116">externalConnection</span></span>](externalconnection.md) | [<span data-ttu-id="32101-117">externalConnection 方法</span><span class="sxs-lookup"><span data-stu-id="32101-117">externalConnection methods</span></span>](externalconnection.md#methods) |
| <span data-ttu-id="32101-118">注册外部数据的架构</span><span class="sxs-lookup"><span data-stu-id="32101-118">Register a schema for the external data</span></span>          | [<span data-ttu-id="32101-119">schema</span><span class="sxs-lookup"><span data-stu-id="32101-119">schema</span></span>](schema.md)                         | [<span data-ttu-id="32101-120">schema 方法</span><span class="sxs-lookup"><span data-stu-id="32101-120">schema methods</span></span>](schema.md#methods) |
| <span data-ttu-id="32101-121">**为操作编制索引**</span><span class="sxs-lookup"><span data-stu-id="32101-121">**Indexing actions**</span></span>                             |                                             |   |
| <span data-ttu-id="32101-122">在索引中添加、更新或删除自定义项</span><span class="sxs-lookup"><span data-stu-id="32101-122">Add, update or delete a custom item in the index</span></span> | [<span data-ttu-id="32101-123">externalItem</span><span class="sxs-lookup"><span data-stu-id="32101-123">externalItem</span></span>](externalitem.md)             | [<span data-ttu-id="32101-124">externalItem 方法</span><span class="sxs-lookup"><span data-stu-id="32101-124">externalItem methods</span></span>](externalItem.md#methods) |

## <a name="known-limitations"></a><span data-ttu-id="32101-125">已知限制</span><span class="sxs-lookup"><span data-stu-id="32101-125">Known limitations</span></span>

<span data-ttu-id="32101-126">当前已知的限制如下：</span><span class="sxs-lookup"><span data-stu-id="32101-126">The following are current known limitations:</span></span>

- <span data-ttu-id="32101-127">组织最多可有 10 个连接。</span><span class="sxs-lookup"><span data-stu-id="32101-127">Organizations are limited to a maximum of 10 connections.</span></span>
- <span data-ttu-id="32101-128">仅支持 Azure Active Directory 标识。</span><span class="sxs-lookup"><span data-stu-id="32101-128">Only Azure Active Directory identities are supported.</span></span>
- <span data-ttu-id="32101-129">每秒只能创建 4 个 `externalItem` 资源项。</span><span class="sxs-lookup"><span data-stu-id="32101-129">You can create only four `externalItem` resources items per second.</span></span>
- <span data-ttu-id="32101-130">应用程序最多可对一个连接执行 4 个并行操作。</span><span class="sxs-lookup"><span data-stu-id="32101-130">An application is limited to four concurrent operations on a connection.</span></span>
- <span data-ttu-id="32101-131">连接的容量限制为 70 万个项，或约 70 GB 的数据。</span><span class="sxs-lookup"><span data-stu-id="32101-131">Connections have a capacity limit of 700,000 items or ~70 GB of data.</span></span>
- <span data-ttu-id="32101-132">`externalItem` 实体的最大大小为 4 MB。</span><span class="sxs-lookup"><span data-stu-id="32101-132">Maximum size of an `externalItem` entity is 4 MB.</span></span>
- <span data-ttu-id="32101-133">不支持对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="32101-133">Sorting results is not supported.</span></span>
- <span data-ttu-id="32101-134">最多可以进行结果排名。</span><span class="sxs-lookup"><span data-stu-id="32101-134">Result ranking is best effort.</span></span>

## <a name="whats-new"></a><span data-ttu-id="32101-135">最近更新</span><span class="sxs-lookup"><span data-stu-id="32101-135">What's new</span></span>
<span data-ttu-id="32101-136">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="32101-136">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="32101-137">后续步骤</span><span class="sxs-lookup"><span data-stu-id="32101-137">Next steps</span></span>

- <span data-ttu-id="32101-138">请参阅 [Microsoft 搜索 API 概述](/graph/search-concept-overview)。</span><span class="sxs-lookup"><span data-stu-id="32101-138">See the [Microsoft Search API overview](/graph/search-concept-overview).</span></span>
- <span data-ttu-id="32101-139">向下钻取 [externalConnection](externalconnection.md)、[schema](schema.md) 和[externalItem](externalitem.md) 资源的方法、属性和关系。</span><span class="sxs-lookup"><span data-stu-id="32101-139">Drill down on the methods, properties, and relationships of the [externalConnection](externalconnection.md), [schema](schema.md), and [externalItem](externalitem.md) resources.</span></span>
- <span data-ttu-id="32101-140">查看 GitHub 中的[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。</span><span class="sxs-lookup"><span data-stu-id="32101-140">Check out the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>


