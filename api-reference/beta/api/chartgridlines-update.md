---
title: 更新 chartgridlines
description: 更新 chartgridlines 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 366d49c57336652a6b34b149d3c04212b6ab1074
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418402"
---
# <a name="update-chartgridlines"></a><span data-ttu-id="50742-103">更新 chartgridlines</span><span class="sxs-lookup"><span data-stu-id="50742-103">Update chartgridlines</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50742-104">更新 chartgridlines 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="50742-104">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="50742-105">权限</span><span class="sxs-lookup"><span data-stu-id="50742-105">Permissions</span></span>
<span data-ttu-id="50742-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50742-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50742-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="50742-108">Permission type</span></span>      | <span data-ttu-id="50742-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50742-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50742-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50742-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50742-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50742-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="50742-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50742-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50742-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50742-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="50742-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="50742-114">Application</span></span> | <span data-ttu-id="50742-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="50742-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50742-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50742-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/majorgridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines
```
## <a name="optional-request-headers"></a><span data-ttu-id="50742-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="50742-117">Optional request headers</span></span>
| <span data-ttu-id="50742-118">名称</span><span class="sxs-lookup"><span data-stu-id="50742-118">Name</span></span>       | <span data-ttu-id="50742-119">说明</span><span class="sxs-lookup"><span data-stu-id="50742-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="50742-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="50742-120">Authorization</span></span>  | <span data-ttu-id="50742-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50742-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="50742-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="50742-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="50742-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="50742-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50742-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="50742-126">Request body</span></span>
<span data-ttu-id="50742-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="50742-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="50742-130">属性</span><span class="sxs-lookup"><span data-stu-id="50742-130">Property</span></span>     | <span data-ttu-id="50742-131">类型</span><span class="sxs-lookup"><span data-stu-id="50742-131">Type</span></span>   |<span data-ttu-id="50742-132">说明</span><span class="sxs-lookup"><span data-stu-id="50742-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50742-133">visible</span><span class="sxs-lookup"><span data-stu-id="50742-133">visible</span></span>|<span data-ttu-id="50742-134">布尔</span><span class="sxs-lookup"><span data-stu-id="50742-134">boolean</span></span>|<span data-ttu-id="50742-135">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="50742-135">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="50742-136">响应</span><span class="sxs-lookup"><span data-stu-id="50742-136">Response</span></span>

<span data-ttu-id="50742-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[workbookChartGridlines](../resources/workbookchartgridlines.md)对象。</span><span class="sxs-lookup"><span data-stu-id="50742-137">If successful, this method returns a `200 OK` response code and updated [workbookChartGridlines](../resources/workbookchartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="50742-138">示例</span><span class="sxs-lookup"><span data-stu-id="50742-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50742-139">请求</span><span class="sxs-lookup"><span data-stu-id="50742-139">Request</span></span>
<span data-ttu-id="50742-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50742-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="50742-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="50742-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="50742-142">C#</span><span class="sxs-lookup"><span data-stu-id="50742-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartgridlines-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50742-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50742-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartgridlines-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="50742-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="50742-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartgridlines-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="50742-145">响应</span><span class="sxs-lookup"><span data-stu-id="50742-145">Response</span></span>
<span data-ttu-id="50742-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50742-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
