---
title: 'WorksheetCollection: add'
description: '。请在上面激活 ( # A1。'
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d3162d29d94e5903f85e8f1ea4b5ea6527daa78b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979963"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="96050-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="96050-103">WorksheetCollection: add</span></span>

<span data-ttu-id="96050-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96050-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96050-p101">向工作簿添加新工作表。工作表将添加到现有工作表的末尾。如果您想要激活新添加的工作表，请对其调用 ".activate()。</span><span class="sxs-lookup"><span data-stu-id="96050-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="96050-108">权限</span><span class="sxs-lookup"><span data-stu-id="96050-108">Permissions</span></span>
<span data-ttu-id="96050-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96050-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96050-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="96050-111">Permission type</span></span>      | <span data-ttu-id="96050-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96050-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96050-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96050-113">Delegated (work or school account)</span></span> | <span data-ttu-id="96050-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96050-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96050-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96050-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96050-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96050-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96050-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="96050-117">Application</span></span> | <span data-ttu-id="96050-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="96050-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96050-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96050-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="96050-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="96050-120">Request headers</span></span>
| <span data-ttu-id="96050-121">名称</span><span class="sxs-lookup"><span data-stu-id="96050-121">Name</span></span>       | <span data-ttu-id="96050-122">说明</span><span class="sxs-lookup"><span data-stu-id="96050-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96050-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96050-123">Authorization</span></span>  | <span data-ttu-id="96050-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96050-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96050-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="96050-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="96050-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="96050-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96050-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="96050-129">Request body</span></span>
<span data-ttu-id="96050-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="96050-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="96050-131">参数</span><span class="sxs-lookup"><span data-stu-id="96050-131">Parameter</span></span>    | <span data-ttu-id="96050-132">类型</span><span class="sxs-lookup"><span data-stu-id="96050-132">Type</span></span>   |<span data-ttu-id="96050-133">说明</span><span class="sxs-lookup"><span data-stu-id="96050-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96050-134">name</span><span class="sxs-lookup"><span data-stu-id="96050-134">name</span></span>|<span data-ttu-id="96050-135">string</span><span class="sxs-lookup"><span data-stu-id="96050-135">string</span></span>|<span data-ttu-id="96050-p105">可选。要添加的工作表的名称。如果指定，名称应唯一。如果未指定，Excel 将确定新工作表的名称。</span><span class="sxs-lookup"><span data-stu-id="96050-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="96050-140">响应</span><span class="sxs-lookup"><span data-stu-id="96050-140">Response</span></span>

<span data-ttu-id="96050-141">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [workbookWorksheet](../resources/workbookworksheet.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96050-141">If successful, this method returns `200 OK` response code and [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96050-142">示例</span><span class="sxs-lookup"><span data-stu-id="96050-142">Example</span></span>
<span data-ttu-id="96050-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="96050-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="96050-144">请求</span><span class="sxs-lookup"><span data-stu-id="96050-144">Request</span></span>
<span data-ttu-id="96050-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96050-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96050-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="96050-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="96050-147">C#</span><span class="sxs-lookup"><span data-stu-id="96050-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96050-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96050-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96050-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96050-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96050-150">Java</span><span class="sxs-lookup"><span data-stu-id="96050-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="96050-151">响应</span><span class="sxs-lookup"><span data-stu-id="96050-151">Response</span></span>
<span data-ttu-id="96050-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96050-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


