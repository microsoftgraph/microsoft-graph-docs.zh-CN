---
title: 'Range: delete'
description: 删除与范围相关的单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1b2e7b338a653b8a3e542a29dd69c9c5673ea29a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607657"
---
# <a name="range-delete"></a><span data-ttu-id="0da8e-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="0da8e-103">Range: delete</span></span>

<span data-ttu-id="0da8e-104">删除与范围相关的单元格。</span><span class="sxs-lookup"><span data-stu-id="0da8e-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="0da8e-105">权限</span><span class="sxs-lookup"><span data-stu-id="0da8e-105">Permissions</span></span>
<span data-ttu-id="0da8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0da8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0da8e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0da8e-108">Permission type</span></span>      | <span data-ttu-id="0da8e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0da8e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0da8e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0da8e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0da8e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0da8e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0da8e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0da8e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0da8e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0da8e-113">Not supported.</span></span>    |
|<span data-ttu-id="0da8e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0da8e-114">Application</span></span> | <span data-ttu-id="0da8e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0da8e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0da8e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0da8e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="0da8e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0da8e-117">Request headers</span></span>
| <span data-ttu-id="0da8e-118">名称</span><span class="sxs-lookup"><span data-stu-id="0da8e-118">Name</span></span>       | <span data-ttu-id="0da8e-119">说明</span><span class="sxs-lookup"><span data-stu-id="0da8e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0da8e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0da8e-120">Authorization</span></span>  | <span data-ttu-id="0da8e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0da8e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0da8e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0da8e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0da8e-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0da8e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0da8e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0da8e-126">Request body</span></span>
<span data-ttu-id="0da8e-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0da8e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0da8e-128">参数</span><span class="sxs-lookup"><span data-stu-id="0da8e-128">Parameter</span></span>    | <span data-ttu-id="0da8e-129">类型</span><span class="sxs-lookup"><span data-stu-id="0da8e-129">Type</span></span>   |<span data-ttu-id="0da8e-130">说明</span><span class="sxs-lookup"><span data-stu-id="0da8e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0da8e-131">Shift</span><span class="sxs-lookup"><span data-stu-id="0da8e-131">shift</span></span>|<span data-ttu-id="0da8e-132">string</span><span class="sxs-lookup"><span data-stu-id="0da8e-132">string</span></span>|<span data-ttu-id="0da8e-133">指定移动单元格的方式。</span><span class="sxs-lookup"><span data-stu-id="0da8e-133">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="0da8e-134">可能的值为: `Up`、 `Left`。</span><span class="sxs-lookup"><span data-stu-id="0da8e-134">The possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="0da8e-135">响应</span><span class="sxs-lookup"><span data-stu-id="0da8e-135">Response</span></span>

<span data-ttu-id="0da8e-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0da8e-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0da8e-138">示例</span><span class="sxs-lookup"><span data-stu-id="0da8e-138">Example</span></span>
<span data-ttu-id="0da8e-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="0da8e-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0da8e-140">请求</span><span class="sxs-lookup"><span data-stu-id="0da8e-140">Request</span></span>
<span data-ttu-id="0da8e-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0da8e-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="0da8e-142">响应</span><span class="sxs-lookup"><span data-stu-id="0da8e-142">Response</span></span>
<span data-ttu-id="0da8e-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0da8e-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0da8e-144">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0da8e-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0da8e-145">语言</span><span class="sxs-lookup"><span data-stu-id="0da8e-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0da8e-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="0da8e-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_delete-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
