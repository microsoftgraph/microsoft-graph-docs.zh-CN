---
title: 打印机： resetDefaults
description: 重置打印机的默认设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d3e2f28e15d12e2a332f995b5b6d8d3e94856228
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947751"
---
# <a name="printer-resetdefaults"></a><span data-ttu-id="8297a-103">打印机： resetDefaults</span><span class="sxs-lookup"><span data-stu-id="8297a-103">printer: resetDefaults</span></span>

<span data-ttu-id="8297a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8297a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8297a-105">重置[打印机](../resources/printer.md)的默认设置。</span><span class="sxs-lookup"><span data-stu-id="8297a-105">Reset a [printer](../resources/printer.md)'s default settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="8297a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8297a-106">Permissions</span></span>
<span data-ttu-id="8297a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8297a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8297a-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="8297a-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="8297a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8297a-110">Permission type</span></span> | <span data-ttu-id="8297a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8297a-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8297a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8297a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="8297a-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="8297a-113">Users.Read.All</span></span> |
|<span data-ttu-id="8297a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8297a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8297a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8297a-115">Not Supported.</span></span>|
|<span data-ttu-id="8297a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8297a-116">Application</span></span>|<span data-ttu-id="8297a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8297a-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8297a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8297a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/resetDefaults
```
## <a name="request-headers"></a><span data-ttu-id="8297a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8297a-119">Request headers</span></span>
| <span data-ttu-id="8297a-120">名称</span><span class="sxs-lookup"><span data-stu-id="8297a-120">Name</span></span>          | <span data-ttu-id="8297a-121">说明</span><span class="sxs-lookup"><span data-stu-id="8297a-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8297a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8297a-122">Authorization</span></span> | <span data-ttu-id="8297a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8297a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8297a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8297a-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8297a-126">响应</span><span class="sxs-lookup"><span data-stu-id="8297a-126">Response</span></span>
<span data-ttu-id="8297a-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8297a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8297a-129">示例</span><span class="sxs-lookup"><span data-stu-id="8297a-129">Example</span></span>
<span data-ttu-id="8297a-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8297a-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8297a-131">请求</span><span class="sxs-lookup"><span data-stu-id="8297a-131">Request</span></span>
<span data-ttu-id="8297a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8297a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8297a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8297a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-resetdefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/resetDefaults
```
# <a name="c"></a>[<span data-ttu-id="8297a-134">C#</span><span class="sxs-lookup"><span data-stu-id="8297a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-resetdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8297a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8297a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-resetdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8297a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8297a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-resetdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8297a-137">响应</span><span class="sxs-lookup"><span data-stu-id="8297a-137">Response</span></span>
<span data-ttu-id="8297a-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8297a-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer: resetDefaults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
