---
title: printJob： cancel
description: 取消打印作业。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: dd341ddc3beff0ece8ba28e1071f217f9cac05ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777052"
---
# <a name="printjob-cancel"></a><span data-ttu-id="e6bcd-103">printJob： cancel</span><span class="sxs-lookup"><span data-stu-id="e6bcd-103">printJob: cancel</span></span>
<span data-ttu-id="e6bcd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6bcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="e6bcd-105">取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="e6bcd-105">Cancel a print job.</span></span> <span data-ttu-id="e6bcd-106">只能代表用户使用委派权限取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="e6bcd-106">Print jobs can be canceled only on behalf of a user, using delegated permissions.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6bcd-107">权限</span><span class="sxs-lookup"><span data-stu-id="e6bcd-107">Permissions</span></span>
<span data-ttu-id="e6bcd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6bcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e6bcd-110">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [获取](printer-get.md) 打印机访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="e6bcd-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="e6bcd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6bcd-111">Permission type</span></span> | <span data-ttu-id="e6bcd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6bcd-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e6bcd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6bcd-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e6bcd-114">PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6bcd-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="e6bcd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6bcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6bcd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6bcd-116">Not Supported.</span></span>|
|<span data-ttu-id="e6bcd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6bcd-117">Application</span></span>| <span data-ttu-id="e6bcd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6bcd-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6bcd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6bcd-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="e6bcd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6bcd-120">Request headers</span></span>
|<span data-ttu-id="e6bcd-121">名称</span><span class="sxs-lookup"><span data-stu-id="e6bcd-121">Name</span></span>|<span data-ttu-id="e6bcd-122">说明</span><span class="sxs-lookup"><span data-stu-id="e6bcd-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e6bcd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6bcd-123">Authorization</span></span>|<span data-ttu-id="e6bcd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6bcd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6bcd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6bcd-126">Request body</span></span>
<span data-ttu-id="e6bcd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e6bcd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6bcd-128">响应</span><span class="sxs-lookup"><span data-stu-id="e6bcd-128">Response</span></span>
<span data-ttu-id="e6bcd-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e6bcd-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e6bcd-131">示例</span><span class="sxs-lookup"><span data-stu-id="e6bcd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e6bcd-132">请求</span><span class="sxs-lookup"><span data-stu-id="e6bcd-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e6bcd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6bcd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob_cancel"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/cancel
```
# <a name="c"></a>[<span data-ttu-id="e6bcd-134">C#</span><span class="sxs-lookup"><span data-stu-id="e6bcd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6bcd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6bcd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6bcd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6bcd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6bcd-137">Java</span><span class="sxs-lookup"><span data-stu-id="e6bcd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e6bcd-138">响应</span><span class="sxs-lookup"><span data-stu-id="e6bcd-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

