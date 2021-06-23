---
title: 获取用户的增量更改
description: Delta 查询可通过调用一系列 delta 函数查询用户的添加、删除或更新。Delta 查询使你无需读取 Microsoft Graph 的整组用户就能够发现用户的更改并进行比较。
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 39253f03175c9c33c6e358afc2e629a77e449a0c
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082060"
---
# <a name="get-incremental-changes-for-users"></a><span data-ttu-id="d984d-104">获取用户的增量更改</span><span class="sxs-lookup"><span data-stu-id="d984d-104">Get incremental changes for users</span></span>

<span data-ttu-id="d984d-p102">[Delta 查询](./delta-query-overview.md)可通过调用一系列 [delta](/graph/api/user-delta?view=graph-rest-1.0) 函数查询用户的添加、删除或更新。Delta 查询使你无需读取 Microsoft Graph 的整组用户就能够发现用户的更改并进行比较。</span><span class="sxs-lookup"><span data-stu-id="d984d-p102">[Delta query](./delta-query-overview.md) lets you query for additions, deletions, or updates to users, by way of a series of [delta](/graph/api/user-delta?view=graph-rest-1.0) function calls. Delta query enables you discover changes to users without having to fetch the entire set of users from Microsoft Graph and compare changes.</span></span>

<span data-ttu-id="d984d-p103">以后，对本地配置文件存储使用同步用户功能的客户端可以将增量查询用于初始完全同步和增量同步。通常，客户会对租户中的所有用户进行初始完全同步，之后定期获取对用户的增量更改。</span><span class="sxs-lookup"><span data-stu-id="d984d-p103">Clients using synchronizing users with a local profile store can use Delta Query for both their initial full synchronization along with incremental synchronizations in the future. Typically, a client would do an initial full synchronization of all the users in a tenant, and subsequently, get incremental changes to users periodically.</span></span>

## <a name="tracking-user-changes"></a><span data-ttu-id="d984d-109">跟踪用户更改</span><span class="sxs-lookup"><span data-stu-id="d984d-109">Tracking user changes</span></span>

<span data-ttu-id="d984d-p104">跟踪用户更改是发出 **delta** 函数的一个或多个 GET 请求。发出 GET 请求与 [列出用户](/graph/api/user-list?view=graph-rest-1.0)的方式非常相似，除了要包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="d984d-p104">Tracking user changes is a round of one or more GET requests with the **delta** function. You make a GET request much like the way you [list users](/graph/api/user-list?view=graph-rest-1.0), except that you include the following:</span></span>

- <span data-ttu-id="d984d-112">**delta** 函数。</span><span class="sxs-lookup"><span data-stu-id="d984d-112">The **delta** function.</span></span>
- <span data-ttu-id="d984d-113">上一个 GET **delta** 函数调用的 [状态令牌](./delta-query-overview.md)（_deltaToken_ 或 _skipToken_）。</span><span class="sxs-lookup"><span data-stu-id="d984d-113">A [state token](./delta-query-overview.md) (_deltaToken_ or _skipToken_) from the previous GET **delta** function call.</span></span>

## <a name="example"></a><span data-ttu-id="d984d-114">示例</span><span class="sxs-lookup"><span data-stu-id="d984d-114">Example</span></span>

<span data-ttu-id="d984d-115">以下示例显示了跟踪用户更改的一系列请求：</span><span class="sxs-lookup"><span data-stu-id="d984d-115">The following example shows a series  requests to track changes to users:</span></span>

1. <span data-ttu-id="d984d-116">[初始请求](#initial-request)和[响应](#initial-response)</span><span class="sxs-lookup"><span data-stu-id="d984d-116">[Initial request](#initial-request) and [response](#initial-response)</span></span>
2. <span data-ttu-id="d984d-117">[nextLink 请求](#nextlink-request)和[响应](#nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="d984d-117">[nextLink request](#nextlink-request) and [response](#nextlink-response)</span></span>
3. <span data-ttu-id="d984d-118">[最终 nextLink 请求](#final-nextlink-request)和[响应](#final-nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="d984d-118">[Final nextLink request](#final-nextlink-request) and [response](#final-nextlink-response)</span></span>
4. <span data-ttu-id="d984d-119">[deltaLink 请求](#deltalink-request)和 [deltaLink 响应](#deltalink-response)</span><span class="sxs-lookup"><span data-stu-id="d984d-119">[deltaLink request](#deltalink-request) and [deltaLink response](#deltalink-response)</span></span>

## <a name="initial-request"></a><span data-ttu-id="d984d-120">初始请求</span><span class="sxs-lookup"><span data-stu-id="d984d-120">Initial request</span></span>

<span data-ttu-id="d984d-121">为开始跟踪用户资源的更改，请在用户资源上发出包含 delta 函数的请求。</span><span class="sxs-lookup"><span data-stu-id="d984d-121">To begin tracking changes in the user resource, you make a request including the delta function on the user resource.</span></span>

<span data-ttu-id="d984d-122">请注意以下事项：</span><span class="sxs-lookup"><span data-stu-id="d984d-122">Note the following:</span></span>

- <span data-ttu-id="d984d-123">请求中包含可选的 $select 查询参数，以演示如何在以后的请求中自动包含查询参数。</span><span class="sxs-lookup"><span data-stu-id="d984d-123">The optional $select query parameter is included in the request to demonstrate how query parameters are automatically included in future requests.</span></span>
- <span data-ttu-id="d984d-p105">初始请求不包括状态令牌。状态令牌将用于后续请求中。</span><span class="sxs-lookup"><span data-stu-id="d984d-p105">The initial request does not include a state token. State tokens will be used in subsequent requests.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

## <a name="initial-response"></a><span data-ttu-id="d984d-126">初始响应</span><span class="sxs-lookup"><span data-stu-id="d984d-126">Initial response</span></span>

<span data-ttu-id="d984d-p106">如果成功，此方法的响应正文返回`200 OK`响应代码和[用户](/graph/api/resources/user?view=graph-rest-1.0)集合对象。假定整组用户过大，则响应还将包含 nextLink 状态令牌。</span><span class="sxs-lookup"><span data-stu-id="d984d-p106">If successful, this method returns `200 OK` response code and [user](/graph/api/resources/user?view=graph-rest-1.0) collection object in the response body. Assuming the entire set of users is too large, the response will also include a nextLink state token.</span></span>

<span data-ttu-id="d984d-p107">本示例中，返回 nextLink URL，表示此会话存在要检索的其他数据页面。初始请求的 $select 查询参数已编码为 nextLink URL。</span><span class="sxs-lookup"><span data-stu-id="d984d-p107">In this example, a nextLink URL is returned indicating there are additional pages of data to be retrieved in the session. The $select query parameter from the initial request is encoded into the nextLink URL.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,givenName,surname)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa",
  "value": [
    {
      "displayName":"Testuser1",
      "givenName":"John",
      "surname":"Doe",
      "id":"ffff7b1a-13b6-477b-8c0c-380905cd99f7"
    },
    {
      "displayName":"Testuser2",
      "givenName":"Jane",
      "surname":"Doe",
      "id":"605d1257-ffff-40b6-8e6f-528a53f5dc55"
    }
  ]
}
```

## <a name="nextlink-request"></a><span data-ttu-id="d984d-131">nextLink 请求</span><span class="sxs-lookup"><span data-stu-id="d984d-131">nextLink request</span></span>

<span data-ttu-id="d984d-p108">第二个请求指定上一个响应中返回的 `skipToken`。请注意不需要 `$select` 参数，因为 `skipToken` 已将其编码且包含其中。</span><span class="sxs-lookup"><span data-stu-id="d984d-p108">The second request specifies the `skipToken` returned from the previous response. Notice the `$select` parameter is not required, as the `skipToken` encodes and includes it.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

## <a name="nextlink-response"></a><span data-ttu-id="d984d-134">nextLink 响应</span><span class="sxs-lookup"><span data-stu-id="d984d-134">nextLink response</span></span>

<span data-ttu-id="d984d-135">该响应包含另一个带新 `skipToken` 值的 `nextLink`，它表示存在更多可用的组。</span><span class="sxs-lookup"><span data-stu-id="d984d-135">The response contains another `nextLink` with a new `skipToken` value, which indicates that more groups are available.</span></span> <span data-ttu-id="d984d-136">应使用 `nextLink` URL 继续发出请求，直到在最终响应中返回 `deltaLink` URL，即使该值为空数组（在某些情况下可能会出现此情况）。</span><span class="sxs-lookup"><span data-stu-id="d984d-136">You should continue making requests using the `nextLink` URL until a `deltaLink` URL is returned in the final response, even if the value is an empty array (this can happen under certain circumstances).</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Testuser3",
      "givenName":"Pat",
      "surname":"Doe",
      "id":"d8c37826-ffff-4cae-b348-e2725b1e814b"
    },
    {
      "displayName":"Testuser4",
      "givenName":"Meghan",
      "surname":"Doe",
      "id":"8b1ee412-cd8f-4d59-ffff-24010edb9f1f"
    }
  ]
}
```

## <a name="final-nextlink-request"></a><span data-ttu-id="d984d-137">最终 nextLink 请求</span><span class="sxs-lookup"><span data-stu-id="d984d-137">Final nextLink request</span></span>

<span data-ttu-id="d984d-138">第三个请求继续使用上次同步请求返回的最新 `skipToken`。</span><span class="sxs-lookup"><span data-stu-id="d984d-138">The third request continues to use the latest `skipToken` returned from the last sync request.</span></span> 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a><span data-ttu-id="d984d-139">最终 nextLink 响应</span><span class="sxs-lookup"><span data-stu-id="d984d-139">Final nextLink response</span></span>

<span data-ttu-id="d984d-p110">当返回 deltaLink URL 时，不再返回关于资源现有状态的数据。为了执行以后的请求，应用程序使用 deltaLink URL 了解资源更改。保存 `deltaToken`，并在请求 URL 中使用它来发现用户更改。</span><span class="sxs-lookup"><span data-stu-id="d984d-p110">When the deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource. Save the `deltaToken` and use it in the request URL to discover changes to users.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser5",
      "givenName":"Al",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "displayName":"Testuser6",
      "givenName":"Sam",
      "surname":"Doe",
      "id":"f6ede700-27d0-4c42-bfb9-4dffff43c74a"
    }
  ]
}
```

## <a name="deltalink-request"></a><span data-ttu-id="d984d-143">deltaLink 请求</span><span class="sxs-lookup"><span data-stu-id="d984d-143">deltaLink request</span></span>

<span data-ttu-id="d984d-144">通过使用[上次响应](#final-nextlink-response)中的 `deltaToken`，你将能够获取上次请求以来的已更改用户（添加、删除或更新）。</span><span class="sxs-lookup"><span data-stu-id="d984d-144">Using the `deltaToken` from the [last response](#final-nextlink-response), you will be able to get changed (by being added, deleted, or updated) users since the last request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a><span data-ttu-id="d984d-145">deltaLink 响应</span><span class="sxs-lookup"><span data-stu-id="d984d-145">deltaLink response</span></span>

<span data-ttu-id="d984d-146">如果未发生更改，则会返回不同 `deltatoken` 且不返回结果。</span><span class="sxs-lookup"><span data-stu-id="d984d-146">If no changes have occurred, a different `deltatoken` is returned with no results.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": []
}
```

<span data-ttu-id="d984d-147">如果发生更改，则返回不同的 `deltatoken`，其中包括已更改用户的集合。</span><span class="sxs-lookup"><span data-stu-id="d984d-147">If changes have occurred, a different `deltatoken` is returned including a collection of changed users.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": [
    {
      "displayName":"Testuser7",
      "givenName":"Joe",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "id":"8ffff70c-1c63-4860-b963-e34ec660931d",
      "@removed": {
         "reason": "changed"
      }
    }
  ]
}
```

<span data-ttu-id="d984d-148">上一个示例响应的一些注意事项如下：</span><span class="sxs-lookup"><span data-stu-id="d984d-148">Some things to note about the previous example response:</span></span>

- <span data-ttu-id="d984d-149">如果用户遭删除，项中包含注释：`@removed` 值为 `"reason": "changed"`。</span><span class="sxs-lookup"><span data-stu-id="d984d-149">When the user is deleted, the item contains an annotation: `@removed` with value of `"reason": "changed"`.</span></span>

- <span data-ttu-id="d984d-150">如果用户遭永久删除，项中包含注释：`@removed` 值为 `"reason": "deleted"`。</span><span class="sxs-lookup"><span data-stu-id="d984d-150">When the user is permanently deleted, the item contains an annotation: `@removed` with value of `"reason": "deleted"`.</span></span>

- <span data-ttu-id="d984d-151">如果用户被创建或恢复，则没有注释。</span><span class="sxs-lookup"><span data-stu-id="d984d-151">When the user is created, or restored, there is no annotation.</span></span>

## <a name="see-also"></a><span data-ttu-id="d984d-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d984d-152">See also</span></span>
<span data-ttu-id="d984d-153">[Microsoft Graph delta 查询](delta-query-overview.md)概述。</span><span class="sxs-lookup"><span data-stu-id="d984d-153">[Microsoft Graph delta query](delta-query-overview.md) overview.</span></span>
