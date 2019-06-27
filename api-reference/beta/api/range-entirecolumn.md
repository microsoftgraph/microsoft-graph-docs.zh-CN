---
title: Range:EntireColumn
description: 获取表示范围整列的对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5679345d8026d174f91c0887e92b0f06cd2e45cf
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266764"
---
# <a name="range-entirecolumn"></a><span data-ttu-id="e0dd9-103">Range:EntireColumn</span><span class="sxs-lookup"><span data-stu-id="e0dd9-103">Range: EntireColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0dd9-104">获取表示范围整列的对象。</span><span class="sxs-lookup"><span data-stu-id="e0dd9-104">Gets an object that represents the entire column of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0dd9-105">权限</span><span class="sxs-lookup"><span data-stu-id="e0dd9-105">Permissions</span></span>
<span data-ttu-id="e0dd9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0dd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0dd9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0dd9-108">Permission type</span></span>      | <span data-ttu-id="e0dd9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0dd9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0dd9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dd9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0dd9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0dd9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0dd9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dd9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0dd9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0dd9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0dd9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0dd9-114">Application</span></span> | <span data-ttu-id="e0dd9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0dd9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0dd9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0dd9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/EntireColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/EntireColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/EntireColumn

```
## <a name="request-headers"></a><span data-ttu-id="e0dd9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0dd9-117">Request headers</span></span>
| <span data-ttu-id="e0dd9-118">名称</span><span class="sxs-lookup"><span data-stu-id="e0dd9-118">Name</span></span>       | <span data-ttu-id="e0dd9-119">说明</span><span class="sxs-lookup"><span data-stu-id="e0dd9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e0dd9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0dd9-120">Authorization</span></span>  | <span data-ttu-id="e0dd9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0dd9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0dd9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e0dd9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e0dd9-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e0dd9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0dd9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0dd9-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e0dd9-127">响应</span><span class="sxs-lookup"><span data-stu-id="e0dd9-127">Response</span></span>

<span data-ttu-id="e0dd9-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0dd9-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0dd9-129">示例</span><span class="sxs-lookup"><span data-stu-id="e0dd9-129">Example</span></span>
<span data-ttu-id="e0dd9-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e0dd9-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e0dd9-131">请求</span><span class="sxs-lookup"><span data-stu-id="e0dd9-131">Request</span></span>
<span data-ttu-id="e0dd9-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0dd9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_entirecolumn"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/EntireColumn
```

##### <a name="response"></a><span data-ttu-id="e0dd9-133">响应</span><span class="sxs-lookup"><span data-stu-id="e0dd9-133">Response</span></span>
<span data-ttu-id="e0dd9-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0dd9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e0dd9-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e0dd9-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e0dd9-138">C#</span><span class="sxs-lookup"><span data-stu-id="e0dd9-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_entirecolumn-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0dd9-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="e0dd9-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_entirecolumn-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e0dd9-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="e0dd9-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_entirecolumn-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: EntireColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-entirecolumn.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/range-entirecolumn.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/range-entirecolumn.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
