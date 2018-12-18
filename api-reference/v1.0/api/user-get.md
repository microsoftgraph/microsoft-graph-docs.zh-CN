---
title: 获取用户
description: 检索用户对象的属性和关系。
author: dkershaw10
ms.openlocfilehash: f26b77ccb21c4b25cc3d869582ce1d4064b16f53
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304660"
---
# <a name="get-a-user"></a><span data-ttu-id="4ed51-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="4ed51-103">Get a user</span></span>

<span data-ttu-id="4ed51-104">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4ed51-104">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="4ed51-p101">注意：获取用户仅返回一组默认属性（*businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName*。使用 `$select` 获取 [user](../resources/user.md) 对象的其他属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4ed51-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ed51-107">权限</span><span class="sxs-lookup"><span data-stu-id="4ed51-107">Permissions</span></span>
<span data-ttu-id="4ed51-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ed51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ed51-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ed51-110">Permission type</span></span>      | <span data-ttu-id="4ed51-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ed51-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ed51-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ed51-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4ed51-113">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ed51-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4ed51-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ed51-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ed51-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ed51-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="4ed51-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ed51-116">Application</span></span> | <span data-ttu-id="4ed51-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ed51-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ed51-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ed51-118">HTTP request</span></span>
<span data-ttu-id="4ed51-119">为某个特定用户：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4ed51-119">For a specific user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="4ed51-120">对于已登录的用户：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4ed51-120">For the signed-in user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ed51-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4ed51-121">Optional query parameters</span></span>
<span data-ttu-id="4ed51-122">此方法支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4ed51-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="4ed51-123">默认情况下，仅返回一组有限的属性（_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_）。</span><span class="sxs-lookup"><span data-stu-id="4ed51-123">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="4ed51-124">若要返回其他属性，必须使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="4ed51-124">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="4ed51-125">例如，若要返回 _displayName_、_givenName_、和 _postalCode_，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="4ed51-125">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ed51-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ed51-126">Request headers</span></span>
| <span data-ttu-id="4ed51-127">标头</span><span class="sxs-lookup"><span data-stu-id="4ed51-127">Header</span></span>       | <span data-ttu-id="4ed51-128">值</span><span class="sxs-lookup"><span data-stu-id="4ed51-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4ed51-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ed51-129">Authorization</span></span>  | <span data-ttu-id="4ed51-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ed51-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ed51-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ed51-132">Content-Type</span></span>   | <span data-ttu-id="4ed51-133">application/json</span><span class="sxs-lookup"><span data-stu-id="4ed51-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ed51-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ed51-134">Request body</span></span>
<span data-ttu-id="4ed51-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ed51-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ed51-136">响应</span><span class="sxs-lookup"><span data-stu-id="4ed51-136">Response</span></span>

<span data-ttu-id="4ed51-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ed51-137">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ed51-138">示例</span><span class="sxs-lookup"><span data-stu-id="4ed51-138">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="4ed51-139">示例 1：标准用户请求</span><span class="sxs-lookup"><span data-stu-id="4ed51-139">Example 1: Standard users request</span></span>

<span data-ttu-id="4ed51-140">默认情况下，仅返回一组有限的属性（_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_）。</span><span class="sxs-lookup"><span data-stu-id="4ed51-140">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="4ed51-141">此示例展示了默认请求和响应。</span><span class="sxs-lookup"><span data-stu-id="4ed51-141">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="4ed51-142">响应</span><span class="sxs-lookup"><span data-stu-id="4ed51-142">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

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
```


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="4ed51-143">示例 2：登录用户请求</span><span class="sxs-lookup"><span data-stu-id="4ed51-143">Example 2: Signed-in user request</span></span>

<span data-ttu-id="4ed51-144">可以将 `/users/{id | userPrincipalName}` 替换为 `/me`，获取登录用户的用户信息。</span><span class="sxs-lookup"><span data-stu-id="4ed51-144">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="4ed51-145">请求</span><span class="sxs-lookup"><span data-stu-id="4ed51-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="4ed51-146">响应</span><span class="sxs-lookup"><span data-stu-id="4ed51-146">Response</span></span>

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
```

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="4ed51-147">示例 3：使用 $select 的用户请求</span><span class="sxs-lookup"><span data-stu-id="4ed51-147">Example 3: Users request using $select</span></span>

<span data-ttu-id="4ed51-148">如果需要其他属性集，可以使用 OData `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="4ed51-148">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="4ed51-149">例如，若要返回 _displayName_、_givenName_、和 _postalCode_，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="4ed51-149">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="4ed51-150">请求</span><span class="sxs-lookup"><span data-stu-id="4ed51-150">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="4ed51-151">响应</span><span class="sxs-lookup"><span data-stu-id="4ed51-151">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "postalCode": "postalCode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
