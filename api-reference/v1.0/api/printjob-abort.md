---
title: printJob： abort
description: 中止打印作业。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f179b30e7c07d9f577ab63c59142a68362a389f1
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517316"
---
# <a name="printjob-abort"></a><span data-ttu-id="03ebd-103">printJob： abort</span><span class="sxs-lookup"><span data-stu-id="03ebd-103">printJob: abort</span></span>

<span data-ttu-id="03ebd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03ebd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="03ebd-105">中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="03ebd-105">Abort a print job.</span></span> <span data-ttu-id="03ebd-106">只有使用应用程序权限的应用程序才能中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="03ebd-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="03ebd-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="03ebd-107">Permissions</span></span>
<span data-ttu-id="03ebd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03ebd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="03ebd-110">除了以下权限之外，应用的租户还必须具有活动的通用打印订阅，并且必须具有 Printer.Read.All 或 Printer.ReadWrite.All 应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="03ebd-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="03ebd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="03ebd-111">Permission type</span></span> | <span data-ttu-id="03ebd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03ebd-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="03ebd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03ebd-113">Delegated (work or school account)</span></span>| <span data-ttu-id="03ebd-114">不支持</span><span class="sxs-lookup"><span data-stu-id="03ebd-114">Not Supported</span></span> |
|<span data-ttu-id="03ebd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03ebd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03ebd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03ebd-116">Not Supported.</span></span>|
|<span data-ttu-id="03ebd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="03ebd-117">Application</span></span>| <span data-ttu-id="03ebd-118">PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All、PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="03ebd-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03ebd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03ebd-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/abort
```

## <a name="request-headers"></a><span data-ttu-id="03ebd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="03ebd-120">Request headers</span></span>
|<span data-ttu-id="03ebd-121">名称</span><span class="sxs-lookup"><span data-stu-id="03ebd-121">Name</span></span>|<span data-ttu-id="03ebd-122">说明</span><span class="sxs-lookup"><span data-stu-id="03ebd-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="03ebd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03ebd-123">Authorization</span></span>|<span data-ttu-id="03ebd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03ebd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03ebd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="03ebd-126">Request body</span></span>
<span data-ttu-id="03ebd-127">在请求正文中，可以选择提供作业中止的原因。</span><span class="sxs-lookup"><span data-stu-id="03ebd-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="03ebd-128">属性</span><span class="sxs-lookup"><span data-stu-id="03ebd-128">Property</span></span>     | <span data-ttu-id="03ebd-129">类型</span><span class="sxs-lookup"><span data-stu-id="03ebd-129">Type</span></span>        | <span data-ttu-id="03ebd-130">Description</span><span class="sxs-lookup"><span data-stu-id="03ebd-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03ebd-131">reason</span><span class="sxs-lookup"><span data-stu-id="03ebd-131">reason</span></span>|<span data-ttu-id="03ebd-132">String</span><span class="sxs-lookup"><span data-stu-id="03ebd-132">String</span></span>|<span data-ttu-id="03ebd-133">作业中止的原因。</span><span class="sxs-lookup"><span data-stu-id="03ebd-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="03ebd-134">响应</span><span class="sxs-lookup"><span data-stu-id="03ebd-134">Response</span></span>

<span data-ttu-id="03ebd-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="03ebd-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03ebd-137">示例</span><span class="sxs-lookup"><span data-stu-id="03ebd-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03ebd-138">请求</span><span class="sxs-lookup"><span data-stu-id="03ebd-138">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="03ebd-139">响应</span><span class="sxs-lookup"><span data-stu-id="03ebd-139">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

