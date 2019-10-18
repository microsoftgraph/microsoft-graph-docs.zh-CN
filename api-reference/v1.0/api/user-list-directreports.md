---
title: 列出 directReports
description: 获取用户的直接下属。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 61a0ab07a5c8b866dc1f21054f3532fc48486388
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729033"
---
# <a name="list-directreports"></a><span data-ttu-id="c2cfb-103">列出 directReports</span><span class="sxs-lookup"><span data-stu-id="c2cfb-103">List directReports</span></span>

<span data-ttu-id="c2cfb-104">获取用户的直接下属。</span><span class="sxs-lookup"><span data-stu-id="c2cfb-104">Get user's direct reports.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2cfb-105">权限</span><span class="sxs-lookup"><span data-stu-id="c2cfb-105">Permissions</span></span>
<span data-ttu-id="c2cfb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2cfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2cfb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2cfb-108">Permission type</span></span>      | <span data-ttu-id="c2cfb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2cfb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2cfb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2cfb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2cfb-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c2cfb-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c2cfb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2cfb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2cfb-113">不支持</span><span class="sxs-lookup"><span data-stu-id="c2cfb-113">Not supported</span></span> |
|<span data-ttu-id="c2cfb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2cfb-114">Application</span></span> | <span data-ttu-id="c2cfb-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2cfb-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2cfb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2cfb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2cfb-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c2cfb-117">Optional query parameters</span></span>
<span data-ttu-id="c2cfb-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c2cfb-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2cfb-119">请求头</span><span class="sxs-lookup"><span data-stu-id="c2cfb-119">Request headers</span></span>
| <span data-ttu-id="c2cfb-120">标头</span><span class="sxs-lookup"><span data-stu-id="c2cfb-120">Header</span></span>       | <span data-ttu-id="c2cfb-121">值</span><span class="sxs-lookup"><span data-stu-id="c2cfb-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="c2cfb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2cfb-122">Authorization</span></span>  | <span data-ttu-id="c2cfb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2cfb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c2cfb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2cfb-125">Content-Type</span></span>   | <span data-ttu-id="c2cfb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2cfb-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2cfb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2cfb-127">Request body</span></span>
<span data-ttu-id="c2cfb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c2cfb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2cfb-129">响应</span><span class="sxs-lookup"><span data-stu-id="c2cfb-129">Response</span></span>

<span data-ttu-id="c2cfb-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c2cfb-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2cfb-131">示例</span><span class="sxs-lookup"><span data-stu-id="c2cfb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2cfb-132">请求</span><span class="sxs-lookup"><span data-stu-id="c2cfb-132">Request</span></span>
<span data-ttu-id="c2cfb-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2cfb-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2cfb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2cfb-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/directReports
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2cfb-135">C#</span><span class="sxs-lookup"><span data-stu-id="c2cfb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2cfb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2cfb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2cfb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2cfb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c2cfb-138">Java</span><span class="sxs-lookup"><span data-stu-id="c2cfb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c2cfb-139">响应</span><span class="sxs-lookup"><span data-stu-id="c2cfb-139">Response</span></span>
<span data-ttu-id="c2cfb-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c2cfb-140">Here is an example of the response.</span></span> 

><span data-ttu-id="c2cfb-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c2cfb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
