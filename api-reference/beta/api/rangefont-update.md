---
title: 更新 rangefont
description: 更新 rangefont 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d5b178d461b80bcdf5d074754fd727a4e24c5fb6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976206"
---
# <a name="update-rangefont"></a><span data-ttu-id="94d6c-103">更新 rangefont</span><span class="sxs-lookup"><span data-stu-id="94d6c-103">Update rangefont</span></span>

<span data-ttu-id="94d6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94d6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94d6c-105">更新 rangefont 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94d6c-105">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94d6c-106">权限</span><span class="sxs-lookup"><span data-stu-id="94d6c-106">Permissions</span></span>
<span data-ttu-id="94d6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94d6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94d6c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="94d6c-109">Permission type</span></span>      | <span data-ttu-id="94d6c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94d6c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94d6c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94d6c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94d6c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94d6c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94d6c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94d6c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94d6c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94d6c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94d6c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="94d6c-115">Application</span></span> | <span data-ttu-id="94d6c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="94d6c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94d6c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94d6c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="94d6c-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="94d6c-118">Optional request headers</span></span>
| <span data-ttu-id="94d6c-119">名称</span><span class="sxs-lookup"><span data-stu-id="94d6c-119">Name</span></span>       | <span data-ttu-id="94d6c-120">说明</span><span class="sxs-lookup"><span data-stu-id="94d6c-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="94d6c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94d6c-121">Authorization</span></span>  | <span data-ttu-id="94d6c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94d6c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94d6c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="94d6c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="94d6c-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="94d6c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94d6c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="94d6c-127">Request body</span></span>
<span data-ttu-id="94d6c-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="94d6c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94d6c-131">属性</span><span class="sxs-lookup"><span data-stu-id="94d6c-131">Property</span></span>     | <span data-ttu-id="94d6c-132">类型</span><span class="sxs-lookup"><span data-stu-id="94d6c-132">Type</span></span>   |<span data-ttu-id="94d6c-133">说明</span><span class="sxs-lookup"><span data-stu-id="94d6c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94d6c-134">bold</span><span class="sxs-lookup"><span data-stu-id="94d6c-134">bold</span></span>|<span data-ttu-id="94d6c-135">布尔</span><span class="sxs-lookup"><span data-stu-id="94d6c-135">boolean</span></span>|<span data-ttu-id="94d6c-136">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="94d6c-136">Represents the bold status of font.</span></span>|
|<span data-ttu-id="94d6c-137">color</span><span class="sxs-lookup"><span data-stu-id="94d6c-137">color</span></span>|<span data-ttu-id="94d6c-138">string</span><span class="sxs-lookup"><span data-stu-id="94d6c-138">string</span></span>|<span data-ttu-id="94d6c-p105">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="94d6c-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="94d6c-142">italic</span><span class="sxs-lookup"><span data-stu-id="94d6c-142">italic</span></span>|<span data-ttu-id="94d6c-143">布尔</span><span class="sxs-lookup"><span data-stu-id="94d6c-143">boolean</span></span>|<span data-ttu-id="94d6c-144">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="94d6c-144">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="94d6c-145">name</span><span class="sxs-lookup"><span data-stu-id="94d6c-145">name</span></span>|<span data-ttu-id="94d6c-146">string</span><span class="sxs-lookup"><span data-stu-id="94d6c-146">string</span></span>|<span data-ttu-id="94d6c-147">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="94d6c-147">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="94d6c-148">大小</span><span class="sxs-lookup"><span data-stu-id="94d6c-148">size</span></span>|<span data-ttu-id="94d6c-149">double</span><span class="sxs-lookup"><span data-stu-id="94d6c-149">double</span></span>|<span data-ttu-id="94d6c-150">字号</span><span class="sxs-lookup"><span data-stu-id="94d6c-150">Font size.</span></span>|
|<span data-ttu-id="94d6c-151">underline</span><span class="sxs-lookup"><span data-stu-id="94d6c-151">underline</span></span>|<span data-ttu-id="94d6c-152">string</span><span class="sxs-lookup"><span data-stu-id="94d6c-152">string</span></span>|<span data-ttu-id="94d6c-p106">应用于字体的下划线类型。可能的值是：`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="94d6c-p106">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="94d6c-155">响应</span><span class="sxs-lookup"><span data-stu-id="94d6c-155">Response</span></span>

<span data-ttu-id="94d6c-156">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [workbookRangeFont](../resources/workbookrangefont.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94d6c-156">If successful, this method returns a `200 OK` response code and updated [workbookRangeFont](../resources/workbookrangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94d6c-157">示例</span><span class="sxs-lookup"><span data-stu-id="94d6c-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94d6c-158">请求</span><span class="sxs-lookup"><span data-stu-id="94d6c-158">Request</span></span>
<span data-ttu-id="94d6c-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94d6c-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94d6c-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="94d6c-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="94d6c-161">C#</span><span class="sxs-lookup"><span data-stu-id="94d6c-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94d6c-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94d6c-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94d6c-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94d6c-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94d6c-164">Java</span><span class="sxs-lookup"><span data-stu-id="94d6c-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangefont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="94d6c-165">响应</span><span class="sxs-lookup"><span data-stu-id="94d6c-165">Response</span></span>
<span data-ttu-id="94d6c-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94d6c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


