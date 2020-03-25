---
title: 删除打印机
description: 删除（注销）打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4f77c6564e321c1e250f89547e7dabad5d1305db
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948031"
---
# <a name="delete-printer"></a><span data-ttu-id="9cac7-103">删除打印机</span><span class="sxs-lookup"><span data-stu-id="9cac7-103">Delete printer</span></span>

<span data-ttu-id="9cac7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cac7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cac7-105">删除（注销）[打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="9cac7-105">Delete (unregister) a [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9cac7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9cac7-106">Permissions</span></span>
<span data-ttu-id="9cac7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cac7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9cac7-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="9cac7-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="9cac7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cac7-110">Permission type</span></span> | <span data-ttu-id="9cac7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cac7-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9cac7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cac7-112">Delegated (work or school account)</span></span>| <span data-ttu-id="9cac7-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="9cac7-113">Users.Read.All</span></span> |
|<span data-ttu-id="9cac7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cac7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cac7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cac7-115">Not Supported.</span></span>|
|<span data-ttu-id="9cac7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cac7-116">Application</span></span>|<span data-ttu-id="9cac7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cac7-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cac7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cac7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9cac7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cac7-119">Request headers</span></span>
| <span data-ttu-id="9cac7-120">名称</span><span class="sxs-lookup"><span data-stu-id="9cac7-120">Name</span></span>          | <span data-ttu-id="9cac7-121">说明</span><span class="sxs-lookup"><span data-stu-id="9cac7-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9cac7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cac7-122">Authorization</span></span> | <span data-ttu-id="9cac7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cac7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cac7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cac7-125">Request body</span></span>
<span data-ttu-id="9cac7-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cac7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cac7-127">响应</span><span class="sxs-lookup"><span data-stu-id="9cac7-127">Response</span></span>
<span data-ttu-id="9cac7-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9cac7-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cac7-130">示例</span><span class="sxs-lookup"><span data-stu-id="9cac7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cac7-131">请求</span><span class="sxs-lookup"><span data-stu-id="9cac7-131">Request</span></span>
<span data-ttu-id="9cac7-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cac7-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9cac7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cac7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printer"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="9cac7-134">C#</span><span class="sxs-lookup"><span data-stu-id="9cac7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cac7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cac7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cac7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cac7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9cac7-137">响应</span><span class="sxs-lookup"><span data-stu-id="9cac7-137">Response</span></span>
<span data-ttu-id="9cac7-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9cac7-138">The following is an example of the response.</span></span>
><span data-ttu-id="9cac7-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9cac7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
