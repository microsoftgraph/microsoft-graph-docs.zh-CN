---
title: todoTaskList： delta
description: 获取已添加、删除或删除的一组 todoTaskList 微软待办。
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ce5cc7202806b62afcc7f64bcd3b2393f2d31753
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048923"
---
# <a name="todotasklist-delta"></a><span data-ttu-id="9bdf7-103">todoTaskList： delta</span><span class="sxs-lookup"><span data-stu-id="9bdf7-103">todoTaskList: delta</span></span>

<span data-ttu-id="9bdf7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bdf7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bdf7-105">获取已添加、删除或删除的一组[todoTaskList](../resources/todotasklist.md)微软待办。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-105">Get a set of [todoTaskList](../resources/todotasklist.md) resources that have been added, deleted, or removed in Microsoft To Do.</span></span>

<span data-ttu-id="9bdf7-106">**todoTaskList** 的 **delta** 函数调用类似于 GET 请求，只不过通过在这些调用中的一 [](/graph/delta-query-overview)个或多个调用中正确应用状态令牌，您可以查询 **todoTaskList** 中的增量更改。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-106">A **delta** function call for **todoTaskList** is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the **todoTaskList**.</span></span> <span data-ttu-id="9bdf7-107">这样，您即可维护和同步用户的 **todoTaskList** 的本地存储，而无需每次从服务器获取所有 **todoTaskList。**</span><span class="sxs-lookup"><span data-stu-id="9bdf7-107">This allows you to maintain and synchronize a local store of a user's **todoTaskList** without having to fetch all the **todoTaskList** from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bdf7-108">权限</span><span class="sxs-lookup"><span data-stu-id="9bdf7-108">Permissions</span></span>
<span data-ttu-id="9bdf7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9bdf7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bdf7-111">Permission type</span></span>      | <span data-ttu-id="9bdf7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9bdf7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bdf7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bdf7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9bdf7-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bdf7-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9bdf7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bdf7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bdf7-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bdf7-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9bdf7-117">应用</span><span class="sxs-lookup"><span data-stu-id="9bdf7-117">Application</span></span> | <span data-ttu-id="9bdf7-118">不支持</span><span class="sxs-lookup"><span data-stu-id="9bdf7-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bdf7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bdf7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/delta
GET /users/{id|userPrincipalName}/todo/lists/delta
```

## <a name="query-parameters"></a><span data-ttu-id="9bdf7-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="9bdf7-120">Query parameters</span></span>

<span data-ttu-id="9bdf7-121">跟踪 **todoTaskList** 资源中的更改将引发一组 delta函数调用。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-121">Tracking changes in **todoTaskList** resources incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="9bdf7-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="9bdf7-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="9bdf7-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="9bdf7-125">在后续请求中，只需复制并应用上一响应中的 或 URL，因为此 URL 已包含所需的编码 `nextLink` `deltaLink` 参数。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-125">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="9bdf7-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="9bdf7-126">Query parameter</span></span>      | <span data-ttu-id="9bdf7-127">类型</span><span class="sxs-lookup"><span data-stu-id="9bdf7-127">Type</span></span>   |<span data-ttu-id="9bdf7-128">说明</span><span class="sxs-lookup"><span data-stu-id="9bdf7-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9bdf7-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="9bdf7-129">$deltatoken</span></span> | <span data-ttu-id="9bdf7-130">string</span><span class="sxs-lookup"><span data-stu-id="9bdf7-130">string</span></span> | <span data-ttu-id="9bdf7-131">对 [同](/graph/delta-query-overview)一 `deltaLink` **todoTaskList** 集合的上一 **个 delta** 函数调用的 URL 中返回的状态令牌，指示完成这一轮更改跟踪。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same **todoTaskList** collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="9bdf7-132">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="9bdf7-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="9bdf7-133">$skiptoken</span></span> | <span data-ttu-id="9bdf7-134">string</span><span class="sxs-lookup"><span data-stu-id="9bdf7-134">string</span></span> | <span data-ttu-id="9bdf7-135">之前的 [delta](/graph/delta-query-overview)函数调用的 URL 中返回的状态令牌，指示同一 `nextLink` **todoTaskList** 集合中还有进一步的更改需要跟踪。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same **todoTaskList** collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="9bdf7-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="9bdf7-136">OData query parameters</span></span>

<span data-ttu-id="9bdf7-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="9bdf7-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bdf7-139">Request headers</span></span>
| <span data-ttu-id="9bdf7-140">名称</span><span class="sxs-lookup"><span data-stu-id="9bdf7-140">Name</span></span>       | <span data-ttu-id="9bdf7-141">类型</span><span class="sxs-lookup"><span data-stu-id="9bdf7-141">Type</span></span> | <span data-ttu-id="9bdf7-142">说明</span><span class="sxs-lookup"><span data-stu-id="9bdf7-142">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="9bdf7-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bdf7-143">Authorization</span></span>  | <span data-ttu-id="9bdf7-144">string</span><span class="sxs-lookup"><span data-stu-id="9bdf7-144">string</span></span>  | <span data-ttu-id="9bdf7-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9bdf7-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9bdf7-147">Content-Type</span></span>  | <span data-ttu-id="9bdf7-148">string</span><span class="sxs-lookup"><span data-stu-id="9bdf7-148">string</span></span>  | <span data-ttu-id="9bdf7-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9bdf7-p107">application/json. Required.</span></span> |
| <span data-ttu-id="9bdf7-151">Prefer</span><span class="sxs-lookup"><span data-stu-id="9bdf7-151">Prefer</span></span> | <span data-ttu-id="9bdf7-152">string</span><span class="sxs-lookup"><span data-stu-id="9bdf7-152">string</span></span>  | <span data-ttu-id="9bdf7-p108">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9bdf7-155">响应</span><span class="sxs-lookup"><span data-stu-id="9bdf7-155">Response</span></span>

<span data-ttu-id="9bdf7-156">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [todoTaskList](../resources/todotasklist.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-156">If successful, this method returns a `200 OK` response code and [todoTaskList](../resources/todotasklist.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bdf7-157">示例</span><span class="sxs-lookup"><span data-stu-id="9bdf7-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="9bdf7-158">请求</span><span class="sxs-lookup"><span data-stu-id="9bdf7-158">Request</span></span>
<span data-ttu-id="9bdf7-159">以下示例演示如何进行初始 **delta** 函数调用，将响应正文中 **todoTaskList** 的最大数目限制为 2。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-159">The following example shows how to make an initial **delta** function call, and limit the maximum number of **todoTaskList** in the response body to 2.</span></span>

<span data-ttu-id="9bdf7-160">若要跟踪 **todoTaskList** 中的更改，可以使用适当的状态令牌进行一次或多次 **delta** 函数调用，获取自上次 delta 查询以来的增量更改集。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-160">To track changes in the **todoTaskList**, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="9bdf7-161">跟踪 **todoTaskList** 和跟踪列表中的 **todoTask** 资源之间的主要区别是 delta 查询请求 URL，查询响应返回 **todoTaskList** 而不是 **todoTask 集合** 。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-161">The main differences between tracking **todoTaskList** and tracking **todoTask** resources in a list are in the delta query request URLs, and the query responses returning **todoTaskList** rather than **todoTask** collections.</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/delta
Prefer: odata.maxpagesize=2
```
### <a name="response"></a><span data-ttu-id="9bdf7-162">响应</span><span class="sxs-lookup"><span data-stu-id="9bdf7-162">Response</span></span>

<span data-ttu-id="9bdf7-163">如果请求成功，响应将包含一个状态令牌，其为 _skipToken_</span><span class="sxs-lookup"><span data-stu-id="9bdf7-163">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="9bdf7-p109">（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-p109">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="9bdf7-166">以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-166">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="9bdf7-167">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9bdf7-167">Note: The response object shown here might be shortened for readability.</span></span>

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
         "id":"AQMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZD"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="9bdf7-168">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9bdf7-168">See also</span></span>

- [<span data-ttu-id="9bdf7-169">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="9bdf7-169">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)

