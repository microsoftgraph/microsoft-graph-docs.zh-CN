---
title: 获取用户
description: 检索用户对象的属性和关系。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e6caed0bcd6a8327068726a403b7531354864a25
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720135"
---
# <a name="get-a-user"></a><span data-ttu-id="2adea-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="2adea-103">Get a user</span></span>

<span data-ttu-id="2adea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2adea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2adea-105">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2adea-105">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="2adea-106">默认情况下，此操作仅返回每位用户较常用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="2adea-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="2adea-107">这些 _默认_ 属性将记录在 [属性](../resources/user.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="2adea-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="2adea-108">要获取 _非_ 默认返回的属性，请对用户执行 [GET](user-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="2adea-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="2adea-109">由于 **用户** 资源支持 [扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取 **用户** 实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="2adea-109">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="2adea-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="2adea-110">Permissions</span></span>
<span data-ttu-id="2adea-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2adea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2adea-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="2adea-113">Permission type</span></span>      | <span data-ttu-id="2adea-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2adea-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2adea-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2adea-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2adea-116">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2adea-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2adea-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2adea-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2adea-118">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2adea-118">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="2adea-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="2adea-119">Application</span></span> | <span data-ttu-id="2adea-120">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2adea-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="2adea-121">调用 `/me` 终结点需要已登录的用户，因此需要委派权限。</span><span class="sxs-lookup"><span data-stu-id="2adea-121">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="2adea-122">使用 `/me` 终结点时不支持应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="2adea-122">Application permissions are not supported when using the `/me` endpoint.</span></span>

<span data-ttu-id="2adea-123">对于特定用户：</span><span class="sxs-lookup"><span data-stu-id="2adea-123">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="2adea-124">对于登录用户：</span><span class="sxs-lookup"><span data-stu-id="2adea-124">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2adea-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2adea-125">Optional query parameters</span></span>

<span data-ttu-id="2adea-126">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2adea-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2adea-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="2adea-127">Request headers</span></span>

| <span data-ttu-id="2adea-128">标头</span><span class="sxs-lookup"><span data-stu-id="2adea-128">Header</span></span>       | <span data-ttu-id="2adea-129">值</span><span class="sxs-lookup"><span data-stu-id="2adea-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="2adea-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2adea-130">Authorization</span></span>  | <span data-ttu-id="2adea-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2adea-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2adea-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2adea-133">Content-Type</span></span>   | <span data-ttu-id="2adea-134">application/json</span><span class="sxs-lookup"><span data-stu-id="2adea-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2adea-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="2adea-135">Request body</span></span>

<span data-ttu-id="2adea-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2adea-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2adea-137">响应</span><span class="sxs-lookup"><span data-stu-id="2adea-137">Response</span></span>

<span data-ttu-id="2adea-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2adea-138">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="2adea-139">当成功处理请求时，此方法会返回 `202 Accepted`，但服务器需要更多时间来完成相关的后台操作。</span><span class="sxs-lookup"><span data-stu-id="2adea-139">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="2adea-140">示例</span><span class="sxs-lookup"><span data-stu-id="2adea-140">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="2adea-141">示例 1：获取已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="2adea-141">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="2adea-142">请求</span><span class="sxs-lookup"><span data-stu-id="2adea-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2adea-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="2adea-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="c"></a>[<span data-ttu-id="2adea-144">C#</span><span class="sxs-lookup"><span data-stu-id="2adea-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2adea-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2adea-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2adea-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2adea-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2adea-147">Java</span><span class="sxs-lookup"><span data-stu-id="2adea-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2adea-148">响应</span><span class="sxs-lookup"><span data-stu-id="2adea-148">Response</span></span>
<span data-ttu-id="2adea-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2adea-149">Here is an example of the response.</span></span> <span data-ttu-id="2adea-150">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2adea-150">Note: The response object shown here may be truncated for brevity.</span></span> 

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

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="2adea-151">示例 2：获取指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="2adea-151">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="2adea-152">请求</span><span class="sxs-lookup"><span data-stu-id="2adea-152">Request</span></span>

<span data-ttu-id="2adea-153">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="2adea-153">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2adea-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="2adea-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="2adea-155">C#</span><span class="sxs-lookup"><span data-stu-id="2adea-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2adea-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2adea-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2adea-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2adea-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2adea-158">Java</span><span class="sxs-lookup"><span data-stu-id="2adea-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2adea-159">响应</span><span class="sxs-lookup"><span data-stu-id="2adea-159">Response</span></span>

<span data-ttu-id="2adea-160">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="2adea-160">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2adea-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2adea-161">See also</span></span>

- [<span data-ttu-id="2adea-162">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2adea-162">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2adea-163">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="2adea-163">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2adea-164">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="2adea-164">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
