---
title: 'Range: insert'
description: 将单个单元格或一系列单元格插入到工作表中取代此区域，并移动其他单元格以留出空间。在现在空白的空间返回新的 Range 对象。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2f5f9d3952afed0cad6430d1ae35078906f6b00f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578680"
---
# <a name="range-insert"></a><span data-ttu-id="fa9a7-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="fa9a7-104">Range: insert</span></span>

<span data-ttu-id="fa9a7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa9a7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa9a7-p102">将单个单元格或一系列单元格插入到工作表中取代此区域，并移动其他单元格以留出空间。在现在空白的空间返回新的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="fa9a7-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa9a7-108">权限</span><span class="sxs-lookup"><span data-stu-id="fa9a7-108">Permissions</span></span>
<span data-ttu-id="fa9a7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa9a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa9a7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa9a7-111">Permission type</span></span>      | <span data-ttu-id="fa9a7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa9a7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa9a7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa9a7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fa9a7-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa9a7-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fa9a7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa9a7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa9a7-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa9a7-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fa9a7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa9a7-117">Application</span></span> | <span data-ttu-id="fa9a7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa9a7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa9a7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa9a7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/insert
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="fa9a7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa9a7-120">Request headers</span></span>
| <span data-ttu-id="fa9a7-121">名称</span><span class="sxs-lookup"><span data-stu-id="fa9a7-121">Name</span></span>       | <span data-ttu-id="fa9a7-122">说明</span><span class="sxs-lookup"><span data-stu-id="fa9a7-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fa9a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa9a7-123">Authorization</span></span>  | <span data-ttu-id="fa9a7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa9a7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa9a7-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fa9a7-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="fa9a7-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="fa9a7-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa9a7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa9a7-129">Request body</span></span>
<span data-ttu-id="fa9a7-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fa9a7-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa9a7-131">参数</span><span class="sxs-lookup"><span data-stu-id="fa9a7-131">Parameter</span></span>    | <span data-ttu-id="fa9a7-132">类型</span><span class="sxs-lookup"><span data-stu-id="fa9a7-132">Type</span></span>   |<span data-ttu-id="fa9a7-133">说明</span><span class="sxs-lookup"><span data-stu-id="fa9a7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa9a7-134">Shift</span><span class="sxs-lookup"><span data-stu-id="fa9a7-134">shift</span></span>|<span data-ttu-id="fa9a7-135">string</span><span class="sxs-lookup"><span data-stu-id="fa9a7-135">string</span></span>|<span data-ttu-id="fa9a7-p106">指定移动单元格的方式。可能的值是：`Down`、`Right`。</span><span class="sxs-lookup"><span data-stu-id="fa9a7-p106">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="fa9a7-138">响应</span><span class="sxs-lookup"><span data-stu-id="fa9a7-138">Response</span></span>

<span data-ttu-id="fa9a7-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa9a7-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa9a7-140">示例</span><span class="sxs-lookup"><span data-stu-id="fa9a7-140">Example</span></span>
<span data-ttu-id="fa9a7-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fa9a7-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fa9a7-142">请求</span><span class="sxs-lookup"><span data-stu-id="fa9a7-142">Request</span></span>
<span data-ttu-id="fa9a7-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa9a7-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa9a7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa9a7-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fa9a7-145">C#</span><span class="sxs-lookup"><span data-stu-id="fa9a7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-insert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa9a7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa9a7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-insert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa9a7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa9a7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-insert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa9a7-148">Java</span><span class="sxs-lookup"><span data-stu-id="fa9a7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-insert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fa9a7-149">响应</span><span class="sxs-lookup"><span data-stu-id="fa9a7-149">Response</span></span>
<span data-ttu-id="fa9a7-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa9a7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


