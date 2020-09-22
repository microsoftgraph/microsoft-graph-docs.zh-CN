---
title: 'TableSort: clear'
description: 清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 32eff7c8f1621cc67bb46b861778c9bbf9a146e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978580"
---
# <a name="tablesort-clear"></a><span data-ttu-id="4e27b-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="4e27b-104">TableSort: clear</span></span>

<span data-ttu-id="4e27b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e27b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e27b-p102">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="4e27b-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="4e27b-108">权限</span><span class="sxs-lookup"><span data-stu-id="4e27b-108">Permissions</span></span>
<span data-ttu-id="4e27b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e27b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e27b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e27b-111">Permission type</span></span>      | <span data-ttu-id="4e27b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e27b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e27b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e27b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4e27b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e27b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4e27b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e27b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e27b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e27b-116">Not supported.</span></span>    |
|<span data-ttu-id="4e27b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e27b-117">Application</span></span> | <span data-ttu-id="4e27b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e27b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e27b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e27b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="4e27b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e27b-120">Request headers</span></span>
| <span data-ttu-id="4e27b-121">名称</span><span class="sxs-lookup"><span data-stu-id="4e27b-121">Name</span></span>       | <span data-ttu-id="4e27b-122">说明</span><span class="sxs-lookup"><span data-stu-id="4e27b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4e27b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e27b-123">Authorization</span></span>  | <span data-ttu-id="4e27b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e27b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e27b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4e27b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="4e27b-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="4e27b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e27b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e27b-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4e27b-130">响应</span><span class="sxs-lookup"><span data-stu-id="4e27b-130">Response</span></span>

<span data-ttu-id="4e27b-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4e27b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e27b-133">示例</span><span class="sxs-lookup"><span data-stu-id="4e27b-133">Example</span></span>
<span data-ttu-id="4e27b-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4e27b-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4e27b-135">请求</span><span class="sxs-lookup"><span data-stu-id="4e27b-135">Request</span></span>
<span data-ttu-id="4e27b-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e27b-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e27b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e27b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="c"></a>[<span data-ttu-id="4e27b-138">C#</span><span class="sxs-lookup"><span data-stu-id="4e27b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e27b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e27b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e27b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e27b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e27b-141">Java</span><span class="sxs-lookup"><span data-stu-id="4e27b-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4e27b-142">响应</span><span class="sxs-lookup"><span data-stu-id="4e27b-142">Response</span></span>
<span data-ttu-id="4e27b-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4e27b-143">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

