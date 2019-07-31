---
title: TableColumn:Range
description: 获取与整个列相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5a56f2896f6d913b4780f389b2f3df891aa2a595
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990979"
---
# <a name="tablecolumn-range"></a><span data-ttu-id="b579f-103">TableColumn:Range</span><span class="sxs-lookup"><span data-stu-id="b579f-103">TableColumn: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b579f-104">获取与整个列相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="b579f-104">Gets the range object associated with the entire column.</span></span>
## <a name="permissions"></a><span data-ttu-id="b579f-105">权限</span><span class="sxs-lookup"><span data-stu-id="b579f-105">Permissions</span></span>
<span data-ttu-id="b579f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b579f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b579f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b579f-108">Permission type</span></span>      | <span data-ttu-id="b579f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b579f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b579f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b579f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b579f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b579f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b579f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b579f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b579f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b579f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b579f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b579f-114">Application</span></span> | <span data-ttu-id="b579f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b579f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b579f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b579f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/Range
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="b579f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b579f-117">Request headers</span></span>
| <span data-ttu-id="b579f-118">名称</span><span class="sxs-lookup"><span data-stu-id="b579f-118">Name</span></span>       | <span data-ttu-id="b579f-119">说明</span><span class="sxs-lookup"><span data-stu-id="b579f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b579f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b579f-120">Authorization</span></span>  | <span data-ttu-id="b579f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b579f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b579f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b579f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b579f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="b579f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b579f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b579f-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b579f-127">响应</span><span class="sxs-lookup"><span data-stu-id="b579f-127">Response</span></span>

<span data-ttu-id="b579f-128">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[workbookRange](../resources/workbookrange.md)) 对象。</span><span class="sxs-lookup"><span data-stu-id="b579f-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md)) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b579f-129">示例</span><span class="sxs-lookup"><span data-stu-id="b579f-129">Example</span></span>
<span data-ttu-id="b579f-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b579f-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b579f-131">请求</span><span class="sxs-lookup"><span data-stu-id="b579f-131">Request</span></span>
<span data-ttu-id="b579f-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b579f-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b579f-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b579f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumn_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/Range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b579f-134">C#</span><span class="sxs-lookup"><span data-stu-id="b579f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b579f-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="b579f-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b579f-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="b579f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b579f-137">Java</span><span class="sxs-lookup"><span data-stu-id="b579f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumn-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b579f-138">响应</span><span class="sxs-lookup"><span data-stu-id="b579f-138">Response</span></span>
<span data-ttu-id="b579f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b579f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
