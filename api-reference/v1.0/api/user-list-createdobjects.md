---
title: List createdObjects
description: 获取由用户创建的 directory 对象列表。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 55d8d87378eddf3b176d0138ed2f8c32b659142c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049371"
---
# <a name="list-createdobjects"></a><span data-ttu-id="70b19-103">List createdObjects</span><span class="sxs-lookup"><span data-stu-id="70b19-103">List createdObjects</span></span>

<span data-ttu-id="70b19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70b19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70b19-105">获取由用户创建的 directory 对象列表。</span><span class="sxs-lookup"><span data-stu-id="70b19-105">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="70b19-106">权限</span><span class="sxs-lookup"><span data-stu-id="70b19-106">Permissions</span></span>
<span data-ttu-id="70b19-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70b19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70b19-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="70b19-109">Permission type</span></span>      | <span data-ttu-id="70b19-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70b19-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70b19-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70b19-111">Delegated (work or school account)</span></span> | <span data-ttu-id="70b19-112">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70b19-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="70b19-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70b19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70b19-114">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70b19-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="70b19-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="70b19-115">Application</span></span> | <span data-ttu-id="70b19-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70b19-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="70b19-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70b19-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="70b19-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="70b19-118">Optional query parameters</span></span>
<span data-ttu-id="70b19-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="70b19-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="70b19-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="70b19-120">Request headers</span></span>
| <span data-ttu-id="70b19-121">标头</span><span class="sxs-lookup"><span data-stu-id="70b19-121">Header</span></span>       | <span data-ttu-id="70b19-122">值</span><span class="sxs-lookup"><span data-stu-id="70b19-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70b19-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70b19-123">Authorization</span></span>  | <span data-ttu-id="70b19-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70b19-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="70b19-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70b19-126">Content-Type</span></span>  | <span data-ttu-id="70b19-127">application/json</span><span class="sxs-lookup"><span data-stu-id="70b19-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70b19-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="70b19-128">Request body</span></span>
<span data-ttu-id="70b19-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="70b19-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70b19-130">响应</span><span class="sxs-lookup"><span data-stu-id="70b19-130">Response</span></span>

<span data-ttu-id="70b19-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="70b19-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70b19-132">示例</span><span class="sxs-lookup"><span data-stu-id="70b19-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70b19-133">请求</span><span class="sxs-lookup"><span data-stu-id="70b19-133">Request</span></span>
<span data-ttu-id="70b19-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70b19-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70b19-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="70b19-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="70b19-136">C#</span><span class="sxs-lookup"><span data-stu-id="70b19-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70b19-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70b19-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70b19-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70b19-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70b19-139">Java</span><span class="sxs-lookup"><span data-stu-id="70b19-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="70b19-140">响应</span><span class="sxs-lookup"><span data-stu-id="70b19-140">Response</span></span>
<span data-ttu-id="70b19-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="70b19-141">Here is an example of the response.</span></span> <span data-ttu-id="70b19-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="70b19-142">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
