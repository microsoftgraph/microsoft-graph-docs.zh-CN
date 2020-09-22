---
title: 'TableSort: reapply'
description: 对表重新应用当前的排序参数。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7a279160b966bca86aea70f376cdd50c3b138441
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032857"
---
# <a name="tablesort-reapply"></a><span data-ttu-id="90f12-103">TableSort: reapply</span><span class="sxs-lookup"><span data-stu-id="90f12-103">TableSort: reapply</span></span>

<span data-ttu-id="90f12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90f12-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90f12-105">对表重新应用当前的排序参数。</span><span class="sxs-lookup"><span data-stu-id="90f12-105">Reapplies the current sorting parameters to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="90f12-106">权限</span><span class="sxs-lookup"><span data-stu-id="90f12-106">Permissions</span></span>
<span data-ttu-id="90f12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90f12-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="90f12-109">Permission type</span></span>      | <span data-ttu-id="90f12-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90f12-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90f12-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90f12-111">Delegated (work or school account)</span></span> | <span data-ttu-id="90f12-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90f12-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90f12-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90f12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90f12-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="90f12-114">Not supported.</span></span>    |
|<span data-ttu-id="90f12-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="90f12-115">Application</span></span> | <span data-ttu-id="90f12-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90f12-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90f12-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90f12-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/reapply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/reapply

```
## <a name="request-headers"></a><span data-ttu-id="90f12-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="90f12-118">Request headers</span></span>
| <span data-ttu-id="90f12-119">名称</span><span class="sxs-lookup"><span data-stu-id="90f12-119">Name</span></span>       | <span data-ttu-id="90f12-120">说明</span><span class="sxs-lookup"><span data-stu-id="90f12-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="90f12-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90f12-121">Authorization</span></span>  | <span data-ttu-id="90f12-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90f12-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90f12-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="90f12-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="90f12-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="90f12-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90f12-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="90f12-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="90f12-128">响应</span><span class="sxs-lookup"><span data-stu-id="90f12-128">Response</span></span>

<span data-ttu-id="90f12-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="90f12-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90f12-131">示例</span><span class="sxs-lookup"><span data-stu-id="90f12-131">Example</span></span>
<span data-ttu-id="90f12-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="90f12-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="90f12-133">请求</span><span class="sxs-lookup"><span data-stu-id="90f12-133">Request</span></span>
<span data-ttu-id="90f12-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90f12-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90f12-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="90f12-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_reapply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply
```
# <a name="c"></a>[<span data-ttu-id="90f12-136">C#</span><span class="sxs-lookup"><span data-stu-id="90f12-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-reapply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90f12-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90f12-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-reapply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90f12-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90f12-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-reapply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90f12-139">Java</span><span class="sxs-lookup"><span data-stu-id="90f12-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-reapply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="90f12-140">响应</span><span class="sxs-lookup"><span data-stu-id="90f12-140">Response</span></span>
<span data-ttu-id="90f12-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="90f12-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort: reapply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

