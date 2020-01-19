---
title: 列出用户
description: 检索用户对象列表。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f9648b505700b05b05a64f977cb94bbd7d92f6e0
ms.sourcegitcommit: bd0daf5c133ab29af9337a5edd3b8509fd2313d5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41232033"
---
# <a name="list-users"></a><span data-ttu-id="876c7-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="876c7-103">List users</span></span>

<span data-ttu-id="876c7-104">检索 [user](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="876c7-104">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="876c7-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="876c7-105">Permissions</span></span>

<span data-ttu-id="876c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="876c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="876c7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="876c7-108">Permission type</span></span>      | <span data-ttu-id="876c7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="876c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="876c7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="876c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="876c7-111">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="876c7-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="876c7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="876c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="876c7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="876c7-113">Not supported.</span></span>    |
|<span data-ttu-id="876c7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="876c7-114">Application</span></span> | <span data-ttu-id="876c7-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="876c7-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="876c7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="876c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="876c7-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="876c7-117">Optional query parameters</span></span>

<span data-ttu-id="876c7-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="876c7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="876c7-119">默认情况下，仅返回一组有限的属性（**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname** 和 **userPrincipalName**）。</span><span class="sxs-lookup"><span data-stu-id="876c7-119">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="876c7-120">若要返回其他属性，请使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="876c7-120">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="876c7-121">例如，若要返回 **displayName**、**givenName** 和 **postalCode**，请将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="876c7-121">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="876c7-122">某些属性无法在用户集合中返回。</span><span class="sxs-lookup"><span data-stu-id="876c7-122">Certain properties cannot be returned within a user collection.</span></span> <span data-ttu-id="876c7-123">以下属性仅在[检索单个用户](./user-get.md)时受支持：**aboutMe**、**birthday**、**hireDate**、**interests**、**mySite**、**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**mailboxSettings**。</span><span class="sxs-lookup"><span data-stu-id="876c7-123">The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="876c7-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="876c7-124">Request headers</span></span>

| <span data-ttu-id="876c7-125">标头</span><span class="sxs-lookup"><span data-stu-id="876c7-125">Header</span></span>        | <span data-ttu-id="876c7-126">值</span><span class="sxs-lookup"><span data-stu-id="876c7-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="876c7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="876c7-127">Authorization</span></span> | <span data-ttu-id="876c7-128">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="876c7-128">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="876c7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="876c7-129">Request body</span></span>

<span data-ttu-id="876c7-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="876c7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="876c7-131">响应</span><span class="sxs-lookup"><span data-stu-id="876c7-131">Response</span></span>

<span data-ttu-id="876c7-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="876c7-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="876c7-133">如果返回大的用户集，则可以[在应用中使用分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="876c7-133">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="876c7-134">示例</span><span class="sxs-lookup"><span data-stu-id="876c7-134">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="876c7-135">示例 1：标准用户请求</span><span class="sxs-lookup"><span data-stu-id="876c7-135">Example 1: Standard users request</span></span>

<span data-ttu-id="876c7-136">默认情况下，仅返回一组有限的属性（**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname**、**userPrincipalName**）。</span><span class="sxs-lookup"><span data-stu-id="876c7-136">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, **userPrincipalName**).</span></span> <span data-ttu-id="876c7-137">此示例展示了默认请求和响应。</span><span class="sxs-lookup"><span data-stu-id="876c7-137">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="876c7-138">请求</span><span class="sxs-lookup"><span data-stu-id="876c7-138">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="876c7-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="876c7-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="876c7-140">C#</span><span class="sxs-lookup"><span data-stu-id="876c7-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="876c7-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="876c7-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="876c7-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="876c7-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="876c7-143">Java</span><span class="sxs-lookup"><span data-stu-id="876c7-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="876c7-144">响应</span><span class="sxs-lookup"><span data-stu-id="876c7-144">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="876c7-145">示例 2：使用 $select 的用户请求</span><span class="sxs-lookup"><span data-stu-id="876c7-145">Example 2: Users request using $select</span></span>

<span data-ttu-id="876c7-146">如果需要其他属性集，可以使用 OData `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="876c7-146">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="876c7-147">例如，若要返回 **displayName**、**givenName**、和 **postalCode**，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="876c7-147">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

##### <a name="request"></a><span data-ttu-id="876c7-148">请求</span><span class="sxs-lookup"><span data-stu-id="876c7-148">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="876c7-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="876c7-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="876c7-150">C#</span><span class="sxs-lookup"><span data-stu-id="876c7-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-properties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="876c7-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="876c7-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-properties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="876c7-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="876c7-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-properties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="876c7-153">Java</span><span class="sxs-lookup"><span data-stu-id="876c7-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-properties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="876c7-154">响应</span><span class="sxs-lookup"><span data-stu-id="876c7-154">Response</span></span>

<span data-ttu-id="876c7-155">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="876c7-155">Note: The response object shown here may be truncated for brevity.</span></span>
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

### <a name="example-3-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="876c7-156">示例 3：使用登录名查找用户帐户</span><span class="sxs-lookup"><span data-stu-id="876c7-156">Example 2: Find a user account using a sign-in name</span></span>

<span data-ttu-id="876c7-157">使用登录名（也称为本地帐户）在 B2C 租户中查找用户帐户。</span><span class="sxs-lookup"><span data-stu-id="876c7-157">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="876c7-158">此请求可由技术支持人员用于在 B2C 租户中查找客户的用户帐户（此示例中，B2C 租户是 contoso.onmicrosoft.com）。</span><span class="sxs-lookup"><span data-stu-id="876c7-158">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="876c7-159">根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="876c7-159">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="876c7-160">请求</span><span class="sxs-lookup"><span data-stu-id="876c7-160">Request</span></span>

<span data-ttu-id="876c7-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="876c7-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```

---

#### <a name="response"></a><span data-ttu-id="876c7-162">响应</span><span class="sxs-lookup"><span data-stu-id="876c7-162">Response</span></span>

<span data-ttu-id="876c7-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="876c7-163">The following is an example of the response.</span></span> 
> <span data-ttu-id="876c7-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="876c7-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
