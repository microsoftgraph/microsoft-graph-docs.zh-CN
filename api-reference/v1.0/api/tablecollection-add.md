---
title: 'TableCollection: add'
description: 创建一个新表。区域源地址确定将在其下添加表的工作表。如果无法添加表（例如，由于地址无效，或者表与另一个表重叠），将抛出错误。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0ef87e1a251ffd65754d9d949af26468b3daed9c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575901"
---
# <a name="tablecollection-add"></a><span data-ttu-id="c4935-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="c4935-105">TableCollection: add</span></span>

<span data-ttu-id="c4935-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4935-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4935-p102">创建一个新表。区域源地址确定将在其下添加表的工作表。如果无法添加表（例如，由于地址无效，或者表与另一个表重叠），将抛出错误。</span><span class="sxs-lookup"><span data-stu-id="c4935-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="c4935-110">错误处理</span><span class="sxs-lookup"><span data-stu-id="c4935-110">Error Handling</span></span>

<span data-ttu-id="c4935-111">此请求有时可能会收到 504 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="c4935-111">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="c4935-112">此错误的适当响应做法是重复发出请求。</span><span class="sxs-lookup"><span data-stu-id="c4935-112">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4935-113">权限</span><span class="sxs-lookup"><span data-stu-id="c4935-113">Permissions</span></span>
<span data-ttu-id="c4935-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4935-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4935-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4935-116">Permission type</span></span>      | <span data-ttu-id="c4935-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4935-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4935-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4935-118">Delegated (work or school account)</span></span> | <span data-ttu-id="c4935-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4935-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4935-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4935-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4935-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4935-121">Not supported.</span></span>    |
|<span data-ttu-id="c4935-122">Application</span><span class="sxs-lookup"><span data-stu-id="c4935-122">Application</span></span> | <span data-ttu-id="c4935-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4935-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4935-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4935-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/add
POST /me/drive/root:/{item-path}:/workbook/tables/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="c4935-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4935-125">Request headers</span></span>
| <span data-ttu-id="c4935-126">名称</span><span class="sxs-lookup"><span data-stu-id="c4935-126">Name</span></span>       | <span data-ttu-id="c4935-127">说明</span><span class="sxs-lookup"><span data-stu-id="c4935-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4935-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4935-128">Authorization</span></span>  | <span data-ttu-id="c4935-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4935-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4935-131">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c4935-131">Workbook-Session-Id</span></span>  | <span data-ttu-id="c4935-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c4935-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4935-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4935-134">Request body</span></span>
<span data-ttu-id="c4935-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c4935-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c4935-136">参数</span><span class="sxs-lookup"><span data-stu-id="c4935-136">Parameter</span></span>    | <span data-ttu-id="c4935-137">类型</span><span class="sxs-lookup"><span data-stu-id="c4935-137">Type</span></span>   |<span data-ttu-id="c4935-138">说明</span><span class="sxs-lookup"><span data-stu-id="c4935-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4935-139">address</span><span class="sxs-lookup"><span data-stu-id="c4935-139">address</span></span>|<span data-ttu-id="c4935-140">string</span><span class="sxs-lookup"><span data-stu-id="c4935-140">string</span></span>|<span data-ttu-id="c4935-p107">表示数据源的 range 对象的地址或名称。如果该地址不包含工作表名称，则使用当前活动的工作表。</span><span class="sxs-lookup"><span data-stu-id="c4935-p107">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="c4935-143">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="c4935-143">hasHeaders</span></span>|<span data-ttu-id="c4935-144">boolean</span><span class="sxs-lookup"><span data-stu-id="c4935-144">boolean</span></span>|<span data-ttu-id="c4935-p108">指示导入的数据是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。</span><span class="sxs-lookup"><span data-stu-id="c4935-p108">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="c4935-148">响应</span><span class="sxs-lookup"><span data-stu-id="c4935-148">Response</span></span>

<span data-ttu-id="c4935-149">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [WorkbookTable](../resources/table.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c4935-149">If successful, this method returns `200 OK` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4935-150">示例</span><span class="sxs-lookup"><span data-stu-id="c4935-150">Example</span></span>
<span data-ttu-id="c4935-151">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c4935-151">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c4935-152">请求</span><span class="sxs-lookup"><span data-stu-id="c4935-152">Request</span></span>
<span data-ttu-id="c4935-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4935-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4935-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4935-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```
# <a name="c"></a>[<span data-ttu-id="c4935-155">C#</span><span class="sxs-lookup"><span data-stu-id="c4935-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4935-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4935-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4935-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4935-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4935-158">Java</span><span class="sxs-lookup"><span data-stu-id="c4935-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c4935-159">响应</span><span class="sxs-lookup"><span data-stu-id="c4935-159">Response</span></span>
<span data-ttu-id="c4935-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4935-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
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
<!-- {
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

