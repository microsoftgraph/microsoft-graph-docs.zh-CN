---
title: 创建 TableColumn
description: 使用此 API 创建新的 TableColumn。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 300ff8804bda1314fa5918f28852b1e013abd064
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278930"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="a0b87-103">创建 TableColumn</span><span class="sxs-lookup"><span data-stu-id="a0b87-103">Create TableColumn</span></span>

<span data-ttu-id="a0b87-104">使用此 API 创建新的 TableColumn。</span><span class="sxs-lookup"><span data-stu-id="a0b87-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="a0b87-105">权限</span><span class="sxs-lookup"><span data-stu-id="a0b87-105">Permissions</span></span>
<span data-ttu-id="a0b87-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0b87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0b87-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0b87-108">Permission type</span></span>      | <span data-ttu-id="a0b87-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0b87-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0b87-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0b87-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0b87-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0b87-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a0b87-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0b87-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0b87-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0b87-113">Not supported.</span></span>    |
|<span data-ttu-id="a0b87-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0b87-114">Application</span></span> | <span data-ttu-id="a0b87-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0b87-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0b87-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0b87-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="a0b87-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0b87-117">Request headers</span></span>
| <span data-ttu-id="a0b87-118">名称</span><span class="sxs-lookup"><span data-stu-id="a0b87-118">Name</span></span>       | <span data-ttu-id="a0b87-119">说明</span><span class="sxs-lookup"><span data-stu-id="a0b87-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a0b87-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0b87-120">Authorization</span></span>  | <span data-ttu-id="a0b87-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0b87-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0b87-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a0b87-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a0b87-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a0b87-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0b87-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0b87-126">Request body</span></span>
<span data-ttu-id="a0b87-127">在请求正文中, 提供[WorkbookTableColumn](../resources/tablecolumn.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0b87-127">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a0b87-128">响应</span><span class="sxs-lookup"><span data-stu-id="a0b87-128">Response</span></span>

<span data-ttu-id="a0b87-129">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[WorkbookTableColumn](../resources/tablecolumn.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a0b87-129">If successful, this method returns `201 Created` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0b87-130">示例</span><span class="sxs-lookup"><span data-stu-id="a0b87-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0b87-131">请求</span><span class="sxs-lookup"><span data-stu-id="a0b87-131">Request</span></span>
<span data-ttu-id="a0b87-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0b87-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="a0b87-133">在请求正文中, 提供[WorkbookTableColumn](../resources/tablecolumn.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0b87-133">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a0b87-134">响应</span><span class="sxs-lookup"><span data-stu-id="a0b87-134">Response</span></span>
<span data-ttu-id="a0b87-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0b87-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a0b87-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a0b87-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a0b87-139">C#</span><span class="sxs-lookup"><span data-stu-id="a0b87-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_tablecolumn_from_table-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0b87-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="a0b87-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_tablecolumn_from_table-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a0b87-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="a0b87-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_tablecolumn_from_table-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-post-columns.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/table-post-columns.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/table-post-columns.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
