---
title: 更新 formatProtection
description: 更新 formatprotection 对象的属性。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: ea3b831639cada667f46aa3f5af1d276efd34e7f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002739"
---
# <a name="update-formatprotection"></a><span data-ttu-id="0e314-103">更新 formatProtection</span><span class="sxs-lookup"><span data-stu-id="0e314-103">Update formatprotection</span></span>

<span data-ttu-id="0e314-104">更新 formatprotection 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e314-104">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e314-105">权限</span><span class="sxs-lookup"><span data-stu-id="0e314-105">Permissions</span></span>
<span data-ttu-id="0e314-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e314-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e314-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e314-108">Permission type</span></span>      | <span data-ttu-id="0e314-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e314-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="0e314-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e314-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e314-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e314-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="0e314-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e314-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e314-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e314-113">Not supported.</span></span>    | 
|<span data-ttu-id="0e314-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e314-114">Application</span></span> | <span data-ttu-id="0e314-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e314-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0e314-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e314-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="0e314-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="0e314-117">Optional request headers</span></span>
| <span data-ttu-id="0e314-118">名称</span><span class="sxs-lookup"><span data-stu-id="0e314-118">Name</span></span>       | <span data-ttu-id="0e314-119">说明</span><span class="sxs-lookup"><span data-stu-id="0e314-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0e314-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e314-120">Authorization</span></span>  | <span data-ttu-id="0e314-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e314-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0e314-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e314-123">Request body</span></span>
<span data-ttu-id="0e314-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0e314-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0e314-127">属性</span><span class="sxs-lookup"><span data-stu-id="0e314-127">Property</span></span>     | <span data-ttu-id="0e314-128">类型</span><span class="sxs-lookup"><span data-stu-id="0e314-128">Type</span></span>   |<span data-ttu-id="0e314-129">说明</span><span class="sxs-lookup"><span data-stu-id="0e314-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e314-130">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="0e314-130">formulaHidden</span></span>|<span data-ttu-id="0e314-131">boolean</span><span class="sxs-lookup"><span data-stu-id="0e314-131">boolean</span></span>|<span data-ttu-id="0e314-p104">表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。</span><span class="sxs-lookup"><span data-stu-id="0e314-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="0e314-134">已锁定</span><span class="sxs-lookup"><span data-stu-id="0e314-134">locked</span></span>|<span data-ttu-id="0e314-135">boolean</span><span class="sxs-lookup"><span data-stu-id="0e314-135">boolean</span></span>|<span data-ttu-id="0e314-p105">指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。</span><span class="sxs-lookup"><span data-stu-id="0e314-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="0e314-138">响应</span><span class="sxs-lookup"><span data-stu-id="0e314-138">Response</span></span>

<span data-ttu-id="0e314-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [FormatProtection](../resources/formatprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e314-139">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e314-140">示例</span><span class="sxs-lookup"><span data-stu-id="0e314-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e314-141">请求</span><span class="sxs-lookup"><span data-stu-id="0e314-141">Request</span></span>
<span data-ttu-id="0e314-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e314-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0e314-143">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0e314-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0e314-144">C#</span><span class="sxs-lookup"><span data-stu-id="0e314-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e314-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e314-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0e314-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="0e314-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0e314-147">Java</span><span class="sxs-lookup"><span data-stu-id="0e314-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-formatprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0e314-148">响应</span><span class="sxs-lookup"><span data-stu-id="0e314-148">Response</span></span>
<span data-ttu-id="0e314-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e314-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
