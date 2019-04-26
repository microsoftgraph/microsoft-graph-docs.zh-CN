---
title: Range:OffsetRange
description: 获取表示与指定区域偏移的区域的对象。返回的区域的尺寸将与该区域匹配。如果强制使生成的区域位于工作表网格的边界之外，则会引发异常。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 5cd6b8251c855e1dd3a059722f8719dae33dd2c9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331893"
---
# <a name="range-offsetrange"></a><span data-ttu-id="53caf-105">Range:OffsetRange</span><span class="sxs-lookup"><span data-stu-id="53caf-105">Range: OffsetRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53caf-p102">获取表示与指定区域偏移的区域的对象。返回的区域的尺寸将与该区域匹配。如果强制使生成的区域位于工作表网格的边界之外，则会引发异常。</span><span class="sxs-lookup"><span data-stu-id="53caf-p102">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="53caf-109">权限</span><span class="sxs-lookup"><span data-stu-id="53caf-109">Permissions</span></span>
<span data-ttu-id="53caf-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53caf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53caf-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="53caf-112">Permission type</span></span>      | <span data-ttu-id="53caf-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53caf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53caf-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53caf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="53caf-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53caf-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53caf-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53caf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53caf-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53caf-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53caf-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="53caf-118">Application</span></span> | <span data-ttu-id="53caf-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="53caf-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53caf-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53caf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="53caf-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="53caf-121">Request headers</span></span>
| <span data-ttu-id="53caf-122">名称</span><span class="sxs-lookup"><span data-stu-id="53caf-122">Name</span></span>       | <span data-ttu-id="53caf-123">说明</span><span class="sxs-lookup"><span data-stu-id="53caf-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53caf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="53caf-124">Authorization</span></span>  | <span data-ttu-id="53caf-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53caf-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53caf-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="53caf-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="53caf-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="53caf-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53caf-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="53caf-130">Request body</span></span>
<span data-ttu-id="53caf-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="53caf-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53caf-132">参数</span><span class="sxs-lookup"><span data-stu-id="53caf-132">Parameter</span></span>    | <span data-ttu-id="53caf-133">类型</span><span class="sxs-lookup"><span data-stu-id="53caf-133">Type</span></span>   |<span data-ttu-id="53caf-134">说明</span><span class="sxs-lookup"><span data-stu-id="53caf-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53caf-135">rowOffset</span><span class="sxs-lookup"><span data-stu-id="53caf-135">rowOffset</span></span>|<span data-ttu-id="53caf-136">数字</span><span class="sxs-lookup"><span data-stu-id="53caf-136">number</span></span>|<span data-ttu-id="53caf-p106">区域偏移的行数（正数、负数或 0）。正数表示向下偏移，负数表示向上偏移。</span><span class="sxs-lookup"><span data-stu-id="53caf-p106">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="53caf-139">columnOffset</span><span class="sxs-lookup"><span data-stu-id="53caf-139">columnOffset</span></span>|<span data-ttu-id="53caf-140">number</span><span class="sxs-lookup"><span data-stu-id="53caf-140">number</span></span>|<span data-ttu-id="53caf-p107">区域偏移的列数（正数、负数或 0）。正数表示向右偏移，负数表示向左偏移。</span><span class="sxs-lookup"><span data-stu-id="53caf-p107">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="53caf-143">响应</span><span class="sxs-lookup"><span data-stu-id="53caf-143">Response</span></span>

<span data-ttu-id="53caf-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53caf-144">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53caf-145">示例</span><span class="sxs-lookup"><span data-stu-id="53caf-145">Example</span></span>
<span data-ttu-id="53caf-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="53caf-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="53caf-147">请求</span><span class="sxs-lookup"><span data-stu-id="53caf-147">Request</span></span>
<span data-ttu-id="53caf-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53caf-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="53caf-149">响应</span><span class="sxs-lookup"><span data-stu-id="53caf-149">Response</span></span>
<span data-ttu-id="53caf-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53caf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
