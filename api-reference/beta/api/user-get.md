---
title: 获取用户
description: 检索用户对象的属性和关系。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b1f274c1bdf2d179ed5ee91e98d7e0e8952d0cbd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451941"
---
# <a name="get-a-user"></a><span data-ttu-id="09241-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="09241-103">Get a user</span></span>

<span data-ttu-id="09241-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09241-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09241-105">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="09241-105">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="09241-106">默认情况下，此操作仅返回每位用户较常用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="09241-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="09241-107">这些_默认_属性将记录在[属性](../resources/user.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="09241-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="09241-108">要获取_非_默认返回的属性，请对用户执行 [GET](user-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="09241-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="09241-109">由于**用户**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**用户**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="09241-109">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="09241-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="09241-110">Permissions</span></span>
<span data-ttu-id="09241-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09241-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09241-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="09241-113">Permission type</span></span>      | <span data-ttu-id="09241-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09241-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09241-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09241-115">Delegated (work or school account)</span></span> | <span data-ttu-id="09241-116">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09241-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="09241-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09241-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09241-118">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09241-118">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="09241-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="09241-119">Application</span></span> | <span data-ttu-id="09241-120">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09241-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09241-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09241-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="09241-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="09241-122">Optional query parameters</span></span>
<span data-ttu-id="09241-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="09241-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="09241-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="09241-124">Request headers</span></span>
| <span data-ttu-id="09241-125">标头</span><span class="sxs-lookup"><span data-stu-id="09241-125">Header</span></span>       | <span data-ttu-id="09241-126">值</span><span class="sxs-lookup"><span data-stu-id="09241-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="09241-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="09241-127">Authorization</span></span>  | <span data-ttu-id="09241-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09241-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="09241-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09241-130">Content-Type</span></span>   | <span data-ttu-id="09241-131">application/json</span><span class="sxs-lookup"><span data-stu-id="09241-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="09241-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="09241-132">Request body</span></span>
<span data-ttu-id="09241-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="09241-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09241-134">响应</span><span class="sxs-lookup"><span data-stu-id="09241-134">Response</span></span>

<span data-ttu-id="09241-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09241-135">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="09241-136">当成功处理请求时，此方法会返回 `202 Accepted`，但服务器需要更多时间来完成相关的后台操作。</span><span class="sxs-lookup"><span data-stu-id="09241-136">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="09241-137">示例</span><span class="sxs-lookup"><span data-stu-id="09241-137">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="09241-138">示例 1：获取已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="09241-138">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="09241-139">请求</span><span class="sxs-lookup"><span data-stu-id="09241-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="09241-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="09241-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="c"></a>[<span data-ttu-id="09241-141">C#</span><span class="sxs-lookup"><span data-stu-id="09241-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09241-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09241-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09241-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09241-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="09241-144">响应</span><span class="sxs-lookup"><span data-stu-id="09241-144">Response</span></span>
<span data-ttu-id="09241-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="09241-145">Here is an example of the response.</span></span> <span data-ttu-id="09241-146">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="09241-146">Note: The response object shown here may be truncated for brevity.</span></span> 

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

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="09241-147">示例 2：获取指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="09241-147">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="09241-148">请求</span><span class="sxs-lookup"><span data-stu-id="09241-148">Request</span></span>

<span data-ttu-id="09241-149">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="09241-149">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="09241-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="09241-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="09241-151">C#</span><span class="sxs-lookup"><span data-stu-id="09241-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09241-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09241-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09241-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09241-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="09241-154">响应</span><span class="sxs-lookup"><span data-stu-id="09241-154">Response</span></span>

<span data-ttu-id="09241-155">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="09241-155">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="09241-156">另请参阅</span><span class="sxs-lookup"><span data-stu-id="09241-156">See also</span></span>

- [<span data-ttu-id="09241-157">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="09241-157">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="09241-158">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="09241-158">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="09241-159">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="09241-159">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
