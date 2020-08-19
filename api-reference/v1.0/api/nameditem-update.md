---
title: 更新 nameditem
description: 更新 nameditem 对象的属性。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f75d034c7f4e5a6e3c8463e21114fc6a6a429a65
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809272"
---
# <a name="update-nameditem"></a><span data-ttu-id="dc38c-103">更新 nameditem</span><span class="sxs-lookup"><span data-stu-id="dc38c-103">Update nameditem</span></span>

<span data-ttu-id="dc38c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc38c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc38c-105">更新 nameditem 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dc38c-105">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc38c-106">权限</span><span class="sxs-lookup"><span data-stu-id="dc38c-106">Permissions</span></span>
<span data-ttu-id="dc38c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc38c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc38c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc38c-109">Permission type</span></span>      | <span data-ttu-id="dc38c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc38c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc38c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc38c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc38c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc38c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc38c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc38c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc38c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc38c-114">Not supported.</span></span>    |
|<span data-ttu-id="dc38c-115">Application</span><span class="sxs-lookup"><span data-stu-id="dc38c-115">Application</span></span> | <span data-ttu-id="dc38c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc38c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc38c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc38c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="dc38c-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="dc38c-118">Optional request headers</span></span>
| <span data-ttu-id="dc38c-119">名称</span><span class="sxs-lookup"><span data-stu-id="dc38c-119">Name</span></span>       | <span data-ttu-id="dc38c-120">说明</span><span class="sxs-lookup"><span data-stu-id="dc38c-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dc38c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc38c-121">Authorization</span></span>  | <span data-ttu-id="dc38c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc38c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc38c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dc38c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dc38c-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="dc38c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc38c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc38c-127">Request body</span></span>
<span data-ttu-id="dc38c-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="dc38c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dc38c-131">属性</span><span class="sxs-lookup"><span data-stu-id="dc38c-131">Property</span></span>     | <span data-ttu-id="dc38c-132">类型</span><span class="sxs-lookup"><span data-stu-id="dc38c-132">Type</span></span>   |<span data-ttu-id="dc38c-133">说明</span><span class="sxs-lookup"><span data-stu-id="dc38c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc38c-134">visible</span><span class="sxs-lookup"><span data-stu-id="dc38c-134">visible</span></span>|<span data-ttu-id="dc38c-135">布尔</span><span class="sxs-lookup"><span data-stu-id="dc38c-135">boolean</span></span>|<span data-ttu-id="dc38c-136">指定对象是否可见。</span><span class="sxs-lookup"><span data-stu-id="dc38c-136">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="dc38c-137">comment</span><span class="sxs-lookup"><span data-stu-id="dc38c-137">comment</span></span>|   <span data-ttu-id="dc38c-138">string</span><span class="sxs-lookup"><span data-stu-id="dc38c-138">string</span></span>  |<span data-ttu-id="dc38c-139">表示与此名称相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="dc38c-139">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="dc38c-140">响应</span><span class="sxs-lookup"><span data-stu-id="dc38c-140">Response</span></span>

<span data-ttu-id="dc38c-141">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [WorkbookNamedItem](../resources/nameditem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc38c-141">If successful, this method returns a `200 OK` response code and updated [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc38c-142">示例</span><span class="sxs-lookup"><span data-stu-id="dc38c-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc38c-143">请求</span><span class="sxs-lookup"><span data-stu-id="dc38c-143">Request</span></span>
<span data-ttu-id="dc38c-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc38c-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc38c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc38c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="dc38c-146">C#</span><span class="sxs-lookup"><span data-stu-id="dc38c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-nameditem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc38c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc38c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-nameditem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc38c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc38c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-nameditem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc38c-149">Java</span><span class="sxs-lookup"><span data-stu-id="dc38c-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-nameditem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dc38c-150">响应</span><span class="sxs-lookup"><span data-stu-id="dc38c-150">Response</span></span>
<span data-ttu-id="dc38c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dc38c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
