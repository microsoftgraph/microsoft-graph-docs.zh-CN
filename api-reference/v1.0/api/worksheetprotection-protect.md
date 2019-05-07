---
title: 'WorksheetProtection: protect'
description: 保护工作表。如果工作表处于受保护状态，则会引发它。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2584cce4bae3f7289ea25900c00a8c5585016ac9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601220"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="ebafc-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="ebafc-104">WorksheetProtection: protect</span></span>

<span data-ttu-id="ebafc-p102">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="ebafc-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebafc-107">权限</span><span class="sxs-lookup"><span data-stu-id="ebafc-107">Permissions</span></span>
<span data-ttu-id="ebafc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebafc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebafc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebafc-110">Permission type</span></span>      | <span data-ttu-id="ebafc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebafc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebafc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebafc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ebafc-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebafc-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ebafc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebafc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebafc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebafc-115">Not supported.</span></span>    |
|<span data-ttu-id="ebafc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebafc-116">Application</span></span> | <span data-ttu-id="ebafc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebafc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebafc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebafc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="ebafc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebafc-119">Request headers</span></span>
| <span data-ttu-id="ebafc-120">名称</span><span class="sxs-lookup"><span data-stu-id="ebafc-120">Name</span></span>       | <span data-ttu-id="ebafc-121">说明</span><span class="sxs-lookup"><span data-stu-id="ebafc-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ebafc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebafc-122">Authorization</span></span>  | <span data-ttu-id="ebafc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebafc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebafc-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ebafc-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ebafc-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ebafc-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebafc-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebafc-128">Request body</span></span>
<span data-ttu-id="ebafc-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ebafc-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ebafc-130">参数</span><span class="sxs-lookup"><span data-stu-id="ebafc-130">Parameter</span></span>    | <span data-ttu-id="ebafc-131">类型</span><span class="sxs-lookup"><span data-stu-id="ebafc-131">Type</span></span>   |<span data-ttu-id="ebafc-132">说明</span><span class="sxs-lookup"><span data-stu-id="ebafc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebafc-133">选项</span><span class="sxs-lookup"><span data-stu-id="ebafc-133">options</span></span>|<span data-ttu-id="ebafc-134">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="ebafc-134">WorkbookWorksheetProtectionOptions</span></span>|<span data-ttu-id="ebafc-p106">可选。工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ebafc-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="ebafc-137">响应</span><span class="sxs-lookup"><span data-stu-id="ebafc-137">Response</span></span>

<span data-ttu-id="ebafc-p107">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ebafc-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebafc-140">示例</span><span class="sxs-lookup"><span data-stu-id="ebafc-140">Example</span></span>
<span data-ttu-id="ebafc-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ebafc-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ebafc-142">请求</span><span class="sxs-lookup"><span data-stu-id="ebafc-142">Request</span></span>
<span data-ttu-id="ebafc-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebafc-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="ebafc-144">响应</span><span class="sxs-lookup"><span data-stu-id="ebafc-144">Response</span></span>
<span data-ttu-id="ebafc-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ebafc-145">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ebafc-146">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ebafc-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ebafc-147">语言</span><span class="sxs-lookup"><span data-stu-id="ebafc-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheetprotection_protect-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ebafc-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="ebafc-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheetprotection_protect-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheetprotection-protect.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheetprotection-protect.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
