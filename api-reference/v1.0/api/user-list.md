---
title: 列出用户
description: 检索用户对象列表。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 362716388f5c479e4b8c4a0009403817fcc80515
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026787"
---
# <a name="list-users"></a><span data-ttu-id="19385-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="19385-103">List users</span></span>

<span data-ttu-id="19385-104">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="19385-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="19385-105">权限</span><span class="sxs-lookup"><span data-stu-id="19385-105">Permissions</span></span>

<span data-ttu-id="19385-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19385-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19385-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="19385-108">Permission type</span></span>      | <span data-ttu-id="19385-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19385-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19385-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19385-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19385-111">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19385-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19385-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19385-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19385-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="19385-113">Not supported.</span></span>    |
|<span data-ttu-id="19385-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="19385-114">Application</span></span> | <span data-ttu-id="19385-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19385-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19385-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19385-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19385-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="19385-117">Optional query parameters</span></span>

<span data-ttu-id="19385-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="19385-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="19385-119">默认情况下，仅返回一组有限的属性（**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname** 和 **userPrincipalName**）。</span><span class="sxs-lookup"><span data-stu-id="19385-119">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> 

<span data-ttu-id="19385-120">若要返回其他属性，请使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="19385-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="19385-121">例如，若要返回 **displayName**、**givenName** 和 **postalCode**，请将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="19385-121">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

<span data-ttu-id="19385-122">某些属性无法在用户集合中返回。</span><span class="sxs-lookup"><span data-stu-id="19385-122">Certain properties cannot be returned within a user collection.</span></span> <span data-ttu-id="19385-123">以下属性仅在[检索单个用户](./user-get.md)时受支持：**aboutMe**、**birthday**、**hireDate**、**interests**、**mySite**、**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**mailboxSettings**。</span><span class="sxs-lookup"><span data-stu-id="19385-123">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings**</span></span>

## <a name="request-headers"></a><span data-ttu-id="19385-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="19385-124">Request headers</span></span>

| <span data-ttu-id="19385-125">标头</span><span class="sxs-lookup"><span data-stu-id="19385-125">Header</span></span>        | <span data-ttu-id="19385-126">值</span><span class="sxs-lookup"><span data-stu-id="19385-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="19385-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="19385-127">Authorization</span></span> | <span data-ttu-id="19385-128">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="19385-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="19385-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19385-129">Content-Type</span></span>  | <span data-ttu-id="19385-130">application/json</span><span class="sxs-lookup"><span data-stu-id="19385-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="19385-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="19385-131">Request body</span></span>

<span data-ttu-id="19385-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19385-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19385-133">响应</span><span class="sxs-lookup"><span data-stu-id="19385-133">Response</span></span>

<span data-ttu-id="19385-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="19385-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="19385-135">如果返回大的用户集，则可以[在应用中使用分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="19385-135">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="19385-136">示例</span><span class="sxs-lookup"><span data-stu-id="19385-136">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="19385-137">示例 1：标准用户请求</span><span class="sxs-lookup"><span data-stu-id="19385-137">Example 1: Standard users request</span></span>

<span data-ttu-id="19385-138">默认情况下，仅返回一组有限的属性（**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname**、**userPrincipalName**）。</span><span class="sxs-lookup"><span data-stu-id="19385-138">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> <span data-ttu-id="19385-139">此示例展示了默认请求和响应。</span><span class="sxs-lookup"><span data-stu-id="19385-139">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="19385-140">请求</span><span class="sxs-lookup"><span data-stu-id="19385-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="19385-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="19385-141">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19385-142">C#</span><span class="sxs-lookup"><span data-stu-id="19385-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19385-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="19385-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19385-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19385-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19385-145">Java</span><span class="sxs-lookup"><span data-stu-id="19385-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19385-146">响应</span><span class="sxs-lookup"><span data-stu-id="19385-146">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="19385-147">示例 2：使用 $select 的用户请求</span><span class="sxs-lookup"><span data-stu-id="19385-147">Example 2: Users request using $select</span></span>

<span data-ttu-id="19385-148">如果需要其他属性集，可以使用 OData `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="19385-148">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="19385-149">例如，若要返回 **displayName**、**givenName**、和 **postalCode**，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="19385-149">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="19385-150">请求</span><span class="sxs-lookup"><span data-stu-id="19385-150">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="19385-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="19385-151">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19385-152">C#</span><span class="sxs-lookup"><span data-stu-id="19385-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-properties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19385-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="19385-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-properties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19385-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19385-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-properties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19385-155">Java</span><span class="sxs-lookup"><span data-stu-id="19385-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-properties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19385-156">响应</span><span class="sxs-lookup"><span data-stu-id="19385-156">Response</span></span>

<span data-ttu-id="19385-157">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="19385-157">Note: The response object shown here may be truncated for brevity.</span></span>
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
