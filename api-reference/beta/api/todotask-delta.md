---
title: todoTask： delta
description: 获取一组指定 todoTaskList 中已添加、删除或更新的 todoTask 资源。
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3c0d1759d1994c1fa9ae405d2a1895982e3ac99a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048916"
---
# <a name="todotask-delta"></a><span data-ttu-id="1b27c-103">todoTask： delta</span><span class="sxs-lookup"><span data-stu-id="1b27c-103">todoTask: delta</span></span>

<span data-ttu-id="1b27c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b27c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b27c-105">获取一组 [指定 todoTaskList](../resources/todotask.md) 中已添加、删除或更新的 [todoTask 资源](../resources/todotasklist.md)。</span><span class="sxs-lookup"><span data-stu-id="1b27c-105">Get a set of [todoTask](../resources/todotask.md) resources that have been added, deleted, or updated in a specified [todoTaskList](../resources/todotasklist.md).</span></span>

<span data-ttu-id="1b27c-106">**todoTaskList** 中 **todoTask** 资源的 **delta** 函数调用类似于 GET 请求，只不过通过在这些调用的一 [](/graph/delta-query-overview)个或多个调用中正确应用状态令牌，您可以在 **todoTaskList** 中查询 **todoTask** 中的增量更改。</span><span class="sxs-lookup"><span data-stu-id="1b27c-106">A **delta** function call for **todoTask** resources in a **todoTaskList** is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the **todoTask** in that **todoTaskList**.</span></span> <span data-ttu-id="1b27c-107">这样，您即可维护和同步用户 **todoTask** 资源的本地存储，而无需每次从服务器提取整个集合。</span><span class="sxs-lookup"><span data-stu-id="1b27c-107">This allows you to maintain and synchronize a local store of a user's **todoTask** resources without having to fetch the entire set from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="1b27c-108">权限</span><span class="sxs-lookup"><span data-stu-id="1b27c-108">Permissions</span></span>
<span data-ttu-id="1b27c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b27c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b27c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b27c-111">Permission type</span></span>      | <span data-ttu-id="1b27c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b27c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b27c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b27c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1b27c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b27c-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1b27c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b27c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b27c-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b27c-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1b27c-117">应用</span><span class="sxs-lookup"><span data-stu-id="1b27c-117">Application</span></span> | <span data-ttu-id="1b27c-118">不支持</span><span class="sxs-lookup"><span data-stu-id="1b27c-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b27c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b27c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/{id}/tasks/delta
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/delta
```

## <a name="query-parameters"></a><span data-ttu-id="1b27c-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="1b27c-120">Query parameters</span></span>

<span data-ttu-id="1b27c-121">跟踪 **todoTask 集合** 中的更改会导致一次或多组 **delta** 函数调用。</span><span class="sxs-lookup"><span data-stu-id="1b27c-121">Tracking changes in a **todoTask** collection incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="1b27c-122">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="1b27c-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="1b27c-123">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="1b27c-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="1b27c-124">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="1b27c-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="1b27c-125">在后续请求中，只需复制并应用上一响应中的 或 URL，因为此 URL 已包含所需的编码 `nextLink` `deltaLink` 参数。</span><span class="sxs-lookup"><span data-stu-id="1b27c-125">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="1b27c-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="1b27c-126">Query parameter</span></span>      | <span data-ttu-id="1b27c-127">类型</span><span class="sxs-lookup"><span data-stu-id="1b27c-127">Type</span></span>   |<span data-ttu-id="1b27c-128">说明</span><span class="sxs-lookup"><span data-stu-id="1b27c-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1b27c-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="1b27c-129">$deltatoken</span></span> | <span data-ttu-id="1b27c-130">string</span><span class="sxs-lookup"><span data-stu-id="1b27c-130">string</span></span> | <span data-ttu-id="1b27c-131">对[同](/graph/delta-query-overview)一 todoTask 集合的上一个 delta 函数调用的 URL 中返回的状态令牌，指示完成这一轮 `deltaLink` 更改跟踪。 </span><span class="sxs-lookup"><span data-stu-id="1b27c-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same todoTask collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="1b27c-132">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="1b27c-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="1b27c-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="1b27c-133">$skiptoken</span></span> | <span data-ttu-id="1b27c-134">string</span><span class="sxs-lookup"><span data-stu-id="1b27c-134">string</span></span> | <span data-ttu-id="1b27c-135">之前的[delta](/graph/delta-query-overview)函数调用的 URL 中返回的状态令牌，指示同一 todoTask 集合中还有进一步 `nextLink` 的更改需要跟踪。 </span><span class="sxs-lookup"><span data-stu-id="1b27c-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same todoTask collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="1b27c-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="1b27c-136">OData query parameters</span></span>

- <span data-ttu-id="1b27c-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="1b27c-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="1b27c-139">Delta 查询支持 `$select` 、 `$top` 和 `$expand` todoTask。</span><span class="sxs-lookup"><span data-stu-id="1b27c-139">Delta query support `$select`, `$top`, and `$expand` for todoTask.</span></span> 
- <span data-ttu-id="1b27c-140">提供对 `$filter` 和 `$orderby` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="1b27c-140">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="1b27c-141">唯一支持的 `$filter` 表达式是 `$filter=receivedDateTime+ge+{value}` 或 `$filter=receivedDateTime+gt+{value}`。</span><span class="sxs-lookup"><span data-stu-id="1b27c-141">The only supported `$filter` expressions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="1b27c-p106">唯一支持的 `$orderby` 表达式是 `$orderby=receivedDateTime+desc`。如果不包含 `$orderby` 表达式，则不能保证返回顺序。</span><span class="sxs-lookup"><span data-stu-id="1b27c-p106">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="1b27c-144">不支持 `$search`。</span><span class="sxs-lookup"><span data-stu-id="1b27c-144">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b27c-145">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b27c-145">Request headers</span></span>
| <span data-ttu-id="1b27c-146">名称</span><span class="sxs-lookup"><span data-stu-id="1b27c-146">Name</span></span>       | <span data-ttu-id="1b27c-147">类型</span><span class="sxs-lookup"><span data-stu-id="1b27c-147">Type</span></span> | <span data-ttu-id="1b27c-148">说明</span><span class="sxs-lookup"><span data-stu-id="1b27c-148">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="1b27c-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b27c-149">Authorization</span></span>  | <span data-ttu-id="1b27c-150">string</span><span class="sxs-lookup"><span data-stu-id="1b27c-150">string</span></span>  | <span data-ttu-id="1b27c-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b27c-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b27c-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b27c-153">Content-Type</span></span>  | <span data-ttu-id="1b27c-154">string</span><span class="sxs-lookup"><span data-stu-id="1b27c-154">string</span></span>  | <span data-ttu-id="1b27c-p108">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1b27c-p108">application/json. Required.</span></span> |
| <span data-ttu-id="1b27c-157">Prefer</span><span class="sxs-lookup"><span data-stu-id="1b27c-157">Prefer</span></span> | <span data-ttu-id="1b27c-158">string</span><span class="sxs-lookup"><span data-stu-id="1b27c-158">string</span></span>  | <span data-ttu-id="1b27c-p109">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="1b27c-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1b27c-161">响应</span><span class="sxs-lookup"><span data-stu-id="1b27c-161">Response</span></span>

<span data-ttu-id="1b27c-162">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [todoTask](../resources/todotask.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="1b27c-162">If successful, this method returns a `200 OK` response code and [todoTask](../resources/todotask.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b27c-163">示例</span><span class="sxs-lookup"><span data-stu-id="1b27c-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b27c-164">请求</span><span class="sxs-lookup"><span data-stu-id="1b27c-164">Request</span></span>
<span data-ttu-id="1b27c-165">若要跟踪自上一轮更改跟踪以来 **todoTaskList** 中 **todoTask** 资源的变化，需要执行一次或多个 **delta** 函数调用，获取增量更改集。</span><span class="sxs-lookup"><span data-stu-id="1b27c-165">To track changes in the **todoTask** resources in a **todoTaskList** since the last round of change tracking, you would make one or more **delta** function calls to get the set of incremental changes.</span></span> <span data-ttu-id="1b27c-166">以下示例显示如何使用 上一轮的最后一个 delta 函数调用返回的 URL 开始下一轮更改跟踪，其中包含 `deltaLink`  `deltaToken` 。</span><span class="sxs-lookup"><span data-stu-id="1b27c-166">The following example shows how to begin a next round of change tracking, using the URL in the `deltaLink` returned from the last **delta** function call of the last round, which contains a `deltaToken`.</span></span> <span data-ttu-id="1b27c-167">此 **delta** 函数调用将响应正文 **中 todoTask** 的最大数目限制为 2。</span><span class="sxs-lookup"><span data-stu-id="1b27c-167">This **delta** function call limits the maximum number of **todoTask** in the response body to 2.</span></span>
 

### <a name="http-request"></a><span data-ttu-id="1b27c-168">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b27c-168">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=w0vf2jHg2mBXU-I2AK0FSWl0dopNtG8u5YoM
Prefer: odata.maxpagesize=2
```


### <a name="response"></a><span data-ttu-id="1b27c-169">响应</span><span class="sxs-lookup"><span data-stu-id="1b27c-169">Response</span></span>
<span data-ttu-id="1b27c-170">如果请求成功，响应将包含一个状态令牌，其为 _skipToken_</span><span class="sxs-lookup"><span data-stu-id="1b27c-170">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="1b27c-p111">（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。</span><span class="sxs-lookup"><span data-stu-id="1b27c-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="1b27c-173">以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。</span><span class="sxs-lookup"><span data-stu-id="1b27c-173">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="1b27c-174">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b27c-174">Note: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
   "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=MoVMZ_DzHG4AhT3WE8VioVS1IXZJ-ArqK5fknOjnKFY",
   "value":[
      {
         "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ9xQ==\"",
         "importance":"normal",
         "isReminderOn":false,
         "status":"notStarted",
         "title":"empty task3",
         "createdDateTime":"2020-08-12T04:54:29.1925206Z",
         "lastModifiedDateTime":"2020-08-12T04:54:29.4903939Z",
         "id":"AAMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZDEwMwBGAAAAAAB5M0K0qlJySLOAgV22zPnuBwDit9FUg_L0SpeANtzxTscbAAMNmhwmAADit9FUg_L0SpeANtzxTscbAAMxlnrYAAA=",
         "body":{
            "content":"",
            "contentType":"text"
         }
      }
   ]
}
```

## <a name="see-also"></a><span data-ttu-id="1b27c-175">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1b27c-175">See also</span></span>

- [<span data-ttu-id="1b27c-176">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="1b27c-176">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)

