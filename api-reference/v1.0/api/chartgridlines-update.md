---
title: 更新 chartgridlines
description: 更新 chartgridlines 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 66f79f31228c9bedc05221d893bf35e158619fcd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054565"
---
# <a name="update-chartgridlines"></a><span data-ttu-id="470e2-103">更新 chartgridlines</span><span class="sxs-lookup"><span data-stu-id="470e2-103">Update chartgridlines</span></span>

<span data-ttu-id="470e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="470e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="470e2-105">更新 chartgridlines 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="470e2-105">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="470e2-106">权限</span><span class="sxs-lookup"><span data-stu-id="470e2-106">Permissions</span></span>
<span data-ttu-id="470e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="470e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="470e2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="470e2-109">Permission type</span></span>      | <span data-ttu-id="470e2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="470e2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="470e2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="470e2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="470e2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="470e2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="470e2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="470e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="470e2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="470e2-114">Not supported.</span></span>    |
|<span data-ttu-id="470e2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="470e2-115">Application</span></span> | <span data-ttu-id="470e2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="470e2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="470e2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="470e2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/majorGridlines
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/majorGridlines
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorGridlines
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorGridlines
```
## <a name="request-headers"></a><span data-ttu-id="470e2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="470e2-118">Request headers</span></span>
| <span data-ttu-id="470e2-119">名称</span><span class="sxs-lookup"><span data-stu-id="470e2-119">Name</span></span>       | <span data-ttu-id="470e2-120">说明</span><span class="sxs-lookup"><span data-stu-id="470e2-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="470e2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="470e2-121">Authorization</span></span>  | <span data-ttu-id="470e2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="470e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="470e2-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="470e2-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="470e2-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="470e2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="470e2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="470e2-127">Request body</span></span>
<span data-ttu-id="470e2-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="470e2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="470e2-131">属性</span><span class="sxs-lookup"><span data-stu-id="470e2-131">Property</span></span>     | <span data-ttu-id="470e2-132">类型</span><span class="sxs-lookup"><span data-stu-id="470e2-132">Type</span></span>   |<span data-ttu-id="470e2-133">说明</span><span class="sxs-lookup"><span data-stu-id="470e2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="470e2-134">visible</span><span class="sxs-lookup"><span data-stu-id="470e2-134">visible</span></span>|<span data-ttu-id="470e2-135">布尔</span><span class="sxs-lookup"><span data-stu-id="470e2-135">boolean</span></span>|<span data-ttu-id="470e2-136">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="470e2-136">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="470e2-137">响应</span><span class="sxs-lookup"><span data-stu-id="470e2-137">Response</span></span>

<span data-ttu-id="470e2-138">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [WorkbookChartGridlines](../resources/chartgridlines.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="470e2-138">If successful, this method returns a `200 OK` response code and updated [WorkbookChartGridlines](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="470e2-139">示例</span><span class="sxs-lookup"><span data-stu-id="470e2-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="470e2-140">请求</span><span class="sxs-lookup"><span data-stu-id="470e2-140">Request</span></span>
<span data-ttu-id="470e2-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="470e2-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="470e2-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="470e2-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="470e2-143">C#</span><span class="sxs-lookup"><span data-stu-id="470e2-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartgridlines-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="470e2-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="470e2-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartgridlines-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="470e2-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="470e2-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartgridlines-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="470e2-146">Java</span><span class="sxs-lookup"><span data-stu-id="470e2-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartgridlines-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="470e2-147">响应</span><span class="sxs-lookup"><span data-stu-id="470e2-147">Response</span></span>
<span data-ttu-id="470e2-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="470e2-148">Here is an example of the response.</span></span> <span data-ttu-id="470e2-149">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="470e2-149">Note: The response object shown here might be shortened for readability.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

