---
title: 'workbookRange: rowsBelow'
description: 获取给定范围下方的一定数量的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2d7b88a62f65fe15434c431afc16e25d78e22be5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278454"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="75329-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="75329-103">workbookRange: rowsBelow</span></span>

<span data-ttu-id="75329-104">获取给定范围下方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="75329-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="75329-105">权限</span><span class="sxs-lookup"><span data-stu-id="75329-105">Permissions</span></span>
<span data-ttu-id="75329-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75329-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75329-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="75329-108">Permission type</span></span>      | <span data-ttu-id="75329-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75329-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75329-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75329-110">Delegated (work or school account)</span></span> | <span data-ttu-id="75329-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75329-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75329-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75329-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75329-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="75329-113">Not supported.</span></span>    |
|<span data-ttu-id="75329-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="75329-114">Application</span></span> | <span data-ttu-id="75329-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="75329-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75329-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75329-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="75329-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="75329-117">Function parameters</span></span>

| <span data-ttu-id="75329-118">参数</span><span class="sxs-lookup"><span data-stu-id="75329-118">Parameter</span></span>    | <span data-ttu-id="75329-119">类型</span><span class="sxs-lookup"><span data-stu-id="75329-119">Type</span></span>   |<span data-ttu-id="75329-120">说明</span><span class="sxs-lookup"><span data-stu-id="75329-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75329-121">count</span><span class="sxs-lookup"><span data-stu-id="75329-121">count</span></span>|<span data-ttu-id="75329-122">Int32</span><span class="sxs-lookup"><span data-stu-id="75329-122">Int32</span></span>| <span data-ttu-id="75329-p102">可选。生成的范围中要包含的行数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="75329-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="75329-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="75329-128">Request headers</span></span>
| <span data-ttu-id="75329-129">名称</span><span class="sxs-lookup"><span data-stu-id="75329-129">Name</span></span>       | <span data-ttu-id="75329-130">说明</span><span class="sxs-lookup"><span data-stu-id="75329-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75329-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="75329-131">Authorization</span></span>  | <span data-ttu-id="75329-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75329-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75329-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="75329-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="75329-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="75329-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75329-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="75329-137">Request body</span></span>
<span data-ttu-id="75329-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="75329-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75329-139">响应</span><span class="sxs-lookup"><span data-stu-id="75329-139">Response</span></span>
<span data-ttu-id="75329-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75329-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75329-141">示例</span><span class="sxs-lookup"><span data-stu-id="75329-141">Example</span></span>
<span data-ttu-id="75329-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="75329-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="75329-143">请求</span><span class="sxs-lookup"><span data-stu-id="75329-143">Request</span></span>
<span data-ttu-id="75329-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75329-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="75329-145">响应</span><span class="sxs-lookup"><span data-stu-id="75329-145">Response</span></span>
<span data-ttu-id="75329-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75329-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="75329-149">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="75329-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="75329-150">C#</span><span class="sxs-lookup"><span data-stu-id="75329-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_rowsBelow-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75329-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="75329-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookrange_rowsBelow-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="75329-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="75329-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookrange_rowsBelow-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="75329-153">如果不带`count`参数调用, 则此函数默认为一行。</span><span class="sxs-lookup"><span data-stu-id="75329-153">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="75329-154">请求</span><span class="sxs-lookup"><span data-stu-id="75329-154">Request</span></span>
<span data-ttu-id="75329-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75329-155">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```

##### <a name="response"></a><span data-ttu-id="75329-156">响应</span><span class="sxs-lookup"><span data-stu-id="75329-156">Response</span></span>
<span data-ttu-id="75329-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75329-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="75329-160">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="75329-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="75329-161">C#</span><span class="sxs-lookup"><span data-stu-id="75329-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_rowsBelow_nocount-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75329-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="75329-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookrange_rowsBelow_nocount-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="75329-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="75329-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookrange_rowsBelow_nocount-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbookrange-rowsbelow.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/workbookrange-rowsbelow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbookrange-rowsbelow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/workbookrange-rowsbelow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbookrange-rowsbelow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
