---
title: Range:UsedRange
description: 返回指定 range 对象的所用范围。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8e413002f0c09cc027ec88777ab95d537ca8b8d2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33610767"
---
# <a name="range-usedrange"></a><span data-ttu-id="8f65f-103">Range:UsedRange</span><span class="sxs-lookup"><span data-stu-id="8f65f-103">Range: UsedRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f65f-104">返回指定 range 对象的所用范围。</span><span class="sxs-lookup"><span data-stu-id="8f65f-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f65f-105">权限</span><span class="sxs-lookup"><span data-stu-id="8f65f-105">Permissions</span></span>
<span data-ttu-id="8f65f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f65f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f65f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f65f-108">Permission type</span></span>      | <span data-ttu-id="8f65f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f65f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f65f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f65f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f65f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f65f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f65f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f65f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f65f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f65f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f65f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f65f-114">Application</span></span> | <span data-ttu-id="8f65f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f65f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f65f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f65f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="8f65f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f65f-117">Request headers</span></span>
| <span data-ttu-id="8f65f-118">名称</span><span class="sxs-lookup"><span data-stu-id="8f65f-118">Name</span></span>       | <span data-ttu-id="8f65f-119">说明</span><span class="sxs-lookup"><span data-stu-id="8f65f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f65f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f65f-120">Authorization</span></span>  | <span data-ttu-id="8f65f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f65f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f65f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8f65f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8f65f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8f65f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f65f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f65f-126">Request body</span></span>
<span data-ttu-id="8f65f-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8f65f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8f65f-128">参数</span><span class="sxs-lookup"><span data-stu-id="8f65f-128">Parameter</span></span>    | <span data-ttu-id="8f65f-129">类型</span><span class="sxs-lookup"><span data-stu-id="8f65f-129">Type</span></span>   |<span data-ttu-id="8f65f-130">说明</span><span class="sxs-lookup"><span data-stu-id="8f65f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f65f-131">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="8f65f-131">valuesOnly</span></span>|<span data-ttu-id="8f65f-132">布尔</span><span class="sxs-lookup"><span data-stu-id="8f65f-132">boolean</span></span>|<span data-ttu-id="8f65f-p104">可选。仅将有值的单元格视为已使用的单元格。</span><span class="sxs-lookup"><span data-stu-id="8f65f-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="8f65f-135">响应</span><span class="sxs-lookup"><span data-stu-id="8f65f-135">Response</span></span>

<span data-ttu-id="8f65f-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f65f-136">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f65f-137">示例</span><span class="sxs-lookup"><span data-stu-id="8f65f-137">Example</span></span>
<span data-ttu-id="8f65f-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8f65f-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8f65f-139">请求</span><span class="sxs-lookup"><span data-stu-id="8f65f-139">Request</span></span>
<span data-ttu-id="8f65f-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f65f-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="8f65f-141">响应</span><span class="sxs-lookup"><span data-stu-id="8f65f-141">Response</span></span>
<span data-ttu-id="8f65f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f65f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8f65f-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8f65f-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8f65f-146">语言</span><span class="sxs-lookup"><span data-stu-id="8f65f-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_usedrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f65f-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f65f-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_usedrange-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
