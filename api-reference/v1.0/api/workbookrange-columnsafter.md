---
title: 'workbookRange: columnsAfter'
description: 获取给定范围右侧的一定数量的列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 57edb0762d5e0d6b3b2061c52cee4d3374415345
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577518"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="e6a8d-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="e6a8d-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="e6a8d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6a8d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6a8d-105">获取给定范围右侧的一定数量的列。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-105">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6a8d-106">权限</span><span class="sxs-lookup"><span data-stu-id="e6a8d-106">Permissions</span></span>
<span data-ttu-id="e6a8d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6a8d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6a8d-109">Permission type</span></span>      | <span data-ttu-id="e6a8d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6a8d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6a8d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6a8d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e6a8d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6a8d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6a8d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6a8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6a8d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-114">Not supported.</span></span>    |
|<span data-ttu-id="e6a8d-115">Application</span><span class="sxs-lookup"><span data-stu-id="e6a8d-115">Application</span></span> | <span data-ttu-id="e6a8d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6a8d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6a8d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range/columnsAfter(count=n)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/columnsAfter(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="e6a8d-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="e6a8d-118">Function parameters</span></span>

| <span data-ttu-id="e6a8d-119">参数</span><span class="sxs-lookup"><span data-stu-id="e6a8d-119">Parameter</span></span>    | <span data-ttu-id="e6a8d-120">类型</span><span class="sxs-lookup"><span data-stu-id="e6a8d-120">Type</span></span>   |<span data-ttu-id="e6a8d-121">说明</span><span class="sxs-lookup"><span data-stu-id="e6a8d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6a8d-122">count</span><span class="sxs-lookup"><span data-stu-id="e6a8d-122">count</span></span>|<span data-ttu-id="e6a8d-123">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a8d-123">Int32</span></span>|<span data-ttu-id="e6a8d-124">可选。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-124">Optional.</span></span> <span data-ttu-id="e6a8d-125">生成的范围中要包含的列数。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-125">The number of columns to include in the resulting range.</span></span> <span data-ttu-id="e6a8d-126">一般来说，使用正数可以在当前范围之外创建一个范围。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-126">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="e6a8d-127">也可以使用负数在当前范围之内创建一个范围。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-127">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="e6a8d-128">默认值为 1</span><span class="sxs-lookup"><span data-stu-id="e6a8d-128">The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e6a8d-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6a8d-129">Request headers</span></span>
| <span data-ttu-id="e6a8d-130">名称</span><span class="sxs-lookup"><span data-stu-id="e6a8d-130">Name</span></span>       | <span data-ttu-id="e6a8d-131">说明</span><span class="sxs-lookup"><span data-stu-id="e6a8d-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6a8d-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6a8d-132">Authorization</span></span>  | <span data-ttu-id="e6a8d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6a8d-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e6a8d-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="e6a8d-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6a8d-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6a8d-138">Request body</span></span>
<span data-ttu-id="e6a8d-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6a8d-140">响应</span><span class="sxs-lookup"><span data-stu-id="e6a8d-140">Response</span></span>
<span data-ttu-id="e6a8d-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6a8d-142">示例</span><span class="sxs-lookup"><span data-stu-id="e6a8d-142">Example</span></span>
<span data-ttu-id="e6a8d-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e6a8d-144">请求</span><span class="sxs-lookup"><span data-stu-id="e6a8d-144">Request</span></span>
<span data-ttu-id="e6a8d-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e6a8d-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6a8d-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsafter",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```
# <a name="c"></a>[<span data-ttu-id="e6a8d-147">C#</span><span class="sxs-lookup"><span data-stu-id="e6a8d-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsafter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6a8d-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6a8d-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsafter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6a8d-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6a8d-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsafter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6a8d-150">Java</span><span class="sxs-lookup"><span data-stu-id="e6a8d-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsafter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e6a8d-151">响应</span><span class="sxs-lookup"><span data-stu-id="e6a8d-151">Response</span></span>
<span data-ttu-id="e6a8d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6a8d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

