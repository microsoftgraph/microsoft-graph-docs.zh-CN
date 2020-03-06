---
title: 'workbookRange: rowsBelow'
description: 获取给定范围下方的一定数量的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 858f05197c9e738eb2ab7fe44d434254bca7b08d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508735"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="5b6de-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="5b6de-103">workbookRange: rowsBelow</span></span>

<span data-ttu-id="5b6de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b6de-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b6de-105">获取给定范围下方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="5b6de-105">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b6de-106">权限</span><span class="sxs-lookup"><span data-stu-id="5b6de-106">Permissions</span></span>
<span data-ttu-id="5b6de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b6de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b6de-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b6de-109">Permission type</span></span>      | <span data-ttu-id="5b6de-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b6de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b6de-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b6de-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5b6de-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b6de-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5b6de-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b6de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b6de-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b6de-114">Not supported.</span></span>    |
|<span data-ttu-id="5b6de-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b6de-115">Application</span></span> | <span data-ttu-id="5b6de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b6de-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b6de-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b6de-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="5b6de-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="5b6de-118">Function parameters</span></span>

| <span data-ttu-id="5b6de-119">参数</span><span class="sxs-lookup"><span data-stu-id="5b6de-119">Parameter</span></span>    | <span data-ttu-id="5b6de-120">类型</span><span class="sxs-lookup"><span data-stu-id="5b6de-120">Type</span></span>   |<span data-ttu-id="5b6de-121">说明</span><span class="sxs-lookup"><span data-stu-id="5b6de-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b6de-122">count</span><span class="sxs-lookup"><span data-stu-id="5b6de-122">count</span></span>|<span data-ttu-id="5b6de-123">Int32</span><span class="sxs-lookup"><span data-stu-id="5b6de-123">Int32</span></span>| <span data-ttu-id="5b6de-p102">可选。生成的范围中要包含的行数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="5b6de-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="5b6de-129">请求头</span><span class="sxs-lookup"><span data-stu-id="5b6de-129">Request headers</span></span>
| <span data-ttu-id="5b6de-130">名称</span><span class="sxs-lookup"><span data-stu-id="5b6de-130">Name</span></span>       | <span data-ttu-id="5b6de-131">说明</span><span class="sxs-lookup"><span data-stu-id="5b6de-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5b6de-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b6de-132">Authorization</span></span>  | <span data-ttu-id="5b6de-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b6de-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b6de-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5b6de-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="5b6de-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5b6de-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b6de-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b6de-138">Request body</span></span>
<span data-ttu-id="5b6de-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5b6de-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b6de-140">响应</span><span class="sxs-lookup"><span data-stu-id="5b6de-140">Response</span></span>
<span data-ttu-id="5b6de-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5b6de-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b6de-142">示例</span><span class="sxs-lookup"><span data-stu-id="5b6de-142">Example</span></span>
<span data-ttu-id="5b6de-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5b6de-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5b6de-144">请求</span><span class="sxs-lookup"><span data-stu-id="5b6de-144">Request</span></span>
<span data-ttu-id="5b6de-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b6de-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b6de-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b6de-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```
# <a name="c"></a>[<span data-ttu-id="5b6de-147">C#</span><span class="sxs-lookup"><span data-stu-id="5b6de-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b6de-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b6de-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b6de-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b6de-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b6de-150">Java</span><span class="sxs-lookup"><span data-stu-id="5b6de-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsbelow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5b6de-151">响应</span><span class="sxs-lookup"><span data-stu-id="5b6de-151">Response</span></span>
<span data-ttu-id="5b6de-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b6de-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="5b6de-155">如果不带`count`参数调用，则此函数默认为一行。</span><span class="sxs-lookup"><span data-stu-id="5b6de-155">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="5b6de-156">请求</span><span class="sxs-lookup"><span data-stu-id="5b6de-156">Request</span></span>
<span data-ttu-id="5b6de-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b6de-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b6de-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b6de-158">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```
# <a name="c"></a>[<span data-ttu-id="5b6de-159">C#</span><span class="sxs-lookup"><span data-stu-id="5b6de-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-nocount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b6de-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b6de-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-nocount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b6de-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b6de-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-nocount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b6de-162">Java</span><span class="sxs-lookup"><span data-stu-id="5b6de-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsbelow-nocount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5b6de-163">响应</span><span class="sxs-lookup"><span data-stu-id="5b6de-163">Response</span></span>
<span data-ttu-id="5b6de-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b6de-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
