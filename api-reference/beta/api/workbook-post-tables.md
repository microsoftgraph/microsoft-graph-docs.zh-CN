---
title: 创建表
description: 使用此 API 创建新的表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2e9bd37bd1899144bf2df93ca196ccbc2cca34a8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051695"
---
# <a name="create-table"></a><span data-ttu-id="f781f-103">创建表</span><span class="sxs-lookup"><span data-stu-id="f781f-103">Create table</span></span>

<span data-ttu-id="f781f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f781f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f781f-105">使用此 API 创建新的表。</span><span class="sxs-lookup"><span data-stu-id="f781f-105">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="f781f-106">权限</span><span class="sxs-lookup"><span data-stu-id="f781f-106">Permissions</span></span>
<span data-ttu-id="f781f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f781f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f781f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f781f-109">Permission type</span></span>      | <span data-ttu-id="f781f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f781f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f781f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f781f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f781f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f781f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f781f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f781f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f781f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f781f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f781f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f781f-115">Application</span></span> | <span data-ttu-id="f781f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f781f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f781f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f781f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/$/add
POST /me/drive/root:/{item-path}:/workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="f781f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f781f-118">Request headers</span></span>
| <span data-ttu-id="f781f-119">名称</span><span class="sxs-lookup"><span data-stu-id="f781f-119">Name</span></span>       | <span data-ttu-id="f781f-120">说明</span><span class="sxs-lookup"><span data-stu-id="f781f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f781f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f781f-121">Authorization</span></span>  | <span data-ttu-id="f781f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f781f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f781f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f781f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f781f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f781f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f781f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f781f-127">Request body</span></span>
<span data-ttu-id="f781f-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f781f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f781f-129">参数</span><span class="sxs-lookup"><span data-stu-id="f781f-129">Parameter</span></span>           | <span data-ttu-id="f781f-130">类型</span><span class="sxs-lookup"><span data-stu-id="f781f-130">Type</span></span>      |<span data-ttu-id="f781f-131">说明</span><span class="sxs-lookup"><span data-stu-id="f781f-131">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="f781f-132">Address</span><span class="sxs-lookup"><span data-stu-id="f781f-132">Address</span></span>  | <span data-ttu-id="f781f-133">string</span><span class="sxs-lookup"><span data-stu-id="f781f-133">string</span></span>| <span data-ttu-id="f781f-p104">区域地址。若要从 `worksheets/{id or name}/tables/add` 路径调用此 API，地址中无需有工作表名称前缀。不过，若要从 `workbook/tables/add` 路径调用此 API，请提供需要在其中创建表的工作表名称（例如：`sheet1!A1:D4`）</span><span class="sxs-lookup"><span data-stu-id="f781f-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="f781f-137">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="f781f-137">hasHeaders</span></span>  | <span data-ttu-id="f781f-138">布尔</span><span class="sxs-lookup"><span data-stu-id="f781f-138">boolean</span></span>|<span data-ttu-id="f781f-p105">指示区域是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。</span><span class="sxs-lookup"><span data-stu-id="f781f-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="f781f-142">响应</span><span class="sxs-lookup"><span data-stu-id="f781f-142">Response</span></span>

<span data-ttu-id="f781f-143">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [workbookTable](../resources/workbooktable.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f781f-143">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f781f-144">示例</span><span class="sxs-lookup"><span data-stu-id="f781f-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f781f-145">请求</span><span class="sxs-lookup"><span data-stu-id="f781f-145">Request</span></span>
<span data-ttu-id="f781f-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f781f-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f781f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="f781f-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
# <a name="c"></a>[<span data-ttu-id="f781f-148">C#</span><span class="sxs-lookup"><span data-stu-id="f781f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-workbook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f781f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f781f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-workbook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f781f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f781f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-workbook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f781f-151">Java</span><span class="sxs-lookup"><span data-stu-id="f781f-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-table-from-workbook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f781f-152">响应</span><span class="sxs-lookup"><span data-stu-id="f781f-152">Response</span></span>
<span data-ttu-id="f781f-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f781f-153">Here is an example of the response.</span></span> <span data-ttu-id="f781f-154">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f781f-154">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


