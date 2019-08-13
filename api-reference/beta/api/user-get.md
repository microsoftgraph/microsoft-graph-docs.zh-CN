---
title: 获取用户
description: 检索用户对象的属性和关系。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 62dfe5b42bd3c2f5cc5c55d6b98e62c9191d7196
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362357"
---
# <a name="get-a-user"></a><span data-ttu-id="80a1f-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="80a1f-103">Get a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80a1f-104">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="80a1f-104">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="80a1f-105">由于**用户**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**用户**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="80a1f-105">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="80a1f-106">权限</span><span class="sxs-lookup"><span data-stu-id="80a1f-106">Permissions</span></span>
<span data-ttu-id="80a1f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80a1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80a1f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="80a1f-109">Permission type</span></span>      | <span data-ttu-id="80a1f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80a1f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80a1f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80a1f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="80a1f-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="80a1f-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="80a1f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80a1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80a1f-114">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80a1f-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="80a1f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80a1f-115">Application</span></span> | <span data-ttu-id="80a1f-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80a1f-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80a1f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80a1f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="80a1f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="80a1f-118">Optional query parameters</span></span>
<span data-ttu-id="80a1f-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="80a1f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="80a1f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="80a1f-120">Request headers</span></span>
| <span data-ttu-id="80a1f-121">标头</span><span class="sxs-lookup"><span data-stu-id="80a1f-121">Header</span></span>       | <span data-ttu-id="80a1f-122">值</span><span class="sxs-lookup"><span data-stu-id="80a1f-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="80a1f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80a1f-123">Authorization</span></span>  | <span data-ttu-id="80a1f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80a1f-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="80a1f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="80a1f-126">Content-Type</span></span>   | <span data-ttu-id="80a1f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="80a1f-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="80a1f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="80a1f-128">Request body</span></span>
<span data-ttu-id="80a1f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80a1f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80a1f-130">响应</span><span class="sxs-lookup"><span data-stu-id="80a1f-130">Response</span></span>

<span data-ttu-id="80a1f-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80a1f-131">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="80a1f-132">当成功处理请求时，此方法会返回 `202 Accepted`，但服务器需要更多时间来完成相关的后台操作。</span><span class="sxs-lookup"><span data-stu-id="80a1f-132">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="80a1f-133">示例</span><span class="sxs-lookup"><span data-stu-id="80a1f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80a1f-134">请求</span><span class="sxs-lookup"><span data-stu-id="80a1f-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="80a1f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="80a1f-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="80a1f-136">C#</span><span class="sxs-lookup"><span data-stu-id="80a1f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80a1f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80a1f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80a1f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80a1f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="80a1f-139">Java</span><span class="sxs-lookup"><span data-stu-id="80a1f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="80a1f-140">响应</span><span class="sxs-lookup"><span data-stu-id="80a1f-140">Response</span></span>
<span data-ttu-id="80a1f-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="80a1f-141">Here is an example of the response.</span></span> <span data-ttu-id="80a1f-142">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="80a1f-142">Note: The response object shown here may be truncated for brevity.</span></span> 

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

## <a name="see-also"></a><span data-ttu-id="80a1f-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="80a1f-143">See also</span></span>

- [<span data-ttu-id="80a1f-144">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="80a1f-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="80a1f-145">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="80a1f-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="80a1f-146">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="80a1f-146">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
