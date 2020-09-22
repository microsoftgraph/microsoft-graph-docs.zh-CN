---
title: 更新 rangefont
description: 更新 rangefont 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 635d1e7304fa1296dd1f1af9c348c11db4b65725
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034285"
---
# <a name="update-rangefont"></a><span data-ttu-id="9b185-103">更新 rangefont</span><span class="sxs-lookup"><span data-stu-id="9b185-103">Update rangefont</span></span>

<span data-ttu-id="9b185-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b185-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b185-105">更新 rangefont 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9b185-105">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9b185-106">权限</span><span class="sxs-lookup"><span data-stu-id="9b185-106">Permissions</span></span>
<span data-ttu-id="9b185-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b185-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b185-109">Permission type</span></span>      | <span data-ttu-id="9b185-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b185-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b185-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b185-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9b185-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b185-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9b185-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b185-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b185-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b185-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9b185-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b185-115">Application</span></span> | <span data-ttu-id="9b185-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b185-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b185-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b185-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="9b185-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="9b185-118">Optional request headers</span></span>
| <span data-ttu-id="9b185-119">名称</span><span class="sxs-lookup"><span data-stu-id="9b185-119">Name</span></span>       | <span data-ttu-id="9b185-120">说明</span><span class="sxs-lookup"><span data-stu-id="9b185-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9b185-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b185-121">Authorization</span></span>  | <span data-ttu-id="9b185-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b185-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b185-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9b185-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9b185-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9b185-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b185-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b185-127">Request body</span></span>
<span data-ttu-id="9b185-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9b185-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9b185-131">属性</span><span class="sxs-lookup"><span data-stu-id="9b185-131">Property</span></span>     | <span data-ttu-id="9b185-132">类型</span><span class="sxs-lookup"><span data-stu-id="9b185-132">Type</span></span>   |<span data-ttu-id="9b185-133">说明</span><span class="sxs-lookup"><span data-stu-id="9b185-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b185-134">bold</span><span class="sxs-lookup"><span data-stu-id="9b185-134">bold</span></span>|<span data-ttu-id="9b185-135">布尔</span><span class="sxs-lookup"><span data-stu-id="9b185-135">boolean</span></span>|<span data-ttu-id="9b185-136">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="9b185-136">Represents the bold status of font.</span></span>|
|<span data-ttu-id="9b185-137">color</span><span class="sxs-lookup"><span data-stu-id="9b185-137">color</span></span>|<span data-ttu-id="9b185-138">string</span><span class="sxs-lookup"><span data-stu-id="9b185-138">string</span></span>|<span data-ttu-id="9b185-p105">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="9b185-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="9b185-142">italic</span><span class="sxs-lookup"><span data-stu-id="9b185-142">italic</span></span>|<span data-ttu-id="9b185-143">布尔</span><span class="sxs-lookup"><span data-stu-id="9b185-143">boolean</span></span>|<span data-ttu-id="9b185-144">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="9b185-144">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="9b185-145">name</span><span class="sxs-lookup"><span data-stu-id="9b185-145">name</span></span>|<span data-ttu-id="9b185-146">string</span><span class="sxs-lookup"><span data-stu-id="9b185-146">string</span></span>|<span data-ttu-id="9b185-147">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="9b185-147">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="9b185-148">大小</span><span class="sxs-lookup"><span data-stu-id="9b185-148">size</span></span>|<span data-ttu-id="9b185-149">double</span><span class="sxs-lookup"><span data-stu-id="9b185-149">double</span></span>|<span data-ttu-id="9b185-150">字号</span><span class="sxs-lookup"><span data-stu-id="9b185-150">Font size.</span></span>|
|<span data-ttu-id="9b185-151">underline</span><span class="sxs-lookup"><span data-stu-id="9b185-151">underline</span></span>|<span data-ttu-id="9b185-152">string</span><span class="sxs-lookup"><span data-stu-id="9b185-152">string</span></span>|<span data-ttu-id="9b185-p106">应用于字体的下划线类型。可能的值是：`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="9b185-p106">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="9b185-155">响应</span><span class="sxs-lookup"><span data-stu-id="9b185-155">Response</span></span>

<span data-ttu-id="9b185-156">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [workbookRangeFont](../resources/workbookrangefont.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b185-156">If successful, this method returns a `200 OK` response code and updated [workbookRangeFont](../resources/workbookrangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9b185-157">示例</span><span class="sxs-lookup"><span data-stu-id="9b185-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b185-158">请求</span><span class="sxs-lookup"><span data-stu-id="9b185-158">Request</span></span>
<span data-ttu-id="9b185-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b185-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b185-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b185-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9b185-161">C#</span><span class="sxs-lookup"><span data-stu-id="9b185-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b185-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b185-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b185-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b185-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9b185-164">响应</span><span class="sxs-lookup"><span data-stu-id="9b185-164">Response</span></span>
<span data-ttu-id="9b185-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9b185-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


