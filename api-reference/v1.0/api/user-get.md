---
title: 获取用户
description: 检索用户对象的属性和关系。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 94ceebb51dfe1d43bea7404213ef8fdb56535701
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579779"
---
# <a name="get-a-user"></a><span data-ttu-id="9afb2-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="9afb2-103">Get a user</span></span>

<span data-ttu-id="9afb2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9afb2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9afb2-105">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9afb2-105">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="9afb2-p101">注意：获取用户仅返回一组默认属性（*businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName*。使用 `$select` 获取 [user](../resources/user.md) 对象的其他属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9afb2-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9afb2-108">权限</span><span class="sxs-lookup"><span data-stu-id="9afb2-108">Permissions</span></span>
<span data-ttu-id="9afb2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9afb2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9afb2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9afb2-111">Permission type</span></span>      | <span data-ttu-id="9afb2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9afb2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9afb2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9afb2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9afb2-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9afb2-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9afb2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9afb2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9afb2-116">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9afb2-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="9afb2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9afb2-117">Application</span></span> | <span data-ttu-id="9afb2-118">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9afb2-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="9afb2-119">调用 `/me` 终结点需要已登录的用户，因此需要委派权限。</span><span class="sxs-lookup"><span data-stu-id="9afb2-119">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="9afb2-120">使用 `/me` 的终结点时不支持应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="9afb2-120">Application permissions are not supported when using the `/me` endpoint.</span></span>

## <a name="http-request"></a><span data-ttu-id="9afb2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9afb2-121">HTTP request</span></span>
<span data-ttu-id="9afb2-122">对于特定用户：</span><span class="sxs-lookup"><span data-stu-id="9afb2-122">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
<span data-ttu-id="9afb2-p104">请注意，当 **userPrincipalName** 以 `$` 字符开头时，请删除 `/users` 后的斜杠 (/)，并将 **userPrincipalName** 括在圆括号和单引号中。有关详细信息，请参阅“[已知问题](/graph/known-issues#users)”列表。</span><span class="sxs-lookup"><span data-stu-id="9afb2-p104">Note that when the **userPrincipalName** begins with a `$` character, remove the slash (/) after `/users` and enclose the **userPrincipalName** in parentheses and single quotes. For details, see the [known issues](/graph/known-issues#users) list.</span></span>

<span data-ttu-id="9afb2-125">对于登录用户：</span><span class="sxs-lookup"><span data-stu-id="9afb2-125">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9afb2-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9afb2-126">Optional query parameters</span></span>
<span data-ttu-id="9afb2-127">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9afb2-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="9afb2-128">默认情况下，仅返回一组有限的属性（_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_）。</span><span class="sxs-lookup"><span data-stu-id="9afb2-128">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="9afb2-129">若要返回其他属性，必须使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="9afb2-129">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="9afb2-130">例如，若要返回 _displayName_、_givenName_、和 _postalCode_，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="9afb2-130">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="9afb2-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="9afb2-131">Request headers</span></span>
| <span data-ttu-id="9afb2-132">标头</span><span class="sxs-lookup"><span data-stu-id="9afb2-132">Header</span></span>       | <span data-ttu-id="9afb2-133">值</span><span class="sxs-lookup"><span data-stu-id="9afb2-133">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="9afb2-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="9afb2-134">Authorization</span></span>  | <span data-ttu-id="9afb2-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9afb2-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9afb2-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9afb2-137">Content-Type</span></span>   | <span data-ttu-id="9afb2-138">application/json</span><span class="sxs-lookup"><span data-stu-id="9afb2-138">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9afb2-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="9afb2-139">Request body</span></span>
<span data-ttu-id="9afb2-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9afb2-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9afb2-141">响应</span><span class="sxs-lookup"><span data-stu-id="9afb2-141">Response</span></span>

<span data-ttu-id="9afb2-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9afb2-142">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="9afb2-143">当成功处理请求时，此方法会返回 `202 Accepted`，但服务器需要更多时间来完成相关的后台操作。</span><span class="sxs-lookup"><span data-stu-id="9afb2-143">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="examples"></a><span data-ttu-id="9afb2-144">示例</span><span class="sxs-lookup"><span data-stu-id="9afb2-144">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="9afb2-145">示例 1：标准用户请求</span><span class="sxs-lookup"><span data-stu-id="9afb2-145">Example 1: Standard users request</span></span>

<span data-ttu-id="9afb2-146">默认情况下，仅返回一组有限的属性（_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_）。</span><span class="sxs-lookup"><span data-stu-id="9afb2-146">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="9afb2-147">此示例展示了默认请求和响应。</span><span class="sxs-lookup"><span data-stu-id="9afb2-147">This example illustrates the default request and response.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_user_1"
} -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="9afb2-148">响应</span><span class="sxs-lookup"><span data-stu-id="9afb2-148">Response</span></span>

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


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="9afb2-149">示例 2：登录用户请求</span><span class="sxs-lookup"><span data-stu-id="9afb2-149">Example 2: Signed-in user request</span></span>

<span data-ttu-id="9afb2-150">可以将 `/users/{id | userPrincipalName}` 替换为 `/me`，获取登录用户的用户信息。</span><span class="sxs-lookup"><span data-stu-id="9afb2-150">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="9afb2-151">请求</span><span class="sxs-lookup"><span data-stu-id="9afb2-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9afb2-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="9afb2-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me
```
# <a name="c"></a>[<span data-ttu-id="9afb2-153">C#</span><span class="sxs-lookup"><span data-stu-id="9afb2-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9afb2-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9afb2-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9afb2-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9afb2-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9afb2-156">Java</span><span class="sxs-lookup"><span data-stu-id="9afb2-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9afb2-157">响应</span><span class="sxs-lookup"><span data-stu-id="9afb2-157">Response</span></span>

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

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="9afb2-158">示例 3：使用 $select 的用户请求</span><span class="sxs-lookup"><span data-stu-id="9afb2-158">Example 3: Users request using $select</span></span>

<span data-ttu-id="9afb2-159">如果需要其他属性集，可以使用 OData `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="9afb2-159">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="9afb2-160">例如，若要返回 _displayName_、_givenName_、和 _postalCode_，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="9afb2-160">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="9afb2-161">请求</span><span class="sxs-lookup"><span data-stu-id="9afb2-161">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_2"
} -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="9afb2-162">响应</span><span class="sxs-lookup"><span data-stu-id="9afb2-162">Response</span></span>
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
