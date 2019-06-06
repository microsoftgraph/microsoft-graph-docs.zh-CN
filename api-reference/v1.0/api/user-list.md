---
title: 列出用户
description: 检索用户对象列表。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb519c1fa613b420581576099687096ec6aaa6f0
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709437"
---
# <a name="list-users"></a><span data-ttu-id="263b3-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="263b3-103">List users</span></span>

<span data-ttu-id="263b3-104">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="263b3-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="263b3-105">权限</span><span class="sxs-lookup"><span data-stu-id="263b3-105">Permissions</span></span>

<span data-ttu-id="263b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="263b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="263b3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="263b3-108">Permission type</span></span>      | <span data-ttu-id="263b3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="263b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="263b3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="263b3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="263b3-111">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="263b3-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="263b3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="263b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="263b3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="263b3-113">Not supported.</span></span>    |
|<span data-ttu-id="263b3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="263b3-114">Application</span></span> | <span data-ttu-id="263b3-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="263b3-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="263b3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="263b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="263b3-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="263b3-117">Optional query parameters</span></span>

<span data-ttu-id="263b3-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="263b3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="263b3-119">默认情况下，仅返回一组有限的属性（**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname** 和 **userPrincipalName**）。</span><span class="sxs-lookup"><span data-stu-id="263b3-119">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> 

<span data-ttu-id="263b3-120">若要返回其他属性，请使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="263b3-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="263b3-121">例如，若要返回 **displayName**、**givenName** 和 **postalCode**，请将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="263b3-121">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

<span data-ttu-id="263b3-122">某些属性无法在用户集合中返回。</span><span class="sxs-lookup"><span data-stu-id="263b3-122">Certain properties cannot be returned within a user collection.</span></span> <span data-ttu-id="263b3-123">以下属性仅在[检索单个用户](./user-get.md)时受支持：**aboutMe**、**birthday**、**hireDate**、**interests**、**mySite**、**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**mailboxSettings**。</span><span class="sxs-lookup"><span data-stu-id="263b3-123">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings**</span></span>

## <a name="request-headers"></a><span data-ttu-id="263b3-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="263b3-124">Request headers</span></span>

| <span data-ttu-id="263b3-125">标头</span><span class="sxs-lookup"><span data-stu-id="263b3-125">Header</span></span>        | <span data-ttu-id="263b3-126">值</span><span class="sxs-lookup"><span data-stu-id="263b3-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="263b3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="263b3-127">Authorization</span></span> | <span data-ttu-id="263b3-128">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="263b3-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="263b3-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="263b3-129">Content-Type</span></span>  | <span data-ttu-id="263b3-130">application/json</span><span class="sxs-lookup"><span data-stu-id="263b3-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="263b3-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="263b3-131">Request body</span></span>

<span data-ttu-id="263b3-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="263b3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="263b3-133">响应</span><span class="sxs-lookup"><span data-stu-id="263b3-133">Response</span></span>

<span data-ttu-id="263b3-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="263b3-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="263b3-135">如果返回大的用户集，则可以[在应用中使用分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="263b3-135">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="263b3-136">示例</span><span class="sxs-lookup"><span data-stu-id="263b3-136">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="263b3-137">示例 1：标准用户请求</span><span class="sxs-lookup"><span data-stu-id="263b3-137">Example 1: Standard users request</span></span>

<span data-ttu-id="263b3-138">默认情况下，仅返回一组有限的属性（**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname**、**userPrincipalName**）。</span><span class="sxs-lookup"><span data-stu-id="263b3-138">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> <span data-ttu-id="263b3-139">此示例展示了默认请求和响应。</span><span class="sxs-lookup"><span data-stu-id="263b3-139">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="263b3-140">请求</span><span class="sxs-lookup"><span data-stu-id="263b3-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="263b3-141">响应</span><span class="sxs-lookup"><span data-stu-id="263b3-141">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="263b3-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="263b3-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="263b3-143">C#</span><span class="sxs-lookup"><span data-stu-id="263b3-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="263b3-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="263b3-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="263b3-145">示例 2：使用 $select 的用户请求</span><span class="sxs-lookup"><span data-stu-id="263b3-145">Example 2: Users request using $select</span></span>

<span data-ttu-id="263b3-146">如果需要其他属性集，可以使用 OData `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="263b3-146">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="263b3-147">例如，若要返回 **displayName**、**givenName**、和 **postalCode**，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`。</span><span class="sxs-lookup"><span data-stu-id="263b3-147">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="263b3-148">请求</span><span class="sxs-lookup"><span data-stu-id="263b3-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```

##### <a name="response"></a><span data-ttu-id="263b3-149">响应</span><span class="sxs-lookup"><span data-stu-id="263b3-149">Response</span></span>

<span data-ttu-id="263b3-150">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="263b3-150">Note: The response object shown here may be truncated for brevity.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="263b3-151">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="263b3-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="263b3-152">C#</span><span class="sxs-lookup"><span data-stu-id="263b3-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users_properties-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="263b3-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="263b3-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users_properties-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/user-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
