---
title: 创建表
description: 使用此 API 创建新的表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 93f8951df02bf8fd52673af717c2a250703d1f9e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420971"
---
# <a name="create-table"></a><span data-ttu-id="13a12-103">创建表</span><span class="sxs-lookup"><span data-stu-id="13a12-103">Create table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13a12-104">使用此 API 创建新的表。</span><span class="sxs-lookup"><span data-stu-id="13a12-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="13a12-105">权限</span><span class="sxs-lookup"><span data-stu-id="13a12-105">Permissions</span></span>
<span data-ttu-id="13a12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13a12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13a12-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="13a12-108">Permission type</span></span>      | <span data-ttu-id="13a12-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13a12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13a12-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13a12-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13a12-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13a12-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="13a12-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13a12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13a12-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13a12-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="13a12-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="13a12-114">Application</span></span> | <span data-ttu-id="13a12-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="13a12-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13a12-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13a12-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="13a12-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="13a12-117">Request headers</span></span>
| <span data-ttu-id="13a12-118">名称</span><span class="sxs-lookup"><span data-stu-id="13a12-118">Name</span></span>       | <span data-ttu-id="13a12-119">说明</span><span class="sxs-lookup"><span data-stu-id="13a12-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="13a12-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="13a12-120">Authorization</span></span>  | <span data-ttu-id="13a12-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13a12-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13a12-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="13a12-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="13a12-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="13a12-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13a12-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="13a12-126">Request body</span></span>
<span data-ttu-id="13a12-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="13a12-127">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="13a12-128">参数</span><span class="sxs-lookup"><span data-stu-id="13a12-128">Parameter</span></span>       | <span data-ttu-id="13a12-129">类型</span><span class="sxs-lookup"><span data-stu-id="13a12-129">Type</span></span>|<span data-ttu-id="13a12-130">说明</span><span class="sxs-lookup"><span data-stu-id="13a12-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="13a12-131">Address</span><span class="sxs-lookup"><span data-stu-id="13a12-131">Address</span></span>  | <span data-ttu-id="13a12-132">string</span><span class="sxs-lookup"><span data-stu-id="13a12-132">string</span></span>| <span data-ttu-id="13a12-133">区域地址。</span><span class="sxs-lookup"><span data-stu-id="13a12-133">Range address.</span></span> <span data-ttu-id="13a12-134">如果要从`worksheets/{id|name}/tables/add`路径调用此 API, 则无需支持地址中的工作表名称前缀。</span><span class="sxs-lookup"><span data-stu-id="13a12-134">If you are calling this API off of `worksheets/{id|name}/tables/add` path, there is no need to support the sheet name prefix in the address.</span></span> <span data-ttu-id="13a12-135">但是, 如果要调用此`workbook/tables/add`路径 off, 请提供需要在其上创建表的工作表名称 (示例:) `sheet1!A1:D4`</span><span class="sxs-lookup"><span data-stu-id="13a12-135">However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="13a12-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="13a12-136">hasHeaders</span></span>  | <span data-ttu-id="13a12-137">布尔</span><span class="sxs-lookup"><span data-stu-id="13a12-137">boolean</span></span>|<span data-ttu-id="13a12-p105">指示区域是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。</span><span class="sxs-lookup"><span data-stu-id="13a12-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="13a12-141">响应</span><span class="sxs-lookup"><span data-stu-id="13a12-141">Response</span></span>

<span data-ttu-id="13a12-142">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[workbookTable](../resources/workbooktable.md)对象。</span><span class="sxs-lookup"><span data-stu-id="13a12-142">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13a12-143">示例</span><span class="sxs-lookup"><span data-stu-id="13a12-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13a12-144">请求</span><span class="sxs-lookup"><span data-stu-id="13a12-144">Request</span></span>
<span data-ttu-id="13a12-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13a12-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="13a12-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="13a12-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "",
  "hasHeaders": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="13a12-147">C#</span><span class="sxs-lookup"><span data-stu-id="13a12-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="13a12-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13a12-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="13a12-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="13a12-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13a12-150">响应</span><span class="sxs-lookup"><span data-stu-id="13a12-150">Response</span></span>
<span data-ttu-id="13a12-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13a12-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
