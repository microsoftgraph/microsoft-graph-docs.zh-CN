---
title: 'WorksheetProtection: protect'
description: 保护工作表。如果工作表处于受保护状态，则会引发它。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 82917ab1b2c1fa20b6331182512ef78c847a426a
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577483"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="d8244-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="d8244-104">WorksheetProtection: protect</span></span>

<span data-ttu-id="d8244-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8244-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8244-p102">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="d8244-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="d8244-108">权限</span><span class="sxs-lookup"><span data-stu-id="d8244-108">Permissions</span></span>
<span data-ttu-id="d8244-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8244-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8244-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8244-111">Permission type</span></span>      | <span data-ttu-id="d8244-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8244-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8244-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8244-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d8244-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8244-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d8244-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8244-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8244-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8244-116">Not supported.</span></span>    |
|<span data-ttu-id="d8244-117">Application</span><span class="sxs-lookup"><span data-stu-id="d8244-117">Application</span></span> | <span data-ttu-id="d8244-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8244-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8244-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8244-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="d8244-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8244-120">Request headers</span></span>
| <span data-ttu-id="d8244-121">名称</span><span class="sxs-lookup"><span data-stu-id="d8244-121">Name</span></span>       | <span data-ttu-id="d8244-122">说明</span><span class="sxs-lookup"><span data-stu-id="d8244-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d8244-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8244-123">Authorization</span></span>  | <span data-ttu-id="d8244-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8244-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8244-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d8244-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="d8244-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d8244-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8244-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8244-129">Request body</span></span>
<span data-ttu-id="d8244-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d8244-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d8244-131">参数</span><span class="sxs-lookup"><span data-stu-id="d8244-131">Parameter</span></span>    | <span data-ttu-id="d8244-132">类型</span><span class="sxs-lookup"><span data-stu-id="d8244-132">Type</span></span>   |<span data-ttu-id="d8244-133">说明</span><span class="sxs-lookup"><span data-stu-id="d8244-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8244-134">选项</span><span class="sxs-lookup"><span data-stu-id="d8244-134">options</span></span>|<span data-ttu-id="d8244-135">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="d8244-135">WorkbookWorksheetProtectionOptions</span></span>|<span data-ttu-id="d8244-p106">可选。工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d8244-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="d8244-138">响应</span><span class="sxs-lookup"><span data-stu-id="d8244-138">Response</span></span>

<span data-ttu-id="d8244-p107">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d8244-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8244-141">示例</span><span class="sxs-lookup"><span data-stu-id="d8244-141">Example</span></span>
<span data-ttu-id="d8244-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d8244-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d8244-143">请求</span><span class="sxs-lookup"><span data-stu-id="d8244-143">Request</span></span>
<span data-ttu-id="d8244-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8244-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8244-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8244-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d8244-146">C#</span><span class="sxs-lookup"><span data-stu-id="d8244-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8244-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8244-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8244-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8244-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8244-149">Java</span><span class="sxs-lookup"><span data-stu-id="d8244-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetprotection-protect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8244-150">响应</span><span class="sxs-lookup"><span data-stu-id="d8244-150">Response</span></span>
<span data-ttu-id="d8244-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d8244-151">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

