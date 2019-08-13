---
title: TableRow:Range
description: 返回与整个行相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 22e457ae8592980dc19872025af5f6210fa3a03c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362992"
---
# <a name="tablerow-range"></a><span data-ttu-id="92ab6-103">TableRow:Range</span><span class="sxs-lookup"><span data-stu-id="92ab6-103">TableRow: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92ab6-104">返回与整个行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="92ab6-104">Returns the range object associated with the entire row.</span></span>
## <a name="permissions"></a><span data-ttu-id="92ab6-105">权限</span><span class="sxs-lookup"><span data-stu-id="92ab6-105">Permissions</span></span>
<span data-ttu-id="92ab6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92ab6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ab6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="92ab6-108">Permission type</span></span>      | <span data-ttu-id="92ab6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92ab6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92ab6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92ab6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="92ab6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92ab6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="92ab6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92ab6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92ab6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92ab6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="92ab6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="92ab6-114">Application</span></span> | <span data-ttu-id="92ab6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="92ab6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92ab6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92ab6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/{index}/Range
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/Range

```
## <a name="request-headers"></a><span data-ttu-id="92ab6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="92ab6-117">Request headers</span></span>
| <span data-ttu-id="92ab6-118">名称</span><span class="sxs-lookup"><span data-stu-id="92ab6-118">Name</span></span>       | <span data-ttu-id="92ab6-119">说明</span><span class="sxs-lookup"><span data-stu-id="92ab6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="92ab6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="92ab6-120">Authorization</span></span>  | <span data-ttu-id="92ab6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92ab6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="92ab6-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="92ab6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="92ab6-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="92ab6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92ab6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="92ab6-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="92ab6-127">响应</span><span class="sxs-lookup"><span data-stu-id="92ab6-127">Response</span></span>

<span data-ttu-id="92ab6-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92ab6-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92ab6-129">示例</span><span class="sxs-lookup"><span data-stu-id="92ab6-129">Example</span></span>
<span data-ttu-id="92ab6-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="92ab6-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="92ab6-131">请求</span><span class="sxs-lookup"><span data-stu-id="92ab6-131">Request</span></span>
<span data-ttu-id="92ab6-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92ab6-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="92ab6-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="92ab6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerow_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/Range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92ab6-134">C#</span><span class="sxs-lookup"><span data-stu-id="92ab6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerow-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92ab6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92ab6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerow-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92ab6-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="92ab6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerow-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="92ab6-137">Java</span><span class="sxs-lookup"><span data-stu-id="92ab6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablerow-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="92ab6-138">响应</span><span class="sxs-lookup"><span data-stu-id="92ab6-138">Response</span></span>
<span data-ttu-id="92ab6-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92ab6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "TableRow: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
