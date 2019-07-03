---
title: 'Filter: clear'
description: 清除给定列上的筛选器。
localization_priority: Normal
ms.openlocfilehash: 24389119c09301618df8f288b908a4c124551018
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459732"
---
# <a name="filter-clear"></a><span data-ttu-id="8cbdc-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="8cbdc-103">Filter: clear</span></span>

<span data-ttu-id="8cbdc-104">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="8cbdc-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="8cbdc-105">权限</span><span class="sxs-lookup"><span data-stu-id="8cbdc-105">Permissions</span></span>
<span data-ttu-id="8cbdc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8cbdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cbdc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cbdc-108">Permission type</span></span>      | <span data-ttu-id="8cbdc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8cbdc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cbdc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cbdc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8cbdc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8cbdc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8cbdc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8cbdc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cbdc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cbdc-113">Not supported.</span></span>    |
|<span data-ttu-id="8cbdc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8cbdc-114">Application</span></span> | <span data-ttu-id="8cbdc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cbdc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cbdc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8cbdc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="8cbdc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8cbdc-117">Request headers</span></span>
| <span data-ttu-id="8cbdc-118">名称</span><span class="sxs-lookup"><span data-stu-id="8cbdc-118">Name</span></span>       | <span data-ttu-id="8cbdc-119">说明</span><span class="sxs-lookup"><span data-stu-id="8cbdc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8cbdc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cbdc-120">Authorization</span></span>  | <span data-ttu-id="8cbdc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8cbdc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cbdc-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8cbdc-123">Request body</span></span>
<span data-ttu-id="8cbdc-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8cbdc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cbdc-125">响应</span><span class="sxs-lookup"><span data-stu-id="8cbdc-125">Response</span></span>

<span data-ttu-id="8cbdc-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8cbdc-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cbdc-128">示例</span><span class="sxs-lookup"><span data-stu-id="8cbdc-128">Example</span></span>
<span data-ttu-id="8cbdc-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8cbdc-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8cbdc-130">请求</span><span class="sxs-lookup"><span data-stu-id="8cbdc-130">Request</span></span>
<span data-ttu-id="8cbdc-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8cbdc-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8cbdc-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8cbdc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8cbdc-133">C#</span><span class="sxs-lookup"><span data-stu-id="8cbdc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8cbdc-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="8cbdc-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8cbdc-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="8cbdc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8cbdc-136">响应</span><span class="sxs-lookup"><span data-stu-id="8cbdc-136">Response</span></span>
<span data-ttu-id="8cbdc-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8cbdc-137">Here is an example of the response.</span></span> 
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
