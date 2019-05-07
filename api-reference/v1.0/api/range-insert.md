---
title: 'Range: insert'
description: 将单个单元格或一系列单元格插入到工作表中取代此区域，并移动其他单元格以留出空间。在现在空白的空间返回新的 Range 对象。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: c6088d2862b5115ba40fee9c885a85c0fa576e22
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607780"
---
# <a name="range-insert"></a><span data-ttu-id="72233-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="72233-104">Range: insert</span></span>

<span data-ttu-id="72233-p102">将单个单元格或一系列单元格插入到工作表中取代此区域，并移动其他单元格以留出空间。在现在空白的空间返回新的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="72233-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="72233-107">权限</span><span class="sxs-lookup"><span data-stu-id="72233-107">Permissions</span></span>
<span data-ttu-id="72233-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72233-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72233-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="72233-110">Permission type</span></span>      | <span data-ttu-id="72233-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72233-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72233-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72233-112">Delegated (work or school account)</span></span> | <span data-ttu-id="72233-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72233-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="72233-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72233-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72233-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="72233-115">Not supported.</span></span>    |
|<span data-ttu-id="72233-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="72233-116">Application</span></span> | <span data-ttu-id="72233-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="72233-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72233-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72233-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="72233-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="72233-119">Request headers</span></span>
| <span data-ttu-id="72233-120">名称</span><span class="sxs-lookup"><span data-stu-id="72233-120">Name</span></span>       | <span data-ttu-id="72233-121">说明</span><span class="sxs-lookup"><span data-stu-id="72233-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="72233-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72233-122">Authorization</span></span>  | <span data-ttu-id="72233-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72233-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72233-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="72233-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="72233-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="72233-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72233-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="72233-128">Request body</span></span>
<span data-ttu-id="72233-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="72233-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="72233-130">参数</span><span class="sxs-lookup"><span data-stu-id="72233-130">Parameter</span></span>    | <span data-ttu-id="72233-131">类型</span><span class="sxs-lookup"><span data-stu-id="72233-131">Type</span></span>   |<span data-ttu-id="72233-132">说明</span><span class="sxs-lookup"><span data-stu-id="72233-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72233-133">Shift</span><span class="sxs-lookup"><span data-stu-id="72233-133">shift</span></span>|<span data-ttu-id="72233-134">string</span><span class="sxs-lookup"><span data-stu-id="72233-134">string</span></span>|<span data-ttu-id="72233-135">指定移动单元格的方式。</span><span class="sxs-lookup"><span data-stu-id="72233-135">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="72233-136">可能的值为: `Down`、 `Right`。</span><span class="sxs-lookup"><span data-stu-id="72233-136">The possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="72233-137">响应</span><span class="sxs-lookup"><span data-stu-id="72233-137">Response</span></span>

<span data-ttu-id="72233-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72233-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72233-139">示例</span><span class="sxs-lookup"><span data-stu-id="72233-139">Example</span></span>
<span data-ttu-id="72233-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="72233-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="72233-141">请求</span><span class="sxs-lookup"><span data-stu-id="72233-141">Request</span></span>
<span data-ttu-id="72233-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72233-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="72233-143">响应</span><span class="sxs-lookup"><span data-stu-id="72233-143">Response</span></span>
<span data-ttu-id="72233-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72233-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="72233-147">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="72233-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="72233-148">语言</span><span class="sxs-lookup"><span data-stu-id="72233-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_insert-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72233-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="72233-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_insert-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-insert.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-insert.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
