---
title: 'Range: delete'
description: 删除与范围相关的单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1900ae6f02414d177f2aea5a90d9c5d940cc6792
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454767"
---
# <a name="range-delete"></a><span data-ttu-id="8c708-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="8c708-103">Range: delete</span></span>

<span data-ttu-id="8c708-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8c708-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c708-105">删除与范围相关的单元格。</span><span class="sxs-lookup"><span data-stu-id="8c708-105">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c708-106">权限</span><span class="sxs-lookup"><span data-stu-id="8c708-106">Permissions</span></span>
<span data-ttu-id="8c708-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c708-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c708-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c708-109">Permission type</span></span>      | <span data-ttu-id="8c708-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c708-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c708-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c708-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8c708-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c708-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c708-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c708-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c708-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c708-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c708-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c708-115">Application</span></span> | <span data-ttu-id="8c708-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c708-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c708-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c708-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="8c708-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c708-118">Request headers</span></span>
| <span data-ttu-id="8c708-119">名称</span><span class="sxs-lookup"><span data-stu-id="8c708-119">Name</span></span>       | <span data-ttu-id="8c708-120">说明</span><span class="sxs-lookup"><span data-stu-id="8c708-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c708-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c708-121">Authorization</span></span>  | <span data-ttu-id="8c708-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c708-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c708-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8c708-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="8c708-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8c708-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c708-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c708-127">Request body</span></span>
<span data-ttu-id="8c708-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8c708-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c708-129">参数</span><span class="sxs-lookup"><span data-stu-id="8c708-129">Parameter</span></span>    | <span data-ttu-id="8c708-130">类型</span><span class="sxs-lookup"><span data-stu-id="8c708-130">Type</span></span>   |<span data-ttu-id="8c708-131">说明</span><span class="sxs-lookup"><span data-stu-id="8c708-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c708-132">Shift</span><span class="sxs-lookup"><span data-stu-id="8c708-132">shift</span></span>|<span data-ttu-id="8c708-133">string</span><span class="sxs-lookup"><span data-stu-id="8c708-133">string</span></span>|<span data-ttu-id="8c708-p104">指定移动单元格的方式。可能的值是：`Up`、`Left`。</span><span class="sxs-lookup"><span data-stu-id="8c708-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="8c708-136">响应</span><span class="sxs-lookup"><span data-stu-id="8c708-136">Response</span></span>

<span data-ttu-id="8c708-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8c708-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c708-139">示例</span><span class="sxs-lookup"><span data-stu-id="8c708-139">Example</span></span>
<span data-ttu-id="8c708-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8c708-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8c708-141">请求</span><span class="sxs-lookup"><span data-stu-id="8c708-141">Request</span></span>
<span data-ttu-id="8c708-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c708-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c708-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c708-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8c708-144">C#</span><span class="sxs-lookup"><span data-stu-id="8c708-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c708-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c708-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c708-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c708-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8c708-147">响应</span><span class="sxs-lookup"><span data-stu-id="8c708-147">Response</span></span>
<span data-ttu-id="8c708-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8c708-148">Here is an example of the response.</span></span> 
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
