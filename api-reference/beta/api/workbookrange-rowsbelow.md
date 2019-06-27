---
title: 'workbookRange: rowsBelow'
description: 获取给定范围下方的一定数量的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 502397e35694401bbec3186cd7279963298afedd
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269382"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="2f469-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="2f469-103">workbookRange: rowsBelow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f469-104">获取给定范围下方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="2f469-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f469-105">权限</span><span class="sxs-lookup"><span data-stu-id="2f469-105">Permissions</span></span>
<span data-ttu-id="2f469-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f469-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f469-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f469-108">Permission type</span></span>      | <span data-ttu-id="2f469-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f469-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f469-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f469-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2f469-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f469-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2f469-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f469-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f469-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f469-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2f469-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f469-114">Application</span></span> | <span data-ttu-id="2f469-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f469-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f469-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f469-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="2f469-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="2f469-117">Function parameters</span></span>

| <span data-ttu-id="2f469-118">参数</span><span class="sxs-lookup"><span data-stu-id="2f469-118">Parameter</span></span>    | <span data-ttu-id="2f469-119">类型</span><span class="sxs-lookup"><span data-stu-id="2f469-119">Type</span></span>   |<span data-ttu-id="2f469-120">说明</span><span class="sxs-lookup"><span data-stu-id="2f469-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f469-121">count</span><span class="sxs-lookup"><span data-stu-id="2f469-121">count</span></span>|<span data-ttu-id="2f469-122">Int32</span><span class="sxs-lookup"><span data-stu-id="2f469-122">Int32</span></span>|<span data-ttu-id="2f469-p102">可选。生成的范围中要包含的行数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="2f469-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2f469-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f469-128">Request headers</span></span>
| <span data-ttu-id="2f469-129">名称</span><span class="sxs-lookup"><span data-stu-id="2f469-129">Name</span></span>       | <span data-ttu-id="2f469-130">说明</span><span class="sxs-lookup"><span data-stu-id="2f469-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2f469-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f469-131">Authorization</span></span>  | <span data-ttu-id="2f469-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f469-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f469-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2f469-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="2f469-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2f469-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f469-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f469-137">Request body</span></span>
<span data-ttu-id="2f469-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2f469-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f469-139">响应</span><span class="sxs-lookup"><span data-stu-id="2f469-139">Response</span></span>

<span data-ttu-id="2f469-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f469-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f469-141">示例</span><span class="sxs-lookup"><span data-stu-id="2f469-141">Example</span></span>
<span data-ttu-id="2f469-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2f469-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2f469-143">请求</span><span class="sxs-lookup"><span data-stu-id="2f469-143">Request</span></span>
<span data-ttu-id="2f469-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f469-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="2f469-145">响应</span><span class="sxs-lookup"><span data-stu-id="2f469-145">Response</span></span>
<span data-ttu-id="2f469-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f469-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2f469-149">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="2f469-149">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f469-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="2f469-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookrange_rowsBelow-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="2f469-151">C#</span><span class="sxs-lookup"><span data-stu-id="2f469-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_rowsBelow-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2f469-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="2f469-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookrange_rowsBelow-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/workbookrange-rowsbelow.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/workbookrange-rowsbelow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookrange-rowsbelow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
