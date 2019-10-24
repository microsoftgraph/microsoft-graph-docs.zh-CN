---
title: 使用 Microsoft Graph Sdk 进行 API 调用
description: 提供有关使用 Sdk 创建 Microsoft Graph HTTP 请求的说明。
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: d4fdd5fc6c9a5b2fb0e8acd6d5484176ef179333
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653515"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a><span data-ttu-id="696ef-103">使用 Microsoft Graph Sdk 进行 API 调用</span><span class="sxs-lookup"><span data-stu-id="696ef-103">Make API calls using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="696ef-104">Microsoft Graph SDK 服务库提供了一个客户端类，您可以将其用作创建所有 API 请求的起始点。</span><span class="sxs-lookup"><span data-stu-id="696ef-104">The Microsoft Graph SDK service libraries provide a client class that you can use as the starting point for creating all API requests.</span></span> <span data-ttu-id="696ef-105">有两种类型的客户端类：一种是使用流畅的接口来创建请求（例如`client.Me.Manager`，），另一种是接受路径字符串（例如`api("/me/manager")`）。</span><span class="sxs-lookup"><span data-stu-id="696ef-105">There are two styles of client class: one uses a fluent interface to create the request (for example, `client.Me.Manager`) and the other  accepts a path string (for example, `api("/me/manager")`).</span></span> <span data-ttu-id="696ef-106">当您拥有 request 对象时，可以指定各种选项（如筛选和排序），最后，选择要执行的操作的类型。</span><span class="sxs-lookup"><span data-stu-id="696ef-106">When you have a request object, you can specify a variety of options such as filtering and sorting, and finally, you select the type of operation you want to perform.</span></span>

## <a name="read-information-from-microsoft-graph"></a><span data-ttu-id="696ef-107">阅读 Microsoft Graph 中的信息</span><span class="sxs-lookup"><span data-stu-id="696ef-107">Read information from Microsoft Graph</span></span>

<span data-ttu-id="696ef-108">若要从 Microsoft Graph 读取信息，首先需要创建 request 对象，然后对该请求运行`GET`方法。</span><span class="sxs-lookup"><span data-stu-id="696ef-108">To read information from Microsoft Graph, you first need to create a request object and then run the `GET` method on the request.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="696ef-109">C#</span><span class="sxs-lookup"><span data-stu-id="696ef-109">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="696ef-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="696ef-110">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]
---

## <a name="use-select-to-control-the-properties-returned"></a><span data-ttu-id="696ef-111">使用 $select 控制返回的属性</span><span class="sxs-lookup"><span data-stu-id="696ef-111">Use $select to control the properties returned</span></span>

<span data-ttu-id="696ef-112">检索实体时，并不会自动检索所有属性;有时需要显式选择它们。</span><span class="sxs-lookup"><span data-stu-id="696ef-112">When retrieving an entity, not all properties are automatically retrieved; sometimes they need to be explicitly selected.</span></span> <span data-ttu-id="696ef-113">此外，在某些情况下，无需返回默认的属性集。</span><span class="sxs-lookup"><span data-stu-id="696ef-113">Also, in some scenarios it isn't necessary to return the default set of properties.</span></span> <span data-ttu-id="696ef-114">仅选择所需的属性可提高请求的性能。</span><span class="sxs-lookup"><span data-stu-id="696ef-114">Selecting just the required properties can improve the performance of the request.</span></span> <span data-ttu-id="696ef-115">您可以自定义*request*对象，以使用`$select`属性列表发出查询参数。</span><span class="sxs-lookup"><span data-stu-id="696ef-115">You can customize the *request* object to emit the `$select` query parameter with a list of properties.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="696ef-116">C#</span><span class="sxs-lookup"><span data-stu-id="696ef-116">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="696ef-117">TypeScript</span><span class="sxs-lookup"><span data-stu-id="696ef-117">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]
---


## <a name="retrieve-a-list-of-entities"></a><span data-ttu-id="696ef-118">检索实体列表</span><span class="sxs-lookup"><span data-stu-id="696ef-118">Retrieve a list of entities</span></span>

<span data-ttu-id="696ef-119">检索实体列表与检索单个实体类似，但有许多其他选项可用于配置请求。</span><span class="sxs-lookup"><span data-stu-id="696ef-119">Retrieving a list of entities is similar to retrieving a single entity except there a number of other options for configuring the request.</span></span> <span data-ttu-id="696ef-120">`$filter`查询参数可用于将结果集减少为与提供的条件匹配的那些行。</span><span class="sxs-lookup"><span data-stu-id="696ef-120">The `$filter` query parameter can be used to reduce the result set to only those rows that match the provided condition.</span></span>  <span data-ttu-id="696ef-121">`$orderBy`查询参数将请求服务器提供按指定属性排序的实体列表。</span><span class="sxs-lookup"><span data-stu-id="696ef-121">The `$orderBy` query parameter will request that the server provide the list of entities sorted by the specified properties.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="696ef-122">C#</span><span class="sxs-lookup"><span data-stu-id="696ef-122">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="696ef-123">TypeScript</span><span class="sxs-lookup"><span data-stu-id="696ef-123">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]
---

<span data-ttu-id="696ef-124">检索实体列表时返回的对象可能是分页的集合。</span><span class="sxs-lookup"><span data-stu-id="696ef-124">The object returned when retrieving a list of entities is likely to be a paged collection.</span></span> <span data-ttu-id="696ef-125">有关如何获取实体的完整列表的详细信息，请参阅[通过集合进行分页](../paging.md)。</span><span class="sxs-lookup"><span data-stu-id="696ef-125">For details about how to get the complete list of entities, see [paging through a collection](../paging.md).</span></span>

## <a name="access-an-item-of-a-collection"></a><span data-ttu-id="696ef-126">访问集合中的项</span><span class="sxs-lookup"><span data-stu-id="696ef-126">Access an item of a collection</span></span>

<span data-ttu-id="696ef-127">对于支持流畅样式的 Sdk，可以使用数组索引访问实体的集合。</span><span class="sxs-lookup"><span data-stu-id="696ef-127">For SDKs that support a fluent style, collections of entities can be accessed using an array index.</span></span> <span data-ttu-id="696ef-128">对于基于模板的 Sdk，足以将项标识符嵌入到集合后面的路径段中。</span><span class="sxs-lookup"><span data-stu-id="696ef-128">For template-based SDKs, it is sufficient to embed the item identifier in the path segment following the collection.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="696ef-129">C#</span><span class="sxs-lookup"><span data-stu-id="696ef-129">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="696ef-130">TypeScript</span><span class="sxs-lookup"><span data-stu-id="696ef-130">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]
---

## <a name="use-expand-to-access-related-entities"></a><span data-ttu-id="696ef-131">使用 $expand 访问相关实体</span><span class="sxs-lookup"><span data-stu-id="696ef-131">Use $expand to access related entities</span></span>

<span data-ttu-id="696ef-132">您可以使用`$expand`筛选器请求与您请求主实体的相关实体或实体集合。</span><span class="sxs-lookup"><span data-stu-id="696ef-132">You can use the `$expand` filter to request a related entity, or collection of entities, at the same that you request the main entity.</span></span>  <span data-ttu-id="696ef-133">Request `Expand()`对象上的\*\* 函数将添加所需的查询参数。</span><span class="sxs-lookup"><span data-stu-id="696ef-133">The `Expand()` function on the *request* object adds the necessary query parameter.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="696ef-134">C#</span><span class="sxs-lookup"><span data-stu-id="696ef-134">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="696ef-135">TypeScript</span><span class="sxs-lookup"><span data-stu-id="696ef-135">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]
---


## <a name="delete-an-entity"></a><span data-ttu-id="696ef-136">删除实体</span><span class="sxs-lookup"><span data-stu-id="696ef-136">Delete an entity</span></span>

<span data-ttu-id="696ef-137">若要删除实体，请采用与检索实体相同的方式构造*请求*。</span><span class="sxs-lookup"><span data-stu-id="696ef-137">To delete an entity, construct the *request* in the same way that you do to retrieve an entity.</span></span> <span data-ttu-id="696ef-138">*Request*对象上的*delete*方法指示要删除实体的愿望。</span><span class="sxs-lookup"><span data-stu-id="696ef-138">The *delete* method on the *request* object indicates the desire to delete the entity.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="696ef-139">C#</span><span class="sxs-lookup"><span data-stu-id="696ef-139">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="696ef-140">TypeScript</span><span class="sxs-lookup"><span data-stu-id="696ef-140">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]
---

## <a name="make-a-post-request-to-create-a-new-entity"></a><span data-ttu-id="696ef-141">发出 POST 请求以创建新实体</span><span class="sxs-lookup"><span data-stu-id="696ef-141">Make a POST request to create a new entity</span></span>

<span data-ttu-id="696ef-142">若要在集合中创建新实体，请调用`add`或`post`方法，并传入包含要用于创建新实体的信息的对象。</span><span class="sxs-lookup"><span data-stu-id="696ef-142">To create a new entity in a collection, call an `add` or `post` method and pass in an object that contains the information to be used to create the new entity.</span></span> <span data-ttu-id="696ef-143">创建的实体的更新版本通常是从调用返回的。</span><span class="sxs-lookup"><span data-stu-id="696ef-143">An updated version of the created entity is usually returned from the call.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="696ef-144">C#</span><span class="sxs-lookup"><span data-stu-id="696ef-144">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="696ef-145">TypeScript</span><span class="sxs-lookup"><span data-stu-id="696ef-145">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]
---

## <a name="updating-an-existing-entity-with-patch"></a><span data-ttu-id="696ef-146">使用修补程序更新现有实体</span><span class="sxs-lookup"><span data-stu-id="696ef-146">Updating an existing entity with PATCH</span></span>

<span data-ttu-id="696ef-147">Microsoft Graph 中的大多数更新都是使用`PATCH`方法执行的，因此只需在传递的对象中包含要更改的属性。</span><span class="sxs-lookup"><span data-stu-id="696ef-147">Most updates in Microsoft Graph are performed using a `PATCH` method and therefore it is only necessary to include the properties that you want to change in the object you pass.</span></span>  

# <a name="ctabcs"></a>[<span data-ttu-id="696ef-148">C#</span><span class="sxs-lookup"><span data-stu-id="696ef-148">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="696ef-149">TypeScript</span><span class="sxs-lookup"><span data-stu-id="696ef-149">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]
---


## <a name="use-http-headers-to-control-request-behavior"></a><span data-ttu-id="696ef-150">使用 HTTP 标头控制请求行为</span><span class="sxs-lookup"><span data-stu-id="696ef-150">Use HTTP headers to control request behavior</span></span>

<span data-ttu-id="696ef-151">您可以使用`header()`函数将自定义标头附加到请求。</span><span class="sxs-lookup"><span data-stu-id="696ef-151">You can use a `header()` function to attach custom headers to a request.</span></span> <span data-ttu-id="696ef-152">许多 Microsoft Graph 方案使用自定义标头来调整请求的行为。</span><span class="sxs-lookup"><span data-stu-id="696ef-152">A number of Microsoft Graph scenarios use custom headers to adjust the behavior of the request.</span></span>
 
# <a name="ctabcs"></a>[<span data-ttu-id="696ef-153">C#</span><span class="sxs-lookup"><span data-stu-id="696ef-153">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="696ef-154">TypeScript</span><span class="sxs-lookup"><span data-stu-id="696ef-154">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]
---

## <a name="provide-custom-query-parameters"></a><span data-ttu-id="696ef-155">提供自定义查询参数</span><span class="sxs-lookup"><span data-stu-id="696ef-155">Provide custom query parameters</span></span>

<span data-ttu-id="696ef-156">在 API 调用允许自定义查询参数的情况下，可以使用`QueryOptions`对象列表提供这些参数值。</span><span class="sxs-lookup"><span data-stu-id="696ef-156">In situations where an API call allows custom query parameters, you can provide those parameter values by using a list of `QueryOptions` objects.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="696ef-157">C#</span><span class="sxs-lookup"><span data-stu-id="696ef-157">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="696ef-158">TypeScript</span><span class="sxs-lookup"><span data-stu-id="696ef-158">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]
---
