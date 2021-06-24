---
title: 获取用户
description: 检索用户对象的属性和关系。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2014b20abe0cdcc37c4bca2f1341aabe425b556c
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108878"
---
# <a name="get-a-user"></a><span data-ttu-id="93329-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="93329-103">Get a user</span></span>

<span data-ttu-id="93329-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93329-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93329-105">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="93329-105">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="93329-106">默认情况下，此操作仅返回每位用户较常用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="93329-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="93329-107">这些 _默认_ 属性将记录在 [属性](../resources/user.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="93329-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="93329-108">要获取 _非_ 默认返回的属性，请对用户执行 [GET](user-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="93329-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="93329-109">由于 **用户** 资源支持 [扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取 **用户** 实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="93329-109">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="93329-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="93329-110">Permissions</span></span>
<span data-ttu-id="93329-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93329-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93329-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="93329-113">Permission type</span></span>      | <span data-ttu-id="93329-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93329-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93329-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93329-115">Delegated (work or school account)</span></span> | <span data-ttu-id="93329-116">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="93329-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="93329-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93329-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93329-118">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93329-118">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="93329-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="93329-119">Application</span></span> | <span data-ttu-id="93329-120">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93329-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="93329-121">调用 `/me` 终结点需要已登录的用户，因此需要委派权限。</span><span class="sxs-lookup"><span data-stu-id="93329-121">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="93329-122">使用 `/me` 的终结点时不支持应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="93329-122">Application permissions are not supported when using the `/me` endpoint.</span></span>

## <a name="http-request"></a><span data-ttu-id="93329-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93329-123">HTTP request</span></span>

<span data-ttu-id="93329-124">对于特定用户：</span><span class="sxs-lookup"><span data-stu-id="93329-124">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

><span data-ttu-id="93329-125">**注意：**</span><span class="sxs-lookup"><span data-stu-id="93329-125">**Note:**</span></span>
> + <span data-ttu-id="93329-p104">当 **userPrincipalName** 以 `$` 字符开头时，请删除 `/users` 后的斜杠 (/)，并将 **userPrincipalName** 放在圆括号和单引号中。例如 `/users('$AdeleVance@contoso.com')`。有关详细信息，请参阅“[已知问题](/graph/known-issues#users)”列表。</span><span class="sxs-lookup"><span data-stu-id="93329-p104">When the **userPrincipalName** begins with a `$` character, remove the slash (/) after `/users` and enclose the **userPrincipalName** in parentheses and single quotes. For example, `/users('$AdeleVance@contoso.com')`. For details, see the [known issues](/graph/known-issues#users) list.</span></span>
> + <span data-ttu-id="93329-129">要使用 **userPrincipalName** 查询 B2B 用户，请对哈希 (#) 字符进行编码。</span><span class="sxs-lookup"><span data-stu-id="93329-129">To query a B2B user using the **userPrincipalName**, encode the hash (#) character.</span></span> <span data-ttu-id="93329-130">也就是说，将 `#` 符号替换为 `%23`。</span><span class="sxs-lookup"><span data-stu-id="93329-130">That is, replace the `#` symbol with `%23`.</span></span> <span data-ttu-id="93329-131">例如，`/users/AdeleVance_adatum.com%23EXT%23@contoso.com`。</span><span class="sxs-lookup"><span data-stu-id="93329-131">For example, `/users/AdeleVance_adatum.com%23EXT%23@contoso.com`.</span></span>

<span data-ttu-id="93329-132">对于登录用户：</span><span class="sxs-lookup"><span data-stu-id="93329-132">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93329-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="93329-133">Optional query parameters</span></span>

<span data-ttu-id="93329-134">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="93329-134">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93329-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="93329-135">Request headers</span></span>

| <span data-ttu-id="93329-136">标头</span><span class="sxs-lookup"><span data-stu-id="93329-136">Header</span></span>       | <span data-ttu-id="93329-137">值</span><span class="sxs-lookup"><span data-stu-id="93329-137">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="93329-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="93329-138">Authorization</span></span>  | <span data-ttu-id="93329-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="93329-p106">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="93329-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93329-141">Content-Type</span></span>   | <span data-ttu-id="93329-142">application/json</span><span class="sxs-lookup"><span data-stu-id="93329-142">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="93329-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="93329-143">Request body</span></span>

<span data-ttu-id="93329-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="93329-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93329-145">响应</span><span class="sxs-lookup"><span data-stu-id="93329-145">Response</span></span>

<span data-ttu-id="93329-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93329-146">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="93329-147">当成功处理请求时，此方法会返回 `202 Accepted`，但服务器需要更多时间来完成相关的后台操作。</span><span class="sxs-lookup"><span data-stu-id="93329-147">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="93329-148">示例</span><span class="sxs-lookup"><span data-stu-id="93329-148">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="93329-149">示例 1：获取已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="93329-149">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="93329-150">请求</span><span class="sxs-lookup"><span data-stu-id="93329-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="93329-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="93329-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="c"></a>[<span data-ttu-id="93329-152">C#</span><span class="sxs-lookup"><span data-stu-id="93329-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93329-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93329-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93329-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93329-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93329-155">Java</span><span class="sxs-lookup"><span data-stu-id="93329-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="93329-156">响应</span><span class="sxs-lookup"><span data-stu-id="93329-156">Response</span></span>
<span data-ttu-id="93329-p107">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="93329-p107">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span> 

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

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="93329-159">示例 2：获取指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="93329-159">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="93329-160">请求</span><span class="sxs-lookup"><span data-stu-id="93329-160">Request</span></span>

<span data-ttu-id="93329-161">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="93329-161">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="93329-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="93329-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="93329-163">C#</span><span class="sxs-lookup"><span data-stu-id="93329-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93329-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93329-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93329-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93329-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93329-166">Java</span><span class="sxs-lookup"><span data-stu-id="93329-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="93329-167">响应</span><span class="sxs-lookup"><span data-stu-id="93329-167">Response</span></span>

<span data-ttu-id="93329-168">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="93329-168">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="93329-169">另请参阅</span><span class="sxs-lookup"><span data-stu-id="93329-169">See also</span></span>

- [<span data-ttu-id="93329-170">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="93329-170">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="93329-171">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="93329-171">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="93329-172">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="93329-172">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
