---
title: Range:OffsetRange
description: 获取表示与指定区域偏移的区域的对象。返回的区域的尺寸将与该区域匹配。如果强制使生成的区域位于工作表网格的边界之外，则会引发异常。
ms.openlocfilehash: 301862e46a571754bcb4032c7c7bf87e3564268f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046207"
---
# <a name="range-offsetrange"></a><span data-ttu-id="60b4f-105">Range:OffsetRange</span><span class="sxs-lookup"><span data-stu-id="60b4f-105">Range: OffsetRange</span></span>

> <span data-ttu-id="60b4f-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="60b4f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60b4f-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="60b4f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60b4f-p103">获取表示与指定区域偏移的区域的对象。返回的区域的尺寸将与该区域匹配。如果强制使生成的区域位于工作表网格的边界之外，则会引发异常。</span><span class="sxs-lookup"><span data-stu-id="60b4f-p103">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="60b4f-111">权限</span><span class="sxs-lookup"><span data-stu-id="60b4f-111">Permissions</span></span>
<span data-ttu-id="60b4f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60b4f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b4f-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="60b4f-114">Permission type</span></span>      | <span data-ttu-id="60b4f-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60b4f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60b4f-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60b4f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="60b4f-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60b4f-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="60b4f-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60b4f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60b4f-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60b4f-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="60b4f-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="60b4f-120">Application</span></span> | <span data-ttu-id="60b4f-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="60b4f-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60b4f-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60b4f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="60b4f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="60b4f-123">Request headers</span></span>
| <span data-ttu-id="60b4f-124">名称</span><span class="sxs-lookup"><span data-stu-id="60b4f-124">Name</span></span>       | <span data-ttu-id="60b4f-125">说明</span><span class="sxs-lookup"><span data-stu-id="60b4f-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="60b4f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="60b4f-126">Authorization</span></span>  | <span data-ttu-id="60b4f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60b4f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60b4f-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="60b4f-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="60b4f-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="60b4f-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60b4f-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="60b4f-132">Request body</span></span>
<span data-ttu-id="60b4f-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="60b4f-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60b4f-134">参数</span><span class="sxs-lookup"><span data-stu-id="60b4f-134">Parameter</span></span>    | <span data-ttu-id="60b4f-135">类型</span><span class="sxs-lookup"><span data-stu-id="60b4f-135">Type</span></span>   |<span data-ttu-id="60b4f-136">说明</span><span class="sxs-lookup"><span data-stu-id="60b4f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60b4f-137">rowOffset</span><span class="sxs-lookup"><span data-stu-id="60b4f-137">rowOffset</span></span>|<span data-ttu-id="60b4f-138">number</span><span class="sxs-lookup"><span data-stu-id="60b4f-138">number</span></span>|<span data-ttu-id="60b4f-p107">区域偏移的行数（正数、负数或 0）。正数表示向下偏移，负数表示向上偏移。</span><span class="sxs-lookup"><span data-stu-id="60b4f-p107">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="60b4f-141">columnOffset</span><span class="sxs-lookup"><span data-stu-id="60b4f-141">columnOffset</span></span>|<span data-ttu-id="60b4f-142">number</span><span class="sxs-lookup"><span data-stu-id="60b4f-142">number</span></span>|<span data-ttu-id="60b4f-p108">区域偏移的列数（正数、负数或 0）。正数表示向右偏移，负数表示向左偏移。</span><span class="sxs-lookup"><span data-stu-id="60b4f-p108">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="60b4f-145">响应</span><span class="sxs-lookup"><span data-stu-id="60b4f-145">Response</span></span>

<span data-ttu-id="60b4f-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60b4f-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60b4f-147">示例</span><span class="sxs-lookup"><span data-stu-id="60b4f-147">Example</span></span>
<span data-ttu-id="60b4f-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="60b4f-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="60b4f-149">请求</span><span class="sxs-lookup"><span data-stu-id="60b4f-149">Request</span></span>
<span data-ttu-id="60b4f-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60b4f-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="60b4f-151">响应</span><span class="sxs-lookup"><span data-stu-id="60b4f-151">Response</span></span>
<span data-ttu-id="60b4f-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60b4f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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