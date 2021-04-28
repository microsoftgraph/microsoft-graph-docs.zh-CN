---
title: 更新 chartaxis
description: 更新 chartaxis 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0b6d30befd31d36ddaad25270126ef98f9d8402f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048832"
---
# <a name="update-chartaxis"></a><span data-ttu-id="7727f-103">更新 chartaxis</span><span class="sxs-lookup"><span data-stu-id="7727f-103">Update chartaxis</span></span>

<span data-ttu-id="7727f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7727f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7727f-105">更新 chartaxis 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7727f-105">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7727f-106">权限</span><span class="sxs-lookup"><span data-stu-id="7727f-106">Permissions</span></span>
<span data-ttu-id="7727f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7727f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7727f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7727f-109">Permission type</span></span>      | <span data-ttu-id="7727f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7727f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7727f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7727f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7727f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7727f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7727f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7727f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7727f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7727f-114">Not supported.</span></span>    |
|<span data-ttu-id="7727f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7727f-115">Application</span></span> | <span data-ttu-id="7727f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7727f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7727f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7727f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="7727f-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="7727f-118">Optional request headers</span></span>
| <span data-ttu-id="7727f-119">名称</span><span class="sxs-lookup"><span data-stu-id="7727f-119">Name</span></span>       | <span data-ttu-id="7727f-120">说明</span><span class="sxs-lookup"><span data-stu-id="7727f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7727f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7727f-121">Authorization</span></span>  | <span data-ttu-id="7727f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7727f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7727f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7727f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7727f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7727f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7727f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7727f-127">Request body</span></span>
<span data-ttu-id="7727f-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7727f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7727f-131">属性</span><span class="sxs-lookup"><span data-stu-id="7727f-131">Property</span></span>     | <span data-ttu-id="7727f-132">类型</span><span class="sxs-lookup"><span data-stu-id="7727f-132">Type</span></span>   |<span data-ttu-id="7727f-133">说明</span><span class="sxs-lookup"><span data-stu-id="7727f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7727f-134">majorUnit</span><span class="sxs-lookup"><span data-stu-id="7727f-134">majorUnit</span></span>|<span data-ttu-id="7727f-135">Json</span><span class="sxs-lookup"><span data-stu-id="7727f-135">Json</span></span>|<span data-ttu-id="7727f-p105">表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="7727f-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="7727f-139">maximum</span><span class="sxs-lookup"><span data-stu-id="7727f-139">maximum</span></span>|<span data-ttu-id="7727f-140">Json</span><span class="sxs-lookup"><span data-stu-id="7727f-140">Json</span></span>|<span data-ttu-id="7727f-p106">表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="7727f-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="7727f-144">minimum</span><span class="sxs-lookup"><span data-stu-id="7727f-144">minimum</span></span>|<span data-ttu-id="7727f-145">Json</span><span class="sxs-lookup"><span data-stu-id="7727f-145">Json</span></span>|<span data-ttu-id="7727f-p107">表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="7727f-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="7727f-149">minorUnit</span><span class="sxs-lookup"><span data-stu-id="7727f-149">minorUnit</span></span>|<span data-ttu-id="7727f-150">Json</span><span class="sxs-lookup"><span data-stu-id="7727f-150">Json</span></span>|<span data-ttu-id="7727f-p108">表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="7727f-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="7727f-154">响应</span><span class="sxs-lookup"><span data-stu-id="7727f-154">Response</span></span>

<span data-ttu-id="7727f-155">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [WorkbookChartAxis](../resources/chartaxis.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7727f-155">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7727f-156">示例</span><span class="sxs-lookup"><span data-stu-id="7727f-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7727f-157">请求</span><span class="sxs-lookup"><span data-stu-id="7727f-157">Request</span></span>
<span data-ttu-id="7727f-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7727f-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7727f-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="7727f-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
# <a name="c"></a>[<span data-ttu-id="7727f-160">C#</span><span class="sxs-lookup"><span data-stu-id="7727f-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxis-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7727f-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7727f-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxis-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7727f-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7727f-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxis-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7727f-163">Java</span><span class="sxs-lookup"><span data-stu-id="7727f-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxis-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7727f-164">响应</span><span class="sxs-lookup"><span data-stu-id="7727f-164">Response</span></span>
<span data-ttu-id="7727f-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7727f-165">Here is an example of the response.</span></span> <span data-ttu-id="7727f-166">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7727f-166">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

