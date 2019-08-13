---
title: 列出经理
description: 获取用户的经理。 返回指定为用户经理的用户或联系人。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 03e8639bdd8bcd95566ae7817fb5a1004377fc0c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327155"
---
# <a name="list-manager"></a><span data-ttu-id="dc8f8-104">列出经理</span><span class="sxs-lookup"><span data-stu-id="dc8f8-104">List manager</span></span>

<span data-ttu-id="dc8f8-105">获取用户的经理。</span><span class="sxs-lookup"><span data-stu-id="dc8f8-105">Get user's manager.</span></span> <span data-ttu-id="dc8f8-106">返回指定为用户经理的用户或联系人。</span><span class="sxs-lookup"><span data-stu-id="dc8f8-106">Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc8f8-107">权限</span><span class="sxs-lookup"><span data-stu-id="dc8f8-107">Permissions</span></span>
<span data-ttu-id="dc8f8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc8f8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc8f8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc8f8-110">Permission type</span></span>      | <span data-ttu-id="dc8f8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc8f8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc8f8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc8f8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dc8f8-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dc8f8-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dc8f8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc8f8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc8f8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc8f8-115">Not supported.</span></span>    |
|<span data-ttu-id="dc8f8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc8f8-116">Application</span></span> | <span data-ttu-id="dc8f8-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc8f8-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc8f8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc8f8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dc8f8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dc8f8-119">Optional query parameters</span></span>
<span data-ttu-id="dc8f8-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dc8f8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dc8f8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc8f8-121">Request headers</span></span>
| <span data-ttu-id="dc8f8-122">标头</span><span class="sxs-lookup"><span data-stu-id="dc8f8-122">Header</span></span>       | <span data-ttu-id="dc8f8-123">值</span><span class="sxs-lookup"><span data-stu-id="dc8f8-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="dc8f8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc8f8-124">Authorization</span></span>  | <span data-ttu-id="dc8f8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc8f8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dc8f8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc8f8-127">Content-Type</span></span>   | <span data-ttu-id="dc8f8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dc8f8-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc8f8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc8f8-129">Request body</span></span>
<span data-ttu-id="dc8f8-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc8f8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc8f8-131">响应</span><span class="sxs-lookup"><span data-stu-id="dc8f8-131">Response</span></span>

<span data-ttu-id="dc8f8-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc8f8-132">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc8f8-133">示例</span><span class="sxs-lookup"><span data-stu-id="dc8f8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc8f8-134">请求</span><span class="sxs-lookup"><span data-stu-id="dc8f8-134">Request</span></span>
<span data-ttu-id="dc8f8-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc8f8-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dc8f8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc8f8-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc8f8-137">C#</span><span class="sxs-lookup"><span data-stu-id="dc8f8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc8f8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc8f8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc8f8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc8f8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc8f8-140">Java</span><span class="sxs-lookup"><span data-stu-id="dc8f8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dc8f8-141">响应</span><span class="sxs-lookup"><span data-stu-id="dc8f8-141">Response</span></span>
<span data-ttu-id="dc8f8-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dc8f8-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
