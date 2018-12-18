---
title: 更新 chartgridlines
description: 更新 chartgridlines 对象的属性。
author: lumine2008
ms.openlocfilehash: db55f639cbe95f80929467b0feefd260a64fc596
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346457"
---
# <a name="update-chartgridlines"></a><span data-ttu-id="c0fb4-103">更新 chartgridlines</span><span class="sxs-lookup"><span data-stu-id="c0fb4-103">Update chartgridlines</span></span>

<span data-ttu-id="c0fb4-104">更新 chartgridlines 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-104">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0fb4-105">权限</span><span class="sxs-lookup"><span data-stu-id="c0fb4-105">Permissions</span></span>
<span data-ttu-id="c0fb4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0fb4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0fb4-108">Permission type</span></span>      | <span data-ttu-id="c0fb4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0fb4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0fb4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0fb4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0fb4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0fb4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0fb4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0fb4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0fb4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-113">Not supported.</span></span>    |
|<span data-ttu-id="c0fb4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0fb4-114">Application</span></span> | <span data-ttu-id="c0fb4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0fb4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0fb4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/majorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorGridlines
```
## <a name="request-headers"></a><span data-ttu-id="c0fb4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0fb4-117">Request headers</span></span>
| <span data-ttu-id="c0fb4-118">Name</span><span class="sxs-lookup"><span data-stu-id="c0fb4-118">Name</span></span>       | <span data-ttu-id="c0fb4-119">说明</span><span class="sxs-lookup"><span data-stu-id="c0fb4-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c0fb4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0fb4-120">Authorization</span></span>  | <span data-ttu-id="c0fb4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0fb4-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c0fb4-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c0fb4-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0fb4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0fb4-126">Request body</span></span>
<span data-ttu-id="c0fb4-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c0fb4-130">属性</span><span class="sxs-lookup"><span data-stu-id="c0fb4-130">Property</span></span>     | <span data-ttu-id="c0fb4-131">类型</span><span class="sxs-lookup"><span data-stu-id="c0fb4-131">Type</span></span>   |<span data-ttu-id="c0fb4-132">说明</span><span class="sxs-lookup"><span data-stu-id="c0fb4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0fb4-133">visible</span><span class="sxs-lookup"><span data-stu-id="c0fb4-133">visible</span></span>|<span data-ttu-id="c0fb4-134">boolean</span><span class="sxs-lookup"><span data-stu-id="c0fb4-134">boolean</span></span>|<span data-ttu-id="c0fb4-135">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-135">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="c0fb4-136">响应</span><span class="sxs-lookup"><span data-stu-id="c0fb4-136">Response</span></span>

<span data-ttu-id="c0fb4-137">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[WorkbookChartGridlines](../resources/chartgridlines.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartGridlines](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0fb4-138">示例</span><span class="sxs-lookup"><span data-stu-id="c0fb4-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0fb4-139">请求</span><span class="sxs-lookup"><span data-stu-id="c0fb4-139">Request</span></span>
<span data-ttu-id="c0fb4-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="c0fb4-141">响应</span><span class="sxs-lookup"><span data-stu-id="c0fb4-141">Response</span></span>
<span data-ttu-id="c0fb4-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->