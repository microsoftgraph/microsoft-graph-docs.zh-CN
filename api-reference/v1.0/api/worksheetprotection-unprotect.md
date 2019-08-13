---
title: 'WorksheetProtection: unprotect'
description: 解除工作表保护
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 43d3c140a2b825c71719f2a06ec28d458f016634
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372837"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="c4fbe-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="c4fbe-103">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="c4fbe-104">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="c4fbe-104">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="c4fbe-105">权限</span><span class="sxs-lookup"><span data-stu-id="c4fbe-105">Permissions</span></span>
<span data-ttu-id="c4fbe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4fbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4fbe-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4fbe-108">Permission type</span></span>      | <span data-ttu-id="c4fbe-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4fbe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4fbe-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4fbe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4fbe-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4fbe-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4fbe-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4fbe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4fbe-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4fbe-113">Not supported.</span></span>    |
|<span data-ttu-id="c4fbe-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4fbe-114">Application</span></span> | <span data-ttu-id="c4fbe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4fbe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4fbe-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4fbe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="c4fbe-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4fbe-117">Request headers</span></span>
| <span data-ttu-id="c4fbe-118">名称</span><span class="sxs-lookup"><span data-stu-id="c4fbe-118">Name</span></span>       | <span data-ttu-id="c4fbe-119">说明</span><span class="sxs-lookup"><span data-stu-id="c4fbe-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4fbe-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4fbe-120">Authorization</span></span>  | <span data-ttu-id="c4fbe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4fbe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4fbe-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c4fbe-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c4fbe-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c4fbe-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4fbe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4fbe-126">Request body</span></span>
<span data-ttu-id="c4fbe-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c4fbe-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c4fbe-128">参数</span><span class="sxs-lookup"><span data-stu-id="c4fbe-128">Parameter</span></span>    | <span data-ttu-id="c4fbe-129">类型</span><span class="sxs-lookup"><span data-stu-id="c4fbe-129">Type</span></span>   |<span data-ttu-id="c4fbe-130">说明</span><span class="sxs-lookup"><span data-stu-id="c4fbe-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4fbe-131">password</span><span class="sxs-lookup"><span data-stu-id="c4fbe-131">password</span></span>|<span data-ttu-id="c4fbe-132">string</span><span class="sxs-lookup"><span data-stu-id="c4fbe-132">string</span></span>|<span data-ttu-id="c4fbe-p104">可选。工作表保护密码。</span><span class="sxs-lookup"><span data-stu-id="c4fbe-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="c4fbe-135">响应</span><span class="sxs-lookup"><span data-stu-id="c4fbe-135">Response</span></span>

<span data-ttu-id="c4fbe-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c4fbe-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4fbe-138">示例</span><span class="sxs-lookup"><span data-stu-id="c4fbe-138">Example</span></span>
<span data-ttu-id="c4fbe-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c4fbe-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c4fbe-140">请求</span><span class="sxs-lookup"><span data-stu-id="c4fbe-140">Request</span></span>
<span data-ttu-id="c4fbe-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4fbe-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c4fbe-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c4fbe-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4fbe-143">C#</span><span class="sxs-lookup"><span data-stu-id="c4fbe-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetprotection-unprotect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4fbe-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4fbe-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetprotection-unprotect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4fbe-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="c4fbe-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetprotection-unprotect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c4fbe-146">Java</span><span class="sxs-lookup"><span data-stu-id="c4fbe-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetprotection-unprotect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c4fbe-147">响应</span><span class="sxs-lookup"><span data-stu-id="c4fbe-147">Response</span></span>
<span data-ttu-id="c4fbe-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c4fbe-148">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
