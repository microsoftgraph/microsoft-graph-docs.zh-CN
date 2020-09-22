---
title: 删除 educationSchool
description: 删除学校。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 14921cfd46bb9c6ac3ac60f7f65c027e9d3bd0aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063708"
---
# <a name="delete-educationschool"></a><span data-ttu-id="c1560-103">删除 educationSchool</span><span class="sxs-lookup"><span data-stu-id="c1560-103">Delete educationSchool</span></span>

<span data-ttu-id="c1560-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1560-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1560-105">删除学校。</span><span class="sxs-lookup"><span data-stu-id="c1560-105">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1560-106">权限</span><span class="sxs-lookup"><span data-stu-id="c1560-106">Permissions</span></span>
<span data-ttu-id="c1560-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1560-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1560-109">Permission type</span></span>      | <span data-ttu-id="c1560-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1560-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1560-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1560-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c1560-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1560-112">Not supported.</span></span>  |
|<span data-ttu-id="c1560-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1560-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c1560-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1560-114">Not supported.</span></span>  |
|<span data-ttu-id="c1560-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1560-115">Application</span></span> | <span data-ttu-id="c1560-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1560-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c1560-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1560-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c1560-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1560-118">Request headers</span></span>
| <span data-ttu-id="c1560-119">标头</span><span class="sxs-lookup"><span data-stu-id="c1560-119">Header</span></span>       | <span data-ttu-id="c1560-120">值</span><span class="sxs-lookup"><span data-stu-id="c1560-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1560-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1560-121">Authorization</span></span>  | <span data-ttu-id="c1560-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1560-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1560-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1560-124">Request body</span></span>
<span data-ttu-id="c1560-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1560-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c1560-126">响应</span><span class="sxs-lookup"><span data-stu-id="c1560-126">Response</span></span>
<span data-ttu-id="c1560-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c1560-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1560-129">示例</span><span class="sxs-lookup"><span data-stu-id="c1560-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1560-130">请求</span><span class="sxs-lookup"><span data-stu-id="c1560-130">Request</span></span>
<span data-ttu-id="c1560-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1560-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1560-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1560-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="c"></a>[<span data-ttu-id="c1560-133">C#</span><span class="sxs-lookup"><span data-stu-id="c1560-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1560-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1560-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1560-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1560-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1560-136">Java</span><span class="sxs-lookup"><span data-stu-id="c1560-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c1560-137">响应</span><span class="sxs-lookup"><span data-stu-id="c1560-137">Response</span></span>
<span data-ttu-id="c1560-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1560-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

