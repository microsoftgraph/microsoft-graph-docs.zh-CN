---
title: 'TableSort: clear'
description: 清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c039cd79e852a4d3531be808ab83d6a2254e97a6
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578743"
---
# <a name="tablesort-clear"></a><span data-ttu-id="df05f-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="df05f-104">TableSort: clear</span></span>

<span data-ttu-id="df05f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df05f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df05f-p102">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="df05f-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="df05f-108">权限</span><span class="sxs-lookup"><span data-stu-id="df05f-108">Permissions</span></span>
<span data-ttu-id="df05f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df05f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df05f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df05f-111">Permission type</span></span>      | <span data-ttu-id="df05f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df05f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df05f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df05f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="df05f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df05f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="df05f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df05f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df05f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df05f-116">Not supported.</span></span>    |
|<span data-ttu-id="df05f-117">Application</span><span class="sxs-lookup"><span data-stu-id="df05f-117">Application</span></span> | <span data-ttu-id="df05f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="df05f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df05f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df05f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="df05f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df05f-120">Request headers</span></span>
| <span data-ttu-id="df05f-121">名称</span><span class="sxs-lookup"><span data-stu-id="df05f-121">Name</span></span>       | <span data-ttu-id="df05f-122">说明</span><span class="sxs-lookup"><span data-stu-id="df05f-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="df05f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df05f-123">Authorization</span></span>  | <span data-ttu-id="df05f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df05f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="df05f-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="df05f-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="df05f-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="df05f-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df05f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="df05f-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="df05f-130">响应</span><span class="sxs-lookup"><span data-stu-id="df05f-130">Response</span></span>

<span data-ttu-id="df05f-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="df05f-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df05f-133">示例</span><span class="sxs-lookup"><span data-stu-id="df05f-133">Example</span></span>
<span data-ttu-id="df05f-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="df05f-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="df05f-135">请求</span><span class="sxs-lookup"><span data-stu-id="df05f-135">Request</span></span>
<span data-ttu-id="df05f-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df05f-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df05f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="df05f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="c"></a>[<span data-ttu-id="df05f-138">C#</span><span class="sxs-lookup"><span data-stu-id="df05f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df05f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df05f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df05f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df05f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df05f-141">Java</span><span class="sxs-lookup"><span data-stu-id="df05f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="df05f-142">响应</span><span class="sxs-lookup"><span data-stu-id="df05f-142">Response</span></span>
<span data-ttu-id="df05f-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="df05f-143">Here is an example of the response.</span></span> 
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

