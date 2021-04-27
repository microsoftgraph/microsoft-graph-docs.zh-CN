---
title: 更新 workbookChartFont
description: 更新 workbookChartFont 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d7d4d43687594f8759606246109e2dfb668fd780
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047425"
---
# <a name="update-chartfont"></a><span data-ttu-id="38050-103">更新 chartfont</span><span class="sxs-lookup"><span data-stu-id="38050-103">Update chartfont</span></span>

<span data-ttu-id="38050-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38050-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38050-105">更新 chartfont 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="38050-105">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="38050-106">权限</span><span class="sxs-lookup"><span data-stu-id="38050-106">Permissions</span></span>
<span data-ttu-id="38050-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38050-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="38050-109">Permission type</span></span>      | <span data-ttu-id="38050-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38050-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38050-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38050-111">Delegated (work or school account)</span></span> | <span data-ttu-id="38050-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38050-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="38050-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38050-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38050-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38050-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="38050-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="38050-115">Application</span></span> | <span data-ttu-id="38050-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="38050-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38050-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38050-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/font
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="38050-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="38050-118">Optional request headers</span></span>
| <span data-ttu-id="38050-119">名称</span><span class="sxs-lookup"><span data-stu-id="38050-119">Name</span></span>       | <span data-ttu-id="38050-120">说明</span><span class="sxs-lookup"><span data-stu-id="38050-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="38050-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="38050-121">Authorization</span></span>  | <span data-ttu-id="38050-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38050-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38050-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="38050-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="38050-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="38050-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38050-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="38050-127">Request body</span></span>
<span data-ttu-id="38050-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="38050-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="38050-131">属性</span><span class="sxs-lookup"><span data-stu-id="38050-131">Property</span></span>     | <span data-ttu-id="38050-132">类型</span><span class="sxs-lookup"><span data-stu-id="38050-132">Type</span></span>   |<span data-ttu-id="38050-133">说明</span><span class="sxs-lookup"><span data-stu-id="38050-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38050-134">bold</span><span class="sxs-lookup"><span data-stu-id="38050-134">bold</span></span>|<span data-ttu-id="38050-135">布尔</span><span class="sxs-lookup"><span data-stu-id="38050-135">boolean</span></span>|<span data-ttu-id="38050-136">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="38050-136">Represents the bold status of font.</span></span>|
|<span data-ttu-id="38050-137">color</span><span class="sxs-lookup"><span data-stu-id="38050-137">color</span></span>|<span data-ttu-id="38050-138">string</span><span class="sxs-lookup"><span data-stu-id="38050-138">string</span></span>|<span data-ttu-id="38050-p105">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="38050-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="38050-142">italic</span><span class="sxs-lookup"><span data-stu-id="38050-142">italic</span></span>|<span data-ttu-id="38050-143">布尔</span><span class="sxs-lookup"><span data-stu-id="38050-143">boolean</span></span>|<span data-ttu-id="38050-144">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="38050-144">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="38050-145">name</span><span class="sxs-lookup"><span data-stu-id="38050-145">name</span></span>|<span data-ttu-id="38050-146">string</span><span class="sxs-lookup"><span data-stu-id="38050-146">string</span></span>|<span data-ttu-id="38050-147">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="38050-147">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="38050-148">大小</span><span class="sxs-lookup"><span data-stu-id="38050-148">size</span></span>|<span data-ttu-id="38050-149">double</span><span class="sxs-lookup"><span data-stu-id="38050-149">double</span></span>|<span data-ttu-id="38050-150">字体大小（例如 11）</span><span class="sxs-lookup"><span data-stu-id="38050-150">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="38050-151">underline</span><span class="sxs-lookup"><span data-stu-id="38050-151">underline</span></span>|<span data-ttu-id="38050-152">string</span><span class="sxs-lookup"><span data-stu-id="38050-152">string</span></span>|<span data-ttu-id="38050-p106">应用于字体的下划线类型。可能的值是：`None`、`Single`。</span><span class="sxs-lookup"><span data-stu-id="38050-p106">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="38050-155">响应</span><span class="sxs-lookup"><span data-stu-id="38050-155">Response</span></span>

<span data-ttu-id="38050-156">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [workbookChartFont](../resources/workbookchartfont.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38050-156">If successful, this method returns a `200 OK` response code and updated [workbookChartFont](../resources/workbookchartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38050-157">示例</span><span class="sxs-lookup"><span data-stu-id="38050-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38050-158">请求</span><span class="sxs-lookup"><span data-stu-id="38050-158">Request</span></span>
<span data-ttu-id="38050-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38050-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38050-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="38050-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
# <a name="c"></a>[<span data-ttu-id="38050-161">C#</span><span class="sxs-lookup"><span data-stu-id="38050-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartfont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38050-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38050-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartfont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38050-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38050-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartfont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38050-164">Java</span><span class="sxs-lookup"><span data-stu-id="38050-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartfont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="38050-165">响应</span><span class="sxs-lookup"><span data-stu-id="38050-165">Response</span></span>
<span data-ttu-id="38050-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="38050-166">Here is an example of the response.</span></span> <span data-ttu-id="38050-167">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="38050-167">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


