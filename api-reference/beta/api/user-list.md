---
title: 列出用户
description: 检索用户对象列表。
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 5da2a929f054e942819786271aac004ed93baee6
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290691"
---
# <a name="list-users"></a><span data-ttu-id="7eb51-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="7eb51-103">List users</span></span>

<span data-ttu-id="7eb51-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eb51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7eb51-105">检索 [user](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="7eb51-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="7eb51-106">默认情况下，此操作仅返回每位用户较常用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="7eb51-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="7eb51-107">这些_默认_属性将记录在[属性](../resources/user.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="7eb51-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="7eb51-108">要获取_非_默认返回的属性，请对用户执行 [GET](user-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="7eb51-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="7eb51-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="7eb51-109">Permissions</span></span>

<span data-ttu-id="7eb51-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7eb51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7eb51-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7eb51-112">Permission type</span></span>      | <span data-ttu-id="7eb51-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7eb51-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7eb51-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7eb51-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7eb51-115">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All、Auditlogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="7eb51-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All, Auditlogs.Read.All</span></span> |
|<span data-ttu-id="7eb51-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7eb51-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7eb51-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7eb51-117">Not supported.</span></span>    |
|<span data-ttu-id="7eb51-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7eb51-118">Application</span></span> | <span data-ttu-id="7eb51-119">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Auditlogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="7eb51-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Auditlogs.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7eb51-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7eb51-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7eb51-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7eb51-121">Optional query parameters</span></span>

<span data-ttu-id="7eb51-122">此方法支持[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)，以帮助自定义响应，包括 `$search` 、 `$count` 和 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="7eb51-122">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="7eb51-123">您可以 `$search` 在**displayName**属性上使用。</span><span class="sxs-lookup"><span data-stu-id="7eb51-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="7eb51-124">为此资源添加或更新项目时，将对其进行专门编制索引，以便 `$count` 与 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="7eb51-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="7eb51-125">在添加或更新项目以及在索引中可用时，可能会出现轻微的延迟。</span><span class="sxs-lookup"><span data-stu-id="7eb51-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7eb51-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="7eb51-126">Request headers</span></span>

| <span data-ttu-id="7eb51-127">标头</span><span class="sxs-lookup"><span data-stu-id="7eb51-127">Header</span></span> | <span data-ttu-id="7eb51-128">值</span><span class="sxs-lookup"><span data-stu-id="7eb51-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="7eb51-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7eb51-129">Authorization</span></span> | <span data-ttu-id="7eb51-130">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="7eb51-130">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="7eb51-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="7eb51-131">ConsistencyLevel</span></span> | <span data-ttu-id="7eb51-132">仍然.</span><span class="sxs-lookup"><span data-stu-id="7eb51-132">eventual.</span></span> <span data-ttu-id="7eb51-133">此标头 `$count` 在使用时 `$search` 或在 `$filter` 与查询参数一起使用时是必需的 `$orderby` 。</span><span class="sxs-lookup"><span data-stu-id="7eb51-133">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="7eb51-134">它使用的索引可能不是最新的对象更改。</span><span class="sxs-lookup"><span data-stu-id="7eb51-134">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7eb51-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="7eb51-135">Request body</span></span>

<span data-ttu-id="7eb51-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7eb51-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7eb51-137">响应</span><span class="sxs-lookup"><span data-stu-id="7eb51-137">Response</span></span>

<span data-ttu-id="7eb51-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7eb51-138">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7eb51-139">示例</span><span class="sxs-lookup"><span data-stu-id="7eb51-139">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="7eb51-140">示例1：获取所有用户</span><span class="sxs-lookup"><span data-stu-id="7eb51-140">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="7eb51-141">请求</span><span class="sxs-lookup"><span data-stu-id="7eb51-141">Request</span></span>

<span data-ttu-id="7eb51-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7eb51-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7eb51-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="7eb51-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="7eb51-144">C#</span><span class="sxs-lookup"><span data-stu-id="7eb51-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7eb51-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7eb51-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7eb51-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7eb51-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7eb51-147">响应</span><span class="sxs-lookup"><span data-stu-id="7eb51-147">Response</span></span>

<span data-ttu-id="7eb51-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7eb51-148">The following is an example of the response.</span></span> 
><span data-ttu-id="7eb51-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7eb51-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="7eb51-151">示例2：使用登录名获取用户帐户</span><span class="sxs-lookup"><span data-stu-id="7eb51-151">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="7eb51-152">使用登录名（也称为本地帐户）查找用户帐户。</span><span class="sxs-lookup"><span data-stu-id="7eb51-152">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="7eb51-153">根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="7eb51-153">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="7eb51-154">请求</span><span class="sxs-lookup"><span data-stu-id="7eb51-154">Request</span></span>

<span data-ttu-id="7eb51-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7eb51-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7eb51-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="7eb51-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="7eb51-157">C#</span><span class="sxs-lookup"><span data-stu-id="7eb51-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7eb51-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7eb51-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7eb51-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7eb51-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7eb51-160">响应</span><span class="sxs-lookup"><span data-stu-id="7eb51-160">Response</span></span>

<span data-ttu-id="7eb51-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7eb51-161">The following is an example of the response.</span></span> 
> <span data-ttu-id="7eb51-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7eb51-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="7eb51-164">示例3：获取用户，包括其上次登录时间</span><span class="sxs-lookup"><span data-stu-id="7eb51-164">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="7eb51-165">请求</span><span class="sxs-lookup"><span data-stu-id="7eb51-165">Request</span></span>

<span data-ttu-id="7eb51-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7eb51-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7eb51-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="7eb51-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="7eb51-168">C#</span><span class="sxs-lookup"><span data-stu-id="7eb51-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7eb51-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7eb51-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7eb51-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7eb51-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7eb51-171">响应</span><span class="sxs-lookup"><span data-stu-id="7eb51-171">Response</span></span>

<span data-ttu-id="7eb51-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7eb51-172">The following is an example of the response.</span></span> 
> <span data-ttu-id="7eb51-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7eb51-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="7eb51-175">示例 4：列出具有特定显示名称的用户的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="7eb51-175">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="7eb51-176">请求</span><span class="sxs-lookup"><span data-stu-id="7eb51-176">Request</span></span>

<span data-ttu-id="7eb51-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7eb51-177">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```

#### <a name="response"></a><span data-ttu-id="7eb51-178">响应</span><span class="sxs-lookup"><span data-stu-id="7eb51-178">Response</span></span>

<span data-ttu-id="7eb51-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7eb51-179">The following is an example of the response.</span></span> 
> <span data-ttu-id="7eb51-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7eb51-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="7eb51-182">示例 5：列出用户在特定时间范围内的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="7eb51-182">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="7eb51-183">请求</span><span class="sxs-lookup"><span data-stu-id="7eb51-183">Request</span></span>

<span data-ttu-id="7eb51-184">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7eb51-184">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="7eb51-185">响应</span><span class="sxs-lookup"><span data-stu-id="7eb51-185">Response</span></span>

<span data-ttu-id="7eb51-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7eb51-186">The following is an example of the response.</span></span> 
> <span data-ttu-id="7eb51-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7eb51-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="7eb51-189">示例6：仅获取用户数</span><span class="sxs-lookup"><span data-stu-id="7eb51-189">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="7eb51-190">请求</span><span class="sxs-lookup"><span data-stu-id="7eb51-190">Request</span></span>

<span data-ttu-id="7eb51-191">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7eb51-191">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7eb51-192">响应</span><span class="sxs-lookup"><span data-stu-id="7eb51-192">Response</span></span>

<span data-ttu-id="7eb51-193">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7eb51-193">The following is an example of the response.</span></span>

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

<span data-ttu-id="7eb51-194">893</span><span class="sxs-lookup"><span data-stu-id="7eb51-194">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="7eb51-195">示例7：使用 $filter 和 $top 获取一个显示名称以 ' a ' 开头的用户，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="7eb51-195">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7eb51-196">请求</span><span class="sxs-lookup"><span data-stu-id="7eb51-196">Request</span></span>

<span data-ttu-id="7eb51-197">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7eb51-197">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7eb51-198">响应</span><span class="sxs-lookup"><span data-stu-id="7eb51-198">Response</span></span>

<span data-ttu-id="7eb51-199">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7eb51-199">The following is an example of the response.</span></span>
><span data-ttu-id="7eb51-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7eb51-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="7eb51-202">示例8：使用 $search 获取显示名称中包含字母 "wa" 的用户，其中包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="7eb51-202">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7eb51-203">请求</span><span class="sxs-lookup"><span data-stu-id="7eb51-203">Request</span></span>

<span data-ttu-id="7eb51-204">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7eb51-204">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7eb51-205">响应</span><span class="sxs-lookup"><span data-stu-id="7eb51-205">Response</span></span>

<span data-ttu-id="7eb51-206">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7eb51-206">The following is an example of the response.</span></span>
><span data-ttu-id="7eb51-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7eb51-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="7eb51-209">示例9：使用 $search 获取显示名称中包含字母 "wa" 或字母 "to" 的用户，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="7eb51-209">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7eb51-210">请求</span><span class="sxs-lookup"><span data-stu-id="7eb51-210">Request</span></span>

<span data-ttu-id="7eb51-211">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7eb51-211">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7eb51-212">响应</span><span class="sxs-lookup"><span data-stu-id="7eb51-212">Response</span></span>

<span data-ttu-id="7eb51-213">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7eb51-213">The following is an example of the response.</span></span> 
> <span data-ttu-id="7eb51-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7eb51-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
