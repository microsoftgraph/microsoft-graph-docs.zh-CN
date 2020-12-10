---
title: printJob：取消
description: 取消打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4c4522ef8fb19226475758986d1245c447358095
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617015"
---
# <a name="printjob-cancel"></a><span data-ttu-id="d5861-103">printJob：取消</span><span class="sxs-lookup"><span data-stu-id="d5861-103">printJob: cancel</span></span>

<span data-ttu-id="d5861-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5861-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5861-105">取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="d5861-105">Cancel a print job.</span></span> <span data-ttu-id="d5861-106">只能代表用户（使用委派权限）取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="d5861-106">Print jobs can be canceled only on behalf of a user, using delegated permissions.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5861-107">权限</span><span class="sxs-lookup"><span data-stu-id="d5861-107">Permissions</span></span>
<span data-ttu-id="d5861-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5861-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d5861-110">除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且具有授予 [获取打印机](printer-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="d5861-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="d5861-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5861-111">Permission type</span></span> | <span data-ttu-id="d5861-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5861-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d5861-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5861-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d5861-114">PrintJob、ReadWriteBasic、PrintJob、All、ReadWriteBasic、All</span><span class="sxs-lookup"><span data-stu-id="d5861-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="d5861-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5861-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5861-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5861-116">Not Supported.</span></span>|
|<span data-ttu-id="d5861-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5861-117">Application</span></span>| <span data-ttu-id="d5861-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5861-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5861-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5861-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="d5861-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5861-120">Request headers</span></span>
| <span data-ttu-id="d5861-121">名称</span><span class="sxs-lookup"><span data-stu-id="d5861-121">Name</span></span>          | <span data-ttu-id="d5861-122">说明</span><span class="sxs-lookup"><span data-stu-id="d5861-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d5861-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5861-123">Authorization</span></span> | <span data-ttu-id="d5861-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5861-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5861-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5861-126">Request body</span></span>
<span data-ttu-id="d5861-127">请求正文应为空。</span><span class="sxs-lookup"><span data-stu-id="d5861-127">Request body should be empty.</span></span>

## <a name="response"></a><span data-ttu-id="d5861-128">响应</span><span class="sxs-lookup"><span data-stu-id="d5861-128">Response</span></span>
<span data-ttu-id="d5861-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d5861-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5861-131">示例</span><span class="sxs-lookup"><span data-stu-id="d5861-131">Example</span></span>
<span data-ttu-id="d5861-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d5861-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="d5861-133">请求</span><span class="sxs-lookup"><span data-stu-id="d5861-133">Request</span></span>
<span data-ttu-id="d5861-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d5861-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d5861-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5861-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-cancel"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/cancel
```
# <a name="c"></a>[<span data-ttu-id="d5861-136">C#</span><span class="sxs-lookup"><span data-stu-id="d5861-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5861-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5861-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5861-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5861-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5861-139">Java</span><span class="sxs-lookup"><span data-stu-id="d5861-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d5861-140">响应</span><span class="sxs-lookup"><span data-stu-id="d5861-140">Response</span></span>
<span data-ttu-id="d5861-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d5861-141">The following is an example of the response.</span></span> 
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
  "description": "printJob: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


