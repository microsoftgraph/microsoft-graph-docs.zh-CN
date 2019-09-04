---
title: Range:UsedRange
description: 返回指定 range 对象的所用范围。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 94a708f16c8e252793d6ef16d11c3f009ddc0530
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729831"
---
# <a name="range-usedrange"></a><span data-ttu-id="79310-103">Range:UsedRange</span><span class="sxs-lookup"><span data-stu-id="79310-103">Range: UsedRange</span></span>

<span data-ttu-id="79310-104">返回指定 range 对象的所用范围。</span><span class="sxs-lookup"><span data-stu-id="79310-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="79310-105">权限</span><span class="sxs-lookup"><span data-stu-id="79310-105">Permissions</span></span>
<span data-ttu-id="79310-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79310-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="79310-108">Permission type</span></span>      | <span data-ttu-id="79310-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79310-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79310-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79310-110">Delegated (work or school account)</span></span> | <span data-ttu-id="79310-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79310-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="79310-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79310-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79310-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="79310-113">Not supported.</span></span>    |
|<span data-ttu-id="79310-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="79310-114">Application</span></span> | <span data-ttu-id="79310-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="79310-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79310-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79310-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="79310-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="79310-117">Request headers</span></span>
| <span data-ttu-id="79310-118">名称</span><span class="sxs-lookup"><span data-stu-id="79310-118">Name</span></span>       | <span data-ttu-id="79310-119">说明</span><span class="sxs-lookup"><span data-stu-id="79310-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79310-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="79310-120">Authorization</span></span>  | <span data-ttu-id="79310-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79310-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79310-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="79310-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="79310-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="79310-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="79310-126">路径参数</span><span class="sxs-lookup"><span data-stu-id="79310-126">Path parameters</span></span>
| <span data-ttu-id="79310-127">参数</span><span class="sxs-lookup"><span data-stu-id="79310-127">Parameter</span></span>    | <span data-ttu-id="79310-128">类型</span><span class="sxs-lookup"><span data-stu-id="79310-128">Type</span></span>   |<span data-ttu-id="79310-129">说明</span><span class="sxs-lookup"><span data-stu-id="79310-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79310-130">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="79310-130">valuesOnly</span></span>|<span data-ttu-id="79310-131">布尔</span><span class="sxs-lookup"><span data-stu-id="79310-131">boolean</span></span>|<span data-ttu-id="79310-p104">可选。仅将有值的单元格视为已使用的单元格。</span><span class="sxs-lookup"><span data-stu-id="79310-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="79310-134">响应</span><span class="sxs-lookup"><span data-stu-id="79310-134">Response</span></span>

<span data-ttu-id="79310-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79310-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79310-136">示例</span><span class="sxs-lookup"><span data-stu-id="79310-136">Example</span></span>
<span data-ttu-id="79310-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="79310-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79310-138">请求</span><span class="sxs-lookup"><span data-stu-id="79310-138">Request</span></span>
<span data-ttu-id="79310-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79310-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79310-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="79310-140">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79310-141">C#</span><span class="sxs-lookup"><span data-stu-id="79310-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79310-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79310-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79310-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="79310-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="79310-144">Java</span><span class="sxs-lookup"><span data-stu-id="79310-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="79310-145">响应</span><span class="sxs-lookup"><span data-stu-id="79310-145">Response</span></span>
<span data-ttu-id="79310-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79310-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="79310-149">下面是一个指定可选`valuesOnly`参数的示例。</span><span class="sxs-lookup"><span data-stu-id="79310-149">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="79310-150">请求</span><span class="sxs-lookup"><span data-stu-id="79310-150">Request</span></span>
<span data-ttu-id="79310-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79310-151">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79310-152">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="79310-152">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79310-153">C#</span><span class="sxs-lookup"><span data-stu-id="79310-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79310-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79310-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79310-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="79310-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="79310-156">Java</span><span class="sxs-lookup"><span data-stu-id="79310-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="79310-157">响应</span><span class="sxs-lookup"><span data-stu-id="79310-157">Response</span></span>

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
