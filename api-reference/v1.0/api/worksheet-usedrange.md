---
title: Worksheet:UsedRange
description: 使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 645814a3f09ac5259047cf73a7b201264c24d067
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36307369"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="9f59b-104">Worksheet:UsedRange</span><span class="sxs-lookup"><span data-stu-id="9f59b-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="9f59b-p102">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="9f59b-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f59b-107">权限</span><span class="sxs-lookup"><span data-stu-id="9f59b-107">Permissions</span></span>
<span data-ttu-id="9f59b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f59b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f59b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f59b-110">Permission type</span></span>      | <span data-ttu-id="9f59b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f59b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f59b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f59b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9f59b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f59b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9f59b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f59b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f59b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f59b-115">Not supported.</span></span>    |
|<span data-ttu-id="9f59b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f59b-116">Application</span></span> | <span data-ttu-id="9f59b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f59b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f59b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f59b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="9f59b-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="9f59b-119">Function parameters</span></span>
<span data-ttu-id="9f59b-120">在请求 URL 中, 可以提供可选参数。</span><span class="sxs-lookup"><span data-stu-id="9f59b-120">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="9f59b-121">参数</span><span class="sxs-lookup"><span data-stu-id="9f59b-121">Parameter</span></span>    | <span data-ttu-id="9f59b-122">类型</span><span class="sxs-lookup"><span data-stu-id="9f59b-122">Type</span></span>   |<span data-ttu-id="9f59b-123">说明</span><span class="sxs-lookup"><span data-stu-id="9f59b-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f59b-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="9f59b-124">valuesOnly</span></span>|<span data-ttu-id="9f59b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f59b-125">Boolean</span></span>|<span data-ttu-id="9f59b-p104">可选。仅将具有值的单元格视为已使用的单元格（忽略格式）。</span><span class="sxs-lookup"><span data-stu-id="9f59b-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9f59b-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f59b-128">Request headers</span></span>
| <span data-ttu-id="9f59b-129">名称</span><span class="sxs-lookup"><span data-stu-id="9f59b-129">Name</span></span>       | <span data-ttu-id="9f59b-130">说明</span><span class="sxs-lookup"><span data-stu-id="9f59b-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9f59b-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f59b-131">Authorization</span></span>  | <span data-ttu-id="9f59b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f59b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f59b-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9f59b-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="9f59b-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9f59b-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f59b-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f59b-137">Request body</span></span>
<span data-ttu-id="9f59b-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f59b-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f59b-139">响应</span><span class="sxs-lookup"><span data-stu-id="9f59b-139">Response</span></span>

<span data-ttu-id="9f59b-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f59b-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f59b-141">示例</span><span class="sxs-lookup"><span data-stu-id="9f59b-141">Example</span></span>
<span data-ttu-id="9f59b-142">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9f59b-142">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9f59b-143">请求</span><span class="sxs-lookup"><span data-stu-id="9f59b-143">Request</span></span>
<span data-ttu-id="9f59b-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f59b-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9f59b-145">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9f59b-145">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9f59b-146">C#</span><span class="sxs-lookup"><span data-stu-id="9f59b-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f59b-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f59b-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9f59b-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="9f59b-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9f59b-149">Java</span><span class="sxs-lookup"><span data-stu-id="9f59b-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9f59b-150">响应</span><span class="sxs-lookup"><span data-stu-id="9f59b-150">Response</span></span>
<span data-ttu-id="9f59b-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f59b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="9f59b-154">或者, 也可以使用可选`valuesOnly`参数调用此函数。</span><span class="sxs-lookup"><span data-stu-id="9f59b-154">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="9f59b-155">请求</span><span class="sxs-lookup"><span data-stu-id="9f59b-155">Request</span></span>
<span data-ttu-id="9f59b-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f59b-156">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9f59b-157">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9f59b-157">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9f59b-158">C#</span><span class="sxs-lookup"><span data-stu-id="9f59b-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f59b-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f59b-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9f59b-160">目标-C</span><span class="sxs-lookup"><span data-stu-id="9f59b-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9f59b-161">Java</span><span class="sxs-lookup"><span data-stu-id="9f59b-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9f59b-162">响应</span><span class="sxs-lookup"><span data-stu-id="9f59b-162">Response</span></span>
<span data-ttu-id="9f59b-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f59b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
