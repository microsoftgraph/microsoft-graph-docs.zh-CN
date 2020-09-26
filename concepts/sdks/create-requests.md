---
title: 使用 Microsoft Graph Sdk 进行 API 调用
description: 提供有关使用 Sdk 创建 Microsoft Graph HTTP 请求的说明。
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 1338cbe7411a3643eaa5c1e1e58cf8d5b9b47c0a
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288281"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a><span data-ttu-id="ead68-103">使用 Microsoft Graph Sdk 进行 API 调用</span><span class="sxs-lookup"><span data-stu-id="ead68-103">Make API calls using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="ead68-104">Microsoft Graph SDK 服务库提供了一个客户端类，您可以将其用作创建所有 API 请求的起始点。</span><span class="sxs-lookup"><span data-stu-id="ead68-104">The Microsoft Graph SDK service libraries provide a client class that you can use as the starting point for creating all API requests.</span></span> <span data-ttu-id="ead68-105">有两种类型的客户端类：一种是使用流畅的接口来创建请求 (例如， `client.Users["user-id"].Manager`) ，另一种是接受路径字符串 (例如， `api("/users/user-id/manager")`) 。</span><span class="sxs-lookup"><span data-stu-id="ead68-105">There are two styles of client class: one uses a fluent interface to create the request (for example, `client.Users["user-id"].Manager`) and the other accepts a path string (for example, `api("/users/user-id/manager")`).</span></span> <span data-ttu-id="ead68-106">当您拥有 request 对象时，可以指定各种选项（如筛选和排序），最后，选择要执行的操作的类型。</span><span class="sxs-lookup"><span data-stu-id="ead68-106">When you have a request object, you can specify a variety of options such as filtering and sorting, and finally, you select the type of operation you want to perform.</span></span>

<span data-ttu-id="ead68-107">还有 [Microsoft Graph POWERSHELL SDK](../powershell/get-started.md)，它根本没有客户端类。</span><span class="sxs-lookup"><span data-stu-id="ead68-107">There is also the [Microsoft Graph PowerShell SDK](../powershell/get-started.md), which has no client class at all.</span></span> <span data-ttu-id="ead68-108">相反，所有请求都表示为 PowerShell 命令。</span><span class="sxs-lookup"><span data-stu-id="ead68-108">Instead, all requests are represented as PowerShell commands.</span></span> <span data-ttu-id="ead68-109">例如，若要获取用户的经理，该命令是 `Get-MgUserManager` 。</span><span class="sxs-lookup"><span data-stu-id="ead68-109">For example, to get a user's manager, the command is `Get-MgUserManager`.</span></span> <span data-ttu-id="ead68-110">有关查找有关 API 调用的命令的详细信息，请参阅 [导航 Microsoft Graph POWERSHELL SDK](../powershell/navigating.md)。</span><span class="sxs-lookup"><span data-stu-id="ead68-110">For more information on finding commands for API calls, see [Navigating the Microsoft Graph PowerShell SDK](../powershell/navigating.md).</span></span>

## <a name="read-information-from-microsoft-graph"></a><span data-ttu-id="ead68-111">阅读 Microsoft Graph 中的信息</span><span class="sxs-lookup"><span data-stu-id="ead68-111">Read information from Microsoft Graph</span></span>

<span data-ttu-id="ead68-112">若要从 Microsoft Graph 读取信息，首先需要创建 request 对象，然后 `GET` 对该请求运行方法。</span><span class="sxs-lookup"><span data-stu-id="ead68-112">To read information from Microsoft Graph, you first need to create a request object and then run the `GET` method on the request.</span></span>

# <a name="c"></a>[<span data-ttu-id="ead68-113">C#</span><span class="sxs-lookup"><span data-stu-id="ead68-113">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[<span data-ttu-id="ead68-114">TypeScript</span><span class="sxs-lookup"><span data-stu-id="ead68-114">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="java"></a>[<span data-ttu-id="ead68-115">Java</span><span class="sxs-lookup"><span data-stu-id="ead68-115">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-read.md)]

# <a name="powershell"></a>[<span data-ttu-id="ead68-116">PowerShell</span><span class="sxs-lookup"><span data-stu-id="ead68-116">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a><span data-ttu-id="ead68-117">使用 $select 控制返回的属性</span><span class="sxs-lookup"><span data-stu-id="ead68-117">Use $select to control the properties returned</span></span>

<span data-ttu-id="ead68-118">检索实体时，并不会自动检索所有属性;有时需要显式选择它们。</span><span class="sxs-lookup"><span data-stu-id="ead68-118">When retrieving an entity, not all properties are automatically retrieved; sometimes they need to be explicitly selected.</span></span> <span data-ttu-id="ead68-119">此外，在某些情况下，无需返回默认的属性集。</span><span class="sxs-lookup"><span data-stu-id="ead68-119">Also, in some scenarios it isn't necessary to return the default set of properties.</span></span> <span data-ttu-id="ead68-120">仅选择所需的属性可提高请求的性能。</span><span class="sxs-lookup"><span data-stu-id="ead68-120">Selecting just the required properties can improve the performance of the request.</span></span> <span data-ttu-id="ead68-121">您可以自定义请求，以将 `$select` 查询参数包含在属性列表中。</span><span class="sxs-lookup"><span data-stu-id="ead68-121">You can customize the request to include the `$select` query parameter with a list of properties.</span></span>

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[<span data-ttu-id="ead68-122">C#</span><span class="sxs-lookup"><span data-stu-id="ead68-122">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[<span data-ttu-id="ead68-123">TypeScript</span><span class="sxs-lookup"><span data-stu-id="ead68-123">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="java"></a>[<span data-ttu-id="ead68-124">Java</span><span class="sxs-lookup"><span data-stu-id="ead68-124">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-select.md)]

# <a name="powershell"></a>[<span data-ttu-id="ead68-125">PowerShell</span><span class="sxs-lookup"><span data-stu-id="ead68-125">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a><span data-ttu-id="ead68-126">检索实体列表</span><span class="sxs-lookup"><span data-stu-id="ead68-126">Retrieve a list of entities</span></span>

<span data-ttu-id="ead68-127">检索实体列表与检索单个实体类似，但有许多其他选项可用于配置请求。</span><span class="sxs-lookup"><span data-stu-id="ead68-127">Retrieving a list of entities is similar to retrieving a single entity except there a number of other options for configuring the request.</span></span> <span data-ttu-id="ead68-128">`$filter`查询参数可用于将结果集减少为与提供的条件匹配的那些行。</span><span class="sxs-lookup"><span data-stu-id="ead68-128">The `$filter` query parameter can be used to reduce the result set to only those rows that match the provided condition.</span></span>  <span data-ttu-id="ead68-129">`$orderBy`查询参数将请求服务器提供按指定属性排序的实体列表。</span><span class="sxs-lookup"><span data-stu-id="ead68-129">The `$orderBy` query parameter will request that the server provide the list of entities sorted by the specified properties.</span></span>

# <a name="c"></a>[<span data-ttu-id="ead68-130">C#</span><span class="sxs-lookup"><span data-stu-id="ead68-130">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[<span data-ttu-id="ead68-131">TypeScript</span><span class="sxs-lookup"><span data-stu-id="ead68-131">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="java"></a>[<span data-ttu-id="ead68-132">Java</span><span class="sxs-lookup"><span data-stu-id="ead68-132">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-list.md)]

# <a name="powershell"></a>[<span data-ttu-id="ead68-133">PowerShell</span><span class="sxs-lookup"><span data-stu-id="ead68-133">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

---

<span data-ttu-id="ead68-134">检索实体列表时返回的对象可能是分页的集合。</span><span class="sxs-lookup"><span data-stu-id="ead68-134">The object returned when retrieving a list of entities is likely to be a paged collection.</span></span> <span data-ttu-id="ead68-135">有关如何获取实体的完整列表的详细信息，请参阅 [通过集合进行分页](../paging.md)。</span><span class="sxs-lookup"><span data-stu-id="ead68-135">For details about how to get the complete list of entities, see [paging through a collection](../paging.md).</span></span>

## <a name="access-an-item-of-a-collection"></a><span data-ttu-id="ead68-136">访问集合中的项</span><span class="sxs-lookup"><span data-stu-id="ead68-136">Access an item of a collection</span></span>

<span data-ttu-id="ead68-137">对于支持流畅样式的 Sdk，可以使用数组索引访问实体的集合。</span><span class="sxs-lookup"><span data-stu-id="ead68-137">For SDKs that support a fluent style, collections of entities can be accessed using an array index.</span></span> <span data-ttu-id="ead68-138">对于基于模板的 Sdk，足以将项标识符嵌入到集合后面的路径段中。</span><span class="sxs-lookup"><span data-stu-id="ead68-138">For template-based SDKs, it is sufficient to embed the item identifier in the path segment following the collection.</span></span> <span data-ttu-id="ead68-139">对于 PowerShell，标识符作为参数传递。</span><span class="sxs-lookup"><span data-stu-id="ead68-139">For PowerShell, identifiers are passed as parameters.</span></span>

# <a name="c"></a>[<span data-ttu-id="ead68-140">C#</span><span class="sxs-lookup"><span data-stu-id="ead68-140">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[<span data-ttu-id="ead68-141">TypeScript</span><span class="sxs-lookup"><span data-stu-id="ead68-141">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="java"></a>[<span data-ttu-id="ead68-142">Java</span><span class="sxs-lookup"><span data-stu-id="ead68-142">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-index.md)]

# <a name="powershell"></a>[<span data-ttu-id="ead68-143">PowerShell</span><span class="sxs-lookup"><span data-stu-id="ead68-143">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a><span data-ttu-id="ead68-144">使用 $expand 访问相关实体</span><span class="sxs-lookup"><span data-stu-id="ead68-144">Use $expand to access related entities</span></span>

<span data-ttu-id="ead68-145">您可以使用 `$expand` 筛选器请求与您请求主实体的相关实体或实体集合。</span><span class="sxs-lookup"><span data-stu-id="ead68-145">You can use the `$expand` filter to request a related entity, or collection of entities, at the same that you request the main entity.</span></span>

# <a name="c"></a>[<span data-ttu-id="ead68-146">C#</span><span class="sxs-lookup"><span data-stu-id="ead68-146">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[<span data-ttu-id="ead68-147">TypeScript</span><span class="sxs-lookup"><span data-stu-id="ead68-147">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="java"></a>[<span data-ttu-id="ead68-148">Java</span><span class="sxs-lookup"><span data-stu-id="ead68-148">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-expand.md)]

# <a name="powershell"></a>[<span data-ttu-id="ead68-149">PowerShell</span><span class="sxs-lookup"><span data-stu-id="ead68-149">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a><span data-ttu-id="ead68-150">删除实体</span><span class="sxs-lookup"><span data-stu-id="ead68-150">Delete an entity</span></span>

<span data-ttu-id="ead68-151">删除请求的构造方式与检索实体的请求相同，但使用的 `DELETE` 是请求而不是 `GET` 。</span><span class="sxs-lookup"><span data-stu-id="ead68-151">Delete requests are constructed in the same way as requests to retrieve an entity, but use a `DELETE` request instead of a `GET`.</span></span>

# <a name="c"></a>[<span data-ttu-id="ead68-152">C#</span><span class="sxs-lookup"><span data-stu-id="ead68-152">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[<span data-ttu-id="ead68-153">TypeScript</span><span class="sxs-lookup"><span data-stu-id="ead68-153">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="java"></a>[<span data-ttu-id="ead68-154">Java</span><span class="sxs-lookup"><span data-stu-id="ead68-154">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-delete.md)]

# <a name="powershell"></a>[<span data-ttu-id="ead68-155">PowerShell</span><span class="sxs-lookup"><span data-stu-id="ead68-155">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a><span data-ttu-id="ead68-156">发出 POST 请求以创建新实体</span><span class="sxs-lookup"><span data-stu-id="ead68-156">Make a POST request to create a new entity</span></span>

<span data-ttu-id="ead68-157">对于支持流畅样式的 Sdk，可以使用方法将新项目添加到集合中 `Add` 。</span><span class="sxs-lookup"><span data-stu-id="ead68-157">For SDKs that support a fluent style, new items can be added to collections with an `Add` method.</span></span> <span data-ttu-id="ead68-158">对于基于模板的 Sdk，request 对象公开了一个 `post` 方法。</span><span class="sxs-lookup"><span data-stu-id="ead68-158">For template-based SDKs, the request object exposes a `post` method.</span></span> <span data-ttu-id="ead68-159">对于 PowerShell， `New-*` 可以使用可接受映射到要添加的实体的参数的命令。</span><span class="sxs-lookup"><span data-stu-id="ead68-159">For PowerShell, a `New-*` command is available that accepts parameters that map to the entity to add.</span></span> <span data-ttu-id="ead68-160">创建的实体通常是从调用返回的。</span><span class="sxs-lookup"><span data-stu-id="ead68-160">The created entity is usually returned from the call.</span></span>

# <a name="c"></a>[<span data-ttu-id="ead68-161">C#</span><span class="sxs-lookup"><span data-stu-id="ead68-161">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[<span data-ttu-id="ead68-162">TypeScript</span><span class="sxs-lookup"><span data-stu-id="ead68-162">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="java"></a>[<span data-ttu-id="ead68-163">Java</span><span class="sxs-lookup"><span data-stu-id="ead68-163">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-create.md)]

# <a name="powershell"></a>[<span data-ttu-id="ead68-164">PowerShell</span><span class="sxs-lookup"><span data-stu-id="ead68-164">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a><span data-ttu-id="ead68-165">使用修补程序更新现有实体</span><span class="sxs-lookup"><span data-stu-id="ead68-165">Updating an existing entity with PATCH</span></span>

<span data-ttu-id="ead68-166">Microsoft Graph 中的大多数更新都是使用 `PATCH` 方法执行的，因此只需在传递的对象中包含要更改的属性。</span><span class="sxs-lookup"><span data-stu-id="ead68-166">Most updates in Microsoft Graph are performed using a `PATCH` method and therefore it is only necessary to include the properties that you want to change in the object you pass.</span></span>

# <a name="c"></a>[<span data-ttu-id="ead68-167">C#</span><span class="sxs-lookup"><span data-stu-id="ead68-167">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[<span data-ttu-id="ead68-168">TypeScript</span><span class="sxs-lookup"><span data-stu-id="ead68-168">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="java"></a>[<span data-ttu-id="ead68-169">Java</span><span class="sxs-lookup"><span data-stu-id="ead68-169">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-update.md)]

# <a name="powershell"></a>[<span data-ttu-id="ead68-170">PowerShell</span><span class="sxs-lookup"><span data-stu-id="ead68-170">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a><span data-ttu-id="ead68-171">使用 HTTP 标头控制请求行为</span><span class="sxs-lookup"><span data-stu-id="ead68-171">Use HTTP headers to control request behavior</span></span>

<span data-ttu-id="ead68-172">您可以使用 `Header()` 函数将自定义标头附加到请求。</span><span class="sxs-lookup"><span data-stu-id="ead68-172">You can use a `Header()` function to attach custom headers to a request.</span></span> <span data-ttu-id="ead68-173">对于 PowerShell，仅在使用方法时才可以添加标头 `Invoke-GraphRequest` 。</span><span class="sxs-lookup"><span data-stu-id="ead68-173">For PowerShell, adding headers is only possible with the `Invoke-GraphRequest` method.</span></span> <span data-ttu-id="ead68-174">许多 Microsoft Graph 方案使用自定义标头来调整请求的行为。</span><span class="sxs-lookup"><span data-stu-id="ead68-174">A number of Microsoft Graph scenarios use custom headers to adjust the behavior of the request.</span></span>

# <a name="c"></a>[<span data-ttu-id="ead68-175">C#</span><span class="sxs-lookup"><span data-stu-id="ead68-175">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[<span data-ttu-id="ead68-176">TypeScript</span><span class="sxs-lookup"><span data-stu-id="ead68-176">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="java"></a>[<span data-ttu-id="ead68-177">Java</span><span class="sxs-lookup"><span data-stu-id="ead68-177">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-headers.md)]

# <a name="powershell"></a>[<span data-ttu-id="ead68-178">PowerShell</span><span class="sxs-lookup"><span data-stu-id="ead68-178">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a><span data-ttu-id="ead68-179">提供自定义查询参数</span><span class="sxs-lookup"><span data-stu-id="ead68-179">Provide custom query parameters</span></span>

<span data-ttu-id="ead68-180">对于支持流畅样式的 Sdk，可以使用对象列表提供自定义查询参数值 `QueryOptions` 。</span><span class="sxs-lookup"><span data-stu-id="ead68-180">For SDKs that support a fluent style, you can provide custom query parameter values by using a list of `QueryOptions` objects.</span></span> <span data-ttu-id="ead68-181">对于基于模板的 Sdk，参数是 URL 编码的，并添加到请求 URI。</span><span class="sxs-lookup"><span data-stu-id="ead68-181">For template-based SDKs, the parameters are URL-encoded and added to the request URI.</span></span> <span data-ttu-id="ead68-182">对于 PowerShell，为给定 API 定义的查询参数作为参数公开给相应的命令。</span><span class="sxs-lookup"><span data-stu-id="ead68-182">For PowerShell, defined query parameters for a given API are exposed as parameters to the corresponding command.</span></span>

# <a name="c"></a>[<span data-ttu-id="ead68-183">C#</span><span class="sxs-lookup"><span data-stu-id="ead68-183">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[<span data-ttu-id="ead68-184">TypeScript</span><span class="sxs-lookup"><span data-stu-id="ead68-184">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="java"></a>[<span data-ttu-id="ead68-185">Java</span><span class="sxs-lookup"><span data-stu-id="ead68-185">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-queryparams.md)]

# <a name="powershell"></a>[<span data-ttu-id="ead68-186">PowerShell</span><span class="sxs-lookup"><span data-stu-id="ead68-186">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

---
