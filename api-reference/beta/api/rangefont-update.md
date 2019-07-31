---
title: 更新 rangefont
description: 更新 rangefont 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b26da12468f0f348b13e8ca53fe9fa92d6104398
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978248"
---
# <a name="update-rangefont"></a><span data-ttu-id="f2483-103">更新 rangefont</span><span class="sxs-lookup"><span data-stu-id="f2483-103">Update rangefont</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2483-104">更新 rangefont 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f2483-104">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2483-105">权限</span><span class="sxs-lookup"><span data-stu-id="f2483-105">Permissions</span></span>
<span data-ttu-id="f2483-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2483-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2483-108">Permission type</span></span>      | <span data-ttu-id="f2483-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2483-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2483-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2483-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f2483-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2483-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f2483-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2483-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2483-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2483-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f2483-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2483-114">Application</span></span> | <span data-ttu-id="f2483-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2483-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2483-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2483-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="f2483-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="f2483-117">Optional request headers</span></span>
| <span data-ttu-id="f2483-118">名称</span><span class="sxs-lookup"><span data-stu-id="f2483-118">Name</span></span>       | <span data-ttu-id="f2483-119">说明</span><span class="sxs-lookup"><span data-stu-id="f2483-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f2483-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2483-120">Authorization</span></span>  | <span data-ttu-id="f2483-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2483-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2483-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f2483-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f2483-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f2483-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2483-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2483-126">Request body</span></span>
<span data-ttu-id="f2483-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f2483-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f2483-130">属性</span><span class="sxs-lookup"><span data-stu-id="f2483-130">Property</span></span>     | <span data-ttu-id="f2483-131">类型</span><span class="sxs-lookup"><span data-stu-id="f2483-131">Type</span></span>   |<span data-ttu-id="f2483-132">说明</span><span class="sxs-lookup"><span data-stu-id="f2483-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2483-133">bold</span><span class="sxs-lookup"><span data-stu-id="f2483-133">bold</span></span>|<span data-ttu-id="f2483-134">boolean</span><span class="sxs-lookup"><span data-stu-id="f2483-134">boolean</span></span>|<span data-ttu-id="f2483-135">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="f2483-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="f2483-136">color</span><span class="sxs-lookup"><span data-stu-id="f2483-136">color</span></span>|<span data-ttu-id="f2483-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f2483-137">string</span></span>|<span data-ttu-id="f2483-p105">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="f2483-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="f2483-141">italic</span><span class="sxs-lookup"><span data-stu-id="f2483-141">italic</span></span>|<span data-ttu-id="f2483-142">布尔</span><span class="sxs-lookup"><span data-stu-id="f2483-142">boolean</span></span>|<span data-ttu-id="f2483-143">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="f2483-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="f2483-144">name</span><span class="sxs-lookup"><span data-stu-id="f2483-144">name</span></span>|<span data-ttu-id="f2483-145">string</span><span class="sxs-lookup"><span data-stu-id="f2483-145">string</span></span>|<span data-ttu-id="f2483-146">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="f2483-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="f2483-147">大小</span><span class="sxs-lookup"><span data-stu-id="f2483-147">size</span></span>|<span data-ttu-id="f2483-148">double</span><span class="sxs-lookup"><span data-stu-id="f2483-148">double</span></span>|<span data-ttu-id="f2483-149">字号</span><span class="sxs-lookup"><span data-stu-id="f2483-149">Font size.</span></span>|
|<span data-ttu-id="f2483-150">underline</span><span class="sxs-lookup"><span data-stu-id="f2483-150">underline</span></span>|<span data-ttu-id="f2483-151">string</span><span class="sxs-lookup"><span data-stu-id="f2483-151">string</span></span>|<span data-ttu-id="f2483-p106">应用于字体的下划线类型。可能的值是：`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="f2483-p106">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="f2483-154">响应</span><span class="sxs-lookup"><span data-stu-id="f2483-154">Response</span></span>

<span data-ttu-id="f2483-155">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[workbookRangeFont](../resources/workbookrangefont.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f2483-155">If successful, this method returns a `200 OK` response code and updated [workbookRangeFont](../resources/workbookrangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2483-156">示例</span><span class="sxs-lookup"><span data-stu-id="f2483-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2483-157">请求</span><span class="sxs-lookup"><span data-stu-id="f2483-157">Request</span></span>
<span data-ttu-id="f2483-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2483-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f2483-159">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f2483-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/font
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f2483-160">C#</span><span class="sxs-lookup"><span data-stu-id="f2483-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2483-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="f2483-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f2483-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="f2483-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f2483-163">Java</span><span class="sxs-lookup"><span data-stu-id="f2483-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangefont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f2483-164">响应</span><span class="sxs-lookup"><span data-stu-id="f2483-164">Response</span></span>
<span data-ttu-id="f2483-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2483-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
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
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
