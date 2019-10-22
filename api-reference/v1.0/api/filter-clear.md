---
title: 'Filter: clear'
description: 清除给定列上的筛选器。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: df54c737a33f31dcbb22bf4776beccd9b8ee2faf
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "36341913"
---
# <a name="filter-clear"></a><span data-ttu-id="e85d8-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="e85d8-103">Filter: clear</span></span>

<span data-ttu-id="e85d8-104">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="e85d8-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="e85d8-105">权限</span><span class="sxs-lookup"><span data-stu-id="e85d8-105">Permissions</span></span>
<span data-ttu-id="e85d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e85d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e85d8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e85d8-108">Permission type</span></span>      | <span data-ttu-id="e85d8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e85d8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e85d8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e85d8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e85d8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e85d8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e85d8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e85d8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e85d8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e85d8-113">Not supported.</span></span>    |
|<span data-ttu-id="e85d8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e85d8-114">Application</span></span> | <span data-ttu-id="e85d8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e85d8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e85d8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e85d8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="e85d8-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e85d8-117">Request headers</span></span>
| <span data-ttu-id="e85d8-118">名称</span><span class="sxs-lookup"><span data-stu-id="e85d8-118">Name</span></span>       | <span data-ttu-id="e85d8-119">说明</span><span class="sxs-lookup"><span data-stu-id="e85d8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e85d8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e85d8-120">Authorization</span></span>  | <span data-ttu-id="e85d8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e85d8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e85d8-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e85d8-123">Request body</span></span>
<span data-ttu-id="e85d8-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e85d8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e85d8-125">响应</span><span class="sxs-lookup"><span data-stu-id="e85d8-125">Response</span></span>

<span data-ttu-id="e85d8-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e85d8-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e85d8-128">示例</span><span class="sxs-lookup"><span data-stu-id="e85d8-128">Example</span></span>
<span data-ttu-id="e85d8-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e85d8-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e85d8-130">请求</span><span class="sxs-lookup"><span data-stu-id="e85d8-130">Request</span></span>
<span data-ttu-id="e85d8-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e85d8-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e85d8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e85d8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e85d8-133">C#</span><span class="sxs-lookup"><span data-stu-id="e85d8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e85d8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e85d8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e85d8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e85d8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e85d8-136">Java</span><span class="sxs-lookup"><span data-stu-id="e85d8-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e85d8-137">响应</span><span class="sxs-lookup"><span data-stu-id="e85d8-137">Response</span></span>
<span data-ttu-id="e85d8-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e85d8-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
