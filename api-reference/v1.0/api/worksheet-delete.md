---
title: 'Worksheet: delete'
description: 从工作簿中删除工作表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d2cfde98485c1f17fa5fe6f08ed8e48e85f855f3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771230"
---
# <a name="worksheet-delete"></a><span data-ttu-id="6a040-103">Worksheet: delete</span><span class="sxs-lookup"><span data-stu-id="6a040-103">Worksheet: delete</span></span>

<span data-ttu-id="6a040-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a040-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a040-105">从工作簿中删除工作表。</span><span class="sxs-lookup"><span data-stu-id="6a040-105">Deletes the worksheet from the workbook.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a040-106">权限</span><span class="sxs-lookup"><span data-stu-id="6a040-106">Permissions</span></span>
<span data-ttu-id="6a040-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a040-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a040-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a040-109">Permission type</span></span>      | <span data-ttu-id="6a040-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a040-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a040-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a040-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6a040-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a040-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6a040-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a040-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a040-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a040-114">Not supported.</span></span>    |
|<span data-ttu-id="6a040-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a040-115">Application</span></span> | <span data-ttu-id="6a040-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a040-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a040-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a040-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="6a040-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a040-118">Request headers</span></span>
| <span data-ttu-id="6a040-119">名称</span><span class="sxs-lookup"><span data-stu-id="6a040-119">Name</span></span>       | <span data-ttu-id="6a040-120">说明</span><span class="sxs-lookup"><span data-stu-id="6a040-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6a040-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a040-121">Authorization</span></span>  | <span data-ttu-id="6a040-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a040-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6a040-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6a040-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="6a040-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6a040-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a040-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a040-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6a040-128">响应</span><span class="sxs-lookup"><span data-stu-id="6a040-128">Response</span></span>

<span data-ttu-id="6a040-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6a040-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a040-131">示例</span><span class="sxs-lookup"><span data-stu-id="6a040-131">Example</span></span>
<span data-ttu-id="6a040-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6a040-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6a040-133">请求</span><span class="sxs-lookup"><span data-stu-id="6a040-133">Request</span></span>
<span data-ttu-id="6a040-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a040-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6a040-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a040-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="6a040-136">C#</span><span class="sxs-lookup"><span data-stu-id="6a040-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a040-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a040-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a040-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a040-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a040-139">Java</span><span class="sxs-lookup"><span data-stu-id="6a040-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6a040-140">响应</span><span class="sxs-lookup"><span data-stu-id="6a040-140">Response</span></span>
<span data-ttu-id="6a040-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6a040-141">Here is an example of the response.</span></span> 
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
  "description": "Worksheet: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

