---
title: 更新工作表
description: 更新 worksheet 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 365ec4c2b3e13fa72c0925ff35c10bc1a85b6c45
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884226"
---
# <a name="update-worksheet"></a><span data-ttu-id="feb9b-103">更新工作表</span><span class="sxs-lookup"><span data-stu-id="feb9b-103">Update worksheet</span></span>

<span data-ttu-id="feb9b-104">更新 worksheet 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="feb9b-104">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="feb9b-105">权限</span><span class="sxs-lookup"><span data-stu-id="feb9b-105">Permissions</span></span>
<span data-ttu-id="feb9b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="feb9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="feb9b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="feb9b-108">Permission type</span></span>      | <span data-ttu-id="feb9b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="feb9b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="feb9b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="feb9b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="feb9b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="feb9b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="feb9b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="feb9b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="feb9b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="feb9b-113">Not supported.</span></span>    |
|<span data-ttu-id="feb9b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="feb9b-114">Application</span></span> | <span data-ttu-id="feb9b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="feb9b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="feb9b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="feb9b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="feb9b-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="feb9b-117">Optional request headers</span></span>
| <span data-ttu-id="feb9b-118">名称</span><span class="sxs-lookup"><span data-stu-id="feb9b-118">Name</span></span>       | <span data-ttu-id="feb9b-119">说明</span><span class="sxs-lookup"><span data-stu-id="feb9b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="feb9b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="feb9b-120">Authorization</span></span>  | <span data-ttu-id="feb9b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="feb9b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="feb9b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="feb9b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="feb9b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="feb9b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="feb9b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="feb9b-126">Request body</span></span>
<span data-ttu-id="feb9b-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="feb9b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="feb9b-130">属性</span><span class="sxs-lookup"><span data-stu-id="feb9b-130">Property</span></span>     | <span data-ttu-id="feb9b-131">类型</span><span class="sxs-lookup"><span data-stu-id="feb9b-131">Type</span></span>   |<span data-ttu-id="feb9b-132">说明</span><span class="sxs-lookup"><span data-stu-id="feb9b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="feb9b-133">name</span><span class="sxs-lookup"><span data-stu-id="feb9b-133">name</span></span>|<span data-ttu-id="feb9b-134">string</span><span class="sxs-lookup"><span data-stu-id="feb9b-134">string</span></span>|<span data-ttu-id="feb9b-135">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="feb9b-135">The display name of the worksheet.</span></span>|
|<span data-ttu-id="feb9b-136">position</span><span class="sxs-lookup"><span data-stu-id="feb9b-136">position</span></span>|<span data-ttu-id="feb9b-137">int</span><span class="sxs-lookup"><span data-stu-id="feb9b-137">int</span></span>|<span data-ttu-id="feb9b-138">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="feb9b-138">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="feb9b-139">visibility</span><span class="sxs-lookup"><span data-stu-id="feb9b-139">visibility</span></span>|<span data-ttu-id="feb9b-140">string</span><span class="sxs-lookup"><span data-stu-id="feb9b-140">string</span></span>|<span data-ttu-id="feb9b-141">工作表的可见性。</span><span class="sxs-lookup"><span data-stu-id="feb9b-141">The Visibility of the worksheet.</span></span> <span data-ttu-id="feb9b-142">可能的值包括 `Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="feb9b-142">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="feb9b-143">响应</span><span class="sxs-lookup"><span data-stu-id="feb9b-143">Response</span></span>

<span data-ttu-id="feb9b-144">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[WorkbookWorksheet](../resources/worksheet.md)对象。</span><span class="sxs-lookup"><span data-stu-id="feb9b-144">If successful, this method returns a `200 OK` response code and updated [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="feb9b-145">示例</span><span class="sxs-lookup"><span data-stu-id="feb9b-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="feb9b-146">请求</span><span class="sxs-lookup"><span data-stu-id="feb9b-146">Request</span></span>
<span data-ttu-id="feb9b-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="feb9b-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="feb9b-148">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="feb9b-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="feb9b-149">C#</span><span class="sxs-lookup"><span data-stu-id="feb9b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="feb9b-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="feb9b-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="feb9b-151">目标-C</span><span class="sxs-lookup"><span data-stu-id="feb9b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="feb9b-152">Java</span><span class="sxs-lookup"><span data-stu-id="feb9b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="feb9b-153">响应</span><span class="sxs-lookup"><span data-stu-id="feb9b-153">Response</span></span>
<span data-ttu-id="feb9b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="feb9b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
