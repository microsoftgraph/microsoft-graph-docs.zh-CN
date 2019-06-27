---
title: 'Range: delete'
description: 删除与范围相关的单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fc9404bd6560973dc3fb256d40320a1df77e801b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267639"
---
# <a name="range-delete"></a><span data-ttu-id="ce155-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="ce155-103">Range: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce155-104">删除与范围相关的单元格。</span><span class="sxs-lookup"><span data-stu-id="ce155-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce155-105">权限</span><span class="sxs-lookup"><span data-stu-id="ce155-105">Permissions</span></span>
<span data-ttu-id="ce155-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce155-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce155-108">Permission type</span></span>      | <span data-ttu-id="ce155-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce155-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce155-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce155-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce155-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce155-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ce155-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce155-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce155-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce155-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ce155-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce155-114">Application</span></span> | <span data-ttu-id="ce155-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce155-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce155-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce155-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="ce155-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce155-117">Request headers</span></span>
| <span data-ttu-id="ce155-118">名称</span><span class="sxs-lookup"><span data-stu-id="ce155-118">Name</span></span>       | <span data-ttu-id="ce155-119">说明</span><span class="sxs-lookup"><span data-stu-id="ce155-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ce155-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce155-120">Authorization</span></span>  | <span data-ttu-id="ce155-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce155-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce155-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ce155-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ce155-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ce155-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce155-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce155-126">Request body</span></span>
<span data-ttu-id="ce155-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ce155-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ce155-128">参数</span><span class="sxs-lookup"><span data-stu-id="ce155-128">Parameter</span></span>    | <span data-ttu-id="ce155-129">类型</span><span class="sxs-lookup"><span data-stu-id="ce155-129">Type</span></span>   |<span data-ttu-id="ce155-130">说明</span><span class="sxs-lookup"><span data-stu-id="ce155-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce155-131">Shift</span><span class="sxs-lookup"><span data-stu-id="ce155-131">shift</span></span>|<span data-ttu-id="ce155-132">string</span><span class="sxs-lookup"><span data-stu-id="ce155-132">string</span></span>|<span data-ttu-id="ce155-p104">指定移动单元格的方式。可能的值是：`Up`、`Left`。</span><span class="sxs-lookup"><span data-stu-id="ce155-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="ce155-135">响应</span><span class="sxs-lookup"><span data-stu-id="ce155-135">Response</span></span>

<span data-ttu-id="ce155-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ce155-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce155-138">示例</span><span class="sxs-lookup"><span data-stu-id="ce155-138">Example</span></span>
<span data-ttu-id="ce155-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ce155-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ce155-140">请求</span><span class="sxs-lookup"><span data-stu-id="ce155-140">Request</span></span>
<span data-ttu-id="ce155-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce155-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="ce155-142">响应</span><span class="sxs-lookup"><span data-stu-id="ce155-142">Response</span></span>
<span data-ttu-id="ce155-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ce155-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ce155-144">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ce155-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ce155-145">C#</span><span class="sxs-lookup"><span data-stu-id="ce155-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce155-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce155-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_delete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ce155-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="ce155-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_delete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
