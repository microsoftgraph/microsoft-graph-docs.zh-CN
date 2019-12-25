---
title: 使用 Microsoft 搜索 API 为数据编制索引
description: 使用 Microsoft Graph 为 Microsoft 搜索服务中的自定义项或外部文件编制索引。
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: f1a39a42f94a072c501c288b55a6b665af0fc640
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870227"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a><span data-ttu-id="08488-103">使用 Microsoft 搜索 API 为数据编制索引</span><span class="sxs-lookup"><span data-stu-id="08488-103">Use the Microsoft Search API to index data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08488-104">可使用 Microsoft Graph 将自定义项或外部文件添加到 [Microsoft 搜索](/microsoftsearch/overview-microsoft-search)体验的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="08488-104">Microsoft Graph lets your app add custom items or external files into search results in the [Microsoft Search](/microsoftsearch/overview-microsoft-search) experience.</span></span>

<span data-ttu-id="08488-105">在无已登录用户的情况下，以应用程序的身份请求为数据编制索引，并使用[包含应用程序权限的访问令牌](/graph/auth-v2-service)进行标识。</span><span class="sxs-lookup"><span data-stu-id="08488-105">Requests to index data are performed on behalf of an application without the presence of a signed-in user, identified using an [access token with application permission](/graph/auth-v2-service).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a><span data-ttu-id="08488-106">常见用例</span><span class="sxs-lookup"><span data-stu-id="08488-106">Common use cases</span></span>

<span data-ttu-id="08488-107">此部分中的 API 用例涉及到构建 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview)，其中包括以下主要步骤：</span><span class="sxs-lookup"><span data-stu-id="08488-107">The use cases for the APIs in this section center around building [Microsoft Graph connectors](/microsoftsearch/connectors-overview), which involves the main steps of:</span></span>

1. <span data-ttu-id="08488-108">与外部数据源[建立连接](../api/external-post-connections.md)。</span><span class="sxs-lookup"><span data-stu-id="08488-108">[Creating a connection](../api/external-post-connections.md) to an external data source</span></span>
2. <span data-ttu-id="08488-109">[创建并注册架构](../api/externalconnection-post-schema.md)，以描述类型及外部数据的索引编制方式。</span><span class="sxs-lookup"><span data-stu-id="08488-109">[Creating and registering a schema](../api/externalconnection-post-schema.md) that describes the type and how to index the external data</span></span>
3. <span data-ttu-id="08488-110">[编制数据的索引](../api/externalconnection-put-items.md)，将其用作外部项或外部文件。</span><span class="sxs-lookup"><span data-stu-id="08488-110">[Indexing the data](../api/externalconnection-put-items.md) as an external item or external file</span></span>

| <span data-ttu-id="08488-111">用例</span><span class="sxs-lookup"><span data-stu-id="08488-111">Use cases</span></span>                                        | <span data-ttu-id="08488-112">REST 资源</span><span class="sxs-lookup"><span data-stu-id="08488-112">REST resources</span></span>                              | <span data-ttu-id="08488-113">另请参阅</span><span class="sxs-lookup"><span data-stu-id="08488-113">See also</span></span> |
|:-------------------------------------------------|:--------------------------------------------|:--|
| <span data-ttu-id="08488-114">**配置操作**</span><span class="sxs-lookup"><span data-stu-id="08488-114">**Configuration actions**</span></span>                        |                                             |   |
| <span data-ttu-id="08488-115">建立、更新或删除连接</span><span class="sxs-lookup"><span data-stu-id="08488-115">Create, update, or delete a connection</span></span>           | [<span data-ttu-id="08488-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="08488-116">externalConnection</span></span>](externalconnection.md) | [<span data-ttu-id="08488-117">externalConnection 方法</span><span class="sxs-lookup"><span data-stu-id="08488-117">externalConnection methods</span></span>](externalconnection.md#methods) |
| <span data-ttu-id="08488-118">注册外部数据的架构</span><span class="sxs-lookup"><span data-stu-id="08488-118">Register a schema for the external data</span></span>          | [<span data-ttu-id="08488-119">schema</span><span class="sxs-lookup"><span data-stu-id="08488-119">schema</span></span>](schema.md)                         | [<span data-ttu-id="08488-120">schema 方法</span><span class="sxs-lookup"><span data-stu-id="08488-120">schema methods</span></span>](schema.md#methods) |
| <span data-ttu-id="08488-121">**为操作编制索引**</span><span class="sxs-lookup"><span data-stu-id="08488-121">**Indexing actions**</span></span>                             |                                             |   |
| <span data-ttu-id="08488-122">在索引中添加、更新或删除自定义项</span><span class="sxs-lookup"><span data-stu-id="08488-122">Add, update or delete a custom item in the index</span></span> | [<span data-ttu-id="08488-123">externalItem</span><span class="sxs-lookup"><span data-stu-id="08488-123">externalItem</span></span>](externalitem.md)             | [<span data-ttu-id="08488-124">externalItem 方法</span><span class="sxs-lookup"><span data-stu-id="08488-124">externalItem methods</span></span>](externalItem.md#methods) |
| <span data-ttu-id="08488-125">在索引中添加、更新或删除文件</span><span class="sxs-lookup"><span data-stu-id="08488-125">Add, update or delete a file in the index</span></span>        | [<span data-ttu-id="08488-126">externalFile</span><span class="sxs-lookup"><span data-stu-id="08488-126">externalFile</span></span>](externalfile.md)             | [<span data-ttu-id="08488-127">externalFile 方法</span><span class="sxs-lookup"><span data-stu-id="08488-127">externalFile methods</span></span>](externalfile.md#methods) |

## <a name="known-limitations"></a><span data-ttu-id="08488-128">已知限制</span><span class="sxs-lookup"><span data-stu-id="08488-128">Known limitations</span></span>

<span data-ttu-id="08488-129">当前已知的限制如下：</span><span class="sxs-lookup"><span data-stu-id="08488-129">The following are current knownlimitations:</span></span>

- <span data-ttu-id="08488-130">组织最多可有 10 个连接。</span><span class="sxs-lookup"><span data-stu-id="08488-130">Organizations are limited to a maximum of 10 connections.</span></span>
- <span data-ttu-id="08488-131">使用 `externalFile` 资源为文件编制索引时不支持自定义属性。</span><span class="sxs-lookup"><span data-stu-id="08488-131">Custom properties are not supported when indexing files using the `externalFile` resource.</span></span>
- <span data-ttu-id="08488-132">仅支持 Azure Active Directory 标识。</span><span class="sxs-lookup"><span data-stu-id="08488-132">Only Azure Active Directory identities are supported.</span></span>
- <span data-ttu-id="08488-133">每秒只能创建 4 个 `externalItem` 或 `externalFile` 资源项。</span><span class="sxs-lookup"><span data-stu-id="08488-133">You can create only four `externalItem` or `externalFile` resources items per second.</span></span>
- <span data-ttu-id="08488-134">应用程序最多可对一个连接执行 4 个并行操作。</span><span class="sxs-lookup"><span data-stu-id="08488-134">An application is limited to 4 concurrent operations on a connection.</span></span>
- <span data-ttu-id="08488-135">连接的容量限制为 70 万个项，或约 70 GB 的数据。</span><span class="sxs-lookup"><span data-stu-id="08488-135">Connections have a capacity limit of 700,000 items or ~70 GB of data.</span></span>
- <span data-ttu-id="08488-136">`externalItem` 或 `externalFile` 实体的最大大小为 4 MB。</span><span class="sxs-lookup"><span data-stu-id="08488-136">Maximum size of an `externalItem` or `externalFile` entity is 4 MB.</span></span>
- <span data-ttu-id="08488-137">不支持对结果进行优化和排序。</span><span class="sxs-lookup"><span data-stu-id="08488-137">Refining and sorting results is not supported.</span></span>
- <span data-ttu-id="08488-138">最多可以进行结果排名。</span><span class="sxs-lookup"><span data-stu-id="08488-138">Result ranking is best effort.</span></span>

## <a name="next-steps"></a><span data-ttu-id="08488-139">后续步骤</span><span class="sxs-lookup"><span data-stu-id="08488-139">Next steps</span></span>

- <span data-ttu-id="08488-140">请参阅 [Microsoft 搜索 API 概述](/graph/search-concept-overview)。</span><span class="sxs-lookup"><span data-stu-id="08488-140">See the [Microsoft Search API overview](/graph/search-concept-overview).</span></span>
- <span data-ttu-id="08488-141">向下钻取 [externalConnection](externalconnection.md)、[schema](schema.md)、[externalItem](externalitem.md) 和 [externalFile](externalfile.md) 资源的方法、属性和关系。</span><span class="sxs-lookup"><span data-stu-id="08488-141">Drill down on the methods, properties, and relationships of the [externalConnection](externalconnection.md), [schema](schema.md), [externalItem](externalitem.md), and [externalFile](externalfile.md) resources.</span></span>
- <span data-ttu-id="08488-142">查看 GitHub 中的[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。</span><span class="sxs-lookup"><span data-stu-id="08488-142">Check out the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>
