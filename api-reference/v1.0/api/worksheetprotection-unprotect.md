---
title: 'WorksheetProtection: unprotect'
description: 解除工作表保护
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5061f31674099b9d07a38e02d88fe1f920cc6c18
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026031"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="91d8f-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="91d8f-103">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="91d8f-104">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="91d8f-104">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="91d8f-105">权限</span><span class="sxs-lookup"><span data-stu-id="91d8f-105">Permissions</span></span>
<span data-ttu-id="91d8f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91d8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91d8f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="91d8f-108">Permission type</span></span>      | <span data-ttu-id="91d8f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91d8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91d8f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91d8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="91d8f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91d8f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="91d8f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91d8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91d8f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="91d8f-113">Not supported.</span></span>    |
|<span data-ttu-id="91d8f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="91d8f-114">Application</span></span> | <span data-ttu-id="91d8f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="91d8f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91d8f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91d8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="91d8f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="91d8f-117">Request headers</span></span>
| <span data-ttu-id="91d8f-118">名称</span><span class="sxs-lookup"><span data-stu-id="91d8f-118">Name</span></span>       | <span data-ttu-id="91d8f-119">说明</span><span class="sxs-lookup"><span data-stu-id="91d8f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="91d8f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="91d8f-120">Authorization</span></span>  | <span data-ttu-id="91d8f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91d8f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91d8f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="91d8f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="91d8f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="91d8f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91d8f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="91d8f-126">Request body</span></span>
<span data-ttu-id="91d8f-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="91d8f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="91d8f-128">参数</span><span class="sxs-lookup"><span data-stu-id="91d8f-128">Parameter</span></span>    | <span data-ttu-id="91d8f-129">类型</span><span class="sxs-lookup"><span data-stu-id="91d8f-129">Type</span></span>   |<span data-ttu-id="91d8f-130">说明</span><span class="sxs-lookup"><span data-stu-id="91d8f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91d8f-131">password</span><span class="sxs-lookup"><span data-stu-id="91d8f-131">password</span></span>|<span data-ttu-id="91d8f-132">string</span><span class="sxs-lookup"><span data-stu-id="91d8f-132">string</span></span>|<span data-ttu-id="91d8f-p104">可选。工作表保护密码。</span><span class="sxs-lookup"><span data-stu-id="91d8f-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="91d8f-135">响应</span><span class="sxs-lookup"><span data-stu-id="91d8f-135">Response</span></span>

<span data-ttu-id="91d8f-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="91d8f-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91d8f-138">示例</span><span class="sxs-lookup"><span data-stu-id="91d8f-138">Example</span></span>
<span data-ttu-id="91d8f-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="91d8f-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="91d8f-140">请求</span><span class="sxs-lookup"><span data-stu-id="91d8f-140">Request</span></span>
<span data-ttu-id="91d8f-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91d8f-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="91d8f-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="91d8f-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="91d8f-143">C#</span><span class="sxs-lookup"><span data-stu-id="91d8f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetprotection-unprotect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91d8f-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="91d8f-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetprotection-unprotect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="91d8f-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="91d8f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetprotection-unprotect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="91d8f-146">Java</span><span class="sxs-lookup"><span data-stu-id="91d8f-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetprotection-unprotect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="91d8f-147">响应</span><span class="sxs-lookup"><span data-stu-id="91d8f-147">Response</span></span>
<span data-ttu-id="91d8f-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="91d8f-148">Here is an example of the response.</span></span> 
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
