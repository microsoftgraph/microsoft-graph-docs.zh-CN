---
title: TableColumn:Range
description: 获取与整个列相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 26be3f41947305b868d9fdbeb5bb862c003eeb60
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034427"
---
# <a name="tablecolumn-range"></a><span data-ttu-id="4278e-103">TableColumn:Range</span><span class="sxs-lookup"><span data-stu-id="4278e-103">TableColumn: Range</span></span>

<span data-ttu-id="4278e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4278e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4278e-105">获取与整个列相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="4278e-105">Gets the range object associated with the entire column.</span></span>
## <a name="permissions"></a><span data-ttu-id="4278e-106">权限</span><span class="sxs-lookup"><span data-stu-id="4278e-106">Permissions</span></span>
<span data-ttu-id="4278e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4278e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4278e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4278e-109">Permission type</span></span>      | <span data-ttu-id="4278e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4278e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4278e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4278e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4278e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4278e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4278e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4278e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4278e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4278e-114">Not supported.</span></span>    |
|<span data-ttu-id="4278e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4278e-115">Application</span></span> | <span data-ttu-id="4278e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4278e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4278e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4278e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="4278e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4278e-118">Request headers</span></span>
| <span data-ttu-id="4278e-119">名称</span><span class="sxs-lookup"><span data-stu-id="4278e-119">Name</span></span>       | <span data-ttu-id="4278e-120">说明</span><span class="sxs-lookup"><span data-stu-id="4278e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4278e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4278e-121">Authorization</span></span>  | <span data-ttu-id="4278e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4278e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4278e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4278e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4278e-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="4278e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4278e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4278e-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4278e-128">响应</span><span class="sxs-lookup"><span data-stu-id="4278e-128">Response</span></span>

<span data-ttu-id="4278e-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4278e-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4278e-130">示例</span><span class="sxs-lookup"><span data-stu-id="4278e-130">Example</span></span>
<span data-ttu-id="4278e-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4278e-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4278e-132">请求</span><span class="sxs-lookup"><span data-stu-id="4278e-132">Request</span></span>
<span data-ttu-id="4278e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4278e-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4278e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4278e-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_range",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range
```
# <a name="c"></a>[<span data-ttu-id="4278e-135">C#</span><span class="sxs-lookup"><span data-stu-id="4278e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4278e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4278e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4278e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4278e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4278e-138">Java</span><span class="sxs-lookup"><span data-stu-id="4278e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumn-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4278e-139">响应</span><span class="sxs-lookup"><span data-stu-id="4278e-139">Response</span></span>
<span data-ttu-id="4278e-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4278e-140">Here is an example of the response.</span></span> <span data-ttu-id="4278e-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4278e-141">Note: The response object shown here might be shortened for readability.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

