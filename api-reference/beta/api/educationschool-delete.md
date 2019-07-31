---
title: 删除 educationSchool
description: 删除学校。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 337bc03df9aec93bdcbfebc84db3467bf8748342
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955199"
---
# <a name="delete-educationschool"></a><span data-ttu-id="0a249-103">删除 educationSchool</span><span class="sxs-lookup"><span data-stu-id="0a249-103">Delete educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a249-104">删除学校。</span><span class="sxs-lookup"><span data-stu-id="0a249-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a249-105">权限</span><span class="sxs-lookup"><span data-stu-id="0a249-105">Permissions</span></span>
<span data-ttu-id="0a249-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a249-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a249-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a249-108">Permission type</span></span>      | <span data-ttu-id="0a249-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a249-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a249-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a249-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0a249-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a249-111">Not supported.</span></span>  |
|<span data-ttu-id="0a249-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a249-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0a249-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a249-113">Not supported.</span></span>  |
|<span data-ttu-id="0a249-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a249-114">Application</span></span> | <span data-ttu-id="0a249-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a249-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0a249-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a249-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0a249-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a249-117">Request headers</span></span>
| <span data-ttu-id="0a249-118">标头</span><span class="sxs-lookup"><span data-stu-id="0a249-118">Header</span></span>       | <span data-ttu-id="0a249-119">值</span><span class="sxs-lookup"><span data-stu-id="0a249-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a249-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a249-120">Authorization</span></span>  | <span data-ttu-id="0a249-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a249-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a249-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a249-123">Request body</span></span>
<span data-ttu-id="0a249-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a249-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0a249-125">响应</span><span class="sxs-lookup"><span data-stu-id="0a249-125">Response</span></span>
<span data-ttu-id="0a249-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0a249-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a249-128">示例</span><span class="sxs-lookup"><span data-stu-id="0a249-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a249-129">请求</span><span class="sxs-lookup"><span data-stu-id="0a249-129">Request</span></span>
<span data-ttu-id="0a249-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0a249-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a249-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0a249-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a249-132">C#</span><span class="sxs-lookup"><span data-stu-id="0a249-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a249-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a249-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a249-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="0a249-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0a249-135">Java</span><span class="sxs-lookup"><span data-stu-id="0a249-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0a249-136">响应</span><span class="sxs-lookup"><span data-stu-id="0a249-136">Response</span></span>
<span data-ttu-id="0a249-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0a249-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
