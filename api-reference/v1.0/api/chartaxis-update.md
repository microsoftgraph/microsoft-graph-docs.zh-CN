---
title: 更新 chartaxis
description: 更新 chartaxis 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8dd30fc559ab8e4fe7bed4067d7e234c0406baea
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578519"
---
# <a name="update-chartaxis"></a><span data-ttu-id="5ba78-103">更新 chartaxis</span><span class="sxs-lookup"><span data-stu-id="5ba78-103">Update chartaxis</span></span>

<span data-ttu-id="5ba78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ba78-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ba78-105">更新 chartaxis 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5ba78-105">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ba78-106">权限</span><span class="sxs-lookup"><span data-stu-id="5ba78-106">Permissions</span></span>
<span data-ttu-id="5ba78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ba78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ba78-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ba78-109">Permission type</span></span>      | <span data-ttu-id="5ba78-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ba78-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ba78-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ba78-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ba78-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ba78-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ba78-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ba78-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ba78-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ba78-114">Not supported.</span></span>    |
|<span data-ttu-id="5ba78-115">Application</span><span class="sxs-lookup"><span data-stu-id="5ba78-115">Application</span></span> | <span data-ttu-id="5ba78-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ba78-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ba78-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ba78-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="5ba78-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="5ba78-118">Optional request headers</span></span>
| <span data-ttu-id="5ba78-119">名称</span><span class="sxs-lookup"><span data-stu-id="5ba78-119">Name</span></span>       | <span data-ttu-id="5ba78-120">说明</span><span class="sxs-lookup"><span data-stu-id="5ba78-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5ba78-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ba78-121">Authorization</span></span>  | <span data-ttu-id="5ba78-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ba78-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ba78-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5ba78-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5ba78-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5ba78-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ba78-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ba78-127">Request body</span></span>
<span data-ttu-id="5ba78-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5ba78-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5ba78-131">属性</span><span class="sxs-lookup"><span data-stu-id="5ba78-131">Property</span></span>     | <span data-ttu-id="5ba78-132">类型</span><span class="sxs-lookup"><span data-stu-id="5ba78-132">Type</span></span>   |<span data-ttu-id="5ba78-133">说明</span><span class="sxs-lookup"><span data-stu-id="5ba78-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ba78-134">majorUnit</span><span class="sxs-lookup"><span data-stu-id="5ba78-134">majorUnit</span></span>|<span data-ttu-id="5ba78-135">Json</span><span class="sxs-lookup"><span data-stu-id="5ba78-135">Json</span></span>|<span data-ttu-id="5ba78-p105">表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="5ba78-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="5ba78-139">maximum</span><span class="sxs-lookup"><span data-stu-id="5ba78-139">maximum</span></span>|<span data-ttu-id="5ba78-140">Json</span><span class="sxs-lookup"><span data-stu-id="5ba78-140">Json</span></span>|<span data-ttu-id="5ba78-p106">表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="5ba78-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="5ba78-144">minimum</span><span class="sxs-lookup"><span data-stu-id="5ba78-144">minimum</span></span>|<span data-ttu-id="5ba78-145">Json</span><span class="sxs-lookup"><span data-stu-id="5ba78-145">Json</span></span>|<span data-ttu-id="5ba78-p107">表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="5ba78-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="5ba78-149">minorUnit</span><span class="sxs-lookup"><span data-stu-id="5ba78-149">minorUnit</span></span>|<span data-ttu-id="5ba78-150">Json</span><span class="sxs-lookup"><span data-stu-id="5ba78-150">Json</span></span>|<span data-ttu-id="5ba78-p108">表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="5ba78-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="5ba78-154">响应</span><span class="sxs-lookup"><span data-stu-id="5ba78-154">Response</span></span>

<span data-ttu-id="5ba78-155">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [WorkbookChartAxis](../resources/chartaxis.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5ba78-155">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ba78-156">示例</span><span class="sxs-lookup"><span data-stu-id="5ba78-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ba78-157">请求</span><span class="sxs-lookup"><span data-stu-id="5ba78-157">Request</span></span>
<span data-ttu-id="5ba78-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ba78-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ba78-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ba78-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ba78-160">C#</span><span class="sxs-lookup"><span data-stu-id="5ba78-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxis-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ba78-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ba78-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxis-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ba78-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ba78-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxis-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ba78-163">Java</span><span class="sxs-lookup"><span data-stu-id="5ba78-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxis-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ba78-164">响应</span><span class="sxs-lookup"><span data-stu-id="5ba78-164">Response</span></span>
<span data-ttu-id="5ba78-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5ba78-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

