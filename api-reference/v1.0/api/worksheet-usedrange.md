---
title: Worksheet:UsedRange
description: 使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: bdf2a49f70e1b2e3d50cc45788904feeeef22207
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884246"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="441e9-104">Worksheet:UsedRange</span><span class="sxs-lookup"><span data-stu-id="441e9-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="441e9-p102">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="441e9-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="441e9-107">权限</span><span class="sxs-lookup"><span data-stu-id="441e9-107">Permissions</span></span>
<span data-ttu-id="441e9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="441e9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="441e9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="441e9-110">Permission type</span></span>      | <span data-ttu-id="441e9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="441e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="441e9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="441e9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="441e9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="441e9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="441e9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="441e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="441e9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="441e9-115">Not supported.</span></span>    |
|<span data-ttu-id="441e9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="441e9-116">Application</span></span> | <span data-ttu-id="441e9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="441e9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="441e9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="441e9-118">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="441e9-119">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="441e9-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="441e9-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="441e9-120">Function parameters</span></span>
<span data-ttu-id="441e9-121">在请求 URL 中, 可以提供可选参数。</span><span class="sxs-lookup"><span data-stu-id="441e9-121">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="441e9-122">参数</span><span class="sxs-lookup"><span data-stu-id="441e9-122">Parameter</span></span>    | <span data-ttu-id="441e9-123">类型</span><span class="sxs-lookup"><span data-stu-id="441e9-123">Type</span></span>   |<span data-ttu-id="441e9-124">说明</span><span class="sxs-lookup"><span data-stu-id="441e9-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="441e9-125">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="441e9-125">valuesOnly</span></span>|<span data-ttu-id="441e9-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="441e9-126">Boolean</span></span>|<span data-ttu-id="441e9-p104">可选。仅将具有值的单元格视为已使用的单元格（忽略格式）。</span><span class="sxs-lookup"><span data-stu-id="441e9-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="441e9-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="441e9-129">Request headers</span></span>
| <span data-ttu-id="441e9-130">名称</span><span class="sxs-lookup"><span data-stu-id="441e9-130">Name</span></span>       | <span data-ttu-id="441e9-131">说明</span><span class="sxs-lookup"><span data-stu-id="441e9-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="441e9-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="441e9-132">Authorization</span></span>  | <span data-ttu-id="441e9-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="441e9-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="441e9-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="441e9-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="441e9-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="441e9-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="441e9-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="441e9-138">Request body</span></span>
<span data-ttu-id="441e9-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="441e9-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="441e9-140">响应</span><span class="sxs-lookup"><span data-stu-id="441e9-140">Response</span></span>

<span data-ttu-id="441e9-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="441e9-141">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="441e9-142">示例</span><span class="sxs-lookup"><span data-stu-id="441e9-142">Example</span></span>
<span data-ttu-id="441e9-143">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="441e9-143">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="441e9-144">请求</span><span class="sxs-lookup"><span data-stu-id="441e9-144">Request</span></span>
<span data-ttu-id="441e9-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="441e9-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="441e9-146">C#</span><span class="sxs-lookup"><span data-stu-id="441e9-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="441e9-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="441e9-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="441e9-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="441e9-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="441e9-149">Java</span><span class="sxs-lookup"><span data-stu-id="441e9-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="441e9-150">响应</span><span class="sxs-lookup"><span data-stu-id="441e9-150">Response</span></span>
<span data-ttu-id="441e9-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="441e9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="441e9-154">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="441e9-154">HTTP</span></span>](#tab/http)
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

<span data-ttu-id="441e9-155">或者, 也可以使用可选`valuesOnly`参数调用此函数。</span><span class="sxs-lookup"><span data-stu-id="441e9-155">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="441e9-156">请求</span><span class="sxs-lookup"><span data-stu-id="441e9-156">Request</span></span>
<span data-ttu-id="441e9-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="441e9-157">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="441e9-158">C#</span><span class="sxs-lookup"><span data-stu-id="441e9-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="441e9-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="441e9-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="441e9-160">目标-C</span><span class="sxs-lookup"><span data-stu-id="441e9-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="441e9-161">Java</span><span class="sxs-lookup"><span data-stu-id="441e9-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="441e9-162">响应</span><span class="sxs-lookup"><span data-stu-id="441e9-162">Response</span></span>
<span data-ttu-id="441e9-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="441e9-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
