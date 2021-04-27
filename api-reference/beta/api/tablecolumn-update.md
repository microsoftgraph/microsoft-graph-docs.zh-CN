---
title: 更新 tablecolumn
description: 更新 tablecolumn 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bcbadc0b6ef767780c5eb9f255ac939dce47dd35
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051835"
---
# <a name="update-tablecolumn"></a><span data-ttu-id="b0356-103">更新 tablecolumn</span><span class="sxs-lookup"><span data-stu-id="b0356-103">Update tablecolumn</span></span>

<span data-ttu-id="b0356-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0356-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0356-105">更新 tablecolumn 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b0356-105">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0356-106">权限</span><span class="sxs-lookup"><span data-stu-id="b0356-106">Permissions</span></span>
<span data-ttu-id="b0356-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0356-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0356-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0356-109">Permission type</span></span>      | <span data-ttu-id="b0356-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0356-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0356-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0356-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0356-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0356-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0356-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0356-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0356-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0356-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0356-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0356-115">Application</span></span> | <span data-ttu-id="b0356-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0356-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0356-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0356-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b0356-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b0356-118">Optional request headers</span></span>
| <span data-ttu-id="b0356-119">名称</span><span class="sxs-lookup"><span data-stu-id="b0356-119">Name</span></span>       | <span data-ttu-id="b0356-120">说明</span><span class="sxs-lookup"><span data-stu-id="b0356-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b0356-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0356-121">Authorization</span></span>  | <span data-ttu-id="b0356-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0356-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0356-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b0356-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b0356-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="b0356-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0356-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0356-127">Request body</span></span>
<span data-ttu-id="b0356-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b0356-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b0356-131">属性</span><span class="sxs-lookup"><span data-stu-id="b0356-131">Property</span></span>     | <span data-ttu-id="b0356-132">类型</span><span class="sxs-lookup"><span data-stu-id="b0356-132">Type</span></span>   |<span data-ttu-id="b0356-133">说明</span><span class="sxs-lookup"><span data-stu-id="b0356-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0356-134">值</span><span class="sxs-lookup"><span data-stu-id="b0356-134">values</span></span>|<span data-ttu-id="b0356-135">Json</span><span class="sxs-lookup"><span data-stu-id="b0356-135">Json</span></span>|<span data-ttu-id="b0356-p105">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="b0356-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="b0356-139">响应</span><span class="sxs-lookup"><span data-stu-id="b0356-139">Response</span></span>

<span data-ttu-id="b0356-140">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [workbookTableColumn](../resources/workbooktablecolumn.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b0356-140">If successful, this method returns a `200 OK` response code and updated [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0356-141">示例</span><span class="sxs-lookup"><span data-stu-id="b0356-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0356-142">请求</span><span class="sxs-lookup"><span data-stu-id="b0356-142">Request</span></span>
<span data-ttu-id="b0356-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0356-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0356-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0356-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
# <a name="c"></a>[<span data-ttu-id="b0356-145">C#</span><span class="sxs-lookup"><span data-stu-id="b0356-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tablecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0356-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0356-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tablecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0356-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0356-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tablecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0356-148">Java</span><span class="sxs-lookup"><span data-stu-id="b0356-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tablecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

> [!NOTE]
> <span data-ttu-id="b0356-149">如果要更新列的多个字段，请使 **值** 成为请求中的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="b0356-149">If you want to update multiple fields of a column, make **values** a string array in the request.</span></span> <span data-ttu-id="b0356-150">例如：`"values": [["a"], [1], [2], [3]]`。</span><span class="sxs-lookup"><span data-stu-id="b0356-150">For example: `"values": [["a"], [1], [2], [3]]`.</span></span>

##### <a name="response"></a><span data-ttu-id="b0356-151">响应</span><span class="sxs-lookup"><span data-stu-id="b0356-151">Response</span></span>
<span data-ttu-id="b0356-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b0356-152">Here is an example of the response.</span></span> <span data-ttu-id="b0356-153">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b0356-153">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": "99",
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


