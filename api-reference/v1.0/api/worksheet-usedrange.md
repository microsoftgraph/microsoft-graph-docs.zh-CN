---
title: Worksheet:UsedRange
description: 使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 43bc6bc3646dadde3b8438977daa5f1b41682582
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575866"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="8e663-104">Worksheet:UsedRange</span><span class="sxs-lookup"><span data-stu-id="8e663-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="8e663-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e663-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e663-p102">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="8e663-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="8e663-108">权限</span><span class="sxs-lookup"><span data-stu-id="8e663-108">Permissions</span></span>
<span data-ttu-id="8e663-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e663-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e663-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e663-111">Permission type</span></span>      | <span data-ttu-id="8e663-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e663-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e663-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e663-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8e663-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e663-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8e663-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e663-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e663-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e663-116">Not supported.</span></span>    |
|<span data-ttu-id="8e663-117">Application</span><span class="sxs-lookup"><span data-stu-id="8e663-117">Application</span></span> | <span data-ttu-id="8e663-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e663-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e663-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e663-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="8e663-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="8e663-120">Function parameters</span></span>
<span data-ttu-id="8e663-121">在请求 URL 中，您可以提供可选参数。</span><span class="sxs-lookup"><span data-stu-id="8e663-121">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="8e663-122">参数</span><span class="sxs-lookup"><span data-stu-id="8e663-122">Parameter</span></span>    | <span data-ttu-id="8e663-123">类型</span><span class="sxs-lookup"><span data-stu-id="8e663-123">Type</span></span>   |<span data-ttu-id="8e663-124">说明</span><span class="sxs-lookup"><span data-stu-id="8e663-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e663-125">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="8e663-125">valuesOnly</span></span>|<span data-ttu-id="8e663-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e663-126">Boolean</span></span>|<span data-ttu-id="8e663-p104">可选。仅将具有值的单元格视为已使用的单元格（忽略格式）。</span><span class="sxs-lookup"><span data-stu-id="8e663-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="8e663-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e663-129">Request headers</span></span>
| <span data-ttu-id="8e663-130">名称</span><span class="sxs-lookup"><span data-stu-id="8e663-130">Name</span></span>       | <span data-ttu-id="8e663-131">说明</span><span class="sxs-lookup"><span data-stu-id="8e663-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8e663-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e663-132">Authorization</span></span>  | <span data-ttu-id="8e663-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e663-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e663-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8e663-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="8e663-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8e663-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e663-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e663-138">Request body</span></span>
<span data-ttu-id="8e663-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e663-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e663-140">响应</span><span class="sxs-lookup"><span data-stu-id="8e663-140">Response</span></span>

<span data-ttu-id="8e663-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e663-141">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e663-142">示例</span><span class="sxs-lookup"><span data-stu-id="8e663-142">Example</span></span>
<span data-ttu-id="8e663-143">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8e663-143">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8e663-144">请求</span><span class="sxs-lookup"><span data-stu-id="8e663-144">Request</span></span>
<span data-ttu-id="8e663-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e663-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e663-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e663-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```
# <a name="c"></a>[<span data-ttu-id="8e663-147">C#</span><span class="sxs-lookup"><span data-stu-id="8e663-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e663-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e663-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e663-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e663-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e663-150">Java</span><span class="sxs-lookup"><span data-stu-id="8e663-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8e663-151">响应</span><span class="sxs-lookup"><span data-stu-id="8e663-151">Response</span></span>
<span data-ttu-id="8e663-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e663-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="8e663-155">或者，可以使用可选参数调用此 `valuesOnly` 函数。</span><span class="sxs-lookup"><span data-stu-id="8e663-155">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="8e663-156">请求</span><span class="sxs-lookup"><span data-stu-id="8e663-156">Request</span></span>
<span data-ttu-id="8e663-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e663-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e663-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e663-158">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```
# <a name="c"></a>[<span data-ttu-id="8e663-159">C#</span><span class="sxs-lookup"><span data-stu-id="8e663-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e663-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e663-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e663-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e663-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e663-162">Java</span><span class="sxs-lookup"><span data-stu-id="8e663-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8e663-163">响应</span><span class="sxs-lookup"><span data-stu-id="8e663-163">Response</span></span>
<span data-ttu-id="8e663-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e663-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

