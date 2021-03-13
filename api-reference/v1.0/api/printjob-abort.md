---
title: printJob： abort
description: 中止打印作业。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 55ee53dd758116edd14149a9dc20270fa49b1679
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771405"
---
# <a name="printjob-abort"></a><span data-ttu-id="b10a5-103">printJob： abort</span><span class="sxs-lookup"><span data-stu-id="b10a5-103">printJob: abort</span></span>

<span data-ttu-id="b10a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b10a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="b10a5-105">中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="b10a5-105">Abort a print job.</span></span> <span data-ttu-id="b10a5-106">只有使用应用程序权限的应用程序才能中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="b10a5-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="b10a5-107">权限</span><span class="sxs-lookup"><span data-stu-id="b10a5-107">Permissions</span></span>
<span data-ttu-id="b10a5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b10a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b10a5-110">除了以下权限之外，应用的租户还必须具有活动的通用打印订阅，并且必须具有 Printer.Read.All 或 Printer.ReadWrite.All 应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="b10a5-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="b10a5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b10a5-111">Permission type</span></span> | <span data-ttu-id="b10a5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b10a5-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b10a5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b10a5-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b10a5-114">不支持</span><span class="sxs-lookup"><span data-stu-id="b10a5-114">Not Supported</span></span> |
|<span data-ttu-id="b10a5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b10a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b10a5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b10a5-116">Not Supported.</span></span>|
|<span data-ttu-id="b10a5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b10a5-117">Application</span></span>| <span data-ttu-id="b10a5-118">PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All、PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b10a5-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b10a5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b10a5-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/abort
```

## <a name="request-headers"></a><span data-ttu-id="b10a5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b10a5-120">Request headers</span></span>
|<span data-ttu-id="b10a5-121">名称</span><span class="sxs-lookup"><span data-stu-id="b10a5-121">Name</span></span>|<span data-ttu-id="b10a5-122">说明</span><span class="sxs-lookup"><span data-stu-id="b10a5-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b10a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b10a5-123">Authorization</span></span>|<span data-ttu-id="b10a5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b10a5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b10a5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b10a5-126">Request body</span></span>
<span data-ttu-id="b10a5-127">在请求正文中，可以选择提供作业中止的原因。</span><span class="sxs-lookup"><span data-stu-id="b10a5-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="b10a5-128">属性</span><span class="sxs-lookup"><span data-stu-id="b10a5-128">Property</span></span>     | <span data-ttu-id="b10a5-129">类型</span><span class="sxs-lookup"><span data-stu-id="b10a5-129">Type</span></span>        | <span data-ttu-id="b10a5-130">说明</span><span class="sxs-lookup"><span data-stu-id="b10a5-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b10a5-131">reason</span><span class="sxs-lookup"><span data-stu-id="b10a5-131">reason</span></span>|<span data-ttu-id="b10a5-132">字符串</span><span class="sxs-lookup"><span data-stu-id="b10a5-132">String</span></span>|<span data-ttu-id="b10a5-133">作业中止的原因。</span><span class="sxs-lookup"><span data-stu-id="b10a5-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="b10a5-134">响应</span><span class="sxs-lookup"><span data-stu-id="b10a5-134">Response</span></span>

<span data-ttu-id="b10a5-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b10a5-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b10a5-137">示例</span><span class="sxs-lookup"><span data-stu-id="b10a5-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b10a5-138">请求</span><span class="sxs-lookup"><span data-stu-id="b10a5-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b10a5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b10a5-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob_abort"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/abort
Content-Type: application/json
Content-length: 26

{
  "reason": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="b10a5-140">C#</span><span class="sxs-lookup"><span data-stu-id="b10a5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-abort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b10a5-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b10a5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-abort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b10a5-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b10a5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-abort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b10a5-143">Java</span><span class="sxs-lookup"><span data-stu-id="b10a5-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-abort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b10a5-144">响应</span><span class="sxs-lookup"><span data-stu-id="b10a5-144">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

