---
title: 获取用户
description: 检索用户对象的属性和关系。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b0fecfe948c59fe184e82f71e83d835cee74c7ff
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107695"
---
# <a name="get-a-user"></a><span data-ttu-id="b94fe-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="b94fe-103">Get a user</span></span>

<span data-ttu-id="b94fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b94fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b94fe-105">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b94fe-105">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="b94fe-p101">注意：获取用户仅返回一组默认属性（*businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName*。使用 `$select` 获取 [user](../resources/user.md) 对象的其他属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b94fe-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b94fe-108">权限</span><span class="sxs-lookup"><span data-stu-id="b94fe-108">Permissions</span></span>
<span data-ttu-id="b94fe-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b94fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b94fe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b94fe-111">Permission type</span></span>      | <span data-ttu-id="b94fe-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b94fe-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b94fe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b94fe-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b94fe-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b94fe-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b94fe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b94fe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b94fe-116">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b94fe-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="b94fe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b94fe-117">Application</span></span> | <span data-ttu-id="b94fe-118">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b94fe-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="b94fe-119">调用 `/me` 终结点需要已登录的用户，因此需要委派权限。</span><span class="sxs-lookup"><span data-stu-id="b94fe-119">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="b94fe-120">使用 `/me` 的终结点时不支持应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="b94fe-120">Application permissions are not supported when using the `/me` endpoint.</span></span>

## <a name="http-request"></a><span data-ttu-id="b94fe-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b94fe-121">HTTP request</span></span>
<span data-ttu-id="b94fe-122">对于特定用户：</span><span class="sxs-lookup"><span data-stu-id="b94fe-122">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

><span data-ttu-id="b94fe-123">**注意：**</span><span class="sxs-lookup"><span data-stu-id="b94fe-123">**Note:**</span></span>
> + <span data-ttu-id="b94fe-p104">当 **userPrincipalName** 以 `$` 字符开头时，请删除 `/users` 后的斜杠 (/)，并将 **userPrincipalName** 放在圆括号和单引号中。例如 `/users('$AdeleVance@contoso.com')`。有关详细信息，请参阅“[已知问题](/graph/known-issues#users)”列表。</span><span class="sxs-lookup"><span data-stu-id="b94fe-p104">When the **userPrincipalName** begins with a `$` character, remove the slash (/) after `/users` and enclose the **userPrincipalName** in parentheses and single quotes. For example, `/users('$AdeleVance@contoso.com')`. For details, see the [known issues](/graph/known-issues#users) list.</span></span>
> + <span data-ttu-id="b94fe-127">要使用 **userPrincipalName** 查询 B2B 用户，请对哈希 (#) 字符进行编码。</span><span class="sxs-lookup"><span data-stu-id="b94fe-127">To query a B2B user using the **userPrincipalName**, encode the hash (#) character.</span></span> <span data-ttu-id="b94fe-128">也就是说，将 `#` 符号替换为 `%23`。</span><span class="sxs-lookup"><span data-stu-id="b94fe-128">That is, replace the `#` symbol with `%23`.</span></span> <span data-ttu-id="b94fe-129">例如，`/users/AdeleVance_adatum.com%23EXT%23@contoso.com`。</span><span class="sxs-lookup"><span data-stu-id="b94fe-129">For example, `/users/AdeleVance_adatum.com%23EXT%23@contoso.com`.</span></span>

<span data-ttu-id="b94fe-130">对于登录用户：</span><span class="sxs-lookup"><span data-stu-id="b94fe-130">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b94fe-131">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b94fe-131">Optional query parameters</span></span>
<span data-ttu-id="b94fe-132">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b94fe-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="b94fe-133">默认情况下，仅返回一组有限的属性（_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_）。</span><span class="sxs-lookup"><span data-stu-id="b94fe-133">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="b94fe-134">若要返回其他属性，必须使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="b94fe-134">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="b94fe-135">例如，若要返回 _displayName_、_givenName_、和 _postalCode_，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="b94fe-135">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="b94fe-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="b94fe-136">Request headers</span></span>
| <span data-ttu-id="b94fe-137">标头</span><span class="sxs-lookup"><span data-stu-id="b94fe-137">Header</span></span>       | <span data-ttu-id="b94fe-138">值</span><span class="sxs-lookup"><span data-stu-id="b94fe-138">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b94fe-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="b94fe-139">Authorization</span></span>  | <span data-ttu-id="b94fe-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b94fe-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b94fe-142">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b94fe-142">Content-Type</span></span>   | <span data-ttu-id="b94fe-143">application/json</span><span class="sxs-lookup"><span data-stu-id="b94fe-143">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b94fe-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="b94fe-144">Request body</span></span>
<span data-ttu-id="b94fe-145">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b94fe-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b94fe-146">响应</span><span class="sxs-lookup"><span data-stu-id="b94fe-146">Response</span></span>

<span data-ttu-id="b94fe-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b94fe-147">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="b94fe-148">当成功处理请求时，此方法会返回 `202 Accepted`，但服务器需要更多时间来完成相关的后台操作。</span><span class="sxs-lookup"><span data-stu-id="b94fe-148">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="examples"></a><span data-ttu-id="b94fe-149">示例</span><span class="sxs-lookup"><span data-stu-id="b94fe-149">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="b94fe-150">示例 1：标准用户请求</span><span class="sxs-lookup"><span data-stu-id="b94fe-150">Example 1: Standard users request</span></span>

<span data-ttu-id="b94fe-151">默认情况下，仅返回一组有限的属性（_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_）。</span><span class="sxs-lookup"><span data-stu-id="b94fe-151">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="b94fe-152">此示例展示了默认请求和响应。</span><span class="sxs-lookup"><span data-stu-id="b94fe-152">This example illustrates the default request and response.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_user_1"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="b94fe-153">响应</span><span class="sxs-lookup"><span data-stu-id="b94fe-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "+1 425 555 0109"
   ],
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "jobTitle": "Retail Manager",
   "mail": "AdeleV@contoso.onmicrosoft.com",
   "mobilePhone": "+1 425 555 0109",
   "officeLocation": "18/2111",
   "preferredLanguage": "en-US",
   "surname": "Vance",
   "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
   "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="b94fe-154">示例 2：登录用户请求</span><span class="sxs-lookup"><span data-stu-id="b94fe-154">Example 2: Signed-in user request</span></span>

<span data-ttu-id="b94fe-155">可以将 `/users/{id | userPrincipalName}` 替换为 `/me`，获取登录用户的用户信息。</span><span class="sxs-lookup"><span data-stu-id="b94fe-155">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="b94fe-156">请求</span><span class="sxs-lookup"><span data-stu-id="b94fe-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b94fe-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="b94fe-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me
```
# <a name="c"></a>[<span data-ttu-id="b94fe-158">C#</span><span class="sxs-lookup"><span data-stu-id="b94fe-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b94fe-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b94fe-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b94fe-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b94fe-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b94fe-161">Java</span><span class="sxs-lookup"><span data-stu-id="b94fe-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b94fe-162">响应</span><span class="sxs-lookup"><span data-stu-id="b94fe-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "+1 425 555 0109"
   ],
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "jobTitle": "Retail Manager",
   "mail": "AdeleV@contoso.onmicrosoft.com",
   "mobilePhone": "+1 425 555 0109",
   "officeLocation": "18/2111",
   "preferredLanguage": "en-US",
   "surname": "Vance",
   "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
   "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="b94fe-163">示例 3：使用 $select 的用户请求</span><span class="sxs-lookup"><span data-stu-id="b94fe-163">Example 3: Users request using $select</span></span>

<span data-ttu-id="b94fe-164">如果需要其他属性集，可以使用 OData `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="b94fe-164">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="b94fe-165">例如，若要返回 _displayName_、_givenName_、和 _postalCode_，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="b94fe-165">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="b94fe-166">请求</span><span class="sxs-lookup"><span data-stu-id="b94fe-166">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b94fe-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="b94fe-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_2"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
# <a name="c"></a>[<span data-ttu-id="b94fe-168">C#</span><span class="sxs-lookup"><span data-stu-id="b94fe-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b94fe-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b94fe-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b94fe-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b94fe-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b94fe-171">Java</span><span class="sxs-lookup"><span data-stu-id="b94fe-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b94fe-172">响应</span><span class="sxs-lookup"><span data-stu-id="b94fe-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "postalCode": "98004"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
