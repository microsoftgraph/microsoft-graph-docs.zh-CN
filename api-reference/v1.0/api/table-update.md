---
title: 更新表
description: 更新 table 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2ad466de2ded72969ddfc2645ef17101d3947f78
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577154"
---
# <a name="update-table"></a><span data-ttu-id="293f2-103">更新表</span><span class="sxs-lookup"><span data-stu-id="293f2-103">Update table</span></span>

<span data-ttu-id="293f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="293f2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="293f2-105">更新 table 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="293f2-105">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="293f2-106">权限</span><span class="sxs-lookup"><span data-stu-id="293f2-106">Permissions</span></span>
<span data-ttu-id="293f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="293f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="293f2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="293f2-109">Permission type</span></span>      | <span data-ttu-id="293f2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="293f2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="293f2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="293f2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="293f2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="293f2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="293f2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="293f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="293f2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="293f2-114">Not supported.</span></span>    |
|<span data-ttu-id="293f2-115">Application</span><span class="sxs-lookup"><span data-stu-id="293f2-115">Application</span></span> | <span data-ttu-id="293f2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="293f2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="293f2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="293f2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="293f2-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="293f2-118">Optional request headers</span></span>
| <span data-ttu-id="293f2-119">名称</span><span class="sxs-lookup"><span data-stu-id="293f2-119">Name</span></span>       | <span data-ttu-id="293f2-120">说明</span><span class="sxs-lookup"><span data-stu-id="293f2-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="293f2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="293f2-121">Authorization</span></span>  | <span data-ttu-id="293f2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="293f2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="293f2-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="293f2-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="293f2-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="293f2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="293f2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="293f2-127">Request body</span></span>
<span data-ttu-id="293f2-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="293f2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="293f2-131">属性</span><span class="sxs-lookup"><span data-stu-id="293f2-131">Property</span></span>     | <span data-ttu-id="293f2-132">类型</span><span class="sxs-lookup"><span data-stu-id="293f2-132">Type</span></span>   |<span data-ttu-id="293f2-133">说明</span><span class="sxs-lookup"><span data-stu-id="293f2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="293f2-134">name</span><span class="sxs-lookup"><span data-stu-id="293f2-134">name</span></span>|<span data-ttu-id="293f2-135">string</span><span class="sxs-lookup"><span data-stu-id="293f2-135">string</span></span>|<span data-ttu-id="293f2-136">表的名称。</span><span class="sxs-lookup"><span data-stu-id="293f2-136">Name of the table.</span></span>|
|<span data-ttu-id="293f2-137">showHeaders</span><span class="sxs-lookup"><span data-stu-id="293f2-137">showHeaders</span></span>|<span data-ttu-id="293f2-138">boolean</span><span class="sxs-lookup"><span data-stu-id="293f2-138">boolean</span></span>|<span data-ttu-id="293f2-p105">指示标头行是否可见。该值可以设置为显示或删除标头行。</span><span class="sxs-lookup"><span data-stu-id="293f2-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="293f2-141">showTotals</span><span class="sxs-lookup"><span data-stu-id="293f2-141">showTotals</span></span>|<span data-ttu-id="293f2-142">boolean</span><span class="sxs-lookup"><span data-stu-id="293f2-142">boolean</span></span>|<span data-ttu-id="293f2-p106">指示总计行是否可见。该值可以设置为显示或删除总计行。</span><span class="sxs-lookup"><span data-stu-id="293f2-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="293f2-145">style</span><span class="sxs-lookup"><span data-stu-id="293f2-145">style</span></span>|<span data-ttu-id="293f2-146">string</span><span class="sxs-lookup"><span data-stu-id="293f2-146">string</span></span>|<span data-ttu-id="293f2-147">表示表格样式的常量值。</span><span class="sxs-lookup"><span data-stu-id="293f2-147">Constant value that represents the Table style.</span></span> <span data-ttu-id="293f2-148">可能的值包括 `TableStyleLight1` ：through `TableStyleLight21` `TableStyleMedium1` 、through  `TableStyleMedium28` `TableStyleDark1` 、through `TableStyleDark11` 。</span><span class="sxs-lookup"><span data-stu-id="293f2-148">The possible values are: `TableStyleLight1` through `TableStyleLight21`, `TableStyleMedium1` through  `TableStyleMedium28`, `TableStyleDark1` through `TableStyleDark11`.</span></span> <span data-ttu-id="293f2-149">还可以指定工作簿中显示的用户定义的自定义样式。</span><span class="sxs-lookup"><span data-stu-id="293f2-149">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="293f2-150">响应</span><span class="sxs-lookup"><span data-stu-id="293f2-150">Response</span></span>

<span data-ttu-id="293f2-151">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [WorkbookTable](../resources/table.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="293f2-151">If successful, this method returns a `200 OK` response code and updated [WorkbookTable](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="293f2-152">示例</span><span class="sxs-lookup"><span data-stu-id="293f2-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="293f2-153">请求</span><span class="sxs-lookup"><span data-stu-id="293f2-153">Request</span></span>
<span data-ttu-id="293f2-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="293f2-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="293f2-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="293f2-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
# <a name="c"></a>[<span data-ttu-id="293f2-156">C#</span><span class="sxs-lookup"><span data-stu-id="293f2-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="293f2-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="293f2-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="293f2-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="293f2-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="293f2-159">Java</span><span class="sxs-lookup"><span data-stu-id="293f2-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-table-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="293f2-160">响应</span><span class="sxs-lookup"><span data-stu-id="293f2-160">Response</span></span>
<span data-ttu-id="293f2-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="293f2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

