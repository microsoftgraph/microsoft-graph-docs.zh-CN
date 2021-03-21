---
title: 添加已命名项
description: 使用用户的公式区域设置，将新名称添加到给定范围的集合。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: 665845d7f1ff1a39cf308eb76f22bb2d83bf4786
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961634"
---
# <a name="add-named-item"></a><span data-ttu-id="31176-103">添加已命名项</span><span class="sxs-lookup"><span data-stu-id="31176-103">Add Named Item</span></span>

<span data-ttu-id="31176-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31176-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31176-105">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="31176-105">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="31176-106">权限</span><span class="sxs-lookup"><span data-stu-id="31176-106">Permissions</span></span>
<span data-ttu-id="31176-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31176-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31176-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31176-109">Permission type</span></span>      | <span data-ttu-id="31176-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31176-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31176-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31176-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31176-112">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="31176-112">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="31176-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31176-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31176-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31176-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="31176-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="31176-115">Application</span></span> | <span data-ttu-id="31176-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="31176-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31176-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31176-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/add
POST /me/drive/root:/{item-path}:/workbook/names/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/names/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="31176-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="31176-118">Request headers</span></span>
| <span data-ttu-id="31176-119">名称</span><span class="sxs-lookup"><span data-stu-id="31176-119">Name</span></span>       | <span data-ttu-id="31176-120">说明</span><span class="sxs-lookup"><span data-stu-id="31176-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="31176-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="31176-121">Authorization</span></span>  | <span data-ttu-id="31176-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31176-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="31176-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="31176-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="31176-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="31176-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31176-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="31176-127">Request body</span></span>
<span data-ttu-id="31176-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="31176-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="31176-129">参数</span><span class="sxs-lookup"><span data-stu-id="31176-129">Parameter</span></span>    | <span data-ttu-id="31176-130">类型</span><span class="sxs-lookup"><span data-stu-id="31176-130">Type</span></span>   |<span data-ttu-id="31176-131">说明</span><span class="sxs-lookup"><span data-stu-id="31176-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31176-132">name</span><span class="sxs-lookup"><span data-stu-id="31176-132">name</span></span>|<span data-ttu-id="31176-133">string</span><span class="sxs-lookup"><span data-stu-id="31176-133">string</span></span>|<span data-ttu-id="31176-134">已命名项的名称。</span><span class="sxs-lookup"><span data-stu-id="31176-134">The name of the named item.</span></span>|
|<span data-ttu-id="31176-135">reference</span><span class="sxs-lookup"><span data-stu-id="31176-135">reference</span></span>|<span data-ttu-id="31176-136">字符串</span><span class="sxs-lookup"><span data-stu-id="31176-136">string</span></span>|<span data-ttu-id="31176-137">名称将引用的公式或区域。</span><span class="sxs-lookup"><span data-stu-id="31176-137">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="31176-138">comment</span><span class="sxs-lookup"><span data-stu-id="31176-138">comment</span></span>|<span data-ttu-id="31176-139">string</span><span class="sxs-lookup"><span data-stu-id="31176-139">string</span></span>|<span data-ttu-id="31176-140">与此已命名项相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="31176-140">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="31176-141">响应</span><span class="sxs-lookup"><span data-stu-id="31176-141">Response</span></span>

<span data-ttu-id="31176-142">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [workbookNamedItem](../resources/workbooknameditem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31176-142">If successful, this method returns `200 OK` response code and [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31176-143">示例</span><span class="sxs-lookup"><span data-stu-id="31176-143">Example</span></span>
<span data-ttu-id="31176-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="31176-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="31176-145">请求</span><span class="sxs-lookup"><span data-stu-id="31176-145">Request</span></span>
<span data-ttu-id="31176-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31176-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="31176-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="31176-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="31176-148">C#</span><span class="sxs-lookup"><span data-stu-id="31176-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31176-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31176-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31176-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31176-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31176-151">Java</span><span class="sxs-lookup"><span data-stu-id="31176-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="31176-152">响应</span><span class="sxs-lookup"><span data-stu-id="31176-152">Response</span></span>
<span data-ttu-id="31176-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31176-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


