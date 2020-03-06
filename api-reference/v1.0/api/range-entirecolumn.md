---
title: Range:EntireColumn
description: 获取表示范围整列的对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6972b4ce44b5cebe7f79958f93996a3ac3b0a730
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510660"
---
# <a name="range-entirecolumn"></a><span data-ttu-id="521cc-103">Range:EntireColumn</span><span class="sxs-lookup"><span data-stu-id="521cc-103">Range: EntireColumn</span></span>

<span data-ttu-id="521cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="521cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="521cc-105">获取表示范围整列的对象。</span><span class="sxs-lookup"><span data-stu-id="521cc-105">Gets an object that represents the entire column of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="521cc-106">权限</span><span class="sxs-lookup"><span data-stu-id="521cc-106">Permissions</span></span>
<span data-ttu-id="521cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="521cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="521cc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="521cc-109">Permission type</span></span>      | <span data-ttu-id="521cc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="521cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="521cc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="521cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="521cc-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="521cc-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="521cc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="521cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="521cc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="521cc-114">Not supported.</span></span>    |
|<span data-ttu-id="521cc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="521cc-115">Application</span></span> | <span data-ttu-id="521cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="521cc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="521cc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="521cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/entireColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/entireColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/entireColumn

```
## <a name="request-headers"></a><span data-ttu-id="521cc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="521cc-118">Request headers</span></span>
| <span data-ttu-id="521cc-119">名称</span><span class="sxs-lookup"><span data-stu-id="521cc-119">Name</span></span>       | <span data-ttu-id="521cc-120">说明</span><span class="sxs-lookup"><span data-stu-id="521cc-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="521cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="521cc-121">Authorization</span></span>  | <span data-ttu-id="521cc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="521cc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="521cc-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="521cc-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="521cc-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="521cc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="521cc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="521cc-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="521cc-128">响应</span><span class="sxs-lookup"><span data-stu-id="521cc-128">Response</span></span>

<span data-ttu-id="521cc-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="521cc-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="521cc-130">示例</span><span class="sxs-lookup"><span data-stu-id="521cc-130">Example</span></span>
<span data-ttu-id="521cc-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="521cc-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="521cc-132">请求</span><span class="sxs-lookup"><span data-stu-id="521cc-132">Request</span></span>
<span data-ttu-id="521cc-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="521cc-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="521cc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="521cc-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_entirecolumn"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/entireColumn
```
# <a name="c"></a>[<span data-ttu-id="521cc-135">C#</span><span class="sxs-lookup"><span data-stu-id="521cc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-entirecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="521cc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="521cc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-entirecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="521cc-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="521cc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-entirecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="521cc-138">Java</span><span class="sxs-lookup"><span data-stu-id="521cc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-entirecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="521cc-139">响应</span><span class="sxs-lookup"><span data-stu-id="521cc-139">Response</span></span>
<span data-ttu-id="521cc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="521cc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: EntireColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
