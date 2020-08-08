---
title: 获取组的增量更改
description: 使用 delta 查询，可通过一系列 delta 函数调用来查询组的添加、删除或更新。 delta 查询可便于发现组的更改
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 947ffe713d02eb55d8fa2630ad31406ef84e70fc
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598253"
---
# <a name="get-incremental-changes-for-groups"></a><span data-ttu-id="02f25-104">获取组的增量更改</span><span class="sxs-lookup"><span data-stu-id="02f25-104">Get incremental changes for groups</span></span>

<span data-ttu-id="02f25-p102">[Delta 查询](./delta-query-overview.md)可通过调用一系列的 [delta](/graph/api/group-delta?view=graph-rest-1.0) 函数来查询组的添加、删除或更新。增量查询使你无需读取 Microsoft Graph 的整个组就能够发现组的更改并进行比较。</span><span class="sxs-lookup"><span data-stu-id="02f25-p102">[Delta query](./delta-query-overview.md) lets you query for additions, deletions, or updates to groups, by way of a series of [delta](/graph/api/group-delta?view=graph-rest-1.0) function calls. Delta query enables you discover changes to groups without having to fetch the entire set of groups from Microsoft Graph and compare changes.</span></span>

<span data-ttu-id="02f25-p103">以后，对本地配置文件存储使用同步组功能的客户端可以将增量查询用于初始完全同步和增量同步。通常，客户会对租户中的所有组进行初始完全同步，之后定期获取对组的增量更改。</span><span class="sxs-lookup"><span data-stu-id="02f25-p103">Clients using synchronizing groups with a local profile store can use Delta Query for both their initial full synchronization along with incremental synchronizations in the future. Typically, a client would do an initial full synchronization of all the groups in a tenant, and subsequently, get incremental changes to groups periodically.</span></span>

## <a name="tracking-group-changes"></a><span data-ttu-id="02f25-109">跟踪组更改</span><span class="sxs-lookup"><span data-stu-id="02f25-109">Tracking group changes</span></span>

<span data-ttu-id="02f25-p104">跟踪组更改是发出 **delta** 函数的一个或多个 GET 请求。发出 GET 请求与[列出组](/graph/api/group-list?view=graph-rest-1.0)的方式非常相似，除了要包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="02f25-p104">Tracking group changes is a round of one or more GET requests with the **delta** function. You make a GET request much like the way you [list groups](/graph/api/group-list?view=graph-rest-1.0), except that you include the following:</span></span>

- <span data-ttu-id="02f25-112">**delta** 函数。</span><span class="sxs-lookup"><span data-stu-id="02f25-112">The **delta** function.</span></span>
- <span data-ttu-id="02f25-113">上一个 GET **delta** 函数调用的[状态令牌](./delta-query-overview.md)（*deltaToken* 或 *skipToken*）。</span><span class="sxs-lookup"><span data-stu-id="02f25-113">A [state token](./delta-query-overview.md) (*deltaToken* or *skipToken*) from the previous GET **delta** function call.</span></span>

## <a name="example"></a><span data-ttu-id="02f25-114">示例</span><span class="sxs-lookup"><span data-stu-id="02f25-114">Example</span></span>

<span data-ttu-id="02f25-115">以下示例显示跟踪组更改的一系列请求：</span><span class="sxs-lookup"><span data-stu-id="02f25-115">The following example shows a series  requests to track changes to groups:</span></span>

1. <span data-ttu-id="02f25-116">[初始请求](#initial-request)和[响应](#initial-response)</span><span class="sxs-lookup"><span data-stu-id="02f25-116">[Initial request](#initial-request) and [response](#initial-response)</span></span>
2. <span data-ttu-id="02f25-117">[nextLink 请求](#nextlink-request)和[响应](#nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="02f25-117">[nextLink request](#nextlink-request) and [response](#nextlink-response)</span></span>
3. <span data-ttu-id="02f25-118">[最终 nextLink 请求](#final-nextlink-request)和[响应](#final-nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="02f25-118">[Final nextLink request](#final-nextlink-request) and [response](#final-nextlink-response)</span></span>
4. <span data-ttu-id="02f25-119">[deltaLink 请求](#deltalink-request)和 [deltaLink 响应](#deltalink-response)</span><span class="sxs-lookup"><span data-stu-id="02f25-119">[deltaLink request](#deltalink-request) and [deltaLink response](#deltalink-response)</span></span>

## <a name="initial-request"></a><span data-ttu-id="02f25-120">初始请求</span><span class="sxs-lookup"><span data-stu-id="02f25-120">Initial request</span></span>

<span data-ttu-id="02f25-121">为开始跟踪组资源的更改，请在组资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="02f25-121">To begin tracking changes in the group resource, you make a request including the delta function on the group resource.</span></span>

<span data-ttu-id="02f25-122">请注意以下几点：</span><span class="sxs-lookup"><span data-stu-id="02f25-122">Note the following:</span></span>

- <span data-ttu-id="02f25-123">请求中包含可选的 `$select` 查询参数，以演示如何在以后的请求中自动包含查询参数。</span><span class="sxs-lookup"><span data-stu-id="02f25-123">The optional `$select` query parameter is included in the request to demonstrate how query parameters are automatically included in future requests.</span></span>
- <span data-ttu-id="02f25-124">可选的 `$select` 查询参数还用于显示如何一起检索组成员和组对象。</span><span class="sxs-lookup"><span data-stu-id="02f25-124">The optional `$select` query parameter is also used to show how group members can be retrieved together with group objects.</span></span> <span data-ttu-id="02f25-125">这允许跟踪成员身份变更，例如当用户被添加到组或从组中删除时。</span><span class="sxs-lookup"><span data-stu-id="02f25-125">This allows tracking of membership changes, such as when users are added or removed from groups.</span></span>
- <span data-ttu-id="02f25-p106">初始请求不包括状态令牌。状态令牌将用于后续请求中。</span><span class="sxs-lookup"><span data-stu-id="02f25-p106">The initial request does not include a state token. State tokens will be used in subsequent requests.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

## <a name="initial-response"></a><span data-ttu-id="02f25-128">初始响应</span><span class="sxs-lookup"><span data-stu-id="02f25-128">Initial response</span></span>

<span data-ttu-id="02f25-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和[组](/graph/api/resources/group?view=graph-rest-1.0)集合对象。</span><span class="sxs-lookup"><span data-stu-id="02f25-129">If successful, this method returns `200 OK` response code and [group](/graph/api/resources/group?view=graph-rest-1.0) collection object in the response body.</span></span> <span data-ttu-id="02f25-130">如果整个组集过大而无法适应一个响应，那么还将包括一个包含状态令牌的 `nextLink`。</span><span class="sxs-lookup"><span data-stu-id="02f25-130">If the entire set of groups is too large to fit in one response, a `nextLink` containing a state token will also be included.</span></span>

<span data-ttu-id="02f25-131">此示例中包含 `nextLink`；原始 `$select` 查询参数则在状态令牌中进行了编码。</span><span class="sxs-lookup"><span data-stu-id="02f25-131">In this example, a `nextLink` was included; the original `$select` query parameter is encoded in the state token.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

><span data-ttu-id="02f25-132">**注意：**`members@delta` 属性包含在第一个组对象 (TestGroup1) 中，并包含此组的两个当前成员。</span><span class="sxs-lookup"><span data-stu-id="02f25-132">**Note:** The `members@delta` property is included in the first group object - TestGroup1 - and contains the two current members of the group.</span></span> <span data-ttu-id="02f25-133">TestGroup2 不包含此属性，因为组中没有任何成员。</span><span class="sxs-lookup"><span data-stu-id="02f25-133">TestGroup2 does not contain that property because the group does not have any members.</span></span>

## <a name="nextlink-request"></a><span data-ttu-id="02f25-134">nextLink 请求</span><span class="sxs-lookup"><span data-stu-id="02f25-134">nextLink request</span></span>

<span data-ttu-id="02f25-135">第二个请求使用上一个响应中的 `nextLink`，其中包含 `skipToken`。</span><span class="sxs-lookup"><span data-stu-id="02f25-135">The second request uses the `nextLink` from the previous response, which contains the `skipToken`.</span></span> <span data-ttu-id="02f25-136">请注意，`$select` 参数不显式出现，因为它在令牌中编码。</span><span class="sxs-lookup"><span data-stu-id="02f25-136">Notice the `$select` parameter is not explicitly present as it is encoded in the token.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a><span data-ttu-id="02f25-137">nextLink 响应</span><span class="sxs-lookup"><span data-stu-id="02f25-137">nextLink response</span></span>

<span data-ttu-id="02f25-138">该响应包含另一个带新 `skipToken` 值的 `nextLink`，它表示存在更多可用的组。</span><span class="sxs-lookup"><span data-stu-id="02f25-138">The response contains another `nextLink` with a new `skipToken` value, which indicates that more groups are available.</span></span> <span data-ttu-id="02f25-139">应使用 `nextLink` URL 继续发出请求，直到在最终响应中返回 `deltaLink` URL，即使该值为空数组（在某些情况下可能会出现此情况）。</span><span class="sxs-lookup"><span data-stu-id="02f25-139">You should continue making requests using the `nextLink` URL until a `deltaLink` URL is returned in the final response, even if the value is an empty array (this can happen under certain circumstances).</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "3c8ac7c4-d365-4df9-abfa-356a9dd7763c"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

## <a name="final-nextlink-request"></a><span data-ttu-id="02f25-140">最终 nextLink 请求</span><span class="sxs-lookup"><span data-stu-id="02f25-140">Final nextLink request</span></span>

<span data-ttu-id="02f25-141">第三个请求再次使用最新的 `nextLink`。</span><span class="sxs-lookup"><span data-stu-id="02f25-141">The third request again uses the latest `nextLink`.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a><span data-ttu-id="02f25-142">最终 nextLink 响应</span><span class="sxs-lookup"><span data-stu-id="02f25-142">Final nextLink response</span></span>

<span data-ttu-id="02f25-143">最后返回 `deltaLink` URL，这意味着没有更多数据反映现有的组状态。</span><span class="sxs-lookup"><span data-stu-id="02f25-143">Finally, the `deltaLink` URL is returned, which means there is no more data for the existing state of groups.</span></span> <span data-ttu-id="02f25-144">对于将来请求，应用程序将使用它所包含的 `deltaLink` 和 `deltaToken` 值来了解有关组的新更改。</span><span class="sxs-lookup"><span data-stu-id="02f25-144">For future requests, the application uses the `deltaLink` and the `deltaToken` value it contains to learn about new changes to groups.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup5",
      "description":"Employees in test group 5",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"TestGroup6",
      "description":"Employees in test group 6",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

## <a name="deltalink-request"></a><span data-ttu-id="02f25-145">deltaLink 请求</span><span class="sxs-lookup"><span data-stu-id="02f25-145">deltaLink request</span></span>

<span data-ttu-id="02f25-146">通过使用[上次响应](#final-nextlink-response)的 `deltaLink`，你将能够获取自上次请求以来对组所做的新更改。</span><span class="sxs-lookup"><span data-stu-id="02f25-146">Using the `deltaLink` from the [last response](#final-nextlink-response), you will be able to get net new changes to groups since the last request.</span></span> <span data-ttu-id="02f25-147">这些更改包括：</span><span class="sxs-lookup"><span data-stu-id="02f25-147">Changes include:</span></span>
- <span data-ttu-id="02f25-148">新创建的组对象。</span><span class="sxs-lookup"><span data-stu-id="02f25-148">Newly created group objects.</span></span>
- <span data-ttu-id="02f25-149">已删除的组对象。</span><span class="sxs-lookup"><span data-stu-id="02f25-149">Deleted group objects.</span></span>
- <span data-ttu-id="02f25-150">属性已更改的组对象（例如，修改了 **displayName**）。</span><span class="sxs-lookup"><span data-stu-id="02f25-150">Group objects for which a property has changed (e.g. **displayName** has been modified).</span></span>
- <span data-ttu-id="02f25-151">已为其添加或移除成员对象的组对象。</span><span class="sxs-lookup"><span data-stu-id="02f25-151">Group objects for which member objects have been added or removed.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a><span data-ttu-id="02f25-152">deltaLink 响应</span><span class="sxs-lookup"><span data-stu-id="02f25-152">deltaLink response</span></span>

<span data-ttu-id="02f25-153">如果未发生更改，则会返回 `deltaLink` 且无返回结果 - `value` 属性为空。</span><span class="sxs-lookup"><span data-stu-id="02f25-153">If no changes have occurred, a `deltaLink` is returned with no results - the `value` property is empty.</span></span> <span data-ttu-id="02f25-154">请确保将应用程序中的以前链接替换为新链接以便在日后调用中使用。</span><span class="sxs-lookup"><span data-stu-id="02f25-154">Make sure to replace the previous link in the application with the new one for use in future calls.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

<span data-ttu-id="02f25-155">如果发生更改，则包含已更改组的集合。</span><span class="sxs-lookup"><span data-stu-id="02f25-155">If changes have occurred, a collection of changed groups is included.</span></span> <span data-ttu-id="02f25-156">响应还包含 `nextLink` 或 `deltaLink`（如果要检索多个更改页面）。</span><span class="sxs-lookup"><span data-stu-id="02f25-156">The response also contains either a `nextLink` - in case there are multiple pages of changes to retrieve - or a `deltaLink`.</span></span> <span data-ttu-id="02f25-157">应像以前一样实现遵循 `nextLinks` 的相同模式，并保留最终的 `deltaLink` 供日后调用。</span><span class="sxs-lookup"><span data-stu-id="02f25-157">You should implement the same pattern of following the `nextLinks` as before and persist the final `deltaLink` for future calls.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
          {
              "displayName": "TestGroup3",
              "description": "A test group for change tracking",
              "id": "2e5807ce-58f3-4a94-9b37-ffff2e085957",
              "members@delta": [
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
                      "@removed": {
                          "reason": "deleted"
                      }
                  },
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "37de1ae3-408f-4702-8636-20824abda004"
                  }
              ]
          }
      ]
}
```

<span data-ttu-id="02f25-158">上面示例响应的一些注意事项如下：</span><span class="sxs-lookup"><span data-stu-id="02f25-158">Some things to note about the example response above:</span></span>

- <span data-ttu-id="02f25-159">这些对象连同一组相同的属性一起返回，这些属性最初通过 `$select` 查询参数指定。</span><span class="sxs-lookup"><span data-stu-id="02f25-159">The objects are returned with the same set of properties originally specified via the `$select` query parameter.</span></span>

- <span data-ttu-id="02f25-160">同时包括更改和未更改的属性。</span><span class="sxs-lookup"><span data-stu-id="02f25-160">Both changed and unchanged properties are included.</span></span> <span data-ttu-id="02f25-161">在上述示例中，`description` 属性具有新值，而 `displayName` 属性未发生更改。</span><span class="sxs-lookup"><span data-stu-id="02f25-161">In the example above, the `description` property has a new value, while the `displayName` property has not changed.</span></span>

- <span data-ttu-id="02f25-162">`members@delta` 包含对成员身份的任何更改。</span><span class="sxs-lookup"><span data-stu-id="02f25-162">`members@delta` contains any changes to membership.</span></span>

  - <span data-ttu-id="02f25-163">列表中的第一个用户已经从组中删除 - 要么删除成员身份，要么删除用户对象本身。</span><span class="sxs-lookup"><span data-stu-id="02f25-163">The first user in the list has been removed from the group - either by removing the membership or by deleting the user object itself.</span></span> <span data-ttu-id="02f25-164">`@removed` 属性对此进行了说明。</span><span class="sxs-lookup"><span data-stu-id="02f25-164">The `@removed` property describes that.</span></span> <span data-ttu-id="02f25-165">只有被永久删除的用户才会从组中删除。</span><span class="sxs-lookup"><span data-stu-id="02f25-165">Only users that have been permanently deleted are removed from groups.</span></span> <span data-ttu-id="02f25-166">临时删除的用户保留自己的组成员资格，除非被永久删除，否则不会显示在增量结果中。</span><span class="sxs-lookup"><span data-stu-id="02f25-166">Users that have been temporary deleted keep their group memberships and will not appear in the delta result until they are permanently deleted.</span></span> <span data-ttu-id="02f25-167">有关详细信息，请参阅[目录（已删除的项）](/graph/api/resources/directory?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="02f25-167">For details, see [directory (deleted items)](/graph/api/resources/directory?view=graph-rest-1.0).</span></span>

  - <span data-ttu-id="02f25-168">第二个用户已添加到组。</span><span class="sxs-lookup"><span data-stu-id="02f25-168">The second user has been added to the group.</span></span>

## <a name="paging-through-members-in-a-large-group"></a><span data-ttu-id="02f25-169">逐页查看大型组中的成员</span><span class="sxs-lookup"><span data-stu-id="02f25-169">Paging through members in a large group</span></span>

<span data-ttu-id="02f25-170">当未指定 `$select` 查询参数，或已显式指定 `$select=members` 参数时，`members@delta` 属性默认包含在组对象中。</span><span class="sxs-lookup"><span data-stu-id="02f25-170">The `members@delta` property is included in group objects by default, when the `$select` query parameter has not been specified, or when the `$select=members` parameter is explicitly specified.</span></span> <span data-ttu-id="02f25-171">对于包含许多成员的组来说，可能所有成员都无法适应单个响应；在本节中，我们将介绍为处理这种情况所应实现的模式。</span><span class="sxs-lookup"><span data-stu-id="02f25-171">For groups with many members it is possible that all members cannot fit into a single response; in this section we describe the pattern you should implement to handle such cases.</span></span>

><span data-ttu-id="02f25-172">**注意：** 此模式既适用于组状态的初始检索，也适用于后续调用，以获取增量更改。</span><span class="sxs-lookup"><span data-stu-id="02f25-172">**Note:** This pattern applies to both the initial retrieval of group state as well as to subsequent calls to get delta changes.</span></span>

<span data-ttu-id="02f25-173">假定正在执行以下增量查询 - 要捕获组的初始完整状态，或要在稍后获取增量更改：</span><span class="sxs-lookup"><span data-stu-id="02f25-173">Let's assume you are executing the following delta query - either to capture the initial full state of groups, or later on to get delta changes:</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

1. <span data-ttu-id="02f25-174">Microsoft Graph 可能返回一个仅包含一个组对象的响应，其中 `members@delta` 属性中有一个大型成员列表：</span><span class="sxs-lookup"><span data-stu-id="02f25-174">Microsoft Graph may return a response that contains just one group object, with a large list of members in the `members@delta` property:</span></span>

<span data-ttu-id="02f25-175">**第一页**</span><span class="sxs-lookup"><span data-stu-id="02f25-175">**First page**</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "37de1ae3-408f-4702-8636-20824abda004"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

2. <span data-ttu-id="02f25-176">如果按照 `nextLink` 操作，可能会再次收到包含同一组对象的响应。</span><span class="sxs-lookup"><span data-stu-id="02f25-176">When you follow the `nextLink` you may receive a response again containing the same group object.</span></span> <span data-ttu-id="02f25-177">将返回相同的属性值，但 `members@delta` 属性现在包含不同的用户列表。</span><span class="sxs-lookup"><span data-stu-id="02f25-177">The same property values will be returned but the `members@delta` property now contains a different list of users.</span></span>

<span data-ttu-id="02f25-178">**第二页**</span><span class="sxs-lookup"><span data-stu-id="02f25-178">**Second page**</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "c08a463b-7b8a-40a4-aa31-f9bf690b9551",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "23423fa6-821e-44b2-aae4-d039d33884c2"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

3. <span data-ttu-id="02f25-179">最终，将以此方式返回整个成员列表，并且其他组将开始在响应中显示。</span><span class="sxs-lookup"><span data-stu-id="02f25-179">Eventually, the entire member list will be returned in this fashion, and other groups will start showing up in the response.</span></span>

<span data-ttu-id="02f25-180">建议使用以下最佳做法来正确处理此模式：</span><span class="sxs-lookup"><span data-stu-id="02f25-180">We recommend the following best practices to correctly handle this pattern:</span></span>
- <span data-ttu-id="02f25-181">始终按照 `nextLink` 操作，并在本地合并每个组的状态：当收到与同一个组相关的响应时，使用它们在应用程序中构建完整的成员身份列表。</span><span class="sxs-lookup"><span data-stu-id="02f25-181">Always follow `nextLink` and locally merge each group's state: as you receive responses related to the same group, use them to build the full membership list in your application.</span></span>
- <span data-ttu-id="02f25-182">最好不要假定响应的特定顺序。</span><span class="sxs-lookup"><span data-stu-id="02f25-182">It is best not to assume a specific sequence of the responses.</span></span> <span data-ttu-id="02f25-183">假设同一组可以显示在 `nextLink` 序列的任意位置，并以合并逻辑进行处理。</span><span class="sxs-lookup"><span data-stu-id="02f25-183">Assume that the same group could show up anywhere in the `nextLink` sequence and handle that in your merge logic.</span></span>


## <a name="see-also"></a><span data-ttu-id="02f25-184">另请参阅</span><span class="sxs-lookup"><span data-stu-id="02f25-184">See also</span></span>
<span data-ttu-id="02f25-185">[Microsoft Graph delta 查询](delta-query-overview.md)概述。</span><span class="sxs-lookup"><span data-stu-id="02f25-185">[Microsoft Graph delta query](delta-query-overview.md) overview.</span></span>
