---
title: 更新 tablerow
description: 更新 tablerow 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4f720830c2ce0f2a7139a08c1cdc53180ec252cb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052668"
---
# <a name="update-tablerow"></a><span data-ttu-id="68e33-103">更新 tablerow</span><span class="sxs-lookup"><span data-stu-id="68e33-103">Update tablerow</span></span>

<span data-ttu-id="68e33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68e33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68e33-105">更新 tablerow 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="68e33-105">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="68e33-106">权限</span><span class="sxs-lookup"><span data-stu-id="68e33-106">Permissions</span></span>
<span data-ttu-id="68e33-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68e33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68e33-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="68e33-109">Permission type</span></span>      | <span data-ttu-id="68e33-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68e33-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68e33-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68e33-111">Delegated (work or school account)</span></span> | <span data-ttu-id="68e33-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68e33-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="68e33-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68e33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68e33-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68e33-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="68e33-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="68e33-115">Application</span></span> | <span data-ttu-id="68e33-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="68e33-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="68e33-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68e33-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/{index}
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-request-headers"></a><span data-ttu-id="68e33-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="68e33-118">Optional request headers</span></span>
| <span data-ttu-id="68e33-119">名称</span><span class="sxs-lookup"><span data-stu-id="68e33-119">Name</span></span>       | <span data-ttu-id="68e33-120">说明</span><span class="sxs-lookup"><span data-stu-id="68e33-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="68e33-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="68e33-121">Authorization</span></span>  | <span data-ttu-id="68e33-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68e33-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="68e33-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="68e33-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="68e33-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="68e33-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68e33-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="68e33-127">Request body</span></span>
<span data-ttu-id="68e33-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="68e33-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="68e33-131">属性</span><span class="sxs-lookup"><span data-stu-id="68e33-131">Property</span></span>     | <span data-ttu-id="68e33-132">类型</span><span class="sxs-lookup"><span data-stu-id="68e33-132">Type</span></span>   |<span data-ttu-id="68e33-133">说明</span><span class="sxs-lookup"><span data-stu-id="68e33-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68e33-134">值</span><span class="sxs-lookup"><span data-stu-id="68e33-134">values</span></span>|<span data-ttu-id="68e33-135">Json</span><span class="sxs-lookup"><span data-stu-id="68e33-135">Json</span></span>|<span data-ttu-id="68e33-p105">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="68e33-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="68e33-139">响应</span><span class="sxs-lookup"><span data-stu-id="68e33-139">Response</span></span>

<span data-ttu-id="68e33-140">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [workbookTableRow](../resources/workbooktablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68e33-140">If successful, this method returns a `200 OK` response code and updated [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="68e33-141">示例</span><span class="sxs-lookup"><span data-stu-id="68e33-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68e33-142">请求</span><span class="sxs-lookup"><span data-stu-id="68e33-142">Request</span></span>
<span data-ttu-id="68e33-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="68e33-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="68e33-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="68e33-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="68e33-145">C#</span><span class="sxs-lookup"><span data-stu-id="68e33-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tablerow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68e33-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68e33-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tablerow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68e33-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68e33-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tablerow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68e33-148">Java</span><span class="sxs-lookup"><span data-stu-id="68e33-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tablerow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="68e33-149">响应</span><span class="sxs-lookup"><span data-stu-id="68e33-149">Response</span></span>
<span data-ttu-id="68e33-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="68e33-150">Here is an example of the response.</span></span> <span data-ttu-id="68e33-151">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="68e33-151">Note: The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->


