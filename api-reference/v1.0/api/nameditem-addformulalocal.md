---
title: 添加已命名项 FormulaLocal
description: 使用用户的公式区域设置，将新名称添加到给定范围的集合。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: a27a3378c8de08a4a70de01ad83ea25d09c25339
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577574"
---
# <a name="add-named-item-formulalocal"></a><span data-ttu-id="8f7c3-103">添加已命名项 FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="8f7c3-103">Add Named Item FormulaLocal</span></span>

<span data-ttu-id="8f7c3-104">命名空间：microsoft.graph 使用公式的用户区域设置将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-104">Namespace: microsoft.graph Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f7c3-105">权限</span><span class="sxs-lookup"><span data-stu-id="8f7c3-105">Permissions</span></span>
<span data-ttu-id="8f7c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f7c3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f7c3-108">Permission type</span></span>      | <span data-ttu-id="8f7c3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f7c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f7c3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f7c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f7c3-111">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f7c3-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="8f7c3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f7c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f7c3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-113">Not supported.</span></span>    |
|<span data-ttu-id="8f7c3-114">Application</span><span class="sxs-lookup"><span data-stu-id="8f7c3-114">Application</span></span> | <span data-ttu-id="8f7c3-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f7c3-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f7c3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f7c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/add
POST /me/drive/root:/{item-path}:/workbook/names/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/names/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="8f7c3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f7c3-117">Request headers</span></span>
| <span data-ttu-id="8f7c3-118">名称</span><span class="sxs-lookup"><span data-stu-id="8f7c3-118">Name</span></span>       | <span data-ttu-id="8f7c3-119">说明</span><span class="sxs-lookup"><span data-stu-id="8f7c3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f7c3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f7c3-120">Authorization</span></span>  | <span data-ttu-id="8f7c3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f7c3-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8f7c3-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8f7c3-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f7c3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f7c3-126">Request body</span></span>
<span data-ttu-id="8f7c3-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8f7c3-128">参数</span><span class="sxs-lookup"><span data-stu-id="8f7c3-128">Parameter</span></span>    | <span data-ttu-id="8f7c3-129">类型</span><span class="sxs-lookup"><span data-stu-id="8f7c3-129">Type</span></span>   |<span data-ttu-id="8f7c3-130">说明</span><span class="sxs-lookup"><span data-stu-id="8f7c3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f7c3-131">name</span><span class="sxs-lookup"><span data-stu-id="8f7c3-131">name</span></span>|<span data-ttu-id="8f7c3-132">string</span><span class="sxs-lookup"><span data-stu-id="8f7c3-132">string</span></span>|<span data-ttu-id="8f7c3-133">已命名项的名称。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-133">The name of the named item.</span></span>|
|<span data-ttu-id="8f7c3-134">公式</span><span class="sxs-lookup"><span data-stu-id="8f7c3-134">formula</span></span>|<span data-ttu-id="8f7c3-135">字符串</span><span class="sxs-lookup"><span data-stu-id="8f7c3-135">string</span></span>|<span data-ttu-id="8f7c3-136">名称将引用的公式或区域。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="8f7c3-137">comment</span><span class="sxs-lookup"><span data-stu-id="8f7c3-137">comment</span></span>|<span data-ttu-id="8f7c3-138">string</span><span class="sxs-lookup"><span data-stu-id="8f7c3-138">string</span></span>|<span data-ttu-id="8f7c3-139">与此已命名项相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="8f7c3-140">响应</span><span class="sxs-lookup"><span data-stu-id="8f7c3-140">Response</span></span>

<span data-ttu-id="8f7c3-141">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [WorkbookNamedItem](../resources/nameditem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-141">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f7c3-142">示例</span><span class="sxs-lookup"><span data-stu-id="8f7c3-142">Example</span></span>
<span data-ttu-id="8f7c3-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8f7c3-144">请求</span><span class="sxs-lookup"><span data-stu-id="8f7c3-144">Request</span></span>
<span data-ttu-id="8f7c3-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f7c3-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f7c3-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```
# <a name="c"></a>[<span data-ttu-id="8f7c3-147">C#</span><span class="sxs-lookup"><span data-stu-id="8f7c3-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f7c3-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f7c3-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f7c3-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f7c3-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f7c3-150">Java</span><span class="sxs-lookup"><span data-stu-id="8f7c3-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8f7c3-151">响应</span><span class="sxs-lookup"><span data-stu-id="8f7c3-151">Response</span></span>
<span data-ttu-id="8f7c3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f7c3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "String",
    "value": "0",
    "visible": true
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

