---
title: 'workbookRange: rowsBelow'
description: 获取给定范围下方的一定数量的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b51bb7fbe40e4c2f1316b42a96fcd4631864db54
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458745"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="ed176-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="ed176-103">workbookRange: rowsBelow</span></span>

<span data-ttu-id="ed176-104">获取给定范围下方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="ed176-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed176-105">权限</span><span class="sxs-lookup"><span data-stu-id="ed176-105">Permissions</span></span>
<span data-ttu-id="ed176-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed176-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed176-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed176-108">Permission type</span></span>      | <span data-ttu-id="ed176-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed176-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed176-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed176-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ed176-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed176-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ed176-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed176-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed176-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed176-113">Not supported.</span></span>    |
|<span data-ttu-id="ed176-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed176-114">Application</span></span> | <span data-ttu-id="ed176-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed176-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed176-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed176-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ed176-117">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ed176-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="ed176-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="ed176-118">Function parameters</span></span>

| <span data-ttu-id="ed176-119">参数</span><span class="sxs-lookup"><span data-stu-id="ed176-119">Parameter</span></span>    | <span data-ttu-id="ed176-120">类型</span><span class="sxs-lookup"><span data-stu-id="ed176-120">Type</span></span>   |<span data-ttu-id="ed176-121">说明</span><span class="sxs-lookup"><span data-stu-id="ed176-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed176-122">count</span><span class="sxs-lookup"><span data-stu-id="ed176-122">count</span></span>|<span data-ttu-id="ed176-123">Int32</span><span class="sxs-lookup"><span data-stu-id="ed176-123">Int32</span></span>| <span data-ttu-id="ed176-p102">可选。生成的范围中要包含的行数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="ed176-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ed176-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed176-129">Request headers</span></span>
| <span data-ttu-id="ed176-130">名称</span><span class="sxs-lookup"><span data-stu-id="ed176-130">Name</span></span>       | <span data-ttu-id="ed176-131">说明</span><span class="sxs-lookup"><span data-stu-id="ed176-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ed176-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed176-132">Authorization</span></span>  | <span data-ttu-id="ed176-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed176-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed176-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ed176-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="ed176-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ed176-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed176-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed176-138">Request body</span></span>
<span data-ttu-id="ed176-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed176-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed176-140">响应</span><span class="sxs-lookup"><span data-stu-id="ed176-140">Response</span></span>
<span data-ttu-id="ed176-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ed176-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed176-142">示例</span><span class="sxs-lookup"><span data-stu-id="ed176-142">Example</span></span>
<span data-ttu-id="ed176-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ed176-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ed176-144">请求</span><span class="sxs-lookup"><span data-stu-id="ed176-144">Request</span></span>
<span data-ttu-id="ed176-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ed176-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ed176-146">C#</span><span class="sxs-lookup"><span data-stu-id="ed176-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed176-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="ed176-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ed176-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="ed176-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ed176-149">响应</span><span class="sxs-lookup"><span data-stu-id="ed176-149">Response</span></span>
<span data-ttu-id="ed176-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ed176-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ed176-153">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ed176-153">HTTP</span></span>](#tab/http)
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

<span data-ttu-id="ed176-154">如果不带`count`参数调用, 则此函数默认为一行。</span><span class="sxs-lookup"><span data-stu-id="ed176-154">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="ed176-155">请求</span><span class="sxs-lookup"><span data-stu-id="ed176-155">Request</span></span>
<span data-ttu-id="ed176-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ed176-156">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ed176-157">C#</span><span class="sxs-lookup"><span data-stu-id="ed176-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-nocount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed176-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="ed176-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-nocount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ed176-159">目标-C</span><span class="sxs-lookup"><span data-stu-id="ed176-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-nocount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ed176-160">响应</span><span class="sxs-lookup"><span data-stu-id="ed176-160">Response</span></span>
<span data-ttu-id="ed176-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ed176-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
