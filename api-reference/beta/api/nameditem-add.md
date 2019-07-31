---
title: 添加已命名项
description: 使用用户的公式区域设置，将新名称添加到给定范围的集合。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a6d3f18043ef6a922f0389b9f3afc2f82af4b0b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992771"
---
# <a name="add-named-item"></a><span data-ttu-id="d1c9a-103">添加已命名项</span><span class="sxs-lookup"><span data-stu-id="d1c9a-103">Add Named Item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1c9a-104">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1c9a-105">权限</span><span class="sxs-lookup"><span data-stu-id="d1c9a-105">Permissions</span></span>
<span data-ttu-id="d1c9a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1c9a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1c9a-108">Permission type</span></span>      | <span data-ttu-id="d1c9a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1c9a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1c9a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1c9a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d1c9a-111">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c9a-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="d1c9a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1c9a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1c9a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1c9a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d1c9a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1c9a-114">Application</span></span> | <span data-ttu-id="d1c9a-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c9a-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1c9a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1c9a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="d1c9a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1c9a-117">Request headers</span></span>
| <span data-ttu-id="d1c9a-118">名称</span><span class="sxs-lookup"><span data-stu-id="d1c9a-118">Name</span></span>       | <span data-ttu-id="d1c9a-119">说明</span><span class="sxs-lookup"><span data-stu-id="d1c9a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d1c9a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1c9a-120">Authorization</span></span>  | <span data-ttu-id="d1c9a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1c9a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d1c9a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d1c9a-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1c9a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1c9a-126">Request body</span></span>
<span data-ttu-id="d1c9a-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d1c9a-128">参数</span><span class="sxs-lookup"><span data-stu-id="d1c9a-128">Parameter</span></span>    | <span data-ttu-id="d1c9a-129">类型</span><span class="sxs-lookup"><span data-stu-id="d1c9a-129">Type</span></span>   |<span data-ttu-id="d1c9a-130">说明</span><span class="sxs-lookup"><span data-stu-id="d1c9a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1c9a-131">name</span><span class="sxs-lookup"><span data-stu-id="d1c9a-131">name</span></span>|<span data-ttu-id="d1c9a-132">string</span><span class="sxs-lookup"><span data-stu-id="d1c9a-132">string</span></span>|<span data-ttu-id="d1c9a-133">已命名项的名称。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-133">The name of the named item.</span></span>|
|<span data-ttu-id="d1c9a-134">reference</span><span class="sxs-lookup"><span data-stu-id="d1c9a-134">reference</span></span>|<span data-ttu-id="d1c9a-135">string</span><span class="sxs-lookup"><span data-stu-id="d1c9a-135">string</span></span>|<span data-ttu-id="d1c9a-136">名称将引用的公式或区域。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="d1c9a-137">comment</span><span class="sxs-lookup"><span data-stu-id="d1c9a-137">comment</span></span>|<span data-ttu-id="d1c9a-138">字符串</span><span class="sxs-lookup"><span data-stu-id="d1c9a-138">string</span></span>|<span data-ttu-id="d1c9a-139">与此已命名项相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="d1c9a-140">响应</span><span class="sxs-lookup"><span data-stu-id="d1c9a-140">Response</span></span>

<span data-ttu-id="d1c9a-141">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[workbookNamedItem](../resources/workbooknameditem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-141">If successful, this method returns `200 OK` response code and [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1c9a-142">示例</span><span class="sxs-lookup"><span data-stu-id="d1c9a-142">Example</span></span>
<span data-ttu-id="d1c9a-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d1c9a-144">请求</span><span class="sxs-lookup"><span data-stu-id="d1c9a-144">Request</span></span>
<span data-ttu-id="d1c9a-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d1c9a-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d1c9a-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d1c9a-147">C#</span><span class="sxs-lookup"><span data-stu-id="d1c9a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1c9a-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="d1c9a-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d1c9a-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="d1c9a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d1c9a-150">Java</span><span class="sxs-lookup"><span data-stu-id="d1c9a-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d1c9a-151">响应</span><span class="sxs-lookup"><span data-stu-id="d1c9a-151">Response</span></span>
<span data-ttu-id="d1c9a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1c9a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
    "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
