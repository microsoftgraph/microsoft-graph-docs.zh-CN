---
title: 列出用户
description: 检索用户对象列表。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eac2031d6de80937598a66dd6086e7419dff3f1f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357540"
---
# <a name="list-users"></a><span data-ttu-id="73b34-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="73b34-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73b34-104">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="73b34-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="73b34-105">权限</span><span class="sxs-lookup"><span data-stu-id="73b34-105">Permissions</span></span>

<span data-ttu-id="73b34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73b34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73b34-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="73b34-108">Permission type</span></span>      | <span data-ttu-id="73b34-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73b34-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73b34-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73b34-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73b34-111">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73b34-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73b34-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73b34-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73b34-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="73b34-113">Not supported.</span></span>    |
|<span data-ttu-id="73b34-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="73b34-114">Application</span></span> | <span data-ttu-id="73b34-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73b34-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73b34-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73b34-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73b34-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="73b34-117">Optional query parameters</span></span>

<span data-ttu-id="73b34-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="73b34-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73b34-119">请求头</span><span class="sxs-lookup"><span data-stu-id="73b34-119">Request headers</span></span>
| <span data-ttu-id="73b34-120">标头</span><span class="sxs-lookup"><span data-stu-id="73b34-120">Header</span></span>        | <span data-ttu-id="73b34-121">值</span><span class="sxs-lookup"><span data-stu-id="73b34-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="73b34-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73b34-122">Authorization</span></span> | <span data-ttu-id="73b34-123">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="73b34-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="73b34-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73b34-124">Content-Type</span></span>  | <span data-ttu-id="73b34-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73b34-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="73b34-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="73b34-126">Request body</span></span>

<span data-ttu-id="73b34-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73b34-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73b34-128">响应</span><span class="sxs-lookup"><span data-stu-id="73b34-128">Response</span></span>

<span data-ttu-id="73b34-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="73b34-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73b34-130">示例</span><span class="sxs-lookup"><span data-stu-id="73b34-130">Example</span></span>

### <a name="example-1-list-all-users"></a><span data-ttu-id="73b34-131">示例 1：列出所有用户</span><span class="sxs-lookup"><span data-stu-id="73b34-131">Example 1: List all users</span></span>

#### <a name="request"></a><span data-ttu-id="73b34-132">请求</span><span class="sxs-lookup"><span data-stu-id="73b34-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="73b34-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="73b34-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73b34-134">C#</span><span class="sxs-lookup"><span data-stu-id="73b34-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73b34-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73b34-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73b34-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73b34-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="73b34-137">响应</span><span class="sxs-lookup"><span data-stu-id="73b34-137">Response</span></span>

<span data-ttu-id="73b34-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="73b34-138">Here is an example of the response.</span></span> 

><span data-ttu-id="73b34-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="73b34-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="73b34-141">示例 2：使用登录名查找用户帐户</span><span class="sxs-lookup"><span data-stu-id="73b34-141">Example 2: Find a user account using a sign-in name</span></span>

<span data-ttu-id="73b34-142">使用登录名（也称为本地帐户）在 B2C 租户中查找用户帐户。</span><span class="sxs-lookup"><span data-stu-id="73b34-142">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="73b34-143">此请求可由技术支持人员用于在 B2C 租户中查找客户的用户帐户（此示例中，B2C 租户是 contoso.onmicrosoft.com）。</span><span class="sxs-lookup"><span data-stu-id="73b34-143">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="73b34-144">根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="73b34-144">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="73b34-145">请求</span><span class="sxs-lookup"><span data-stu-id="73b34-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="73b34-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="73b34-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```http
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73b34-147">C#</span><span class="sxs-lookup"><span data-stu-id="73b34-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73b34-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73b34-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73b34-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73b34-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="73b34-150">响应</span><span class="sxs-lookup"><span data-stu-id="73b34-150">Response</span></span>

<span data-ttu-id="73b34-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="73b34-151">Here is an example of the response.</span></span> 

> <span data-ttu-id="73b34-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="73b34-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
