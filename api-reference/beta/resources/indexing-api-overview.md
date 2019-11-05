---
title: 使用 Microsoft 搜索 API 为数据编制索引
description: 借助 Microsoft Graph，应用可以为 Microsoft 搜索服务中的自定义项或外部文件编制索引。
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: cac6d8e9d399e13554e9a9ef44fe8d869c0ad70d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938946"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a><span data-ttu-id="d9f3f-103">使用 Microsoft 搜索 API 为数据编制索引</span><span class="sxs-lookup"><span data-stu-id="d9f3f-103">Use the Microsoft Search API to index data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9f3f-104">借助 Microsoft Graph，应用可以将自定义项或外部文件添加到 [Microsoft 搜索](/microsoftsearch/overview-microsoft-search)体验的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-104">Microsoft Graph lets your app add custom items or external files into search results in the [Microsoft Search](/microsoftsearch/overview-microsoft-search) experience.</span></span>

<span data-ttu-id="d9f3f-105">在无已登录用户的情况下，以应用程序的身份请求为数据编制索引，并使用[包含应用程序权限的访问令牌](/graph/auth-v2-service)进行标识。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-105">Requests to index data are performed on behalf of an application without the presence of a signed-in user, identified using an [access token with application permission](/graph/auth-v2-service).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="d9f3f-106">常见用例</span><span class="sxs-lookup"><span data-stu-id="d9f3f-106">Common use cases</span></span>

<span data-ttu-id="d9f3f-107">此部分中的 API 用例以生成 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview)为中心，其中涉及以下方面的主要步骤：</span><span class="sxs-lookup"><span data-stu-id="d9f3f-107">The use cases for the APIs in this section center around building [Microsoft Graph connectors](/microsoftsearch/connectors-overview), which involves the main steps of:</span></span>

1. <span data-ttu-id="d9f3f-108">与外部数据源[建立连接](../api/external-post-connections.md)</span><span class="sxs-lookup"><span data-stu-id="d9f3f-108">[SQLClose](../api/external-post-connections.md) closes a connection to an external data source.</span></span>
2. <span data-ttu-id="d9f3f-109">[创建并注册架构](../api/externalconnection-post-schema.md)，以描述类型以及如何为外部数据编制索引</span><span class="sxs-lookup"><span data-stu-id="d9f3f-109">[Creating and registering a schema](../api/externalconnection-post-schema.md) that describes the type and how to index the external data</span></span>
3. <span data-ttu-id="d9f3f-110">[为数据编制索引](../api/externalconnection-put-items.md)作为外部项或外部文件</span><span class="sxs-lookup"><span data-stu-id="d9f3f-110">[Indexing the data](../api/externalconnection-put-items.md) as an external item or external file</span></span>

| <span data-ttu-id="d9f3f-111">用例</span><span class="sxs-lookup"><span data-stu-id="d9f3f-111">Use cases</span></span>                                        | <span data-ttu-id="d9f3f-112">REST 资源</span><span class="sxs-lookup"><span data-stu-id="d9f3f-112">REST resources</span></span>                              | <span data-ttu-id="d9f3f-113">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d9f3f-113">See also</span></span> |
|:-------------------------------------------------|:--------------------------------------------|:--|
| <span data-ttu-id="d9f3f-114">**配置操作**</span><span class="sxs-lookup"><span data-stu-id="d9f3f-114">**Configuration actions**</span></span>                        |                                             |   |
| <span data-ttu-id="d9f3f-115">建立、更新或删除连接</span><span class="sxs-lookup"><span data-stu-id="d9f3f-115">Create, get, update, or delete a business</span></span>           | [<span data-ttu-id="d9f3f-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="d9f3f-116">externalConnection</span></span>](externalconnection.md) | [<span data-ttu-id="d9f3f-117">externalConnection 的方法</span><span class="sxs-lookup"><span data-stu-id="d9f3f-117">Methods of externalConnection</span></span>](externalconnection.md#methods) |
| <span data-ttu-id="d9f3f-118">注册外部数据的架构</span><span class="sxs-lookup"><span data-stu-id="d9f3f-118">Register a schema for the external data</span></span>          | [<span data-ttu-id="d9f3f-119">schema</span><span class="sxs-lookup"><span data-stu-id="d9f3f-119">SCHEMA</span></span>](schema.md)                         | [<span data-ttu-id="d9f3f-120">schema 的方法</span><span class="sxs-lookup"><span data-stu-id="d9f3f-120">Methods of schema</span></span>](schema.md#methods) |
| <span data-ttu-id="d9f3f-121">**为操作编制索引**</span><span class="sxs-lookup"><span data-stu-id="d9f3f-121">**Indexing actions**</span></span>                             |                                             |   |
| <span data-ttu-id="d9f3f-122">在索引中添加、更新或删除自定义项</span><span class="sxs-lookup"><span data-stu-id="d9f3f-122">Add, update or delete a custom item in the index</span></span> | [<span data-ttu-id="d9f3f-123">externalItem</span><span class="sxs-lookup"><span data-stu-id="d9f3f-123">externalItem</span></span>](externalitem.md)             | [<span data-ttu-id="d9f3f-124">externalItem 的方法</span><span class="sxs-lookup"><span data-stu-id="d9f3f-124">Methods of externalItem</span></span>](externalItem.md#methods) |
| <span data-ttu-id="d9f3f-125">在索引中添加、更新或删除文件</span><span class="sxs-lookup"><span data-stu-id="d9f3f-125">Add, update or delete a file in the index</span></span>        | [<span data-ttu-id="d9f3f-126">externalFile</span><span class="sxs-lookup"><span data-stu-id="d9f3f-126">externalFile</span></span>](externalfile.md)             | [<span data-ttu-id="d9f3f-127">externalFile 的方法</span><span class="sxs-lookup"><span data-stu-id="d9f3f-127">Methods of externalFile</span></span>](externalfile.md#methods) |

## <a name="known-limitations"></a><span data-ttu-id="d9f3f-128">已知限制</span><span class="sxs-lookup"><span data-stu-id="d9f3f-128">Known limitations</span></span>

<span data-ttu-id="d9f3f-129">在预览期间，请注意以下限制。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-129">Note the following limitations during preview.</span></span>

- <span data-ttu-id="d9f3f-130">组织最多可有 10 个连接。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-130">Organizations are limited to a maximum of 10 connections.</span></span>
- <span data-ttu-id="d9f3f-131">使用 `externalFile` 资源为文件编制索引时，不支持自定义属性。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-131">No support for custom properties when indexing files using the `externalFile` resource.</span></span>
- <span data-ttu-id="d9f3f-132">仅支持 Azure Active Directory 标识。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-132">Only Azure Active Directory identities are supported.</span></span>
- <span data-ttu-id="d9f3f-133">创建 `externalItem` 或 `externalFile` 资源时，每秒的上限为 4 个项。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-133">Creating `externalItem` or `externalFile` resources is limited to 4 items per second.</span></span>
- <span data-ttu-id="d9f3f-134">应用程序最多可对连接执行 4 个并行操作。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-134">An application is limited to 4 concurrent operations on a connection.</span></span>
- <span data-ttu-id="d9f3f-135">连接的容量限制为 70 万个项，或约 70 GB 的数据。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-135">Connections have a capacity limit of 700,000 items or ~70 GB of data.</span></span>
- <span data-ttu-id="d9f3f-136">`externalItem` 或 `externalFile` 实体的最大大小为 4 MB。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-136">Maximum size of an `externalItem` or `externalFile` entity is 4 MB.</span></span>
- <span data-ttu-id="d9f3f-137">不支持对结果进行优化和排序。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-137">No support for refining and sorting results.</span></span>
- <span data-ttu-id="d9f3f-138">最多可以进行结果排名。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-138">Result ranking is best effort.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d9f3f-139">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d9f3f-139">Next steps</span></span>

- [<span data-ttu-id="d9f3f-140">Microsoft 搜索 API 概述</span><span class="sxs-lookup"><span data-stu-id="d9f3f-140">Microsoft Bookings API overview</span></span>](/graph/search-concept-overview)
- <span data-ttu-id="d9f3f-141">向下钻取 [externalConnection](externalconnection.md)、[schema](schema.md)、[externalItem](externalitem.md) 和 [externalFile](externalfile.md) 资源的方法、属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-141">Drill down on the [methods](externalconnection.md), [properties](schema.md), and [relationships](externalitem.md) of the [message](externalfile.md) and mailFolder resources.</span></span>
- <span data-ttu-id="d9f3f-142">查看 GitHub 中的[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。</span><span class="sxs-lookup"><span data-stu-id="d9f3f-142">Check out the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>
