---
title: 更新工作表
description: 更新 worksheet 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 83c1e896209c59f43520448b03b293becbd2c775
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055615"
---
# <a name="update-worksheet"></a><span data-ttu-id="82813-103">更新工作表</span><span class="sxs-lookup"><span data-stu-id="82813-103">Update worksheet</span></span>

<span data-ttu-id="82813-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82813-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82813-105">更新 worksheet 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="82813-105">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="82813-106">权限</span><span class="sxs-lookup"><span data-stu-id="82813-106">Permissions</span></span>
<span data-ttu-id="82813-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82813-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82813-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="82813-109">Permission type</span></span>      | <span data-ttu-id="82813-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82813-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82813-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82813-111">Delegated (work or school account)</span></span> | <span data-ttu-id="82813-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82813-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="82813-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82813-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82813-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="82813-114">Not supported.</span></span>    |
|<span data-ttu-id="82813-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="82813-115">Application</span></span> | <span data-ttu-id="82813-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="82813-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82813-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82813-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="82813-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="82813-118">Optional request headers</span></span>
| <span data-ttu-id="82813-119">名称</span><span class="sxs-lookup"><span data-stu-id="82813-119">Name</span></span>       | <span data-ttu-id="82813-120">说明</span><span class="sxs-lookup"><span data-stu-id="82813-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="82813-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="82813-121">Authorization</span></span>  | <span data-ttu-id="82813-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82813-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82813-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="82813-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="82813-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="82813-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82813-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="82813-127">Request body</span></span>
<span data-ttu-id="82813-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="82813-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="82813-131">属性</span><span class="sxs-lookup"><span data-stu-id="82813-131">Property</span></span>     | <span data-ttu-id="82813-132">类型</span><span class="sxs-lookup"><span data-stu-id="82813-132">Type</span></span>   |<span data-ttu-id="82813-133">说明</span><span class="sxs-lookup"><span data-stu-id="82813-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82813-134">name</span><span class="sxs-lookup"><span data-stu-id="82813-134">name</span></span>|<span data-ttu-id="82813-135">string</span><span class="sxs-lookup"><span data-stu-id="82813-135">string</span></span>|<span data-ttu-id="82813-136">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="82813-136">The display name of the worksheet.</span></span>|
|<span data-ttu-id="82813-137">position</span><span class="sxs-lookup"><span data-stu-id="82813-137">position</span></span>|<span data-ttu-id="82813-138">int</span><span class="sxs-lookup"><span data-stu-id="82813-138">int</span></span>|<span data-ttu-id="82813-139">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="82813-139">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="82813-140">visibility</span><span class="sxs-lookup"><span data-stu-id="82813-140">visibility</span></span>|<span data-ttu-id="82813-141">string</span><span class="sxs-lookup"><span data-stu-id="82813-141">string</span></span>|<span data-ttu-id="82813-142">工作表的可见性。</span><span class="sxs-lookup"><span data-stu-id="82813-142">The Visibility of the worksheet.</span></span> <span data-ttu-id="82813-143">可能的值包括 `Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="82813-143">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="82813-144">响应</span><span class="sxs-lookup"><span data-stu-id="82813-144">Response</span></span>

<span data-ttu-id="82813-145">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [WorkbookWorksheet](../resources/worksheet.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="82813-145">If successful, this method returns a `200 OK` response code and updated [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82813-146">示例</span><span class="sxs-lookup"><span data-stu-id="82813-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82813-147">请求</span><span class="sxs-lookup"><span data-stu-id="82813-147">Request</span></span>
<span data-ttu-id="82813-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82813-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82813-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="82813-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
# <a name="c"></a>[<span data-ttu-id="82813-150">C#</span><span class="sxs-lookup"><span data-stu-id="82813-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82813-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82813-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82813-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82813-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82813-153">Java</span><span class="sxs-lookup"><span data-stu-id="82813-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82813-154">响应</span><span class="sxs-lookup"><span data-stu-id="82813-154">Response</span></span>
<span data-ttu-id="82813-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="82813-155">Here is an example of the response.</span></span> <span data-ttu-id="82813-156">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="82813-156">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

