---
title: workbookTable： range
description: 获取与整个表相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6ba01f948a6b21dc2b53c52682f92f428bb2df95
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576520"
---
# <a name="workbooktable-range"></a><span data-ttu-id="1332e-103">workbookTable： range</span><span class="sxs-lookup"><span data-stu-id="1332e-103">workbookTable: range</span></span>

<span data-ttu-id="1332e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1332e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1332e-105">获取与整个表相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="1332e-105">Gets the range object associated with the entire table.</span></span>
## <a name="permissions"></a><span data-ttu-id="1332e-106">权限</span><span class="sxs-lookup"><span data-stu-id="1332e-106">Permissions</span></span>
<span data-ttu-id="1332e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1332e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1332e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1332e-109">Permission type</span></span>      | <span data-ttu-id="1332e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1332e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1332e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1332e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1332e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1332e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1332e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1332e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1332e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1332e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1332e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1332e-115">Application</span></span> | <span data-ttu-id="1332e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1332e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1332e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1332e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/Range
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/Range
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/Range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="1332e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1332e-118">Request headers</span></span>
| <span data-ttu-id="1332e-119">名称</span><span class="sxs-lookup"><span data-stu-id="1332e-119">Name</span></span>       | <span data-ttu-id="1332e-120">说明</span><span class="sxs-lookup"><span data-stu-id="1332e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1332e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1332e-121">Authorization</span></span>  | <span data-ttu-id="1332e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1332e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1332e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1332e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1332e-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1332e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1332e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1332e-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1332e-128">响应</span><span class="sxs-lookup"><span data-stu-id="1332e-128">Response</span></span>

<span data-ttu-id="1332e-129">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1332e-129">If successful, this method returns a `200 OK` response code and a [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1332e-130">示例</span><span class="sxs-lookup"><span data-stu-id="1332e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1332e-131">请求</span><span class="sxs-lookup"><span data-stu-id="1332e-131">Request</span></span>
<span data-ttu-id="1332e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1332e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1332e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1332e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/Range
```
# <a name="c"></a>[<span data-ttu-id="1332e-134">C#</span><span class="sxs-lookup"><span data-stu-id="1332e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1332e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1332e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1332e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1332e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1332e-137">Java</span><span class="sxs-lookup"><span data-stu-id="1332e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1332e-138">响应</span><span class="sxs-lookup"><span data-stu-id="1332e-138">Response</span></span>
<span data-ttu-id="1332e-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1332e-139">The following is an example of the response.</span></span> 

><span data-ttu-id="1332e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1332e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Table: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


