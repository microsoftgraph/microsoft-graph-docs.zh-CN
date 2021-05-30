---
title: List ownedObjects
description: 获取用户拥有的 directory 对象的列表。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e0f256351c270a67fd5ef0af293797b9b27f52c9
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703648"
---
# <a name="list-ownedobjects"></a><span data-ttu-id="9dbc4-103">List ownedObjects</span><span class="sxs-lookup"><span data-stu-id="9dbc4-103">List ownedObjects</span></span>

<span data-ttu-id="9dbc4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dbc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dbc4-105">获取用户拥有的 directory 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9dbc4-105">Get the list of directory objects that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="9dbc4-106">权限</span><span class="sxs-lookup"><span data-stu-id="9dbc4-106">Permissions</span></span>
<span data-ttu-id="9dbc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9dbc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dbc4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9dbc4-109">Permission type</span></span>      | <span data-ttu-id="9dbc4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9dbc4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dbc4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9dbc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9dbc4-112">User.Read、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9dbc4-112">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9dbc4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9dbc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dbc4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dbc4-114">Not supported.</span></span>    |
|<span data-ttu-id="9dbc4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9dbc4-115">Application</span></span> | <span data-ttu-id="9dbc4-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dbc4-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="9dbc4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9dbc4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9dbc4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9dbc4-118">Optional query parameters</span></span>
<span data-ttu-id="9dbc4-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9dbc4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9dbc4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9dbc4-120">Request headers</span></span>
| <span data-ttu-id="9dbc4-121">标头</span><span class="sxs-lookup"><span data-stu-id="9dbc4-121">Header</span></span>       | <span data-ttu-id="9dbc4-122">值</span><span class="sxs-lookup"><span data-stu-id="9dbc4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9dbc4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dbc4-123">Authorization</span></span>  | <span data-ttu-id="9dbc4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9dbc4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9dbc4-126">接受</span><span class="sxs-lookup"><span data-stu-id="9dbc4-126">Accept</span></span>  | <span data-ttu-id="9dbc4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9dbc4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dbc4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9dbc4-128">Request body</span></span>
<span data-ttu-id="9dbc4-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9dbc4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dbc4-130">响应</span><span class="sxs-lookup"><span data-stu-id="9dbc4-130">Response</span></span>

<span data-ttu-id="9dbc4-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9dbc4-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9dbc4-132">示例</span><span class="sxs-lookup"><span data-stu-id="9dbc4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9dbc4-133">请求</span><span class="sxs-lookup"><span data-stu-id="9dbc4-133">Request</span></span>
<span data-ttu-id="9dbc4-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9dbc4-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9dbc4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dbc4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="9dbc4-136">C#</span><span class="sxs-lookup"><span data-stu-id="9dbc4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9dbc4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dbc4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9dbc4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dbc4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9dbc4-139">Java</span><span class="sxs-lookup"><span data-stu-id="9dbc4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ownedobjects-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9dbc4-140">响应</span><span class="sxs-lookup"><span data-stu-id="9dbc4-140">Response</span></span>
<span data-ttu-id="9dbc4-p103">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9dbc4-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
