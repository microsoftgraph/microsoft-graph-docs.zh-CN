---
title: 更新工作表
description: 更新 worksheet 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a1b77656aef9bc4e0daeb90705d8394205fd4d4e
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575024"
---
# <a name="update-worksheet"></a><span data-ttu-id="1f6d8-103">更新工作表</span><span class="sxs-lookup"><span data-stu-id="1f6d8-103">Update worksheet</span></span>

<span data-ttu-id="1f6d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f6d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f6d8-105">更新 worksheet 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-105">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f6d8-106">权限</span><span class="sxs-lookup"><span data-stu-id="1f6d8-106">Permissions</span></span>
<span data-ttu-id="1f6d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f6d8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f6d8-109">Permission type</span></span>      | <span data-ttu-id="1f6d8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f6d8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f6d8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f6d8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f6d8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f6d8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f6d8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f6d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f6d8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-114">Not supported.</span></span>    |
|<span data-ttu-id="1f6d8-115">Application</span><span class="sxs-lookup"><span data-stu-id="1f6d8-115">Application</span></span> | <span data-ttu-id="1f6d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f6d8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f6d8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1f6d8-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="1f6d8-118">Optional request headers</span></span>
| <span data-ttu-id="1f6d8-119">名称</span><span class="sxs-lookup"><span data-stu-id="1f6d8-119">Name</span></span>       | <span data-ttu-id="1f6d8-120">说明</span><span class="sxs-lookup"><span data-stu-id="1f6d8-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1f6d8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f6d8-121">Authorization</span></span>  | <span data-ttu-id="1f6d8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f6d8-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1f6d8-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1f6d8-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f6d8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f6d8-127">Request body</span></span>
<span data-ttu-id="1f6d8-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1f6d8-131">属性</span><span class="sxs-lookup"><span data-stu-id="1f6d8-131">Property</span></span>     | <span data-ttu-id="1f6d8-132">类型</span><span class="sxs-lookup"><span data-stu-id="1f6d8-132">Type</span></span>   |<span data-ttu-id="1f6d8-133">说明</span><span class="sxs-lookup"><span data-stu-id="1f6d8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f6d8-134">name</span><span class="sxs-lookup"><span data-stu-id="1f6d8-134">name</span></span>|<span data-ttu-id="1f6d8-135">string</span><span class="sxs-lookup"><span data-stu-id="1f6d8-135">string</span></span>|<span data-ttu-id="1f6d8-136">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-136">The display name of the worksheet.</span></span>|
|<span data-ttu-id="1f6d8-137">position</span><span class="sxs-lookup"><span data-stu-id="1f6d8-137">position</span></span>|<span data-ttu-id="1f6d8-138">int</span><span class="sxs-lookup"><span data-stu-id="1f6d8-138">int</span></span>|<span data-ttu-id="1f6d8-139">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-139">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="1f6d8-140">visibility</span><span class="sxs-lookup"><span data-stu-id="1f6d8-140">visibility</span></span>|<span data-ttu-id="1f6d8-141">string</span><span class="sxs-lookup"><span data-stu-id="1f6d8-141">string</span></span>|<span data-ttu-id="1f6d8-142">工作表的可见性。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-142">The Visibility of the worksheet.</span></span> <span data-ttu-id="1f6d8-143">可能的值包括 `Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-143">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="1f6d8-144">响应</span><span class="sxs-lookup"><span data-stu-id="1f6d8-144">Response</span></span>

<span data-ttu-id="1f6d8-145">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [WorkbookWorksheet](../resources/worksheet.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-145">If successful, this method returns a `200 OK` response code and updated [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f6d8-146">示例</span><span class="sxs-lookup"><span data-stu-id="1f6d8-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f6d8-147">请求</span><span class="sxs-lookup"><span data-stu-id="1f6d8-147">Request</span></span>
<span data-ttu-id="1f6d8-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f6d8-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f6d8-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1f6d8-150">C#</span><span class="sxs-lookup"><span data-stu-id="1f6d8-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f6d8-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f6d8-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f6d8-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f6d8-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f6d8-153">Java</span><span class="sxs-lookup"><span data-stu-id="1f6d8-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1f6d8-154">响应</span><span class="sxs-lookup"><span data-stu-id="1f6d8-154">Response</span></span>
<span data-ttu-id="1f6d8-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f6d8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

