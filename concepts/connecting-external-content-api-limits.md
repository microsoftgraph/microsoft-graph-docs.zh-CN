---
title: Microsoft Graph 连接器 API 限制
description: Microsoft Graph 连接器 API 限制
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 6ab757d16a10f2291ad9bac5034e9fe7357a7188
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645734"
---
# <a name="microsoft-graph-connector-api-limits"></a><span data-ttu-id="846a6-103">Microsoft Graph 连接器 API 限制</span><span class="sxs-lookup"><span data-stu-id="846a6-103">Microsoft Graph connector API limits</span></span>

<span data-ttu-id="846a6-104">本主题介绍 Microsoft Graph 连接器的实施和运行限制。</span><span class="sxs-lookup"><span data-stu-id="846a6-104">This topic describes implementation and operational limits for Microsoft Graph connectors.</span></span> <span data-ttu-id="846a6-105">设计连接器时，请牢记这些限制。</span><span class="sxs-lookup"><span data-stu-id="846a6-105">Keep these limits in mind when designing connectors.</span></span>

## <a name="connection-limits"></a><span data-ttu-id="846a6-106">连接限制</span><span class="sxs-lookup"><span data-stu-id="846a6-106">Connection limits</span></span>

| <span data-ttu-id="846a6-107">**限制**</span><span class="sxs-lookup"><span data-stu-id="846a6-107">**Limit**</span></span> | <span data-ttu-id="846a6-108">**说明**</span><span class="sxs-lookup"><span data-stu-id="846a6-108">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="846a6-109">**10 连接**</span><span class="sxs-lookup"><span data-stu-id="846a6-109">**10 connections**</span></span> | <span data-ttu-id="846a6-110">每个 Microsoft 365 租户的最大[连接](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true)资源数。</span><span class="sxs-lookup"><span data-stu-id="846a6-110">The maximum number of [connection](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) resources per Microsoft 365 tenant.</span></span> |
| <span data-ttu-id="846a6-111">**700,000 项**</span><span class="sxs-lookup"><span data-stu-id="846a6-111">**700,000 items**</span></span> | <span data-ttu-id="846a6-112">每个连接最多[项目](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)数量。</span><span class="sxs-lookup"><span data-stu-id="846a6-112">The maximum number of [items](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) per connection.</span></span> |
| <span data-ttu-id="846a6-113">**70 GB**</span><span class="sxs-lookup"><span data-stu-id="846a6-113">**70 GB**</span></span> | <span data-ttu-id="846a6-114">连接的最大字节大小。</span><span class="sxs-lookup"><span data-stu-id="846a6-114">The maximum byte size of a connection.</span></span> |

## <a name="schema-limits"></a><span data-ttu-id="846a6-115">架构限制</span><span class="sxs-lookup"><span data-stu-id="846a6-115">Schema limits</span></span>

| <span data-ttu-id="846a6-116">**限制**</span><span class="sxs-lookup"><span data-stu-id="846a6-116">**Limit**</span></span> | <span data-ttu-id="846a6-117">**说明**</span><span class="sxs-lookup"><span data-stu-id="846a6-117">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="846a6-118">**128 个属性**</span><span class="sxs-lookup"><span data-stu-id="846a6-118">**128 properties**</span></span> | <span data-ttu-id="846a6-119">可以在[架构](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true)中定义的最大数量的属性，用于表征通过连接引入的数据。</span><span class="sxs-lookup"><span data-stu-id="846a6-119">The maximum number of properties that can be defined in a [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true), characterizing the data ingested through a connection.</span></span> |

## <a name="group-limits"></a><span data-ttu-id="846a6-120">组限制</span><span class="sxs-lookup"><span data-stu-id="846a6-120">Group limits</span></span>

| <span data-ttu-id="846a6-121">**限制**</span><span class="sxs-lookup"><span data-stu-id="846a6-121">**Limit**</span></span> | <span data-ttu-id="846a6-122">**说明**</span><span class="sxs-lookup"><span data-stu-id="846a6-122">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="846a6-123">100,000</span><span class="sxs-lookup"><span data-stu-id="846a6-123">100,000</span></span> | <span data-ttu-id="846a6-124">每个 Microsoft 365 租户[外部组](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true)最大数量。</span><span class="sxs-lookup"><span data-stu-id="846a6-124">The maximum number of [external groups](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) per Microsoft 365 tenant.</span></span> |
| <span data-ttu-id="846a6-125">**1000 个请求/秒**</span><span class="sxs-lookup"><span data-stu-id="846a6-125">**1000 requests/sec**</span></span> | <span data-ttu-id="846a6-126">组管理[限制](#throttling)阈值中每秒允许的最大请求数。</span><span class="sxs-lookup"><span data-stu-id="846a6-126">The maximum number of requests allowed per second in the group administration [throttling](#throttling) threshold.</span></span> |

## <a name="item-ingestion"></a><span data-ttu-id="846a6-127">项引入</span><span class="sxs-lookup"><span data-stu-id="846a6-127">Item ingestion</span></span>

| <span data-ttu-id="846a6-128">**限制**</span><span class="sxs-lookup"><span data-stu-id="846a6-128">**Limit**</span></span> | <span data-ttu-id="846a6-129">**说明**</span><span class="sxs-lookup"><span data-stu-id="846a6-129">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="846a6-130">**每秒 4 个项目（每小时 250 MB）**</span><span class="sxs-lookup"><span data-stu-id="846a6-130">**4 items/sec (250 MB/hour)**</span></span> | <span data-ttu-id="846a6-131">通过连接引入项目的吞吐量限制。</span><span class="sxs-lookup"><span data-stu-id="846a6-131">The throughput limit to ingest items through a connection.</span></span> |
| <span data-ttu-id="846a6-132">**4 MB**</span><span class="sxs-lookup"><span data-stu-id="846a6-132">**4 MB**</span></span> | <span data-ttu-id="846a6-133">项目的最大大小；[引入项目为其建立索引](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true)时，此限制适用于请求正文。</span><span class="sxs-lookup"><span data-stu-id="846a6-133">The maximum size of an item; this limit applies to the request body when [ingesting and indexing an item](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true).</span></span> |
| <span data-ttu-id="846a6-134">**N/A**</span><span class="sxs-lookup"><span data-stu-id="846a6-134">**N/A**</span></span> | <span data-ttu-id="846a6-135">属性的最大大小。</span><span class="sxs-lookup"><span data-stu-id="846a6-135">The maximum size of a property.</span></span> |

## <a name="throttling"></a><span data-ttu-id="846a6-136">限制</span><span class="sxs-lookup"><span data-stu-id="846a6-136">Throttling</span></span>

<span data-ttu-id="846a6-p102">超出[限制](throttling.md)阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。</span><span class="sxs-lookup"><span data-stu-id="846a6-p102">When a [throttling](throttling.md) threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>
