---
title: Range:UsedRange
description: 返回指定 range 对象的所用范围。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f5761a90cafafc00abb00ec40318a3fac176b5c4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051562"
---
# <a name="range-usedrange"></a><span data-ttu-id="12b8d-103">Range:UsedRange</span><span class="sxs-lookup"><span data-stu-id="12b8d-103">Range: UsedRange</span></span>

<span data-ttu-id="12b8d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12b8d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12b8d-105">返回指定 range 对象的所用范围。</span><span class="sxs-lookup"><span data-stu-id="12b8d-105">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="12b8d-106">权限</span><span class="sxs-lookup"><span data-stu-id="12b8d-106">Permissions</span></span>
<span data-ttu-id="12b8d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12b8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12b8d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="12b8d-109">Permission type</span></span>      | <span data-ttu-id="12b8d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12b8d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12b8d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12b8d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="12b8d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b8d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="12b8d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12b8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12b8d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="12b8d-114">Not supported.</span></span>    |
|<span data-ttu-id="12b8d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="12b8d-115">Application</span></span> | <span data-ttu-id="12b8d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12b8d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12b8d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12b8d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="12b8d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="12b8d-118">Request headers</span></span>
| <span data-ttu-id="12b8d-119">名称</span><span class="sxs-lookup"><span data-stu-id="12b8d-119">Name</span></span>       | <span data-ttu-id="12b8d-120">说明</span><span class="sxs-lookup"><span data-stu-id="12b8d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="12b8d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="12b8d-121">Authorization</span></span>  | <span data-ttu-id="12b8d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="12b8d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12b8d-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="12b8d-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="12b8d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="12b8d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="12b8d-127">路径参数</span><span class="sxs-lookup"><span data-stu-id="12b8d-127">Path parameters</span></span>
| <span data-ttu-id="12b8d-128">参数</span><span class="sxs-lookup"><span data-stu-id="12b8d-128">Parameter</span></span>    | <span data-ttu-id="12b8d-129">类型</span><span class="sxs-lookup"><span data-stu-id="12b8d-129">Type</span></span>   |<span data-ttu-id="12b8d-130">说明</span><span class="sxs-lookup"><span data-stu-id="12b8d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12b8d-131">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="12b8d-131">valuesOnly</span></span>|<span data-ttu-id="12b8d-132">布尔</span><span class="sxs-lookup"><span data-stu-id="12b8d-132">boolean</span></span>|<span data-ttu-id="12b8d-p104">可选。仅将有值的单元格视为已使用的单元格。</span><span class="sxs-lookup"><span data-stu-id="12b8d-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="12b8d-135">响应</span><span class="sxs-lookup"><span data-stu-id="12b8d-135">Response</span></span>

<span data-ttu-id="12b8d-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12b8d-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12b8d-137">示例</span><span class="sxs-lookup"><span data-stu-id="12b8d-137">Example</span></span>
<span data-ttu-id="12b8d-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="12b8d-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="12b8d-139">请求</span><span class="sxs-lookup"><span data-stu-id="12b8d-139">Request</span></span>
<span data-ttu-id="12b8d-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12b8d-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12b8d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="12b8d-141">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```
# <a name="c"></a>[<span data-ttu-id="12b8d-142">C#</span><span class="sxs-lookup"><span data-stu-id="12b8d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12b8d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12b8d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12b8d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12b8d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12b8d-145">Java</span><span class="sxs-lookup"><span data-stu-id="12b8d-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="12b8d-146">响应</span><span class="sxs-lookup"><span data-stu-id="12b8d-146">Response</span></span>
<span data-ttu-id="12b8d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12b8d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="12b8d-150">下面是一个指定可选参数的示例 `valuesOnly` 。</span><span class="sxs-lookup"><span data-stu-id="12b8d-150">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="12b8d-151">请求</span><span class="sxs-lookup"><span data-stu-id="12b8d-151">Request</span></span>
<span data-ttu-id="12b8d-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12b8d-152">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12b8d-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="12b8d-153">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```
# <a name="c"></a>[<span data-ttu-id="12b8d-154">C#</span><span class="sxs-lookup"><span data-stu-id="12b8d-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12b8d-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12b8d-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12b8d-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12b8d-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12b8d-157">Java</span><span class="sxs-lookup"><span data-stu-id="12b8d-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="12b8d-158">响应</span><span class="sxs-lookup"><span data-stu-id="12b8d-158">Response</span></span>

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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

