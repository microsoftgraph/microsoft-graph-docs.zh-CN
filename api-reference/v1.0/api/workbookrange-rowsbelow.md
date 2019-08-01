---
title: 'workbookRange: rowsBelow'
description: 获取给定范围下方的一定数量的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ff336468f8a5dae7e157cd9355a5733bdcd44500
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026332"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="1b49e-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="1b49e-103">workbookRange: rowsBelow</span></span>

<span data-ttu-id="1b49e-104">获取给定范围下方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="1b49e-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b49e-105">权限</span><span class="sxs-lookup"><span data-stu-id="1b49e-105">Permissions</span></span>
<span data-ttu-id="1b49e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b49e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b49e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b49e-108">Permission type</span></span>      | <span data-ttu-id="1b49e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b49e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b49e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b49e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1b49e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b49e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1b49e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b49e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b49e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b49e-113">Not supported.</span></span>    |
|<span data-ttu-id="1b49e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b49e-114">Application</span></span> | <span data-ttu-id="1b49e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b49e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b49e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b49e-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1b49e-117">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1b49e-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="1b49e-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="1b49e-118">Function parameters</span></span>

| <span data-ttu-id="1b49e-119">参数</span><span class="sxs-lookup"><span data-stu-id="1b49e-119">Parameter</span></span>    | <span data-ttu-id="1b49e-120">类型</span><span class="sxs-lookup"><span data-stu-id="1b49e-120">Type</span></span>   |<span data-ttu-id="1b49e-121">说明</span><span class="sxs-lookup"><span data-stu-id="1b49e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b49e-122">count</span><span class="sxs-lookup"><span data-stu-id="1b49e-122">count</span></span>|<span data-ttu-id="1b49e-123">Int32</span><span class="sxs-lookup"><span data-stu-id="1b49e-123">Int32</span></span>| <span data-ttu-id="1b49e-p102">可选。生成的范围中要包含的行数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="1b49e-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="1b49e-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b49e-129">Request headers</span></span>
| <span data-ttu-id="1b49e-130">名称</span><span class="sxs-lookup"><span data-stu-id="1b49e-130">Name</span></span>       | <span data-ttu-id="1b49e-131">说明</span><span class="sxs-lookup"><span data-stu-id="1b49e-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1b49e-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b49e-132">Authorization</span></span>  | <span data-ttu-id="1b49e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b49e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b49e-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1b49e-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="1b49e-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1b49e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b49e-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b49e-138">Request body</span></span>
<span data-ttu-id="1b49e-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1b49e-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b49e-140">响应</span><span class="sxs-lookup"><span data-stu-id="1b49e-140">Response</span></span>
<span data-ttu-id="1b49e-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1b49e-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b49e-142">示例</span><span class="sxs-lookup"><span data-stu-id="1b49e-142">Example</span></span>
<span data-ttu-id="1b49e-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1b49e-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1b49e-144">请求</span><span class="sxs-lookup"><span data-stu-id="1b49e-144">Request</span></span>
<span data-ttu-id="1b49e-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b49e-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b49e-146">C#</span><span class="sxs-lookup"><span data-stu-id="1b49e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b49e-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="1b49e-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b49e-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="1b49e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1b49e-149">Java</span><span class="sxs-lookup"><span data-stu-id="1b49e-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsbelow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1b49e-150">响应</span><span class="sxs-lookup"><span data-stu-id="1b49e-150">Response</span></span>
<span data-ttu-id="1b49e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b49e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1b49e-154">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1b49e-154">HTTP</span></span>](#tab/http)
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

<span data-ttu-id="1b49e-155">如果不带`count`参数调用, 则此函数默认为一行。</span><span class="sxs-lookup"><span data-stu-id="1b49e-155">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="1b49e-156">请求</span><span class="sxs-lookup"><span data-stu-id="1b49e-156">Request</span></span>
<span data-ttu-id="1b49e-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b49e-157">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b49e-158">C#</span><span class="sxs-lookup"><span data-stu-id="1b49e-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-nocount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b49e-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="1b49e-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-nocount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b49e-160">目标-C</span><span class="sxs-lookup"><span data-stu-id="1b49e-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-nocount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1b49e-161">Java</span><span class="sxs-lookup"><span data-stu-id="1b49e-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsbelow-nocount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1b49e-162">响应</span><span class="sxs-lookup"><span data-stu-id="1b49e-162">Response</span></span>
<span data-ttu-id="1b49e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b49e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
