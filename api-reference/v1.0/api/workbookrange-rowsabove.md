---
title: 'workbookRange: rowsAbove'
description: 获取给定范围上方的一定数量的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 99df3b4ecb3d8a4f1de798cd6fdb3318cf51183f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575873"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="7397e-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="7397e-103">workbookRange: rowsAbove</span></span>

<span data-ttu-id="7397e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7397e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7397e-105">获取给定范围上方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="7397e-105">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="7397e-106">权限</span><span class="sxs-lookup"><span data-stu-id="7397e-106">Permissions</span></span>
<span data-ttu-id="7397e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7397e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7397e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7397e-109">Permission type</span></span>      | <span data-ttu-id="7397e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7397e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7397e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7397e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7397e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7397e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7397e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7397e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7397e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7397e-114">Not supported.</span></span>    |
|<span data-ttu-id="7397e-115">Application</span><span class="sxs-lookup"><span data-stu-id="7397e-115">Application</span></span> | <span data-ttu-id="7397e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7397e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7397e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7397e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range/rowsAbove(count=n)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="7397e-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="7397e-118">Function parameters</span></span>

| <span data-ttu-id="7397e-119">参数</span><span class="sxs-lookup"><span data-stu-id="7397e-119">Parameter</span></span>    | <span data-ttu-id="7397e-120">类型</span><span class="sxs-lookup"><span data-stu-id="7397e-120">Type</span></span>   |<span data-ttu-id="7397e-121">说明</span><span class="sxs-lookup"><span data-stu-id="7397e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7397e-122">count</span><span class="sxs-lookup"><span data-stu-id="7397e-122">count</span></span>|<span data-ttu-id="7397e-123">Int32</span><span class="sxs-lookup"><span data-stu-id="7397e-123">Int32</span></span>|<span data-ttu-id="7397e-p102">可选。生成的范围中要包含的行数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="7397e-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="7397e-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="7397e-129">Request headers</span></span>
| <span data-ttu-id="7397e-130">名称</span><span class="sxs-lookup"><span data-stu-id="7397e-130">Name</span></span>       | <span data-ttu-id="7397e-131">说明</span><span class="sxs-lookup"><span data-stu-id="7397e-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7397e-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="7397e-132">Authorization</span></span>  | <span data-ttu-id="7397e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7397e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7397e-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7397e-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="7397e-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7397e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7397e-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="7397e-138">Request body</span></span>
<span data-ttu-id="7397e-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7397e-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7397e-140">响应</span><span class="sxs-lookup"><span data-stu-id="7397e-140">Response</span></span>
<span data-ttu-id="7397e-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7397e-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7397e-142">示例</span><span class="sxs-lookup"><span data-stu-id="7397e-142">Example</span></span>
<span data-ttu-id="7397e-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7397e-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7397e-144">请求</span><span class="sxs-lookup"><span data-stu-id="7397e-144">Request</span></span>
<span data-ttu-id="7397e-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7397e-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7397e-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="7397e-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```
# <a name="c"></a>[<span data-ttu-id="7397e-147">C#</span><span class="sxs-lookup"><span data-stu-id="7397e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsabove-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7397e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7397e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsabove-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7397e-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7397e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsabove-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7397e-150">Java</span><span class="sxs-lookup"><span data-stu-id="7397e-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsabove-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7397e-151">响应</span><span class="sxs-lookup"><span data-stu-id="7397e-151">Response</span></span>
<span data-ttu-id="7397e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7397e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<span data-ttu-id="7397e-155">如果调用时不带可选 `count` 参数，则此函数返回区域上方的单个行。</span><span class="sxs-lookup"><span data-stu-id="7397e-155">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="7397e-156">请求</span><span class="sxs-lookup"><span data-stu-id="7397e-156">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7397e-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="7397e-157">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```
# <a name="c"></a>[<span data-ttu-id="7397e-158">C#</span><span class="sxs-lookup"><span data-stu-id="7397e-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsabove-nocount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7397e-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7397e-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsabove-nocount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7397e-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7397e-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsabove-nocount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7397e-161">Java</span><span class="sxs-lookup"><span data-stu-id="7397e-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsabove-nocount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7397e-162">响应</span><span class="sxs-lookup"><span data-stu-id="7397e-162">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

