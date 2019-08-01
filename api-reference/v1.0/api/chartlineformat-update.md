---
title: 更新 chartlineformat
description: 更新 chartlineformat 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2f8730bf44280519df844be38f21eb4d672c21e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003425"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="b9954-103">更新 chartlineformat</span><span class="sxs-lookup"><span data-stu-id="b9954-103">Update chartlineformat</span></span>

<span data-ttu-id="b9954-104">更新 chartlineformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b9954-104">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9954-105">权限</span><span class="sxs-lookup"><span data-stu-id="b9954-105">Permissions</span></span>
<span data-ttu-id="b9954-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9954-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9954-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9954-108">Permission type</span></span>      | <span data-ttu-id="b9954-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9954-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9954-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9954-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b9954-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9954-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9954-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9954-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9954-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9954-113">Not supported.</span></span>    |
|<span data-ttu-id="b9954-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9954-114">Application</span></span> | <span data-ttu-id="b9954-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9954-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9954-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9954-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="b9954-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b9954-117">Optional request headers</span></span>
| <span data-ttu-id="b9954-118">名称</span><span class="sxs-lookup"><span data-stu-id="b9954-118">Name</span></span>       | <span data-ttu-id="b9954-119">说明</span><span class="sxs-lookup"><span data-stu-id="b9954-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b9954-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9954-120">Authorization</span></span>  | <span data-ttu-id="b9954-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9954-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9954-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b9954-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b9954-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="b9954-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9954-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9954-126">Request body</span></span>
<span data-ttu-id="b9954-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b9954-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b9954-130">属性</span><span class="sxs-lookup"><span data-stu-id="b9954-130">Property</span></span>     | <span data-ttu-id="b9954-131">类型</span><span class="sxs-lookup"><span data-stu-id="b9954-131">Type</span></span>   |<span data-ttu-id="b9954-132">说明</span><span class="sxs-lookup"><span data-stu-id="b9954-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9954-133">color</span><span class="sxs-lookup"><span data-stu-id="b9954-133">color</span></span>|<span data-ttu-id="b9954-134">string</span><span class="sxs-lookup"><span data-stu-id="b9954-134">string</span></span>|<span data-ttu-id="b9954-135">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="b9954-135">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="b9954-136">响应</span><span class="sxs-lookup"><span data-stu-id="b9954-136">Response</span></span>

<span data-ttu-id="b9954-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[WorkbookChartLineFormat](../resources/chartlineformat.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b9954-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9954-138">示例</span><span class="sxs-lookup"><span data-stu-id="b9954-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9954-139">请求</span><span class="sxs-lookup"><span data-stu-id="b9954-139">Request</span></span>
<span data-ttu-id="b9954-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9954-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b9954-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b9954-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b9954-142">C#</span><span class="sxs-lookup"><span data-stu-id="b9954-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlineformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9954-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="b9954-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlineformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b9954-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="b9954-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlineformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b9954-145">Java</span><span class="sxs-lookup"><span data-stu-id="b9954-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartlineformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b9954-146">响应</span><span class="sxs-lookup"><span data-stu-id="b9954-146">Response</span></span>
<span data-ttu-id="b9954-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9954-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
