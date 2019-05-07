---
title: Worksheet:Range
description: 获取地址或名称指定的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b1ad7b8c1c23400c02ab1833217c86f00b67f493
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601413"
---
# <a name="worksheet-range"></a><span data-ttu-id="45c57-103">Worksheet:Range</span><span class="sxs-lookup"><span data-stu-id="45c57-103">Worksheet: Range</span></span>

<span data-ttu-id="45c57-104">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="45c57-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="45c57-105">权限</span><span class="sxs-lookup"><span data-stu-id="45c57-105">Permissions</span></span>
<span data-ttu-id="45c57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45c57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45c57-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="45c57-108">Permission type</span></span>      | <span data-ttu-id="45c57-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45c57-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45c57-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45c57-110">Delegated (work or school account)</span></span> | <span data-ttu-id="45c57-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45c57-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="45c57-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45c57-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45c57-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="45c57-113">Not supported.</span></span>    |
|<span data-ttu-id="45c57-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="45c57-114">Application</span></span> | <span data-ttu-id="45c57-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="45c57-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45c57-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45c57-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="45c57-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="45c57-117">Request headers</span></span>
| <span data-ttu-id="45c57-118">名称</span><span class="sxs-lookup"><span data-stu-id="45c57-118">Name</span></span>       | <span data-ttu-id="45c57-119">说明</span><span class="sxs-lookup"><span data-stu-id="45c57-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="45c57-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="45c57-120">Authorization</span></span>  | <span data-ttu-id="45c57-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45c57-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45c57-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="45c57-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="45c57-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="45c57-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="45c57-126">函数参数</span><span class="sxs-lookup"><span data-stu-id="45c57-126">Function parameters</span></span>

| <span data-ttu-id="45c57-127">参数</span><span class="sxs-lookup"><span data-stu-id="45c57-127">Parameter</span></span>    | <span data-ttu-id="45c57-128">类型</span><span class="sxs-lookup"><span data-stu-id="45c57-128">Type</span></span>   |<span data-ttu-id="45c57-129">说明</span><span class="sxs-lookup"><span data-stu-id="45c57-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45c57-130">address</span><span class="sxs-lookup"><span data-stu-id="45c57-130">address</span></span>|<span data-ttu-id="45c57-131">string</span><span class="sxs-lookup"><span data-stu-id="45c57-131">string</span></span>|<span data-ttu-id="45c57-p104">可选。区域的地址或名称。如果未指定，则返回整个工作表区域。</span><span class="sxs-lookup"><span data-stu-id="45c57-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="45c57-135">响应</span><span class="sxs-lookup"><span data-stu-id="45c57-135">Response</span></span>

<span data-ttu-id="45c57-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45c57-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45c57-137">示例</span><span class="sxs-lookup"><span data-stu-id="45c57-137">Example</span></span>
<span data-ttu-id="45c57-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="45c57-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="45c57-139">请求</span><span class="sxs-lookup"><span data-stu-id="45c57-139">Request</span></span>
<span data-ttu-id="45c57-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45c57-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="45c57-141">响应</span><span class="sxs-lookup"><span data-stu-id="45c57-141">Response</span></span>
<span data-ttu-id="45c57-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45c57-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="45c57-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="45c57-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="45c57-146">语言</span><span class="sxs-lookup"><span data-stu-id="45c57-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45c57-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="45c57-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_range-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="45c57-148">如果未指定`address`可选参数, 则此函数返回整个工作表区域。</span><span class="sxs-lookup"><span data-stu-id="45c57-148">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="45c57-149">请求</span><span class="sxs-lookup"><span data-stu-id="45c57-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="45c57-150">响应</span><span class="sxs-lookup"><span data-stu-id="45c57-150">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="45c57-151">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="45c57-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="45c57-152">语言</span><span class="sxs-lookup"><span data-stu-id="45c57-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_range_noaddress-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45c57-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="45c57-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_range_noaddress-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
