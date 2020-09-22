---
title: Range:OffsetRange
description: 获取表示与指定区域偏移的区域的对象。返回的区域的尺寸将与该区域匹配。如果强制使生成的区域位于工作表网格的边界之外，则会引发异常。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1cf0cc130fdabc34b60530c64c5dd2968eee90b9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051542"
---
# <a name="range-offsetrange"></a><span data-ttu-id="c4878-105">Range:OffsetRange</span><span class="sxs-lookup"><span data-stu-id="c4878-105">Range: OffsetRange</span></span>

<span data-ttu-id="c4878-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4878-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4878-p102">获取表示与指定区域偏移的区域的对象。返回的区域的尺寸将与该区域匹配。如果强制使生成的区域位于工作表网格的边界之外，则会引发异常。</span><span class="sxs-lookup"><span data-stu-id="c4878-p102">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4878-110">权限</span><span class="sxs-lookup"><span data-stu-id="c4878-110">Permissions</span></span>
<span data-ttu-id="c4878-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4878-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4878-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4878-113">Permission type</span></span>      | <span data-ttu-id="c4878-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4878-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4878-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4878-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c4878-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4878-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4878-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4878-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4878-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4878-118">Not supported.</span></span>    |
|<span data-ttu-id="c4878-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4878-119">Application</span></span> | <span data-ttu-id="c4878-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4878-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4878-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4878-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/offsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/offsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/offsetRange

```
## <a name="request-headers"></a><span data-ttu-id="c4878-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4878-122">Request headers</span></span>
| <span data-ttu-id="c4878-123">名称</span><span class="sxs-lookup"><span data-stu-id="c4878-123">Name</span></span>       | <span data-ttu-id="c4878-124">说明</span><span class="sxs-lookup"><span data-stu-id="c4878-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4878-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4878-125">Authorization</span></span>  | <span data-ttu-id="c4878-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4878-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4878-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c4878-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="c4878-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c4878-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4878-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4878-131">Request body</span></span>
<span data-ttu-id="c4878-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c4878-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c4878-133">参数</span><span class="sxs-lookup"><span data-stu-id="c4878-133">Parameter</span></span>    | <span data-ttu-id="c4878-134">类型</span><span class="sxs-lookup"><span data-stu-id="c4878-134">Type</span></span>   |<span data-ttu-id="c4878-135">说明</span><span class="sxs-lookup"><span data-stu-id="c4878-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4878-136">rowOffset</span><span class="sxs-lookup"><span data-stu-id="c4878-136">rowOffset</span></span>|<span data-ttu-id="c4878-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c4878-137">Int32</span></span>|<span data-ttu-id="c4878-p106">区域偏移的行数（正数、负数或 0）。正数表示向下偏移，负数表示向上偏移。</span><span class="sxs-lookup"><span data-stu-id="c4878-p106">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="c4878-140">columnOffset</span><span class="sxs-lookup"><span data-stu-id="c4878-140">columnOffset</span></span>|<span data-ttu-id="c4878-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c4878-141">Int32</span></span>|<span data-ttu-id="c4878-p107">区域偏移的列数（正数、负数或 0）。正数表示向右偏移，负数表示向左偏移。</span><span class="sxs-lookup"><span data-stu-id="c4878-p107">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="c4878-144">响应</span><span class="sxs-lookup"><span data-stu-id="c4878-144">Response</span></span>

<span data-ttu-id="c4878-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c4878-145">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4878-146">示例</span><span class="sxs-lookup"><span data-stu-id="c4878-146">Example</span></span>
<span data-ttu-id="c4878-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c4878-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c4878-148">请求</span><span class="sxs-lookup"><span data-stu-id="c4878-148">Request</span></span>
<span data-ttu-id="c4878-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4878-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/offsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": 3,
  "columnOffset": 5
}
```

##### <a name="response"></a><span data-ttu-id="c4878-150">响应</span><span class="sxs-lookup"><span data-stu-id="c4878-150">Response</span></span>
<span data-ttu-id="c4878-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4878-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

