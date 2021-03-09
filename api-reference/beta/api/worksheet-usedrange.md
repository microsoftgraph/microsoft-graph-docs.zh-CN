---
title: Worksheet:UsedRange
description: 使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3da9ece84c8c6fedd36a08bb6f489eaa89bb8b7c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578146"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="613fd-104">Worksheet:UsedRange</span><span class="sxs-lookup"><span data-stu-id="613fd-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="613fd-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="613fd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="613fd-p102">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="613fd-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="613fd-108">权限</span><span class="sxs-lookup"><span data-stu-id="613fd-108">Permissions</span></span>
<span data-ttu-id="613fd-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="613fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="613fd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="613fd-111">Permission type</span></span>      | <span data-ttu-id="613fd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="613fd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="613fd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="613fd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="613fd-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="613fd-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="613fd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="613fd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="613fd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="613fd-116">Not supported.</span></span>    |
|<span data-ttu-id="613fd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="613fd-117">Application</span></span> | <span data-ttu-id="613fd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="613fd-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="613fd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="613fd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/UsedRange

```

## <a name="function-parameters"></a><span data-ttu-id="613fd-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="613fd-120">Function parameters</span></span>
<span data-ttu-id="613fd-121">在请求 URL 中，提供可选的查询参数。</span><span class="sxs-lookup"><span data-stu-id="613fd-121">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="613fd-122">参数</span><span class="sxs-lookup"><span data-stu-id="613fd-122">Parameter</span></span>    | <span data-ttu-id="613fd-123">类型</span><span class="sxs-lookup"><span data-stu-id="613fd-123">Type</span></span>   |<span data-ttu-id="613fd-124">说明</span><span class="sxs-lookup"><span data-stu-id="613fd-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="613fd-125">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="613fd-125">valuesOnly</span></span>|<span data-ttu-id="613fd-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="613fd-126">Boolean</span></span>|<span data-ttu-id="613fd-p104">可选。仅将具有值的单元格视为已使用的单元格（忽略格式）。</span><span class="sxs-lookup"><span data-stu-id="613fd-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="613fd-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="613fd-129">Request headers</span></span>
| <span data-ttu-id="613fd-130">名称</span><span class="sxs-lookup"><span data-stu-id="613fd-130">Name</span></span>       | <span data-ttu-id="613fd-131">说明</span><span class="sxs-lookup"><span data-stu-id="613fd-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="613fd-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="613fd-132">Authorization</span></span>  | <span data-ttu-id="613fd-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="613fd-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="613fd-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="613fd-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="613fd-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="613fd-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="613fd-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="613fd-138">Request body</span></span>
<span data-ttu-id="613fd-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="613fd-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="613fd-140">响应</span><span class="sxs-lookup"><span data-stu-id="613fd-140">Response</span></span>

<span data-ttu-id="613fd-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="613fd-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="613fd-142">示例</span><span class="sxs-lookup"><span data-stu-id="613fd-142">Example</span></span>
<span data-ttu-id="613fd-143">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="613fd-143">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="613fd-144">请求</span><span class="sxs-lookup"><span data-stu-id="613fd-144">Request</span></span>
<span data-ttu-id="613fd-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="613fd-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="613fd-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="613fd-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
```
# <a name="c"></a>[<span data-ttu-id="613fd-147">C#</span><span class="sxs-lookup"><span data-stu-id="613fd-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="613fd-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="613fd-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="613fd-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="613fd-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="613fd-150">Java</span><span class="sxs-lookup"><span data-stu-id="613fd-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="613fd-151">响应</span><span class="sxs-lookup"><span data-stu-id="613fd-151">Response</span></span>
<span data-ttu-id="613fd-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="613fd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


