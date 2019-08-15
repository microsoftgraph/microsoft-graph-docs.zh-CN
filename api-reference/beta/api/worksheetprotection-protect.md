---
title: 'workbookWorksheetProtection: 保护'
description: 保护工作表。 如果工作表处于受保护状态，则会引发它。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cc5865e87152e7a3b2a43d9fb2397dc98b7e551f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420882"
---
# <a name="workbookworksheetprotection-protect"></a><span data-ttu-id="bf015-104">workbookWorksheetProtection: 保护</span><span class="sxs-lookup"><span data-stu-id="bf015-104">workbookWorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf015-p102">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="bf015-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="bf015-107">权限</span><span class="sxs-lookup"><span data-stu-id="bf015-107">Permissions</span></span>
<span data-ttu-id="bf015-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf015-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf015-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf015-110">Permission type</span></span>      | <span data-ttu-id="bf015-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf015-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf015-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf015-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bf015-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf015-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bf015-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf015-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf015-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf015-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bf015-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf015-116">Application</span></span> | <span data-ttu-id="bf015-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf015-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf015-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf015-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="bf015-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf015-119">Request headers</span></span>
| <span data-ttu-id="bf015-120">名称</span><span class="sxs-lookup"><span data-stu-id="bf015-120">Name</span></span>       | <span data-ttu-id="bf015-121">说明</span><span class="sxs-lookup"><span data-stu-id="bf015-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bf015-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf015-122">Authorization</span></span>  | <span data-ttu-id="bf015-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf015-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf015-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bf015-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="bf015-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="bf015-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf015-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf015-128">Request body</span></span>
<span data-ttu-id="bf015-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="bf015-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bf015-130">参数</span><span class="sxs-lookup"><span data-stu-id="bf015-130">Parameter</span></span>    | <span data-ttu-id="bf015-131">类型</span><span class="sxs-lookup"><span data-stu-id="bf015-131">Type</span></span>   |<span data-ttu-id="bf015-132">说明</span><span class="sxs-lookup"><span data-stu-id="bf015-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf015-133">选项</span><span class="sxs-lookup"><span data-stu-id="bf015-133">options</span></span>|[<span data-ttu-id="bf015-134">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="bf015-134">workbookWorksheetProtectionOptions</span></span>](../resources/workbookworksheetprotectionoptions.md)|<span data-ttu-id="bf015-p106">可选。工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="bf015-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="bf015-137">响应</span><span class="sxs-lookup"><span data-stu-id="bf015-137">Response</span></span>

<span data-ttu-id="bf015-p107">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bf015-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf015-140">示例</span><span class="sxs-lookup"><span data-stu-id="bf015-140">Example</span></span>
<span data-ttu-id="bf015-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="bf015-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bf015-142">请求</span><span class="sxs-lookup"><span data-stu-id="bf015-142">Request</span></span>
<span data-ttu-id="bf015-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf015-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bf015-144">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bf015-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookworksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bf015-145">C#</span><span class="sxs-lookup"><span data-stu-id="bf015-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf015-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf015-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bf015-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="bf015-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bf015-148">响应</span><span class="sxs-lookup"><span data-stu-id="bf015-148">Response</span></span>
<span data-ttu-id="bf015-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bf015-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
