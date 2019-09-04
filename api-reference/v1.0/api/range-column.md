---
title: Range:Column
description: 获取范围中包含的列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fa3c54928498b3cad7aeb70666436e1bd4fbcb5c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728417"
---
# <a name="range-column"></a><span data-ttu-id="7c4cd-103">Range:Column</span><span class="sxs-lookup"><span data-stu-id="7c4cd-103">Range: Column</span></span>

<span data-ttu-id="7c4cd-104">获取范围中包含的列。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c4cd-105">权限</span><span class="sxs-lookup"><span data-stu-id="7c4cd-105">Permissions</span></span>
<span data-ttu-id="7c4cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c4cd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c4cd-108">Permission type</span></span>      | <span data-ttu-id="7c4cd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c4cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c4cd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c4cd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c4cd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c4cd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c4cd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c4cd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c4cd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-113">Not supported.</span></span>    |
|<span data-ttu-id="7c4cd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c4cd-114">Application</span></span> | <span data-ttu-id="7c4cd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c4cd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c4cd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="7c4cd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c4cd-117">Request headers</span></span>
| <span data-ttu-id="7c4cd-118">名称</span><span class="sxs-lookup"><span data-stu-id="7c4cd-118">Name</span></span>       | <span data-ttu-id="7c4cd-119">说明</span><span class="sxs-lookup"><span data-stu-id="7c4cd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c4cd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c4cd-120">Authorization</span></span>  | <span data-ttu-id="7c4cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c4cd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7c4cd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7c4cd-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="7c4cd-126">路径参数</span><span class="sxs-lookup"><span data-stu-id="7c4cd-126">Path parameters</span></span>
<span data-ttu-id="7c4cd-127">在请求路径中, 提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-127">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="7c4cd-128">参数</span><span class="sxs-lookup"><span data-stu-id="7c4cd-128">Parameter</span></span>    | <span data-ttu-id="7c4cd-129">类型</span><span class="sxs-lookup"><span data-stu-id="7c4cd-129">Type</span></span>   |<span data-ttu-id="7c4cd-130">说明</span><span class="sxs-lookup"><span data-stu-id="7c4cd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c4cd-131">column</span><span class="sxs-lookup"><span data-stu-id="7c4cd-131">column</span></span>|<span data-ttu-id="7c4cd-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7c4cd-132">Int32</span></span>|<span data-ttu-id="7c4cd-p104">要检索的区域的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="7c4cd-135">响应</span><span class="sxs-lookup"><span data-stu-id="7c4cd-135">Response</span></span>

<span data-ttu-id="7c4cd-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c4cd-137">示例</span><span class="sxs-lookup"><span data-stu-id="7c4cd-137">Example</span></span>
<span data-ttu-id="7c4cd-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7c4cd-139">请求</span><span class="sxs-lookup"><span data-stu-id="7c4cd-139">Request</span></span>
<span data-ttu-id="7c4cd-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7c4cd-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7c4cd-141">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7c4cd-142">C#</span><span class="sxs-lookup"><span data-stu-id="7c4cd-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c4cd-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c4cd-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7c4cd-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="7c4cd-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7c4cd-145">Java</span><span class="sxs-lookup"><span data-stu-id="7c4cd-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7c4cd-146">响应</span><span class="sxs-lookup"><span data-stu-id="7c4cd-146">Response</span></span>
<span data-ttu-id="7c4cd-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c4cd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
