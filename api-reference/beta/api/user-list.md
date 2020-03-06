---
title: 列出用户
description: 检索用户对象列表。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4a59b6e9a4c79b13c78350283961899e93412f6c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451747"
---
# <a name="list-users"></a><span data-ttu-id="b792b-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="b792b-103">List users</span></span>

<span data-ttu-id="b792b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b792b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b792b-105">检索 [user](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="b792b-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="b792b-106">默认情况下，此操作仅返回每位用户较常用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="b792b-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="b792b-107">这些_默认_属性将记录在[属性](../resources/user.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="b792b-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="b792b-108">要获取_非_默认返回的属性，请对用户执行 [GET](user-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="b792b-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="b792b-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="b792b-109">Permissions</span></span>

<span data-ttu-id="b792b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b792b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b792b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b792b-112">Permission type</span></span>      | <span data-ttu-id="b792b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b792b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b792b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b792b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b792b-115">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b792b-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b792b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b792b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b792b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b792b-117">Not supported.</span></span>    |
|<span data-ttu-id="b792b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b792b-118">Application</span></span> | <span data-ttu-id="b792b-119">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b792b-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b792b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b792b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b792b-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b792b-121">Optional query parameters</span></span>

<span data-ttu-id="b792b-122">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b792b-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b792b-123">请求头</span><span class="sxs-lookup"><span data-stu-id="b792b-123">Request headers</span></span>
| <span data-ttu-id="b792b-124">标头</span><span class="sxs-lookup"><span data-stu-id="b792b-124">Header</span></span>        | <span data-ttu-id="b792b-125">值</span><span class="sxs-lookup"><span data-stu-id="b792b-125">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="b792b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b792b-126">Authorization</span></span> | <span data-ttu-id="b792b-127">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="b792b-127">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b792b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b792b-128">Request body</span></span>

<span data-ttu-id="b792b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b792b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b792b-130">响应</span><span class="sxs-lookup"><span data-stu-id="b792b-130">Response</span></span>

<span data-ttu-id="b792b-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b792b-131">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b792b-132">示例</span><span class="sxs-lookup"><span data-stu-id="b792b-132">Example</span></span>

### <a name="example-1-list-all-users"></a><span data-ttu-id="b792b-133">示例 1：列出所有用户</span><span class="sxs-lookup"><span data-stu-id="b792b-133">Example 1: List all users</span></span>

#### <a name="request"></a><span data-ttu-id="b792b-134">请求</span><span class="sxs-lookup"><span data-stu-id="b792b-134">Request</span></span>

<span data-ttu-id="b792b-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b792b-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b792b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b792b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="b792b-137">C#</span><span class="sxs-lookup"><span data-stu-id="b792b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b792b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b792b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b792b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b792b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b792b-140">响应</span><span class="sxs-lookup"><span data-stu-id="b792b-140">Response</span></span>

<span data-ttu-id="b792b-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b792b-141">The following is an example of the response.</span></span> 
><span data-ttu-id="b792b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b792b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="b792b-144">示例 2：使用登录名查找用户帐户</span><span class="sxs-lookup"><span data-stu-id="b792b-144">Example 2: Find a user account using a sign-in name</span></span>

<span data-ttu-id="b792b-145">使用登录名（也称为本地帐户）在 B2C 租户中查找用户帐户。</span><span class="sxs-lookup"><span data-stu-id="b792b-145">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="b792b-146">此请求可由技术支持人员用于在 B2C 租户中查找客户的用户帐户（此示例中，B2C 租户是 contoso.onmicrosoft.com）。</span><span class="sxs-lookup"><span data-stu-id="b792b-146">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="b792b-147">根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="b792b-147">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="b792b-148">请求</span><span class="sxs-lookup"><span data-stu-id="b792b-148">Request</span></span>

<span data-ttu-id="b792b-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b792b-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b792b-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="b792b-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="b792b-151">C#</span><span class="sxs-lookup"><span data-stu-id="b792b-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b792b-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b792b-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b792b-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b792b-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b792b-154">响应</span><span class="sxs-lookup"><span data-stu-id="b792b-154">Response</span></span>

<span data-ttu-id="b792b-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b792b-155">The following is an example of the response.</span></span> 
> <span data-ttu-id="b792b-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b792b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 108

{
  "value": [
    {
      "displayName": "John Smith",
      "id": "4c7be08b-361f-41a8-b1ef-1712f7a3dfb2"
    }
  ]
}
```

### <a name="example-3--list-users-including-their-last-sign-in-time"></a><span data-ttu-id="b792b-158">示例3：列出用户（包括其上次登录时间）</span><span class="sxs-lookup"><span data-stu-id="b792b-158">Example 3:  List users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="b792b-159">请求</span><span class="sxs-lookup"><span data-stu-id="b792b-159">Request</span></span>

<span data-ttu-id="b792b-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b792b-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b792b-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="b792b-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="b792b-162">C#</span><span class="sxs-lookup"><span data-stu-id="b792b-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b792b-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b792b-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b792b-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b792b-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b792b-165">响应</span><span class="sxs-lookup"><span data-stu-id="b792b-165">Response</span></span>

<span data-ttu-id="b792b-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b792b-166">The following is an example of the response.</span></span> 
> <span data-ttu-id="b792b-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b792b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
