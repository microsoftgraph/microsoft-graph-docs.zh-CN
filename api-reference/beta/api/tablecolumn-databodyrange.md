---
title: 'TableColumn: DataBodyRange'
description: 获取与列的数据体相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e6041108d550307a9001881a223527ca41fc3f11
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637796"
---
# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="178cb-103">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="178cb-103">TableColumn: DataBodyRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="178cb-104">获取与列的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="178cb-104">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="178cb-105">权限</span><span class="sxs-lookup"><span data-stu-id="178cb-105">Permissions</span></span>
<span data-ttu-id="178cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="178cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="178cb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="178cb-108">Permission type</span></span>      | <span data-ttu-id="178cb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="178cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="178cb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="178cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="178cb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="178cb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="178cb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="178cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="178cb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="178cb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="178cb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="178cb-114">Application</span></span> | <span data-ttu-id="178cb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="178cb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="178cb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="178cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/DataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/DataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="178cb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="178cb-117">Request headers</span></span>
| <span data-ttu-id="178cb-118">名称</span><span class="sxs-lookup"><span data-stu-id="178cb-118">Name</span></span>       | <span data-ttu-id="178cb-119">说明</span><span class="sxs-lookup"><span data-stu-id="178cb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="178cb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="178cb-120">Authorization</span></span>  | <span data-ttu-id="178cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="178cb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="178cb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="178cb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="178cb-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="178cb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="178cb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="178cb-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="178cb-127">响应</span><span class="sxs-lookup"><span data-stu-id="178cb-127">Response</span></span>

<span data-ttu-id="178cb-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="178cb-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="178cb-129">示例</span><span class="sxs-lookup"><span data-stu-id="178cb-129">Example</span></span>
<span data-ttu-id="178cb-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="178cb-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="178cb-131">请求</span><span class="sxs-lookup"><span data-stu-id="178cb-131">Request</span></span>
<span data-ttu-id="178cb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="178cb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_databodyrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/DataBodyRange
```

##### <a name="response"></a><span data-ttu-id="178cb-133">响应</span><span class="sxs-lookup"><span data-stu-id="178cb-133">Response</span></span>
<span data-ttu-id="178cb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="178cb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="178cb-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="178cb-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="178cb-138">语言</span><span class="sxs-lookup"><span data-stu-id="178cb-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablecolumn_databodyrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="178cb-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="178cb-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecolumn_databodyrange-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecolumn-databodyrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablecolumn-databodyrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
