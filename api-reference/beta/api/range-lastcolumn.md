---
title: Range:LastColumn
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 51b41cedcdc623dc5783e4d051a88446b446e9d7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267590"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="8a97c-103">Range:LastColumn</span><span class="sxs-lookup"><span data-stu-id="8a97c-103">Range: LastColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a97c-p101">获取区域内的最后一列。例如，“B2:D5”的最后一列是“D2:D5”。</span><span class="sxs-lookup"><span data-stu-id="8a97c-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="8a97c-106">权限</span><span class="sxs-lookup"><span data-stu-id="8a97c-106">Permissions</span></span>
<span data-ttu-id="8a97c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a97c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a97c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a97c-109">Permission type</span></span>      | <span data-ttu-id="8a97c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a97c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a97c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a97c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8a97c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a97c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8a97c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a97c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a97c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a97c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8a97c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a97c-115">Application</span></span> | <span data-ttu-id="8a97c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a97c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a97c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a97c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/LastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastColumn

```
## <a name="request-headers"></a><span data-ttu-id="8a97c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a97c-118">Request headers</span></span>
| <span data-ttu-id="8a97c-119">名称</span><span class="sxs-lookup"><span data-stu-id="8a97c-119">Name</span></span>       | <span data-ttu-id="8a97c-120">说明</span><span class="sxs-lookup"><span data-stu-id="8a97c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8a97c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a97c-121">Authorization</span></span>  | <span data-ttu-id="8a97c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a97c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a97c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8a97c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="8a97c-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8a97c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a97c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a97c-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8a97c-128">响应</span><span class="sxs-lookup"><span data-stu-id="8a97c-128">Response</span></span>

<span data-ttu-id="8a97c-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a97c-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a97c-130">示例</span><span class="sxs-lookup"><span data-stu-id="8a97c-130">Example</span></span>
<span data-ttu-id="8a97c-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8a97c-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8a97c-132">请求</span><span class="sxs-lookup"><span data-stu-id="8a97c-132">Request</span></span>
<span data-ttu-id="8a97c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a97c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/LastColumn
```

##### <a name="response"></a><span data-ttu-id="8a97c-134">响应</span><span class="sxs-lookup"><span data-stu-id="8a97c-134">Response</span></span>
<span data-ttu-id="8a97c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a97c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8a97c-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8a97c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8a97c-139">C#</span><span class="sxs-lookup"><span data-stu-id="8a97c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_lastcolumn-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8a97c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="8a97c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_lastcolumn-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8a97c-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="8a97c-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_lastcolumn-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-lastcolumn.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/range-lastcolumn.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/range-lastcolumn.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
