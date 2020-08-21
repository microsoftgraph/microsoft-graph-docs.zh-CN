---
title: todoTaskList： delta
description: 获取一组在 Microsoft To Do 中已添加、删除或删除的 todoTaskList 资源。
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b5d3acdc5b4b052744c26e95564c0e5abe1660ca
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849883"
---
# <a name="todotasklist-delta"></a><span data-ttu-id="cdca2-103">todoTaskList： delta</span><span class="sxs-lookup"><span data-stu-id="cdca2-103">todoTaskList: delta</span></span>

<span data-ttu-id="cdca2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdca2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdca2-105">获取一组在 Microsoft To Do 中已添加、删除或删除的 [todoTaskList](../resources/todotasklist.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="cdca2-105">Get a set of [todoTaskList](../resources/todotasklist.md) resources that have been added, deleted, or removed in Microsoft To Do.</span></span>

<span data-ttu-id="cdca2-106">**todoTaskList**的**delta**函数调用与 GET 请求相似，但通过在这些调用中正确应用[状态](/graph/delta-query-overview)令牌除外，你可以在**todoTaskList 中查询增量更改**。</span><span class="sxs-lookup"><span data-stu-id="cdca2-106">A **delta** function call for **todoTaskList** is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the **todoTaskList**.</span></span> <span data-ttu-id="cdca2-107">这允许你维护和同步用户的**todoTaskList**的本地存储，而无需每次都**从服务器中获取所有 todoTaskList。**</span><span class="sxs-lookup"><span data-stu-id="cdca2-107">This allows you to maintain and synchronize a local store of a user's **todoTaskList** without having to fetch all the **todoTaskList** from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdca2-108">权限</span><span class="sxs-lookup"><span data-stu-id="cdca2-108">Permissions</span></span>
<span data-ttu-id="cdca2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdca2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cdca2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdca2-111">Permission type</span></span>      | <span data-ttu-id="cdca2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdca2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdca2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdca2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cdca2-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdca2-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cdca2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdca2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdca2-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdca2-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cdca2-117">应用</span><span class="sxs-lookup"><span data-stu-id="cdca2-117">Application</span></span> | <span data-ttu-id="cdca2-118">不支持</span><span class="sxs-lookup"><span data-stu-id="cdca2-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdca2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdca2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/delta
GET /users/{id|userPrincipalName}/todo/lists/delta
```

## <a name="query-parameters"></a><span data-ttu-id="cdca2-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="cdca2-120">Query parameters</span></span>

<span data-ttu-id="cdca2-121">跟踪 **todoTaskList 资源更改** 会使用一个或多个 **delta 函数** 调用。</span><span class="sxs-lookup"><span data-stu-id="cdca2-121">Tracking changes in **todoTaskList** resources incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="cdca2-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="cdca2-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="cdca2-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="cdca2-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="cdca2-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="cdca2-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="cdca2-125">在后续请求中，只需复制并应用之前响应中的或 `nextLink` `deltaLink` URL，因为此 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="cdca2-125">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="cdca2-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="cdca2-126">Query parameter</span></span>      | <span data-ttu-id="cdca2-127">类型</span><span class="sxs-lookup"><span data-stu-id="cdca2-127">Type</span></span>   |<span data-ttu-id="cdca2-128">说明</span><span class="sxs-lookup"><span data-stu-id="cdca2-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cdca2-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="cdca2-129">$deltatoken</span></span> | <span data-ttu-id="cdca2-130">string</span><span class="sxs-lookup"><span data-stu-id="cdca2-130">string</span></span> | <span data-ttu-id="cdca2-131">在[针对同](/graph/delta-query-overview)一 `deltaLink` **todoTaskList**集合**的上一个 delta**函数调用的 URL 中返回的状态令牌，指示该组更改跟踪的完成状态。</span><span class="sxs-lookup"><span data-stu-id="cdca2-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same **todoTaskList** collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="cdca2-132">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="cdca2-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="cdca2-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="cdca2-133">$skiptoken</span></span> | <span data-ttu-id="cdca2-134">string</span><span class="sxs-lookup"><span data-stu-id="cdca2-134">string</span></span> | <span data-ttu-id="cdca2-135">在 [上一](/graph/delta-query-overview) `nextLink` **个 delta 函数调用** 的 URL 中返回的状态令牌，指示同一 **todoTaskList 集合中有进一步的** 更改需要跟踪。</span><span class="sxs-lookup"><span data-stu-id="cdca2-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same **todoTaskList** collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="cdca2-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="cdca2-136">OData query parameters</span></span>

<span data-ttu-id="cdca2-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="cdca2-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="cdca2-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdca2-139">Request headers</span></span>
| <span data-ttu-id="cdca2-140">名称</span><span class="sxs-lookup"><span data-stu-id="cdca2-140">Name</span></span>       | <span data-ttu-id="cdca2-141">类型</span><span class="sxs-lookup"><span data-stu-id="cdca2-141">Type</span></span> | <span data-ttu-id="cdca2-142">说明</span><span class="sxs-lookup"><span data-stu-id="cdca2-142">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="cdca2-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdca2-143">Authorization</span></span>  | <span data-ttu-id="cdca2-144">string</span><span class="sxs-lookup"><span data-stu-id="cdca2-144">string</span></span>  | <span data-ttu-id="cdca2-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cdca2-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cdca2-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdca2-147">Content-Type</span></span>  | <span data-ttu-id="cdca2-148">string</span><span class="sxs-lookup"><span data-stu-id="cdca2-148">string</span></span>  | <span data-ttu-id="cdca2-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cdca2-p107">application/json. Required.</span></span> |
| <span data-ttu-id="cdca2-151">Prefer</span><span class="sxs-lookup"><span data-stu-id="cdca2-151">Prefer</span></span> | <span data-ttu-id="cdca2-152">string</span><span class="sxs-lookup"><span data-stu-id="cdca2-152">string</span></span>  | <span data-ttu-id="cdca2-p108">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="cdca2-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="cdca2-155">响应</span><span class="sxs-lookup"><span data-stu-id="cdca2-155">Response</span></span>

<span data-ttu-id="cdca2-156">如果成功，此方法在响应 `200 OK` 正文中返回 [响应代码和 todoTaskList](../resources/todotasklist.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="cdca2-156">If successful, this method returns a `200 OK` response code and [todoTaskList](../resources/todotasklist.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdca2-157">示例</span><span class="sxs-lookup"><span data-stu-id="cdca2-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="cdca2-158">请求</span><span class="sxs-lookup"><span data-stu-id="cdca2-158">Request</span></span>
<span data-ttu-id="cdca2-159">以下示例演示了如何执行单 **一 delta** 函数调用，并将响应 **正文中的 todoTaskList** 最大数目限制为 2。</span><span class="sxs-lookup"><span data-stu-id="cdca2-159">The following example shows how to make a single **delta** function call, and limit the maximum number of **todoTaskList** in the response body to 2.</span></span>

<span data-ttu-id="cdca2-160">若要跟踪 **todoTaskList 中的更改**，要使用正确的状态令牌执行一次或多次 **delta** 函数调用来获取上次增量查询后的增量更改集。</span><span class="sxs-lookup"><span data-stu-id="cdca2-160">To track changes in the **todoTaskList**, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="cdca2-161">跟踪 **todoTaskList 和跟踪列表中的** **todoTask** 资源之间的主要差异在增量查询请求 URL 中，查询响应 **将返回 todoTaskList** 而不是 **todoTask** 集合中。</span><span class="sxs-lookup"><span data-stu-id="cdca2-161">The main differences between tracking **todoTaskList** and tracking **todoTask** resources in a list are in the delta query request URLs, and the query responses returning **todoTaskList** rather than **todoTask** collections.</span></span>

### <a name="http-request"></a><span data-ttu-id="cdca2-162">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdca2-162">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/delta?$skiptoken=l7WI41swwioT5csv4k99nvQqyku0jaGqMhc6XyFff5qQTQ7RJOr
Prefer: odata.maxpagesize=2
```
### <a name="response"></a><span data-ttu-id="cdca2-163">响应</span><span class="sxs-lookup"><span data-stu-id="cdca2-163">Response</span></span>

<span data-ttu-id="cdca2-164">如果请求成功，响应将包含一个状态令牌，其为 _skipToken_</span><span class="sxs-lookup"><span data-stu-id="cdca2-164">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="cdca2-p109">（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。</span><span class="sxs-lookup"><span data-stu-id="cdca2-p109">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="cdca2-167">以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。</span><span class="sxs-lookup"><span data-stu-id="cdca2-167">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="cdca2-p110">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cdca2-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/delta?$skiptoken=ldfdgdgfoT5csv4k99nvQqyku0jaGqMhc6XyFff5qQTQ7RJOr",
  "value": [
    {
      "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ93w==\"",
         "displayName":"List1",
         "isOwner":true,
         "isShared":false,
         "wellknownListName":"none",
         "id":"AQMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZD
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="cdca2-170">另请参阅</span><span class="sxs-lookup"><span data-stu-id="cdca2-170">See also</span></span>

- [<span data-ttu-id="cdca2-171">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="cdca2-171">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)