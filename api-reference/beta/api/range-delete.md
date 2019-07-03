---
title: 'Range: delete'
description: 删除与范围相关的单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 47dfca5e45a00522188b5806528632db0a9139cf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447171"
---
# <a name="range-delete"></a><span data-ttu-id="583a9-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="583a9-103">Range: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="583a9-104">删除与范围相关的单元格。</span><span class="sxs-lookup"><span data-stu-id="583a9-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="583a9-105">权限</span><span class="sxs-lookup"><span data-stu-id="583a9-105">Permissions</span></span>
<span data-ttu-id="583a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="583a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="583a9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="583a9-108">Permission type</span></span>      | <span data-ttu-id="583a9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="583a9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="583a9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="583a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="583a9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="583a9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="583a9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="583a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="583a9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="583a9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="583a9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="583a9-114">Application</span></span> | <span data-ttu-id="583a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="583a9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="583a9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="583a9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="583a9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="583a9-117">Request headers</span></span>
| <span data-ttu-id="583a9-118">名称</span><span class="sxs-lookup"><span data-stu-id="583a9-118">Name</span></span>       | <span data-ttu-id="583a9-119">说明</span><span class="sxs-lookup"><span data-stu-id="583a9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="583a9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="583a9-120">Authorization</span></span>  | <span data-ttu-id="583a9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="583a9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="583a9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="583a9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="583a9-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="583a9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="583a9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="583a9-126">Request body</span></span>
<span data-ttu-id="583a9-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="583a9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="583a9-128">参数</span><span class="sxs-lookup"><span data-stu-id="583a9-128">Parameter</span></span>    | <span data-ttu-id="583a9-129">类型</span><span class="sxs-lookup"><span data-stu-id="583a9-129">Type</span></span>   |<span data-ttu-id="583a9-130">说明</span><span class="sxs-lookup"><span data-stu-id="583a9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="583a9-131">Shift</span><span class="sxs-lookup"><span data-stu-id="583a9-131">shift</span></span>|<span data-ttu-id="583a9-132">string</span><span class="sxs-lookup"><span data-stu-id="583a9-132">string</span></span>|<span data-ttu-id="583a9-p104">指定移动单元格的方式。可能的值是：`Up`、`Left`。</span><span class="sxs-lookup"><span data-stu-id="583a9-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="583a9-135">响应</span><span class="sxs-lookup"><span data-stu-id="583a9-135">Response</span></span>

<span data-ttu-id="583a9-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="583a9-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="583a9-138">示例</span><span class="sxs-lookup"><span data-stu-id="583a9-138">Example</span></span>
<span data-ttu-id="583a9-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="583a9-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="583a9-140">请求</span><span class="sxs-lookup"><span data-stu-id="583a9-140">Request</span></span>
<span data-ttu-id="583a9-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="583a9-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="583a9-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="583a9-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="583a9-143">C#</span><span class="sxs-lookup"><span data-stu-id="583a9-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="583a9-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="583a9-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="583a9-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="583a9-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="583a9-146">响应</span><span class="sxs-lookup"><span data-stu-id="583a9-146">Response</span></span>
<span data-ttu-id="583a9-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="583a9-147">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
