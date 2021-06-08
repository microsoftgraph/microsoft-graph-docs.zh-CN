---
title: 'Range: unmerge'
description: 将范围单元格取消合并为各个单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d5958121e761c17f5acb6cebebe154eac4cee66c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785898"
---
# <a name="range-unmerge"></a><span data-ttu-id="7faed-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="7faed-103">Range: unmerge</span></span>

<span data-ttu-id="7faed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7faed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7faed-105">将范围单元格取消合并为各个单元格。</span><span class="sxs-lookup"><span data-stu-id="7faed-105">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="7faed-106">权限</span><span class="sxs-lookup"><span data-stu-id="7faed-106">Permissions</span></span>
<span data-ttu-id="7faed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7faed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7faed-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7faed-109">Permission type</span></span>      | <span data-ttu-id="7faed-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7faed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7faed-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7faed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7faed-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7faed-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7faed-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7faed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7faed-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7faed-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7faed-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7faed-115">Application</span></span> | <span data-ttu-id="7faed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7faed-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7faed-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7faed-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/unmerge
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/unmerge
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/unmerge
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="7faed-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7faed-118">Request headers</span></span>
| <span data-ttu-id="7faed-119">名称</span><span class="sxs-lookup"><span data-stu-id="7faed-119">Name</span></span>       | <span data-ttu-id="7faed-120">说明</span><span class="sxs-lookup"><span data-stu-id="7faed-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7faed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7faed-121">Authorization</span></span>  | <span data-ttu-id="7faed-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7faed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7faed-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7faed-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7faed-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7faed-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7faed-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7faed-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7faed-128">响应</span><span class="sxs-lookup"><span data-stu-id="7faed-128">Response</span></span>

<span data-ttu-id="7faed-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7faed-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7faed-131">示例</span><span class="sxs-lookup"><span data-stu-id="7faed-131">Example</span></span>
<span data-ttu-id="7faed-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7faed-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7faed-133">请求</span><span class="sxs-lookup"><span data-stu-id="7faed-133">Request</span></span>
<span data-ttu-id="7faed-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7faed-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7faed-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7faed-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/unmerge
```
# <a name="c"></a>[<span data-ttu-id="7faed-136">C#</span><span class="sxs-lookup"><span data-stu-id="7faed-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-unmerge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7faed-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7faed-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-unmerge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7faed-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7faed-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-unmerge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7faed-139">Java</span><span class="sxs-lookup"><span data-stu-id="7faed-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-unmerge-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7faed-140">响应</span><span class="sxs-lookup"><span data-stu-id="7faed-140">Response</span></span>
<span data-ttu-id="7faed-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7faed-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: unmerge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


