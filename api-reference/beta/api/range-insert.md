---
title: 'Range: insert'
description: 将单个单元格或一系列单元格插入到工作表中取代此区域，并移动其他单元格以留出空间。在现在空白的空间返回新的 Range 对象。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: daa52980d2cec9eb987810dd6083a2b5f723b462
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055104"
---
# <a name="range-insert"></a><span data-ttu-id="a563b-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="a563b-104">Range: insert</span></span>

<span data-ttu-id="a563b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a563b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a563b-p102">将单个单元格或一系列单元格插入到工作表中取代此区域，并移动其他单元格以留出空间。在现在空白的空间返回新的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="a563b-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="a563b-108">权限</span><span class="sxs-lookup"><span data-stu-id="a563b-108">Permissions</span></span>
<span data-ttu-id="a563b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a563b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a563b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a563b-111">Permission type</span></span>      | <span data-ttu-id="a563b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a563b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a563b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a563b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a563b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a563b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a563b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a563b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a563b-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a563b-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a563b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a563b-117">Application</span></span> | <span data-ttu-id="a563b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a563b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a563b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a563b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/insert
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="a563b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a563b-120">Request headers</span></span>
| <span data-ttu-id="a563b-121">名称</span><span class="sxs-lookup"><span data-stu-id="a563b-121">Name</span></span>       | <span data-ttu-id="a563b-122">说明</span><span class="sxs-lookup"><span data-stu-id="a563b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a563b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a563b-123">Authorization</span></span>  | <span data-ttu-id="a563b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a563b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a563b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a563b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="a563b-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a563b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a563b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a563b-129">Request body</span></span>
<span data-ttu-id="a563b-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a563b-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a563b-131">参数</span><span class="sxs-lookup"><span data-stu-id="a563b-131">Parameter</span></span>    | <span data-ttu-id="a563b-132">类型</span><span class="sxs-lookup"><span data-stu-id="a563b-132">Type</span></span>   |<span data-ttu-id="a563b-133">说明</span><span class="sxs-lookup"><span data-stu-id="a563b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a563b-134">Shift</span><span class="sxs-lookup"><span data-stu-id="a563b-134">shift</span></span>|<span data-ttu-id="a563b-135">string</span><span class="sxs-lookup"><span data-stu-id="a563b-135">string</span></span>|<span data-ttu-id="a563b-p106">指定移动单元格的方式。可能的值是：`Down`、`Right`。</span><span class="sxs-lookup"><span data-stu-id="a563b-p106">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="a563b-138">响应</span><span class="sxs-lookup"><span data-stu-id="a563b-138">Response</span></span>

<span data-ttu-id="a563b-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a563b-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a563b-140">示例</span><span class="sxs-lookup"><span data-stu-id="a563b-140">Example</span></span>
<span data-ttu-id="a563b-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a563b-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a563b-142">请求</span><span class="sxs-lookup"><span data-stu-id="a563b-142">Request</span></span>
<span data-ttu-id="a563b-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a563b-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a563b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a563b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```
# <a name="c"></a>[<span data-ttu-id="a563b-145">C#</span><span class="sxs-lookup"><span data-stu-id="a563b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-insert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a563b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a563b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-insert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a563b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a563b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-insert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a563b-148">Java</span><span class="sxs-lookup"><span data-stu-id="a563b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-insert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a563b-149">响应</span><span class="sxs-lookup"><span data-stu-id="a563b-149">Response</span></span>
<span data-ttu-id="a563b-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a563b-150">Here is an example of the response.</span></span> <span data-ttu-id="a563b-151">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a563b-151">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


