---
title: Get taskTrigger
description: 从打印机获取任务触发器。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 3976b61801d6f7bff3a1355666849a8e46f56c70
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053564"
---
# <a name="get-tasktrigger"></a><span data-ttu-id="fe78a-103">Get taskTrigger</span><span class="sxs-lookup"><span data-stu-id="fe78a-103">Get taskTrigger</span></span>

<span data-ttu-id="fe78a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe78a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe78a-105">从 [打印机获取](../resources/printtasktrigger.md) 任务 [触发器](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="fe78a-105">Get a [task trigger](../resources/printtasktrigger.md) from a [printer](../resources/printer.md).</span></span>

<span data-ttu-id="fe78a-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="fe78a-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe78a-107">权限</span><span class="sxs-lookup"><span data-stu-id="fe78a-107">Permissions</span></span>
<span data-ttu-id="fe78a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe78a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fe78a-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="fe78a-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="fe78a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe78a-111">Permission type</span></span> | <span data-ttu-id="fe78a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe78a-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fe78a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe78a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="fe78a-114">Printer.Read.All、Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="fe78a-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="fe78a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe78a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe78a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe78a-116">Not Supported.</span></span>|
|<span data-ttu-id="fe78a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe78a-117">Application</span></span>|<span data-ttu-id="fe78a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe78a-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe78a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe78a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fe78a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe78a-120">Request headers</span></span>
| <span data-ttu-id="fe78a-121">名称</span><span class="sxs-lookup"><span data-stu-id="fe78a-121">Name</span></span>      |<span data-ttu-id="fe78a-122">说明</span><span class="sxs-lookup"><span data-stu-id="fe78a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fe78a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe78a-123">Authorization</span></span> | <span data-ttu-id="fe78a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe78a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe78a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe78a-126">Request body</span></span>
<span data-ttu-id="fe78a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe78a-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fe78a-128">响应</span><span class="sxs-lookup"><span data-stu-id="fe78a-128">Response</span></span>
<span data-ttu-id="fe78a-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printTaskTrigger](../resources/printtasktrigger.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe78a-129">If successful, this method returns a `200 OK` response code and [printTaskTrigger](../resources/printtasktrigger.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe78a-130">示例</span><span class="sxs-lookup"><span data-stu-id="fe78a-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe78a-131">请求</span><span class="sxs-lookup"><span data-stu-id="fe78a-131">Request</span></span>
<span data-ttu-id="fe78a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fe78a-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fe78a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe78a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_tasktrigger"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{printerId}/taskTriggers/{taskTriggerId}
```
# <a name="c"></a>[<span data-ttu-id="fe78a-134">C#</span><span class="sxs-lookup"><span data-stu-id="fe78a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe78a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe78a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe78a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe78a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe78a-137">Java</span><span class="sxs-lookup"><span data-stu-id="fe78a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-tasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="fe78a-138">响应</span><span class="sxs-lookup"><span data-stu-id="fe78a-138">Response</span></span>
<span data-ttu-id="fe78a-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fe78a-139">The following is an example of the response.</span></span>
><span data-ttu-id="fe78a-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fe78a-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 181

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/taskTriggers/$entity",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get taskTrigger",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


