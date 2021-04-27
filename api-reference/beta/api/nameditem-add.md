---
title: 添加已命名项
description: 使用用户的公式区域设置，将新名称添加到给定范围的集合。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: 8af8841ddb8b9ac0c7e46197e83dea8ce3ad6134
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052143"
---
# <a name="add-named-item"></a><span data-ttu-id="1740e-103">添加已命名项</span><span class="sxs-lookup"><span data-stu-id="1740e-103">Add Named Item</span></span>

<span data-ttu-id="1740e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1740e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1740e-105">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="1740e-105">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="1740e-106">权限</span><span class="sxs-lookup"><span data-stu-id="1740e-106">Permissions</span></span>
<span data-ttu-id="1740e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1740e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1740e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1740e-109">Permission type</span></span>      | <span data-ttu-id="1740e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1740e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1740e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1740e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1740e-112">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="1740e-112">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="1740e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1740e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1740e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1740e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1740e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1740e-115">Application</span></span> | <span data-ttu-id="1740e-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="1740e-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1740e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1740e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/add
POST /me/drive/root:/{item-path}:/workbook/names/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/names/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="1740e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1740e-118">Request headers</span></span>
| <span data-ttu-id="1740e-119">名称</span><span class="sxs-lookup"><span data-stu-id="1740e-119">Name</span></span>       | <span data-ttu-id="1740e-120">说明</span><span class="sxs-lookup"><span data-stu-id="1740e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1740e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1740e-121">Authorization</span></span>  | <span data-ttu-id="1740e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1740e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1740e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1740e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1740e-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1740e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1740e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1740e-127">Request body</span></span>
<span data-ttu-id="1740e-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1740e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1740e-129">参数</span><span class="sxs-lookup"><span data-stu-id="1740e-129">Parameter</span></span>    | <span data-ttu-id="1740e-130">类型</span><span class="sxs-lookup"><span data-stu-id="1740e-130">Type</span></span>   |<span data-ttu-id="1740e-131">说明</span><span class="sxs-lookup"><span data-stu-id="1740e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1740e-132">name</span><span class="sxs-lookup"><span data-stu-id="1740e-132">name</span></span>|<span data-ttu-id="1740e-133">string</span><span class="sxs-lookup"><span data-stu-id="1740e-133">string</span></span>|<span data-ttu-id="1740e-134">已命名项的名称。</span><span class="sxs-lookup"><span data-stu-id="1740e-134">The name of the named item.</span></span>|
|<span data-ttu-id="1740e-135">reference</span><span class="sxs-lookup"><span data-stu-id="1740e-135">reference</span></span>|<span data-ttu-id="1740e-136">字符串</span><span class="sxs-lookup"><span data-stu-id="1740e-136">string</span></span>|<span data-ttu-id="1740e-137">名称将引用的公式或区域。</span><span class="sxs-lookup"><span data-stu-id="1740e-137">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="1740e-138">comment</span><span class="sxs-lookup"><span data-stu-id="1740e-138">comment</span></span>|<span data-ttu-id="1740e-139">string</span><span class="sxs-lookup"><span data-stu-id="1740e-139">string</span></span>|<span data-ttu-id="1740e-140">与此已命名项相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="1740e-140">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="1740e-141">响应</span><span class="sxs-lookup"><span data-stu-id="1740e-141">Response</span></span>

<span data-ttu-id="1740e-142">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [workbookNamedItem](../resources/workbooknameditem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1740e-142">If successful, this method returns `200 OK` response code and [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1740e-143">示例</span><span class="sxs-lookup"><span data-stu-id="1740e-143">Example</span></span>
<span data-ttu-id="1740e-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1740e-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1740e-145">请求</span><span class="sxs-lookup"><span data-stu-id="1740e-145">Request</span></span>
<span data-ttu-id="1740e-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1740e-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1740e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="1740e-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add_1"
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
# <a name="c"></a>[<span data-ttu-id="1740e-148">C#</span><span class="sxs-lookup"><span data-stu-id="1740e-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1740e-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1740e-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1740e-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1740e-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1740e-151">Java</span><span class="sxs-lookup"><span data-stu-id="1740e-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1740e-152">响应</span><span class="sxs-lookup"><span data-stu-id="1740e-152">Response</span></span>
<span data-ttu-id="1740e-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1740e-153">Here is an example of the response.</span></span> <span data-ttu-id="1740e-154">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1740e-154">Note: The response object shown here might be shortened for readability.</span></span>
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


