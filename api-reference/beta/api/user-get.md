---
title: 获取用户
description: 检索用户对象的属性和关系。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 95d0839341f158821eeb51f9aea252155462241d
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335665"
---
# <a name="get-a-user"></a><span data-ttu-id="3cfe5-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="3cfe5-103">Get a user</span></span>

<span data-ttu-id="3cfe5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cfe5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cfe5-105">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-105">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="3cfe5-106">默认情况下，此操作仅返回每位用户较常用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="3cfe5-107">这些 _默认_ 属性将记录在 [属性](../resources/user.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="3cfe5-108">要获取 _非_ 默认返回的属性，请对用户执行 [GET](user-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="3cfe5-109">由于 **用户** 资源支持 [扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取 **用户** 实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-109">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cfe5-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="3cfe5-110">Permissions</span></span>
<span data-ttu-id="3cfe5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cfe5-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cfe5-113">Permission type</span></span>      | <span data-ttu-id="3cfe5-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cfe5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cfe5-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cfe5-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3cfe5-116">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3cfe5-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3cfe5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cfe5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cfe5-118">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cfe5-118">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="3cfe5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cfe5-119">Application</span></span> | <span data-ttu-id="3cfe5-120">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cfe5-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="3cfe5-121">调用 `/me` 终结点需要已登录的用户，因此需要委派权限。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-121">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="3cfe5-122">使用 `/me` 的终结点时不支持应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-122">Application permissions are not supported when using the `/me` endpoint.</span></span>

## <a name="http-request"></a><span data-ttu-id="3cfe5-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cfe5-123">HTTP request</span></span>

<span data-ttu-id="3cfe5-124">对于特定用户：</span><span class="sxs-lookup"><span data-stu-id="3cfe5-124">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="3cfe5-125">请注意，当 **userPrincipalName** 以 `$` 字符开头时，请删除 `/users` 后的斜杠 （/），并将 **userPrincipalName** 括在圆括号和单引号中。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-125">Note that when the **userPrincipalName** begins with a `$` character, remove the slash (/) after `/users` and enclose the **userPrincipalName** in parentheses and single quotes.</span></span> <span data-ttu-id="3cfe5-126">有关详细信息，请参阅[已知问题列表](/graph/known-issues#users)。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-126">For details, see the [known issues](/graph/known-issues#users) list.</span></span>

<span data-ttu-id="3cfe5-127">对于登录用户：</span><span class="sxs-lookup"><span data-stu-id="3cfe5-127">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3cfe5-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3cfe5-128">Optional query parameters</span></span>

<span data-ttu-id="3cfe5-129">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-129">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cfe5-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cfe5-130">Request headers</span></span>

| <span data-ttu-id="3cfe5-131">标头</span><span class="sxs-lookup"><span data-stu-id="3cfe5-131">Header</span></span>       | <span data-ttu-id="3cfe5-132">值</span><span class="sxs-lookup"><span data-stu-id="3cfe5-132">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="3cfe5-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cfe5-133">Authorization</span></span>  | <span data-ttu-id="3cfe5-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="3cfe5-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3cfe5-136">Content-Type</span></span>   | <span data-ttu-id="3cfe5-137">application/json</span><span class="sxs-lookup"><span data-stu-id="3cfe5-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cfe5-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cfe5-138">Request body</span></span>

<span data-ttu-id="3cfe5-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cfe5-140">响应</span><span class="sxs-lookup"><span data-stu-id="3cfe5-140">Response</span></span>

<span data-ttu-id="3cfe5-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-141">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="3cfe5-142">当成功处理请求时，此方法会返回 `202 Accepted`，但服务器需要更多时间来完成相关的后台操作。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-142">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="3cfe5-143">示例</span><span class="sxs-lookup"><span data-stu-id="3cfe5-143">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="3cfe5-144">示例 1：获取已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="3cfe5-144">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="3cfe5-145">请求</span><span class="sxs-lookup"><span data-stu-id="3cfe5-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3cfe5-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfe5-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="c"></a>[<span data-ttu-id="3cfe5-147">C#</span><span class="sxs-lookup"><span data-stu-id="3cfe5-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cfe5-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cfe5-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cfe5-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cfe5-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cfe5-150">Java</span><span class="sxs-lookup"><span data-stu-id="3cfe5-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3cfe5-151">响应</span><span class="sxs-lookup"><span data-stu-id="3cfe5-151">Response</span></span>
<span data-ttu-id="3cfe5-p106">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-p106">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span> 

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

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="3cfe5-154">示例 2：获取指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="3cfe5-154">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="3cfe5-155">请求</span><span class="sxs-lookup"><span data-stu-id="3cfe5-155">Request</span></span>

<span data-ttu-id="3cfe5-156">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-156">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3cfe5-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfe5-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="3cfe5-158">C#</span><span class="sxs-lookup"><span data-stu-id="3cfe5-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cfe5-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cfe5-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cfe5-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cfe5-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cfe5-161">Java</span><span class="sxs-lookup"><span data-stu-id="3cfe5-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3cfe5-162">响应</span><span class="sxs-lookup"><span data-stu-id="3cfe5-162">Response</span></span>

<span data-ttu-id="3cfe5-163">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="3cfe5-163">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3cfe5-164">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3cfe5-164">See also</span></span>

- [<span data-ttu-id="3cfe5-165">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3cfe5-165">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3cfe5-166">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="3cfe5-166">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="3cfe5-167">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="3cfe5-167">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
