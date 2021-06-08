---
title: printJob： cancel
description: 取消打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b2eb7c40f1f2474752b316a412dbb4c382152741
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787511"
---
# <a name="printjob-cancel"></a><span data-ttu-id="4d397-103">printJob： cancel</span><span class="sxs-lookup"><span data-stu-id="4d397-103">printJob: cancel</span></span>

<span data-ttu-id="4d397-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d397-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d397-105">取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="4d397-105">Cancel a print job.</span></span> <span data-ttu-id="4d397-106">只能代表用户使用委派权限取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="4d397-106">Print jobs can be canceled only on behalf of a user, using delegated permissions.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d397-107">权限</span><span class="sxs-lookup"><span data-stu-id="4d397-107">Permissions</span></span>
<span data-ttu-id="4d397-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d397-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4d397-110">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [获取](printer-get.md) 打印机访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="4d397-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="4d397-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d397-111">Permission type</span></span> | <span data-ttu-id="4d397-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d397-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4d397-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d397-113">Delegated (work or school account)</span></span>| <span data-ttu-id="4d397-114">PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d397-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="4d397-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d397-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d397-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d397-116">Not Supported.</span></span>|
|<span data-ttu-id="4d397-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d397-117">Application</span></span>| <span data-ttu-id="4d397-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d397-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d397-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d397-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="4d397-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d397-120">Request headers</span></span>
| <span data-ttu-id="4d397-121">名称</span><span class="sxs-lookup"><span data-stu-id="4d397-121">Name</span></span>          | <span data-ttu-id="4d397-122">说明</span><span class="sxs-lookup"><span data-stu-id="4d397-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4d397-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d397-123">Authorization</span></span> | <span data-ttu-id="4d397-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4d397-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d397-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d397-126">Request body</span></span>
<span data-ttu-id="4d397-127">请求正文应为空。</span><span class="sxs-lookup"><span data-stu-id="4d397-127">Request body should be empty.</span></span>

## <a name="response"></a><span data-ttu-id="4d397-128">响应</span><span class="sxs-lookup"><span data-stu-id="4d397-128">Response</span></span>
<span data-ttu-id="4d397-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4d397-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d397-131">示例</span><span class="sxs-lookup"><span data-stu-id="4d397-131">Example</span></span>
<span data-ttu-id="4d397-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4d397-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="4d397-133">请求</span><span class="sxs-lookup"><span data-stu-id="4d397-133">Request</span></span>
<span data-ttu-id="4d397-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4d397-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4d397-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d397-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-cancel"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/cancel
```
# <a name="c"></a>[<span data-ttu-id="4d397-136">C#</span><span class="sxs-lookup"><span data-stu-id="4d397-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d397-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d397-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d397-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d397-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d397-139">Java</span><span class="sxs-lookup"><span data-stu-id="4d397-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d397-140">响应</span><span class="sxs-lookup"><span data-stu-id="4d397-140">Response</span></span>
<span data-ttu-id="4d397-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4d397-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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


