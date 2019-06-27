---
title: Range:Column
description: 获取范围中包含的列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a99ee6c1321ea0988a26251cac4a3f4ea7bdc509
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276060"
---
# <a name="range-column"></a><span data-ttu-id="9f1f1-103">Range:Column</span><span class="sxs-lookup"><span data-stu-id="9f1f1-103">Range: Column</span></span>

<span data-ttu-id="9f1f1-104">获取范围中包含的列。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f1f1-105">权限</span><span class="sxs-lookup"><span data-stu-id="9f1f1-105">Permissions</span></span>
<span data-ttu-id="9f1f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f1f1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f1f1-108">Permission type</span></span>      | <span data-ttu-id="9f1f1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f1f1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f1f1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f1f1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f1f1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f1f1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9f1f1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f1f1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f1f1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-113">Not supported.</span></span>    |
|<span data-ttu-id="9f1f1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f1f1-114">Application</span></span> | <span data-ttu-id="9f1f1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f1f1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f1f1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="9f1f1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f1f1-117">Request headers</span></span>
| <span data-ttu-id="9f1f1-118">名称</span><span class="sxs-lookup"><span data-stu-id="9f1f1-118">Name</span></span>       | <span data-ttu-id="9f1f1-119">说明</span><span class="sxs-lookup"><span data-stu-id="9f1f1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9f1f1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f1f1-120">Authorization</span></span>  | <span data-ttu-id="9f1f1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f1f1-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9f1f1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9f1f1-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="9f1f1-126">路径参数</span><span class="sxs-lookup"><span data-stu-id="9f1f1-126">Path parameters</span></span>
<span data-ttu-id="9f1f1-127">在请求路径中, 提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-127">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="9f1f1-128">参数</span><span class="sxs-lookup"><span data-stu-id="9f1f1-128">Parameter</span></span>    | <span data-ttu-id="9f1f1-129">类型</span><span class="sxs-lookup"><span data-stu-id="9f1f1-129">Type</span></span>   |<span data-ttu-id="9f1f1-130">说明</span><span class="sxs-lookup"><span data-stu-id="9f1f1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f1f1-131">column</span><span class="sxs-lookup"><span data-stu-id="9f1f1-131">column</span></span>|<span data-ttu-id="9f1f1-132">Int32</span><span class="sxs-lookup"><span data-stu-id="9f1f1-132">Int32</span></span>|<span data-ttu-id="9f1f1-p104">要检索的区域的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="9f1f1-135">响应</span><span class="sxs-lookup"><span data-stu-id="9f1f1-135">Response</span></span>

<span data-ttu-id="9f1f1-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f1f1-137">示例</span><span class="sxs-lookup"><span data-stu-id="9f1f1-137">Example</span></span>
<span data-ttu-id="9f1f1-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9f1f1-139">请求</span><span class="sxs-lookup"><span data-stu-id="9f1f1-139">Request</span></span>
<span data-ttu-id="9f1f1-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```

##### <a name="response"></a><span data-ttu-id="9f1f1-141">响应</span><span class="sxs-lookup"><span data-stu-id="9f1f1-141">Response</span></span>
<span data-ttu-id="9f1f1-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f1f1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9f1f1-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="9f1f1-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9f1f1-146">C#</span><span class="sxs-lookup"><span data-stu-id="9f1f1-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_column-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f1f1-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="9f1f1-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_column-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9f1f1-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="9f1f1-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_column-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-column.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/range-column.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-column.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
