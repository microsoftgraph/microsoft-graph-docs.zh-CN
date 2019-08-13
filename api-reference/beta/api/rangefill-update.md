---
title: 更新 rangefill
description: 更新 rangefill 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 01c7c72786fe9af3cb252665c91149d07e7dd495
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360706"
---
# <a name="update-rangefill"></a><span data-ttu-id="0b127-103">更新 rangefill</span><span class="sxs-lookup"><span data-stu-id="0b127-103">Update rangefill</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b127-104">更新 rangefill 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b127-104">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b127-105">权限</span><span class="sxs-lookup"><span data-stu-id="0b127-105">Permissions</span></span>
<span data-ttu-id="0b127-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b127-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b127-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b127-108">Permission type</span></span>      | <span data-ttu-id="0b127-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b127-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b127-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b127-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0b127-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b127-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b127-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b127-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b127-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b127-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b127-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b127-114">Application</span></span> | <span data-ttu-id="0b127-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b127-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b127-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b127-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="0b127-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="0b127-117">Optional request headers</span></span>
| <span data-ttu-id="0b127-118">名称</span><span class="sxs-lookup"><span data-stu-id="0b127-118">Name</span></span>       | <span data-ttu-id="0b127-119">说明</span><span class="sxs-lookup"><span data-stu-id="0b127-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0b127-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b127-120">Authorization</span></span>  | <span data-ttu-id="0b127-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b127-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b127-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0b127-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0b127-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0b127-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b127-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b127-126">Request body</span></span>
<span data-ttu-id="0b127-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0b127-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0b127-130">属性</span><span class="sxs-lookup"><span data-stu-id="0b127-130">Property</span></span>     | <span data-ttu-id="0b127-131">类型</span><span class="sxs-lookup"><span data-stu-id="0b127-131">Type</span></span>   |<span data-ttu-id="0b127-132">说明</span><span class="sxs-lookup"><span data-stu-id="0b127-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b127-133">color</span><span class="sxs-lookup"><span data-stu-id="0b127-133">color</span></span>|<span data-ttu-id="0b127-134">string</span><span class="sxs-lookup"><span data-stu-id="0b127-134">string</span></span>|<span data-ttu-id="0b127-135">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="0b127-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="0b127-136">响应</span><span class="sxs-lookup"><span data-stu-id="0b127-136">Response</span></span>

<span data-ttu-id="0b127-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[workbookRangeFill](../resources/workbookrangefill.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b127-137">If successful, this method returns a `200 OK` response code and updated [workbookRangeFill](../resources/workbookrangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b127-138">示例</span><span class="sxs-lookup"><span data-stu-id="0b127-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b127-139">请求</span><span class="sxs-lookup"><span data-stu-id="0b127-139">Request</span></span>
<span data-ttu-id="0b127-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b127-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b127-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0b127-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b127-142">C#</span><span class="sxs-lookup"><span data-stu-id="0b127-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b127-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b127-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b127-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="0b127-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0b127-145">Java</span><span class="sxs-lookup"><span data-stu-id="0b127-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangefill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b127-146">响应</span><span class="sxs-lookup"><span data-stu-id="0b127-146">Response</span></span>
<span data-ttu-id="0b127-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b127-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
