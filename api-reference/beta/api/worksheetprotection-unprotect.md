---
title: workbookWorksheetProtection：unprotect
description: 解除工作表保护
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a55ddc339261c95733a6719a88a73bf24c00855f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787693"
---
# <a name="workbookworksheetprotection-unprotect"></a><span data-ttu-id="d7313-103">workbookWorksheetProtection：unprotect</span><span class="sxs-lookup"><span data-stu-id="d7313-103">workbookWorksheetProtection: unprotect</span></span>

<span data-ttu-id="d7313-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7313-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7313-105">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="d7313-105">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="d7313-106">权限</span><span class="sxs-lookup"><span data-stu-id="d7313-106">Permissions</span></span>
<span data-ttu-id="d7313-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7313-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7313-109">Permission type</span></span>      | <span data-ttu-id="d7313-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7313-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7313-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7313-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d7313-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7313-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7313-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7313-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7313-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7313-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7313-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7313-115">Application</span></span> | <span data-ttu-id="d7313-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7313-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7313-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7313-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="d7313-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7313-118">Request headers</span></span>
| <span data-ttu-id="d7313-119">名称</span><span class="sxs-lookup"><span data-stu-id="d7313-119">Name</span></span>       | <span data-ttu-id="d7313-120">说明</span><span class="sxs-lookup"><span data-stu-id="d7313-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7313-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7313-121">Authorization</span></span>  | <span data-ttu-id="d7313-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7313-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7313-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d7313-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d7313-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d7313-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7313-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7313-127">Request body</span></span>
<span data-ttu-id="d7313-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d7313-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d7313-129">参数</span><span class="sxs-lookup"><span data-stu-id="d7313-129">Parameter</span></span>    | <span data-ttu-id="d7313-130">类型</span><span class="sxs-lookup"><span data-stu-id="d7313-130">Type</span></span>   |<span data-ttu-id="d7313-131">说明</span><span class="sxs-lookup"><span data-stu-id="d7313-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7313-132">password</span><span class="sxs-lookup"><span data-stu-id="d7313-132">password</span></span>|<span data-ttu-id="d7313-133">string</span><span class="sxs-lookup"><span data-stu-id="d7313-133">string</span></span>|<span data-ttu-id="d7313-p104">可选。工作表保护密码。</span><span class="sxs-lookup"><span data-stu-id="d7313-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="d7313-136">响应</span><span class="sxs-lookup"><span data-stu-id="d7313-136">Response</span></span>

<span data-ttu-id="d7313-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d7313-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7313-139">示例</span><span class="sxs-lookup"><span data-stu-id="d7313-139">Example</span></span>
<span data-ttu-id="d7313-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d7313-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7313-141">请求</span><span class="sxs-lookup"><span data-stu-id="d7313-141">Request</span></span>
<span data-ttu-id="d7313-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7313-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d7313-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7313-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookworksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d7313-144">C#</span><span class="sxs-lookup"><span data-stu-id="d7313-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-unprotect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7313-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7313-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-unprotect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7313-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7313-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-unprotect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d7313-147">响应</span><span class="sxs-lookup"><span data-stu-id="d7313-147">Response</span></span>
<span data-ttu-id="d7313-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d7313-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


