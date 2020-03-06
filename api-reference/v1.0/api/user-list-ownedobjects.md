---
title: List ownedObjects
description: 获取用户拥有的 directory 对象的列表。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c270a913fa86d426f06d06f04ee7f55fd94c1270
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509043"
---
# <a name="list-ownedobjects"></a><span data-ttu-id="6ee03-103">List ownedObjects</span><span class="sxs-lookup"><span data-stu-id="6ee03-103">List ownedObjects</span></span>

<span data-ttu-id="6ee03-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ee03-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ee03-105">获取用户拥有的 directory 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="6ee03-105">Get the list of directory objects that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ee03-106">权限</span><span class="sxs-lookup"><span data-stu-id="6ee03-106">Permissions</span></span>
<span data-ttu-id="6ee03-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ee03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ee03-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ee03-109">Permission type</span></span>      | <span data-ttu-id="6ee03-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ee03-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ee03-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ee03-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6ee03-112">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ee03-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ee03-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ee03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ee03-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ee03-114">Not supported.</span></span>    |
|<span data-ttu-id="6ee03-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ee03-115">Application</span></span> | <span data-ttu-id="6ee03-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ee03-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6ee03-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ee03-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ee03-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6ee03-118">Optional query parameters</span></span>
<span data-ttu-id="6ee03-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6ee03-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6ee03-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ee03-120">Request headers</span></span>
| <span data-ttu-id="6ee03-121">标头</span><span class="sxs-lookup"><span data-stu-id="6ee03-121">Header</span></span>       | <span data-ttu-id="6ee03-122">值</span><span class="sxs-lookup"><span data-stu-id="6ee03-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6ee03-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ee03-123">Authorization</span></span>  | <span data-ttu-id="6ee03-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ee03-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6ee03-126">接受</span><span class="sxs-lookup"><span data-stu-id="6ee03-126">Accept</span></span>  | <span data-ttu-id="6ee03-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6ee03-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ee03-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ee03-128">Request body</span></span>
<span data-ttu-id="6ee03-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ee03-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ee03-130">响应</span><span class="sxs-lookup"><span data-stu-id="6ee03-130">Response</span></span>

<span data-ttu-id="6ee03-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6ee03-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ee03-132">示例</span><span class="sxs-lookup"><span data-stu-id="6ee03-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ee03-133">请求</span><span class="sxs-lookup"><span data-stu-id="6ee03-133">Request</span></span>
<span data-ttu-id="6ee03-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ee03-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ee03-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ee03-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="6ee03-136">C#</span><span class="sxs-lookup"><span data-stu-id="6ee03-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ee03-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ee03-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ee03-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ee03-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ee03-139">Java</span><span class="sxs-lookup"><span data-stu-id="6ee03-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ownedobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6ee03-140">响应</span><span class="sxs-lookup"><span data-stu-id="6ee03-140">Response</span></span>
<span data-ttu-id="6ee03-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ee03-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
