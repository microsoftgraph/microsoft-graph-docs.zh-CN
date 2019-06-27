---
title: TableRow:Range
description: 返回与整个行相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6b1ff4f10080e89ab60e17b6733f7bd6b01cc437
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278748"
---
# <a name="tablerow-range"></a><span data-ttu-id="ce738-103">TableRow:Range</span><span class="sxs-lookup"><span data-stu-id="ce738-103">TableRow: Range</span></span>

<span data-ttu-id="ce738-104">返回与整个行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="ce738-104">Returns the range object associated with the entire row.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce738-105">权限</span><span class="sxs-lookup"><span data-stu-id="ce738-105">Permissions</span></span>
<span data-ttu-id="ce738-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce738-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce738-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce738-108">Permission type</span></span>      | <span data-ttu-id="ce738-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce738-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce738-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce738-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce738-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce738-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ce738-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce738-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce738-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce738-113">Not supported.</span></span>    |
|<span data-ttu-id="ce738-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce738-114">Application</span></span> | <span data-ttu-id="ce738-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce738-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce738-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce738-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows/{index}/range
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/range

```
## <a name="request-headers"></a><span data-ttu-id="ce738-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce738-117">Request headers</span></span>
| <span data-ttu-id="ce738-118">名称</span><span class="sxs-lookup"><span data-stu-id="ce738-118">Name</span></span>       | <span data-ttu-id="ce738-119">说明</span><span class="sxs-lookup"><span data-stu-id="ce738-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ce738-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce738-120">Authorization</span></span>  | <span data-ttu-id="ce738-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce738-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce738-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ce738-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ce738-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ce738-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce738-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce738-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ce738-127">响应</span><span class="sxs-lookup"><span data-stu-id="ce738-127">Response</span></span>

<span data-ttu-id="ce738-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce738-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce738-129">示例</span><span class="sxs-lookup"><span data-stu-id="ce738-129">Example</span></span>
<span data-ttu-id="ce738-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ce738-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ce738-131">请求</span><span class="sxs-lookup"><span data-stu-id="ce738-131">Request</span></span>
<span data-ttu-id="ce738-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce738-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerow_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/range
```

##### <a name="response"></a><span data-ttu-id="ce738-133">响应</span><span class="sxs-lookup"><span data-stu-id="ce738-133">Response</span></span>
<span data-ttu-id="ce738-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce738-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ce738-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ce738-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ce738-138">C#</span><span class="sxs-lookup"><span data-stu-id="ce738-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablerow_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce738-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce738-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablerow_range-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ce738-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="ce738-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablerow_range-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablerow-range.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/tablerow-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablerow-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
