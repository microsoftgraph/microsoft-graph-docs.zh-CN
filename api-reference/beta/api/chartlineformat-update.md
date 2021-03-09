---
title: 更新 chartlineformat
description: 更新 chartlineformat 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f959390fc226dd0b85152585e3c848b002fcd290
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574464"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="7b44a-103">更新 chartlineformat</span><span class="sxs-lookup"><span data-stu-id="7b44a-103">Update chartlineformat</span></span>

<span data-ttu-id="7b44a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b44a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b44a-105">更新 chartlineformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7b44a-105">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7b44a-106">权限</span><span class="sxs-lookup"><span data-stu-id="7b44a-106">Permissions</span></span>
<span data-ttu-id="7b44a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b44a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b44a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b44a-109">Permission type</span></span>      | <span data-ttu-id="7b44a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b44a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b44a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b44a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b44a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b44a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7b44a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b44a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b44a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b44a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7b44a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b44a-115">Application</span></span> | <span data-ttu-id="7b44a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b44a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b44a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b44a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines/format/line
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="7b44a-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="7b44a-118">Optional request headers</span></span>
| <span data-ttu-id="7b44a-119">名称</span><span class="sxs-lookup"><span data-stu-id="7b44a-119">Name</span></span>       | <span data-ttu-id="7b44a-120">说明</span><span class="sxs-lookup"><span data-stu-id="7b44a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7b44a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b44a-121">Authorization</span></span>  | <span data-ttu-id="7b44a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b44a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b44a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7b44a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7b44a-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7b44a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b44a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b44a-127">Request body</span></span>
<span data-ttu-id="7b44a-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7b44a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7b44a-131">属性</span><span class="sxs-lookup"><span data-stu-id="7b44a-131">Property</span></span>     | <span data-ttu-id="7b44a-132">类型</span><span class="sxs-lookup"><span data-stu-id="7b44a-132">Type</span></span>   |<span data-ttu-id="7b44a-133">说明</span><span class="sxs-lookup"><span data-stu-id="7b44a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b44a-134">color</span><span class="sxs-lookup"><span data-stu-id="7b44a-134">color</span></span>|<span data-ttu-id="7b44a-135">string</span><span class="sxs-lookup"><span data-stu-id="7b44a-135">string</span></span>|<span data-ttu-id="7b44a-136">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="7b44a-136">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="7b44a-137">响应</span><span class="sxs-lookup"><span data-stu-id="7b44a-137">Response</span></span>

<span data-ttu-id="7b44a-138">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [workbookChartLineFormat](../resources/workbookchartlineformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b44a-138">If successful, this method returns a `200 OK` response code and updated [workbookChartLineFormat](../resources/workbookchartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7b44a-139">示例</span><span class="sxs-lookup"><span data-stu-id="7b44a-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b44a-140">请求</span><span class="sxs-lookup"><span data-stu-id="7b44a-140">Request</span></span>
<span data-ttu-id="7b44a-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b44a-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7b44a-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b44a-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="c"></a>[<span data-ttu-id="7b44a-143">C#</span><span class="sxs-lookup"><span data-stu-id="7b44a-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlineformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b44a-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b44a-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlineformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b44a-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b44a-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlineformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b44a-146">Java</span><span class="sxs-lookup"><span data-stu-id="7b44a-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartlineformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7b44a-147">响应</span><span class="sxs-lookup"><span data-stu-id="7b44a-147">Response</span></span>
<span data-ttu-id="7b44a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7b44a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


