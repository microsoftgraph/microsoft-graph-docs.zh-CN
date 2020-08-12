---
title: 列出用户
description: 检索用户对象列表。
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 38d9f6044a90e422d68e55466ffd1e6191c54caf
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643916"
---
# <a name="list-users"></a><span data-ttu-id="ededb-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="ededb-103">List users</span></span>

<span data-ttu-id="ededb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ededb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ededb-105">检索 [user](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="ededb-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="ededb-106">默认情况下，此操作仅返回每位用户较常用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="ededb-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="ededb-107">这些_默认_属性将记录在[属性](../resources/user.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="ededb-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="ededb-108">要获取_非_默认返回的属性，请对用户执行 [GET](user-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="ededb-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="ededb-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="ededb-109">Permissions</span></span>

<span data-ttu-id="ededb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ededb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ededb-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ededb-112">Permission type</span></span>      | <span data-ttu-id="ededb-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ededb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ededb-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ededb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ededb-115">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ededb-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ededb-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ededb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ededb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ededb-117">Not supported.</span></span>    |
|<span data-ttu-id="ededb-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ededb-118">Application</span></span> | <span data-ttu-id="ededb-119">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ededb-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ededb-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ededb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ededb-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ededb-121">Optional query parameters</span></span>

<span data-ttu-id="ededb-122">此方法支持[OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="ededb-122">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="ededb-123">`$search`可以用在 **displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="ededb-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="ededb-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="ededb-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="ededb-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="ededb-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ededb-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="ededb-126">Request headers</span></span>

| <span data-ttu-id="ededb-127">标头</span><span class="sxs-lookup"><span data-stu-id="ededb-127">Header</span></span> | <span data-ttu-id="ededb-128">值</span><span class="sxs-lookup"><span data-stu-id="ededb-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="ededb-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ededb-129">Authorization</span></span> | <span data-ttu-id="ededb-130">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="ededb-130">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="ededb-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="ededb-131">ConsistencyLevel</span></span> | <span data-ttu-id="ededb-132">最终。</span><span class="sxs-lookup"><span data-stu-id="ededb-132">eventual.</span></span> <span data-ttu-id="ededb-133">当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="ededb-133">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="ededb-134">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="ededb-134">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ededb-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="ededb-135">Request body</span></span>

<span data-ttu-id="ededb-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ededb-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ededb-137">响应</span><span class="sxs-lookup"><span data-stu-id="ededb-137">Response</span></span>

<span data-ttu-id="ededb-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ededb-138">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ededb-139">示例</span><span class="sxs-lookup"><span data-stu-id="ededb-139">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="ededb-140">示例 1：列出所有用户</span><span class="sxs-lookup"><span data-stu-id="ededb-140">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="ededb-141">请求</span><span class="sxs-lookup"><span data-stu-id="ededb-141">Request</span></span>

<span data-ttu-id="ededb-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ededb-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ededb-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="ededb-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="ededb-144">C#</span><span class="sxs-lookup"><span data-stu-id="ededb-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ededb-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ededb-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ededb-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ededb-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ededb-147">响应</span><span class="sxs-lookup"><span data-stu-id="ededb-147">Response</span></span>

<span data-ttu-id="ededb-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ededb-148">The following is an example of the response.</span></span> 
><span data-ttu-id="ededb-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ededb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value":[
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "otherMails":["contoso1@gmail.com"],
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="ededb-151">示例 2：使用登录名创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="ededb-151">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="ededb-152">使用登录名（也称为本地帐户）查找用户帐户。</span><span class="sxs-lookup"><span data-stu-id="ededb-152">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="ededb-153">根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="ededb-153">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="ededb-154">请求</span><span class="sxs-lookup"><span data-stu-id="ededb-154">Request</span></span>

<span data-ttu-id="ededb-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ededb-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ededb-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ededb-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="ededb-157">C#</span><span class="sxs-lookup"><span data-stu-id="ededb-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ededb-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ededb-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ededb-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ededb-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ededb-160">响应</span><span class="sxs-lookup"><span data-stu-id="ededb-160">Response</span></span>

<span data-ttu-id="ededb-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ededb-161">The following is an example of the response.</span></span> 
> <span data-ttu-id="ededb-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ededb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "John Smith"
    }
  ]
}
```

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="ededb-164">示例3：列出用户，包括其上次登录时间</span><span class="sxs-lookup"><span data-stu-id="ededb-164">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="ededb-165">请求</span><span class="sxs-lookup"><span data-stu-id="ededb-165">Request</span></span>

<span data-ttu-id="ededb-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ededb-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ededb-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="ededb-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="ededb-168">C#</span><span class="sxs-lookup"><span data-stu-id="ededb-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ededb-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ededb-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ededb-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ededb-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ededb-171">响应</span><span class="sxs-lookup"><span data-stu-id="ededb-171">Response</span></span>

<span data-ttu-id="ededb-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ededb-172">The following is an example of the response.</span></span> 
> <span data-ttu-id="ededb-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ededb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(displayName,userPrincipalName,signInActivity)",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-07-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="ededb-175">示例 4：列出具有特定显示名称的用户的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="ededb-175">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="ededb-176">请求</span><span class="sxs-lookup"><span data-stu-id="ededb-176">Request</span></span>

<span data-ttu-id="ededb-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ededb-177">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="ededb-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="ededb-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="ededb-179">C#</span><span class="sxs-lookup"><span data-stu-id="ededb-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ededb-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ededb-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ededb-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ededb-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ededb-182">响应</span><span class="sxs-lookup"><span data-stu-id="ededb-182">Response</span></span>

<span data-ttu-id="ededb-183">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ededb-183">The following is an example of the response.</span></span> 
> <span data-ttu-id="ededb-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ededb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
  "value": [
    {
      "displayName": "Eric Solomon",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    }
  ]
}
```

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="ededb-186">示例 5：列出用户在特定时间范围内的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="ededb-186">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="ededb-187">请求</span><span class="sxs-lookup"><span data-stu-id="ededb-187">Request</span></span>

<span data-ttu-id="ededb-188">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ededb-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="ededb-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="ededb-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="ededb-190">C#</span><span class="sxs-lookup"><span data-stu-id="ededb-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ededb-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ededb-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ededb-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ededb-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ededb-193">响应</span><span class="sxs-lookup"><span data-stu-id="ededb-193">Response</span></span>

<span data-ttu-id="ededb-194">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ededb-194">The following is an example of the response.</span></span> 
> <span data-ttu-id="ededb-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ededb-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-05-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-04-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="ededb-197">示例 6：仅获取用户数量</span><span class="sxs-lookup"><span data-stu-id="ededb-197">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="ededb-198">请求</span><span class="sxs-lookup"><span data-stu-id="ededb-198">Request</span></span>

<span data-ttu-id="ededb-199">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ededb-199">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ededb-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="ededb-200">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ededb-201">C#</span><span class="sxs-lookup"><span data-stu-id="ededb-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ededb-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ededb-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ededb-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ededb-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ededb-204">响应</span><span class="sxs-lookup"><span data-stu-id="ededb-204">Response</span></span>

<span data-ttu-id="ededb-205">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ededb-205">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="ededb-206">893</span><span class="sxs-lookup"><span data-stu-id="ededb-206">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="ededb-207">示例 7：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="ededb-207">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ededb-208">请求</span><span class="sxs-lookup"><span data-stu-id="ededb-208">Request</span></span>

<span data-ttu-id="ededb-209">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ededb-209">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ededb-210">HTTP</span><span class="sxs-lookup"><span data-stu-id="ededb-210">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ededb-211">C#</span><span class="sxs-lookup"><span data-stu-id="ededb-211">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ededb-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ededb-212">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ededb-213">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ededb-213">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ededb-214">响应</span><span class="sxs-lookup"><span data-stu-id="ededb-214">Response</span></span>

<span data-ttu-id="ededb-215">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ededb-215">The following is an example of the response.</span></span>
><span data-ttu-id="ededb-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ededb-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mail":"a@contoso.com",
      "mailNickname":"a_contoso.com#EXT#",
      "otherMails":["a@contoso.com"],
      "proxyAddresses":["SMTP:a@contoso.com"],
      "userPrincipalName":"a_contoso.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="ededb-218">示例 8：使用 $search 获取显示名称中包含字母“wa”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="ededb-218">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ededb-219">请求</span><span class="sxs-lookup"><span data-stu-id="ededb-219">Request</span></span>

<span data-ttu-id="ededb-220">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ededb-220">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ededb-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="ededb-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ededb-222">C#</span><span class="sxs-lookup"><span data-stu-id="ededb-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-wa-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ededb-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ededb-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-wa-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ededb-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ededb-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-wa-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ededb-225">响应</span><span class="sxs-lookup"><span data-stu-id="ededb-225">Response</span></span>

<span data-ttu-id="ededb-226">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ededb-226">The following is an example of the response.</span></span>
><span data-ttu-id="ededb-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ededb-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    }
  ]
}

```

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="ededb-229">示例 9：使用 $search 获取名称显示中包含字母“wa”或者包含字母“to”的的用户，包括返回对象的数量</span><span class="sxs-lookup"><span data-stu-id="ededb-229">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ededb-230">请求</span><span class="sxs-lookup"><span data-stu-id="ededb-230">Request</span></span>

<span data-ttu-id="ededb-231">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ededb-231">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ededb-232">响应</span><span class="sxs-lookup"><span data-stu-id="ededb-232">Response</span></span>

<span data-ttu-id="ededb-233">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ededb-233">The following is an example of the response.</span></span> 
> <span data-ttu-id="ededb-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ededb-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    },
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
