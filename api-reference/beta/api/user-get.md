---
title: 获取用户
description: 检索用户对象的属性和关系。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c3bb42bd8acaecde27bb2df2e9d80eb4e2a70f3e
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275754"
---
# <a name="get-a-user"></a><span data-ttu-id="66528-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="66528-103">Get a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66528-104">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66528-104">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="66528-105">由于**用户**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**用户**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="66528-105">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="66528-106">权限</span><span class="sxs-lookup"><span data-stu-id="66528-106">Permissions</span></span>
<span data-ttu-id="66528-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66528-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66528-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="66528-109">Permission type</span></span>      | <span data-ttu-id="66528-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66528-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66528-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66528-111">Delegated (work or school account)</span></span> | <span data-ttu-id="66528-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66528-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66528-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66528-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66528-114">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66528-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="66528-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="66528-115">Application</span></span> | <span data-ttu-id="66528-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66528-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66528-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66528-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66528-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="66528-118">Optional query parameters</span></span>
<span data-ttu-id="66528-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="66528-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="66528-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="66528-120">Request headers</span></span>
| <span data-ttu-id="66528-121">标头</span><span class="sxs-lookup"><span data-stu-id="66528-121">Header</span></span>       | <span data-ttu-id="66528-122">值</span><span class="sxs-lookup"><span data-stu-id="66528-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="66528-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66528-123">Authorization</span></span>  | <span data-ttu-id="66528-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66528-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="66528-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66528-126">Content-Type</span></span>   | <span data-ttu-id="66528-127">application/json</span><span class="sxs-lookup"><span data-stu-id="66528-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="66528-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="66528-128">Request body</span></span>
<span data-ttu-id="66528-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66528-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66528-130">响应</span><span class="sxs-lookup"><span data-stu-id="66528-130">Response</span></span>

<span data-ttu-id="66528-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66528-131">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="66528-132">当成功处理请求时，此方法会返回 `202 Accepted`，但服务器需要更多时间来完成相关的后台操作。</span><span class="sxs-lookup"><span data-stu-id="66528-132">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="66528-133">示例</span><span class="sxs-lookup"><span data-stu-id="66528-133">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="66528-134">示例 1：获取已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="66528-134">Example 1: Get the photo of the signed-in user in the largest available size</span></span>

#### <a name="request"></a><span data-ttu-id="66528-135">请求</span><span class="sxs-lookup"><span data-stu-id="66528-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="66528-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="66528-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="66528-137">C#</span><span class="sxs-lookup"><span data-stu-id="66528-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66528-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66528-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="66528-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66528-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="66528-140">响应</span><span class="sxs-lookup"><span data-stu-id="66528-140">Response</span></span>
<span data-ttu-id="66528-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="66528-141">Here is an example of the response.</span></span> <span data-ttu-id="66528-142">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="66528-142">Note: The response object shown here may be truncated for brevity.</span></span> 

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

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="66528-143">示例 2：获取指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="66528-143">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="66528-144">请求</span><span class="sxs-lookup"><span data-stu-id="66528-144">Request</span></span>

<span data-ttu-id="66528-145">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="66528-145">The following example shows how to create a request context.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}
```

#### <a name="response"></a><span data-ttu-id="66528-146">响应</span><span class="sxs-lookup"><span data-stu-id="66528-146">Response</span></span>

<span data-ttu-id="66528-147">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="66528-147">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="66528-148">另请参阅</span><span class="sxs-lookup"><span data-stu-id="66528-148">See also</span></span>

- [<span data-ttu-id="66528-149">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="66528-149">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="66528-150">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="66528-150">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="66528-151">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="66528-151">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
