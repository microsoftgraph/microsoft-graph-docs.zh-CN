---
title: Table:HeaderRowRange
description: 获取与表的标头行相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d1bb69d94ef1d85173bd2bbd1a6ad331c588d0f5
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578750"
---
# <a name="table-headerrowrange"></a><span data-ttu-id="9cb24-103">Table:HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="9cb24-103">Table: HeaderRowRange</span></span>

<span data-ttu-id="9cb24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cb24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9cb24-105">获取与表的标头行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="9cb24-105">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="9cb24-106">权限</span><span class="sxs-lookup"><span data-stu-id="9cb24-106">Permissions</span></span>
<span data-ttu-id="9cb24-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cb24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cb24-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cb24-109">Permission type</span></span>      | <span data-ttu-id="9cb24-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cb24-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cb24-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cb24-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9cb24-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cb24-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9cb24-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cb24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cb24-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cb24-114">Not supported.</span></span>    |
|<span data-ttu-id="9cb24-115">Application</span><span class="sxs-lookup"><span data-stu-id="9cb24-115">Application</span></span> | <span data-ttu-id="9cb24-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cb24-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cb24-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cb24-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/headerRowRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/headerRowRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/headerRowRange

```
## <a name="request-headers"></a><span data-ttu-id="9cb24-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cb24-118">Request headers</span></span>
| <span data-ttu-id="9cb24-119">名称</span><span class="sxs-lookup"><span data-stu-id="9cb24-119">Name</span></span>       | <span data-ttu-id="9cb24-120">说明</span><span class="sxs-lookup"><span data-stu-id="9cb24-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9cb24-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cb24-121">Authorization</span></span>  | <span data-ttu-id="9cb24-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cb24-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9cb24-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9cb24-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9cb24-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9cb24-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cb24-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cb24-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9cb24-128">响应</span><span class="sxs-lookup"><span data-stu-id="9cb24-128">Response</span></span>

<span data-ttu-id="9cb24-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9cb24-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cb24-130">示例</span><span class="sxs-lookup"><span data-stu-id="9cb24-130">Example</span></span>
<span data-ttu-id="9cb24-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9cb24-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9cb24-132">请求</span><span class="sxs-lookup"><span data-stu-id="9cb24-132">Request</span></span>
<span data-ttu-id="9cb24-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9cb24-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9cb24-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cb24-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_headerrowrange",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange
```
# <a name="c"></a>[<span data-ttu-id="9cb24-135">C#</span><span class="sxs-lookup"><span data-stu-id="9cb24-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-headerrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cb24-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cb24-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-headerrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cb24-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cb24-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-headerrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cb24-138">Java</span><span class="sxs-lookup"><span data-stu-id="9cb24-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-headerrowrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9cb24-139">响应</span><span class="sxs-lookup"><span data-stu-id="9cb24-139">Response</span></span>
<span data-ttu-id="9cb24-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9cb24-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

