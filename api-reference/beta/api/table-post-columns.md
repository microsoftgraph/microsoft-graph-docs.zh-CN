---
title: 创建 TableColumn
description: 使用此 API 创建新的 TableColumn。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b1239c9506fcaf92fddf175ba8c5517ca4e938ba
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458038"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="53bb9-103">创建 TableColumn</span><span class="sxs-lookup"><span data-stu-id="53bb9-103">Create TableColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53bb9-104">使用此 API 创建新的 TableColumn。</span><span class="sxs-lookup"><span data-stu-id="53bb9-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="53bb9-105">权限</span><span class="sxs-lookup"><span data-stu-id="53bb9-105">Permissions</span></span>
<span data-ttu-id="53bb9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53bb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53bb9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="53bb9-108">Permission type</span></span>      | <span data-ttu-id="53bb9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53bb9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53bb9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53bb9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53bb9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53bb9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53bb9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53bb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53bb9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53bb9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53bb9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="53bb9-114">Application</span></span> | <span data-ttu-id="53bb9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53bb9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53bb9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53bb9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="53bb9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="53bb9-117">Request headers</span></span>
| <span data-ttu-id="53bb9-118">名称</span><span class="sxs-lookup"><span data-stu-id="53bb9-118">Name</span></span>       | <span data-ttu-id="53bb9-119">说明</span><span class="sxs-lookup"><span data-stu-id="53bb9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53bb9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="53bb9-120">Authorization</span></span>  | <span data-ttu-id="53bb9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53bb9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53bb9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="53bb9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="53bb9-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="53bb9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53bb9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="53bb9-126">Request body</span></span>
<span data-ttu-id="53bb9-127">在请求正文中, 提供[workbookTableColumn](../resources/workbooktablecolumn.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53bb9-127">In the request body, supply a JSON representation of [workbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="53bb9-128">响应</span><span class="sxs-lookup"><span data-stu-id="53bb9-128">Response</span></span>

<span data-ttu-id="53bb9-129">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[workbookTableColumn](../resources/workbooktablecolumn.md)对象。</span><span class="sxs-lookup"><span data-stu-id="53bb9-129">If successful, this method returns `201 Created` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53bb9-130">示例</span><span class="sxs-lookup"><span data-stu-id="53bb9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53bb9-131">请求</span><span class="sxs-lookup"><span data-stu-id="53bb9-131">Request</span></span>
<span data-ttu-id="53bb9-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53bb9-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="53bb9-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="53bb9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="53bb9-134">C#</span><span class="sxs-lookup"><span data-stu-id="53bb9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tablecolumn-from-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53bb9-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="53bb9-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tablecolumn-from-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53bb9-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="53bb9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tablecolumn-from-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="53bb9-137">在请求正文中, 提供[workbookTableColumn](../resources/workbooktablecolumn.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53bb9-137">In the request body, supply a JSON representation of [workbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="53bb9-138">响应</span><span class="sxs-lookup"><span data-stu-id="53bb9-138">Response</span></span>
<span data-ttu-id="53bb9-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53bb9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
