---
title: 更新 formatProtection
description: 更新 formatprotection 对象的属性。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 43f7b9f1c0f7e8885f871b7e760a78e866a4cf0f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573696"
---
# <a name="update-formatprotection"></a><span data-ttu-id="9a8d5-103">更新 formatProtection</span><span class="sxs-lookup"><span data-stu-id="9a8d5-103">Update formatprotection</span></span>

<span data-ttu-id="9a8d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a8d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a8d5-105">更新 formatprotection 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9a8d5-105">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a8d5-106">权限</span><span class="sxs-lookup"><span data-stu-id="9a8d5-106">Permissions</span></span>
<span data-ttu-id="9a8d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a8d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a8d5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a8d5-109">Permission type</span></span>      | <span data-ttu-id="9a8d5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a8d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a8d5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a8d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a8d5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a8d5-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a8d5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a8d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a8d5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a8d5-114">Not supported.</span></span>    |
|<span data-ttu-id="9a8d5-115">Application</span><span class="sxs-lookup"><span data-stu-id="9a8d5-115">Application</span></span> | <span data-ttu-id="9a8d5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a8d5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a8d5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a8d5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format/protection
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/protection
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="9a8d5-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="9a8d5-118">Optional request headers</span></span>
| <span data-ttu-id="9a8d5-119">名称</span><span class="sxs-lookup"><span data-stu-id="9a8d5-119">Name</span></span>       | <span data-ttu-id="9a8d5-120">说明</span><span class="sxs-lookup"><span data-stu-id="9a8d5-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9a8d5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a8d5-121">Authorization</span></span>  | <span data-ttu-id="9a8d5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9a8d5-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9a8d5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a8d5-124">Request body</span></span>
<span data-ttu-id="9a8d5-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9a8d5-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9a8d5-128">属性</span><span class="sxs-lookup"><span data-stu-id="9a8d5-128">Property</span></span>     | <span data-ttu-id="9a8d5-129">类型</span><span class="sxs-lookup"><span data-stu-id="9a8d5-129">Type</span></span>   |<span data-ttu-id="9a8d5-130">说明</span><span class="sxs-lookup"><span data-stu-id="9a8d5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a8d5-131">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="9a8d5-131">formulaHidden</span></span>|<span data-ttu-id="9a8d5-132">boolean</span><span class="sxs-lookup"><span data-stu-id="9a8d5-132">boolean</span></span>|<span data-ttu-id="9a8d5-p104">表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。</span><span class="sxs-lookup"><span data-stu-id="9a8d5-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="9a8d5-135">已锁定</span><span class="sxs-lookup"><span data-stu-id="9a8d5-135">locked</span></span>|<span data-ttu-id="9a8d5-136">boolean</span><span class="sxs-lookup"><span data-stu-id="9a8d5-136">boolean</span></span>|<span data-ttu-id="9a8d5-p105">指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。</span><span class="sxs-lookup"><span data-stu-id="9a8d5-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="9a8d5-139">响应</span><span class="sxs-lookup"><span data-stu-id="9a8d5-139">Response</span></span>

<span data-ttu-id="9a8d5-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [FormatProtection](../resources/formatprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9a8d5-140">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a8d5-141">示例</span><span class="sxs-lookup"><span data-stu-id="9a8d5-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a8d5-142">请求</span><span class="sxs-lookup"><span data-stu-id="9a8d5-142">Request</span></span>
<span data-ttu-id="9a8d5-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9a8d5-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a8d5-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a8d5-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
# <a name="c"></a>[<span data-ttu-id="9a8d5-145">C#</span><span class="sxs-lookup"><span data-stu-id="9a8d5-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a8d5-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a8d5-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a8d5-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a8d5-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a8d5-148">Java</span><span class="sxs-lookup"><span data-stu-id="9a8d5-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-formatprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a8d5-149">响应</span><span class="sxs-lookup"><span data-stu-id="9a8d5-149">Response</span></span>
<span data-ttu-id="9a8d5-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a8d5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

