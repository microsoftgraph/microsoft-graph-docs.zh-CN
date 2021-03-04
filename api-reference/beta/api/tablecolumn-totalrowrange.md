---
title: 'TableColumn: TotalRowRange'
description: 获取与列的总计行相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f72017881e1072033f4e6f222bd8725d8d3c2a06
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440624"
---
# <a name="tablecolumn-totalrowrange"></a><span data-ttu-id="5cbc8-103">TableColumn: TotalRowRange</span><span class="sxs-lookup"><span data-stu-id="5cbc8-103">TableColumn: TotalRowRange</span></span>

<span data-ttu-id="5cbc8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cbc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cbc8-105">获取与列的总计行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="5cbc8-105">Gets the range object associated with the totals row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="5cbc8-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5cbc8-106">Permissions</span></span>
<span data-ttu-id="5cbc8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5cbc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cbc8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cbc8-109">Permission type</span></span>      | <span data-ttu-id="5cbc8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5cbc8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cbc8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cbc8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5cbc8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cbc8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5cbc8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5cbc8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cbc8-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cbc8-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5cbc8-115">Application</span><span class="sxs-lookup"><span data-stu-id="5cbc8-115">Application</span></span> | <span data-ttu-id="5cbc8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cbc8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cbc8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cbc8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns/{id|name}/TotalRowRange
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/TotalRowRange

```
## <a name="request-headers"></a><span data-ttu-id="5cbc8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cbc8-118">Request headers</span></span>
| <span data-ttu-id="5cbc8-119">名称</span><span class="sxs-lookup"><span data-stu-id="5cbc8-119">Name</span></span>       | <span data-ttu-id="5cbc8-120">说明</span><span class="sxs-lookup"><span data-stu-id="5cbc8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5cbc8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cbc8-121">Authorization</span></span>  | <span data-ttu-id="5cbc8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5cbc8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5cbc8-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5cbc8-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5cbc8-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5cbc8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cbc8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cbc8-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5cbc8-128">响应</span><span class="sxs-lookup"><span data-stu-id="5cbc8-128">Response</span></span>

<span data-ttu-id="5cbc8-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5cbc8-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cbc8-130">示例</span><span class="sxs-lookup"><span data-stu-id="5cbc8-130">Example</span></span>
<span data-ttu-id="5cbc8-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5cbc8-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5cbc8-132">请求</span><span class="sxs-lookup"><span data-stu-id="5cbc8-132">Request</span></span>
<span data-ttu-id="5cbc8-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5cbc8-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5cbc8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5cbc8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumn_totalrowrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/TotalRowRange
```
# <a name="c"></a>[<span data-ttu-id="5cbc8-135">C#</span><span class="sxs-lookup"><span data-stu-id="5cbc8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-totalrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5cbc8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5cbc8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-totalrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5cbc8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5cbc8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-totalrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5cbc8-138">Java</span><span class="sxs-lookup"><span data-stu-id="5cbc8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumn-totalrowrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5cbc8-139">响应</span><span class="sxs-lookup"><span data-stu-id="5cbc8-139">Response</span></span>
<span data-ttu-id="5cbc8-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5cbc8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: TotalRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


