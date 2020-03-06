---
title: 列出经理
description: 获取用户的经理。 返回指定为用户经理的用户或联系人。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1f73127c95981bc22d4269e7a8e57aa570e64f2b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509071"
---
# <a name="list-manager"></a><span data-ttu-id="ffbf1-104">列出经理</span><span class="sxs-lookup"><span data-stu-id="ffbf1-104">List manager</span></span>

<span data-ttu-id="ffbf1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffbf1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffbf1-106">获取用户的经理。</span><span class="sxs-lookup"><span data-stu-id="ffbf1-106">Get user's manager.</span></span> <span data-ttu-id="ffbf1-107">返回指定为用户经理的用户或组织联系人。</span><span class="sxs-lookup"><span data-stu-id="ffbf1-107">Returns the user or organizational contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="ffbf1-108">权限</span><span class="sxs-lookup"><span data-stu-id="ffbf1-108">Permissions</span></span>
<span data-ttu-id="ffbf1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffbf1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffbf1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffbf1-111">Permission type</span></span>      | <span data-ttu-id="ffbf1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ffbf1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffbf1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffbf1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ffbf1-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ffbf1-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ffbf1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffbf1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffbf1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffbf1-116">Not supported.</span></span>    |
|<span data-ttu-id="ffbf1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffbf1-117">Application</span></span> | <span data-ttu-id="ffbf1-118">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffbf1-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ffbf1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffbf1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ffbf1-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ffbf1-120">Optional query parameters</span></span>
<span data-ttu-id="ffbf1-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ffbf1-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ffbf1-122">请求头</span><span class="sxs-lookup"><span data-stu-id="ffbf1-122">Request headers</span></span>
| <span data-ttu-id="ffbf1-123">标头</span><span class="sxs-lookup"><span data-stu-id="ffbf1-123">Header</span></span>       | <span data-ttu-id="ffbf1-124">值</span><span class="sxs-lookup"><span data-stu-id="ffbf1-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="ffbf1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffbf1-125">Authorization</span></span>  | <span data-ttu-id="ffbf1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ffbf1-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ffbf1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffbf1-128">Request body</span></span>
<span data-ttu-id="ffbf1-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ffbf1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffbf1-130">响应</span><span class="sxs-lookup"><span data-stu-id="ffbf1-130">Response</span></span>

<span data-ttu-id="ffbf1-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ffbf1-131">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ffbf1-132">示例</span><span class="sxs-lookup"><span data-stu-id="ffbf1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ffbf1-133">请求</span><span class="sxs-lookup"><span data-stu-id="ffbf1-133">Request</span></span>
<span data-ttu-id="ffbf1-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ffbf1-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ffbf1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffbf1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
# <a name="c"></a>[<span data-ttu-id="ffbf1-136">C#</span><span class="sxs-lookup"><span data-stu-id="ffbf1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ffbf1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffbf1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ffbf1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffbf1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ffbf1-139">Java</span><span class="sxs-lookup"><span data-stu-id="ffbf1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ffbf1-140">响应</span><span class="sxs-lookup"><span data-stu-id="ffbf1-140">Response</span></span>
<span data-ttu-id="ffbf1-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ffbf1-141">The following is an example of the response.</span></span>
><span data-ttu-id="ffbf1-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ffbf1-142">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
