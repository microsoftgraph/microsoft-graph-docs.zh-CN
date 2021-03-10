---
title: Range:LastCell
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a9f87a1d0546736530102e37fd8f74d792e48bd1
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577728"
---
# <a name="range-lastcell"></a><span data-ttu-id="e645e-103">Range:LastCell</span><span class="sxs-lookup"><span data-stu-id="e645e-103">Range: LastCell</span></span>

<span data-ttu-id="e645e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e645e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e645e-p101">获取区域内的最后一个单元格。例如，“B2:D5”的最后一个单元格是“D5”。</span><span class="sxs-lookup"><span data-stu-id="e645e-p101">Gets the last cell within the range. For example, the last cell of "B2:D5" is "D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="e645e-107">权限</span><span class="sxs-lookup"><span data-stu-id="e645e-107">Permissions</span></span>
<span data-ttu-id="e645e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e645e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e645e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e645e-110">Permission type</span></span>      | <span data-ttu-id="e645e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e645e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e645e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e645e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e645e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e645e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e645e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e645e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e645e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e645e-115">Not supported.</span></span>    |
|<span data-ttu-id="e645e-116">Application</span><span class="sxs-lookup"><span data-stu-id="e645e-116">Application</span></span> | <span data-ttu-id="e645e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e645e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e645e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e645e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/lastCell
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/lastCell
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/lastCell
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/lastCell
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/lastCell
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/lastCell

```
## <a name="request-headers"></a><span data-ttu-id="e645e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e645e-119">Request headers</span></span>
| <span data-ttu-id="e645e-120">名称</span><span class="sxs-lookup"><span data-stu-id="e645e-120">Name</span></span>       | <span data-ttu-id="e645e-121">说明</span><span class="sxs-lookup"><span data-stu-id="e645e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e645e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e645e-122">Authorization</span></span>  | <span data-ttu-id="e645e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e645e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e645e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e645e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e645e-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e645e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e645e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e645e-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e645e-129">响应</span><span class="sxs-lookup"><span data-stu-id="e645e-129">Response</span></span>

<span data-ttu-id="e645e-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e645e-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e645e-131">示例</span><span class="sxs-lookup"><span data-stu-id="e645e-131">Example</span></span>
<span data-ttu-id="e645e-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e645e-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e645e-133">请求</span><span class="sxs-lookup"><span data-stu-id="e645e-133">Request</span></span>
<span data-ttu-id="e645e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e645e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e645e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e645e-135">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastcell"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastCell
```
# <a name="c"></a>[<span data-ttu-id="e645e-136">C#</span><span class="sxs-lookup"><span data-stu-id="e645e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastcell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e645e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e645e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastcell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e645e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e645e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastcell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e645e-139">Java</span><span class="sxs-lookup"><span data-stu-id="e645e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-lastcell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e645e-140">响应</span><span class="sxs-lookup"><span data-stu-id="e645e-140">Response</span></span>
<span data-ttu-id="e645e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e645e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastCell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

