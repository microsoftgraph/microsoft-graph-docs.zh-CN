---
title: Worksheet:UsedRange
description: 使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: deac7a5e33be0abfba5dd5efab3aaf28f42cddee
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728831"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="2dff6-104">Worksheet:UsedRange</span><span class="sxs-lookup"><span data-stu-id="2dff6-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="2dff6-p102">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="2dff6-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="2dff6-107">权限</span><span class="sxs-lookup"><span data-stu-id="2dff6-107">Permissions</span></span>
<span data-ttu-id="2dff6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2dff6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dff6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2dff6-110">Permission type</span></span>      | <span data-ttu-id="2dff6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2dff6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dff6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2dff6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2dff6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2dff6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2dff6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2dff6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dff6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2dff6-115">Not supported.</span></span>    |
|<span data-ttu-id="2dff6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2dff6-116">Application</span></span> | <span data-ttu-id="2dff6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2dff6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2dff6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2dff6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="2dff6-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="2dff6-119">Function parameters</span></span>
<span data-ttu-id="2dff6-120">在请求 URL 中, 可以提供可选参数。</span><span class="sxs-lookup"><span data-stu-id="2dff6-120">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="2dff6-121">参数</span><span class="sxs-lookup"><span data-stu-id="2dff6-121">Parameter</span></span>    | <span data-ttu-id="2dff6-122">类型</span><span class="sxs-lookup"><span data-stu-id="2dff6-122">Type</span></span>   |<span data-ttu-id="2dff6-123">说明</span><span class="sxs-lookup"><span data-stu-id="2dff6-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dff6-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="2dff6-124">valuesOnly</span></span>|<span data-ttu-id="2dff6-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dff6-125">Boolean</span></span>|<span data-ttu-id="2dff6-p104">可选。仅将具有值的单元格视为已使用的单元格（忽略格式）。</span><span class="sxs-lookup"><span data-stu-id="2dff6-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2dff6-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="2dff6-128">Request headers</span></span>
| <span data-ttu-id="2dff6-129">名称</span><span class="sxs-lookup"><span data-stu-id="2dff6-129">Name</span></span>       | <span data-ttu-id="2dff6-130">说明</span><span class="sxs-lookup"><span data-stu-id="2dff6-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2dff6-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="2dff6-131">Authorization</span></span>  | <span data-ttu-id="2dff6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2dff6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2dff6-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2dff6-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="2dff6-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2dff6-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dff6-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="2dff6-137">Request body</span></span>
<span data-ttu-id="2dff6-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2dff6-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2dff6-139">响应</span><span class="sxs-lookup"><span data-stu-id="2dff6-139">Response</span></span>

<span data-ttu-id="2dff6-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2dff6-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dff6-141">示例</span><span class="sxs-lookup"><span data-stu-id="2dff6-141">Example</span></span>
<span data-ttu-id="2dff6-142">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2dff6-142">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2dff6-143">请求</span><span class="sxs-lookup"><span data-stu-id="2dff6-143">Request</span></span>
<span data-ttu-id="2dff6-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2dff6-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2dff6-145">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2dff6-145">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2dff6-146">C#</span><span class="sxs-lookup"><span data-stu-id="2dff6-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2dff6-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2dff6-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2dff6-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="2dff6-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2dff6-149">Java</span><span class="sxs-lookup"><span data-stu-id="2dff6-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2dff6-150">响应</span><span class="sxs-lookup"><span data-stu-id="2dff6-150">Response</span></span>
<span data-ttu-id="2dff6-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2dff6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="2dff6-154">或者, 也可以使用可选`valuesOnly`参数调用此函数。</span><span class="sxs-lookup"><span data-stu-id="2dff6-154">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="2dff6-155">请求</span><span class="sxs-lookup"><span data-stu-id="2dff6-155">Request</span></span>
<span data-ttu-id="2dff6-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2dff6-156">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2dff6-157">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2dff6-157">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2dff6-158">C#</span><span class="sxs-lookup"><span data-stu-id="2dff6-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2dff6-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2dff6-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2dff6-160">目标-C</span><span class="sxs-lookup"><span data-stu-id="2dff6-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2dff6-161">Java</span><span class="sxs-lookup"><span data-stu-id="2dff6-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2dff6-162">响应</span><span class="sxs-lookup"><span data-stu-id="2dff6-162">Response</span></span>
<span data-ttu-id="2dff6-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2dff6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
