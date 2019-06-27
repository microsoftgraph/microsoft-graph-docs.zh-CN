---
title: 更新 tablerow
description: 更新 tablerow 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cf03055177048b2389ee82ccc2c3dc7ac79045bc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270831"
---
# <a name="update-tablerow"></a><span data-ttu-id="e6c36-103">更新 tablerow</span><span class="sxs-lookup"><span data-stu-id="e6c36-103">Update tablerow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6c36-104">更新 tablerow 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e6c36-104">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6c36-105">权限</span><span class="sxs-lookup"><span data-stu-id="e6c36-105">Permissions</span></span>
<span data-ttu-id="e6c36-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6c36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6c36-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6c36-108">Permission type</span></span>      | <span data-ttu-id="e6c36-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6c36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6c36-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6c36-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e6c36-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6c36-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6c36-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6c36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6c36-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6c36-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6c36-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6c36-114">Application</span></span> | <span data-ttu-id="e6c36-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6c36-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6c36-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6c36-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows/{index}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e6c36-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="e6c36-117">Optional request headers</span></span>
| <span data-ttu-id="e6c36-118">名称</span><span class="sxs-lookup"><span data-stu-id="e6c36-118">Name</span></span>       | <span data-ttu-id="e6c36-119">说明</span><span class="sxs-lookup"><span data-stu-id="e6c36-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e6c36-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6c36-120">Authorization</span></span>  | <span data-ttu-id="e6c36-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6c36-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6c36-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e6c36-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e6c36-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e6c36-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6c36-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6c36-126">Request body</span></span>
<span data-ttu-id="e6c36-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e6c36-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e6c36-130">属性</span><span class="sxs-lookup"><span data-stu-id="e6c36-130">Property</span></span>     | <span data-ttu-id="e6c36-131">类型</span><span class="sxs-lookup"><span data-stu-id="e6c36-131">Type</span></span>   |<span data-ttu-id="e6c36-132">说明</span><span class="sxs-lookup"><span data-stu-id="e6c36-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6c36-133">values</span><span class="sxs-lookup"><span data-stu-id="e6c36-133">values</span></span>|<span data-ttu-id="e6c36-134">Json</span><span class="sxs-lookup"><span data-stu-id="e6c36-134">Json</span></span>|<span data-ttu-id="e6c36-p105">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="e6c36-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="e6c36-138">响应</span><span class="sxs-lookup"><span data-stu-id="e6c36-138">Response</span></span>

<span data-ttu-id="e6c36-139">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[workbookTableRow](../resources/workbooktablerow.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e6c36-139">If successful, this method returns a `200 OK` response code and updated [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6c36-140">示例</span><span class="sxs-lookup"><span data-stu-id="e6c36-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6c36-141">请求</span><span class="sxs-lookup"><span data-stu-id="e6c36-141">Request</span></span>
<span data-ttu-id="e6c36-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6c36-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="e6c36-143">响应</span><span class="sxs-lookup"><span data-stu-id="e6c36-143">Response</span></span>
<span data-ttu-id="e6c36-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6c36-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e6c36-147">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e6c36-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e6c36-148">C#</span><span class="sxs-lookup"><span data-stu-id="e6c36-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_tablerow-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6c36-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6c36-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_tablerow-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e6c36-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="e6c36-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_tablerow-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablerow-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tablerow-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablerow-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
