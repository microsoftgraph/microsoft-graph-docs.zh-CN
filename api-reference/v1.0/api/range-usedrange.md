---
title: Range:UsedRange
description: 返回指定 range 对象的所用范围。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 97ea9cd720b38b774aa262eee53a1457bc2c842d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607926"
---
# <a name="range-usedrange"></a><span data-ttu-id="de811-103">Range:UsedRange</span><span class="sxs-lookup"><span data-stu-id="de811-103">Range: UsedRange</span></span>

<span data-ttu-id="de811-104">返回指定 range 对象的所用范围。</span><span class="sxs-lookup"><span data-stu-id="de811-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="de811-105">权限</span><span class="sxs-lookup"><span data-stu-id="de811-105">Permissions</span></span>
<span data-ttu-id="de811-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de811-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de811-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="de811-108">Permission type</span></span>      | <span data-ttu-id="de811-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de811-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de811-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de811-110">Delegated (work or school account)</span></span> | <span data-ttu-id="de811-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de811-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="de811-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de811-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de811-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="de811-113">Not supported.</span></span>    |
|<span data-ttu-id="de811-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="de811-114">Application</span></span> | <span data-ttu-id="de811-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="de811-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de811-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de811-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="de811-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="de811-117">Request headers</span></span>
| <span data-ttu-id="de811-118">名称</span><span class="sxs-lookup"><span data-stu-id="de811-118">Name</span></span>       | <span data-ttu-id="de811-119">说明</span><span class="sxs-lookup"><span data-stu-id="de811-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="de811-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="de811-120">Authorization</span></span>  | <span data-ttu-id="de811-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de811-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de811-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="de811-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="de811-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="de811-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="de811-126">路径参数</span><span class="sxs-lookup"><span data-stu-id="de811-126">Path parameters</span></span>
| <span data-ttu-id="de811-127">参数</span><span class="sxs-lookup"><span data-stu-id="de811-127">Parameter</span></span>    | <span data-ttu-id="de811-128">类型</span><span class="sxs-lookup"><span data-stu-id="de811-128">Type</span></span>   |<span data-ttu-id="de811-129">说明</span><span class="sxs-lookup"><span data-stu-id="de811-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de811-130">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="de811-130">valuesOnly</span></span>|<span data-ttu-id="de811-131">布尔</span><span class="sxs-lookup"><span data-stu-id="de811-131">boolean</span></span>|<span data-ttu-id="de811-p104">可选。仅将有值的单元格视为已使用的单元格。</span><span class="sxs-lookup"><span data-stu-id="de811-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="de811-134">响应</span><span class="sxs-lookup"><span data-stu-id="de811-134">Response</span></span>

<span data-ttu-id="de811-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de811-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de811-136">示例</span><span class="sxs-lookup"><span data-stu-id="de811-136">Example</span></span>
<span data-ttu-id="de811-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="de811-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="de811-138">请求</span><span class="sxs-lookup"><span data-stu-id="de811-138">Request</span></span>
<span data-ttu-id="de811-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de811-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```

##### <a name="response"></a><span data-ttu-id="de811-140">响应</span><span class="sxs-lookup"><span data-stu-id="de811-140">Response</span></span>
<span data-ttu-id="de811-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de811-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="de811-144">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="de811-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="de811-145">语言</span><span class="sxs-lookup"><span data-stu-id="de811-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_usedrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de811-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="de811-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_usedrange-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="de811-147">下面是一个指定可选`valuesOnly`参数的示例。</span><span class="sxs-lookup"><span data-stu-id="de811-147">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="de811-148">请求</span><span class="sxs-lookup"><span data-stu-id="de811-148">Request</span></span>
<span data-ttu-id="de811-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de811-149">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="de811-150">响应</span><span class="sxs-lookup"><span data-stu-id="de811-150">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="de811-151">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="de811-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="de811-152">语言</span><span class="sxs-lookup"><span data-stu-id="de811-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_usedrange_valuesonly-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de811-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="de811-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_usedrange_valuesonly-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
