---
title: 更新 charttitle
description: 更新 charttitle 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 58c9259ef5f118a4cac999e3b3f288fd6ab3e0f8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443159"
---
# <a name="update-charttitle"></a><span data-ttu-id="03175-103">更新 charttitle</span><span class="sxs-lookup"><span data-stu-id="03175-103">Update charttitle</span></span>

<span data-ttu-id="03175-104">更新 charttitle 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="03175-104">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="03175-105">权限</span><span class="sxs-lookup"><span data-stu-id="03175-105">Permissions</span></span>
<span data-ttu-id="03175-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03175-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03175-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="03175-108">Permission type</span></span>      | <span data-ttu-id="03175-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03175-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03175-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03175-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03175-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03175-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03175-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03175-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03175-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="03175-113">Not supported.</span></span>    |
|<span data-ttu-id="03175-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="03175-114">Application</span></span> | <span data-ttu-id="03175-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="03175-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03175-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03175-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="03175-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="03175-117">Optional request headers</span></span>
| <span data-ttu-id="03175-118">名称</span><span class="sxs-lookup"><span data-stu-id="03175-118">Name</span></span>       | <span data-ttu-id="03175-119">说明</span><span class="sxs-lookup"><span data-stu-id="03175-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="03175-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="03175-120">Authorization</span></span>  | <span data-ttu-id="03175-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03175-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03175-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="03175-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="03175-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="03175-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03175-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="03175-126">Request body</span></span>
<span data-ttu-id="03175-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="03175-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="03175-130">属性</span><span class="sxs-lookup"><span data-stu-id="03175-130">Property</span></span>     | <span data-ttu-id="03175-131">类型</span><span class="sxs-lookup"><span data-stu-id="03175-131">Type</span></span>   |<span data-ttu-id="03175-132">说明</span><span class="sxs-lookup"><span data-stu-id="03175-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03175-133">overlay</span><span class="sxs-lookup"><span data-stu-id="03175-133">overlay</span></span>|<span data-ttu-id="03175-134">布尔</span><span class="sxs-lookup"><span data-stu-id="03175-134">boolean</span></span>|<span data-ttu-id="03175-135">表示图表标题是否将叠加在图表上的布尔值。</span><span class="sxs-lookup"><span data-stu-id="03175-135">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="03175-136">text</span><span class="sxs-lookup"><span data-stu-id="03175-136">text</span></span>|<span data-ttu-id="03175-137">string</span><span class="sxs-lookup"><span data-stu-id="03175-137">string</span></span>|<span data-ttu-id="03175-138">表示图表的标题文本。</span><span class="sxs-lookup"><span data-stu-id="03175-138">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="03175-139">visible</span><span class="sxs-lookup"><span data-stu-id="03175-139">visible</span></span>|<span data-ttu-id="03175-140">布尔</span><span class="sxs-lookup"><span data-stu-id="03175-140">boolean</span></span>|<span data-ttu-id="03175-141">表示 chart title 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="03175-141">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="03175-142">响应</span><span class="sxs-lookup"><span data-stu-id="03175-142">Response</span></span>

<span data-ttu-id="03175-143">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[WorkbookChartTitle](../resources/charttitle.md)对象。</span><span class="sxs-lookup"><span data-stu-id="03175-143">If successful, this method returns a `200 OK` response code and updated [WorkbookChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03175-144">示例</span><span class="sxs-lookup"><span data-stu-id="03175-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03175-145">请求</span><span class="sxs-lookup"><span data-stu-id="03175-145">Request</span></span>
<span data-ttu-id="03175-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03175-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="03175-147">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="03175-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="03175-148">C#</span><span class="sxs-lookup"><span data-stu-id="03175-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-charttitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="03175-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="03175-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-charttitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="03175-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="03175-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-charttitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="03175-151">响应</span><span class="sxs-lookup"><span data-stu-id="03175-151">Response</span></span>
<span data-ttu-id="03175-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03175-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
