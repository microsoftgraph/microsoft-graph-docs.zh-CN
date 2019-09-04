---
title: Worksheet:Range
description: 获取地址或名称指定的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5aecc0100d0915c16afa72a95e162fa2907b4a55
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728832"
---
# <a name="worksheet-range"></a><span data-ttu-id="c3ee2-103">Worksheet:Range</span><span class="sxs-lookup"><span data-stu-id="c3ee2-103">Worksheet: Range</span></span>

<span data-ttu-id="c3ee2-104">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="c3ee2-105">权限</span><span class="sxs-lookup"><span data-stu-id="c3ee2-105">Permissions</span></span>
<span data-ttu-id="c3ee2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3ee2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3ee2-108">Permission type</span></span>      | <span data-ttu-id="c3ee2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3ee2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3ee2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3ee2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3ee2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3ee2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c3ee2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3ee2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3ee2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-113">Not supported.</span></span>    |
|<span data-ttu-id="c3ee2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3ee2-114">Application</span></span> | <span data-ttu-id="c3ee2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3ee2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3ee2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="c3ee2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3ee2-117">Request headers</span></span>
| <span data-ttu-id="c3ee2-118">名称</span><span class="sxs-lookup"><span data-stu-id="c3ee2-118">Name</span></span>       | <span data-ttu-id="c3ee2-119">说明</span><span class="sxs-lookup"><span data-stu-id="c3ee2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c3ee2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3ee2-120">Authorization</span></span>  | <span data-ttu-id="c3ee2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3ee2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c3ee2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c3ee2-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="c3ee2-126">函数参数</span><span class="sxs-lookup"><span data-stu-id="c3ee2-126">Function parameters</span></span>

| <span data-ttu-id="c3ee2-127">参数</span><span class="sxs-lookup"><span data-stu-id="c3ee2-127">Parameter</span></span>    | <span data-ttu-id="c3ee2-128">类型</span><span class="sxs-lookup"><span data-stu-id="c3ee2-128">Type</span></span>   |<span data-ttu-id="c3ee2-129">说明</span><span class="sxs-lookup"><span data-stu-id="c3ee2-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3ee2-130">address</span><span class="sxs-lookup"><span data-stu-id="c3ee2-130">address</span></span>|<span data-ttu-id="c3ee2-131">string</span><span class="sxs-lookup"><span data-stu-id="c3ee2-131">string</span></span>|<span data-ttu-id="c3ee2-p104">可选。区域的地址或名称。如果未指定，则返回整个工作表区域。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="c3ee2-135">响应</span><span class="sxs-lookup"><span data-stu-id="c3ee2-135">Response</span></span>

<span data-ttu-id="c3ee2-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3ee2-137">示例</span><span class="sxs-lookup"><span data-stu-id="c3ee2-137">Example</span></span>
<span data-ttu-id="c3ee2-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c3ee2-139">请求</span><span class="sxs-lookup"><span data-stu-id="c3ee2-139">Request</span></span>
<span data-ttu-id="c3ee2-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c3ee2-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c3ee2-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3ee2-142">C#</span><span class="sxs-lookup"><span data-stu-id="c3ee2-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3ee2-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3ee2-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3ee2-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="c3ee2-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3ee2-145">Java</span><span class="sxs-lookup"><span data-stu-id="c3ee2-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c3ee2-146">响应</span><span class="sxs-lookup"><span data-stu-id="c3ee2-146">Response</span></span>
<span data-ttu-id="c3ee2-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="c3ee2-150">如果未指定`address`可选参数, 则此函数返回整个工作表区域。</span><span class="sxs-lookup"><span data-stu-id="c3ee2-150">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="c3ee2-151">请求</span><span class="sxs-lookup"><span data-stu-id="c3ee2-151">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3ee2-152">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c3ee2-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3ee2-153">C#</span><span class="sxs-lookup"><span data-stu-id="c3ee2-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-noaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3ee2-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3ee2-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-noaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3ee2-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="c3ee2-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-noaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3ee2-156">Java</span><span class="sxs-lookup"><span data-stu-id="c3ee2-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-noaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c3ee2-157">响应</span><span class="sxs-lookup"><span data-stu-id="c3ee2-157">Response</span></span>

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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
