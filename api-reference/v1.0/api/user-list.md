---
title: 列出用户
description: 检索用户对象列表。
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d20e60757fce6b2981ce4db1d06ffe29930e3539
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634877"
---
# <a name="list-users"></a><span data-ttu-id="a6410-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="a6410-103">List users</span></span>

<span data-ttu-id="a6410-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6410-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6410-105">检索 [user](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="a6410-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6410-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a6410-106">Permissions</span></span>

<span data-ttu-id="a6410-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6410-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6410-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6410-109">Permission type</span></span>      | <span data-ttu-id="a6410-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6410-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6410-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6410-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a6410-112">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6410-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a6410-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6410-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6410-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6410-114">Not supported.</span></span>    |
|<span data-ttu-id="a6410-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6410-115">Application</span></span> | <span data-ttu-id="a6410-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6410-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6410-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6410-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6410-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a6410-118">Optional query parameters</span></span>

<span data-ttu-id="a6410-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a6410-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="a6410-120">默认情况下，仅返回一组有限的属性（**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname** 和 **userPrincipalName**）。</span><span class="sxs-lookup"><span data-stu-id="a6410-120">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="a6410-121">若要返回其他属性，请使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="a6410-121">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="a6410-122">例如，若要返回 **displayName**、**givenName** 和 **postalCode**，请将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="a6410-122">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="a6410-123">某些属性无法在用户集合中返回。</span><span class="sxs-lookup"><span data-stu-id="a6410-123">Certain properties cannot be returned within a user collection.</span></span> <span data-ttu-id="a6410-124">以下属性仅在[检索单个用户](./user-get.md)时受支持：**aboutMe**、**birthday**、**hireDate**、**interests**、**mySite**、**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**mailboxSettings**。</span><span class="sxs-lookup"><span data-stu-id="a6410-124">The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6410-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6410-125">Request headers</span></span>

| <span data-ttu-id="a6410-126">标头</span><span class="sxs-lookup"><span data-stu-id="a6410-126">Header</span></span>        | <span data-ttu-id="a6410-127">值</span><span class="sxs-lookup"><span data-stu-id="a6410-127">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="a6410-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6410-128">Authorization</span></span> | <span data-ttu-id="a6410-129">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="a6410-129">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6410-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6410-130">Request body</span></span>

<span data-ttu-id="a6410-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6410-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6410-132">响应</span><span class="sxs-lookup"><span data-stu-id="a6410-132">Response</span></span>

<span data-ttu-id="a6410-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a6410-133">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="a6410-134">如果返回大的用户集，则可以[在应用中使用分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="a6410-134">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="a6410-135">示例</span><span class="sxs-lookup"><span data-stu-id="a6410-135">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="a6410-136">示例 1：标准用户请求</span><span class="sxs-lookup"><span data-stu-id="a6410-136">Example 1: Standard users request</span></span>

<span data-ttu-id="a6410-137">默认情况下，仅返回一组有限的属性（**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname**、**userPrincipalName**）。</span><span class="sxs-lookup"><span data-stu-id="a6410-137">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, **userPrincipalName**).</span></span> <span data-ttu-id="a6410-138">此示例展示了默认请求和响应。</span><span class="sxs-lookup"><span data-stu-id="a6410-138">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="a6410-139">请求</span><span class="sxs-lookup"><span data-stu-id="a6410-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a6410-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6410-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="a6410-141">C#</span><span class="sxs-lookup"><span data-stu-id="a6410-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6410-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6410-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6410-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6410-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6410-144">Java</span><span class="sxs-lookup"><span data-stu-id="a6410-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a6410-145">响应</span><span class="sxs-lookup"><span data-stu-id="a6410-145">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="a6410-146">示例 2：使用 $select 的用户请求</span><span class="sxs-lookup"><span data-stu-id="a6410-146">Example 2: Users request using $select</span></span>

<span data-ttu-id="a6410-147">如果需要其他属性集，可以使用 OData `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="a6410-147">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="a6410-148">例如，若要返回 **displayName**、**givenName**、和 **postalCode**，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="a6410-148">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

##### <a name="request"></a><span data-ttu-id="a6410-149">请求</span><span class="sxs-lookup"><span data-stu-id="a6410-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a6410-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6410-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```
# <a name="c"></a>[<span data-ttu-id="a6410-151">C#</span><span class="sxs-lookup"><span data-stu-id="a6410-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-properties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6410-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6410-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-properties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6410-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6410-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-properties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6410-154">Java</span><span class="sxs-lookup"><span data-stu-id="a6410-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-properties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a6410-155">响应</span><span class="sxs-lookup"><span data-stu-id="a6410-155">Response</span></span>

<span data-ttu-id="a6410-156">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a6410-156">Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
    }
  ]
}
```

### <a name="example-3-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="a6410-157">示例 3：使用登录名查找用户帐户</span><span class="sxs-lookup"><span data-stu-id="a6410-157">Example 3: Find a user account using a sign-in name</span></span>

<span data-ttu-id="a6410-158">使用登录名（也称为本地帐户）在 B2C 租户中查找用户帐户。</span><span class="sxs-lookup"><span data-stu-id="a6410-158">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="a6410-159">此请求可由技术支持人员用于在 B2C 租户中查找客户的用户帐户（此示例中，B2C 租户是 contoso.onmicrosoft.com）。</span><span class="sxs-lookup"><span data-stu-id="a6410-159">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="a6410-160">根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="a6410-160">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="a6410-161">请求</span><span class="sxs-lookup"><span data-stu-id="a6410-161">Request</span></span>

<span data-ttu-id="a6410-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a6410-162">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a6410-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6410-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="a6410-164">C#</span><span class="sxs-lookup"><span data-stu-id="a6410-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6410-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6410-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6410-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6410-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6410-167">Java</span><span class="sxs-lookup"><span data-stu-id="a6410-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="a6410-168">响应</span><span class="sxs-lookup"><span data-stu-id="a6410-168">Response</span></span>

<span data-ttu-id="a6410-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a6410-169">The following is an example of the response.</span></span> 
> <span data-ttu-id="a6410-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a6410-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
