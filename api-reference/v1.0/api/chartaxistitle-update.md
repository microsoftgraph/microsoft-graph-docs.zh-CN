---
title: 更新 chartaxistitle
description: 更新 chartaxistitle 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 07503fd8a90aecdf07737ddf0cf2c11438777a51
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048825"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="11d5e-103">更新 chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="11d5e-103">Update chartaxistitle</span></span>

<span data-ttu-id="11d5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11d5e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11d5e-105">更新 chartaxistitle 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="11d5e-105">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="11d5e-106">权限</span><span class="sxs-lookup"><span data-stu-id="11d5e-106">Permissions</span></span>
<span data-ttu-id="11d5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11d5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11d5e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="11d5e-109">Permission type</span></span>      | <span data-ttu-id="11d5e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11d5e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11d5e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11d5e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11d5e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11d5e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="11d5e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11d5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11d5e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="11d5e-114">Not supported.</span></span>    |
|<span data-ttu-id="11d5e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="11d5e-115">Application</span></span> | <span data-ttu-id="11d5e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="11d5e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11d5e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11d5e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="11d5e-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="11d5e-118">Optional request headers</span></span>
| <span data-ttu-id="11d5e-119">名称</span><span class="sxs-lookup"><span data-stu-id="11d5e-119">Name</span></span>       | <span data-ttu-id="11d5e-120">说明</span><span class="sxs-lookup"><span data-stu-id="11d5e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="11d5e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="11d5e-121">Authorization</span></span>  | <span data-ttu-id="11d5e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="11d5e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11d5e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="11d5e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="11d5e-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="11d5e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11d5e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="11d5e-127">Request body</span></span>
<span data-ttu-id="11d5e-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="11d5e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="11d5e-131">属性</span><span class="sxs-lookup"><span data-stu-id="11d5e-131">Property</span></span>     | <span data-ttu-id="11d5e-132">类型</span><span class="sxs-lookup"><span data-stu-id="11d5e-132">Type</span></span>   |<span data-ttu-id="11d5e-133">说明</span><span class="sxs-lookup"><span data-stu-id="11d5e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11d5e-134">text</span><span class="sxs-lookup"><span data-stu-id="11d5e-134">text</span></span>|<span data-ttu-id="11d5e-135">string</span><span class="sxs-lookup"><span data-stu-id="11d5e-135">string</span></span>|<span data-ttu-id="11d5e-136">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="11d5e-136">Represents the axis title.</span></span>|
|<span data-ttu-id="11d5e-137">visible</span><span class="sxs-lookup"><span data-stu-id="11d5e-137">visible</span></span>|<span data-ttu-id="11d5e-138">布尔</span><span class="sxs-lookup"><span data-stu-id="11d5e-138">boolean</span></span>|<span data-ttu-id="11d5e-139">指定坐标轴标题可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="11d5e-139">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="11d5e-140">响应</span><span class="sxs-lookup"><span data-stu-id="11d5e-140">Response</span></span>

<span data-ttu-id="11d5e-141">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [WorkbookChartAxisTitle](../resources/chartaxistitle.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="11d5e-141">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="11d5e-142">示例</span><span class="sxs-lookup"><span data-stu-id="11d5e-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11d5e-143">请求</span><span class="sxs-lookup"><span data-stu-id="11d5e-143">Request</span></span>
<span data-ttu-id="11d5e-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="11d5e-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11d5e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="11d5e-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="11d5e-146">C#</span><span class="sxs-lookup"><span data-stu-id="11d5e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxistitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11d5e-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11d5e-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxistitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11d5e-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11d5e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxistitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11d5e-149">Java</span><span class="sxs-lookup"><span data-stu-id="11d5e-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxistitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="11d5e-150">响应</span><span class="sxs-lookup"><span data-stu-id="11d5e-150">Response</span></span>
<span data-ttu-id="11d5e-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="11d5e-151">Here is an example of the response.</span></span> <span data-ttu-id="11d5e-152">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="11d5e-152">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

