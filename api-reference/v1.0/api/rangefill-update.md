---
title: 更新 rangefill
description: 更新 rangefill 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5184a13a8f5faebad37ca59841ec68c5d45a3907
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787603"
---
# <a name="update-rangefill"></a><span data-ttu-id="472cb-103">更新 rangefill</span><span class="sxs-lookup"><span data-stu-id="472cb-103">Update rangefill</span></span>

<span data-ttu-id="472cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="472cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="472cb-105">更新 rangefill 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="472cb-105">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="472cb-106">权限</span><span class="sxs-lookup"><span data-stu-id="472cb-106">Permissions</span></span>
<span data-ttu-id="472cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="472cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="472cb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="472cb-109">Permission type</span></span>      | <span data-ttu-id="472cb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="472cb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="472cb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="472cb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="472cb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="472cb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="472cb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="472cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="472cb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="472cb-114">Not supported.</span></span>    |
|<span data-ttu-id="472cb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="472cb-115">Application</span></span> | <span data-ttu-id="472cb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="472cb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="472cb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="472cb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/fill
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="472cb-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="472cb-118">Optional request headers</span></span>
| <span data-ttu-id="472cb-119">名称</span><span class="sxs-lookup"><span data-stu-id="472cb-119">Name</span></span>       | <span data-ttu-id="472cb-120">说明</span><span class="sxs-lookup"><span data-stu-id="472cb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="472cb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="472cb-121">Authorization</span></span>  | <span data-ttu-id="472cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="472cb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="472cb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="472cb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="472cb-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="472cb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="472cb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="472cb-127">Request body</span></span>
<span data-ttu-id="472cb-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="472cb-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="472cb-131">属性</span><span class="sxs-lookup"><span data-stu-id="472cb-131">Property</span></span>     | <span data-ttu-id="472cb-132">类型</span><span class="sxs-lookup"><span data-stu-id="472cb-132">Type</span></span>   |<span data-ttu-id="472cb-133">说明</span><span class="sxs-lookup"><span data-stu-id="472cb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="472cb-134">color</span><span class="sxs-lookup"><span data-stu-id="472cb-134">color</span></span>|<span data-ttu-id="472cb-135">string</span><span class="sxs-lookup"><span data-stu-id="472cb-135">string</span></span>|<span data-ttu-id="472cb-136">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="472cb-136">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="472cb-137">响应</span><span class="sxs-lookup"><span data-stu-id="472cb-137">Response</span></span>

<span data-ttu-id="472cb-138">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [WorkbookRangeFill](../resources/rangefill.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="472cb-138">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="472cb-139">示例</span><span class="sxs-lookup"><span data-stu-id="472cb-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="472cb-140">请求</span><span class="sxs-lookup"><span data-stu-id="472cb-140">Request</span></span>
<span data-ttu-id="472cb-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="472cb-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="472cb-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="472cb-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="c"></a>[<span data-ttu-id="472cb-143">C#</span><span class="sxs-lookup"><span data-stu-id="472cb-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="472cb-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="472cb-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="472cb-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="472cb-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="472cb-146">Java</span><span class="sxs-lookup"><span data-stu-id="472cb-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangefill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="472cb-147">响应</span><span class="sxs-lookup"><span data-stu-id="472cb-147">Response</span></span>
<span data-ttu-id="472cb-p105">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="472cb-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

