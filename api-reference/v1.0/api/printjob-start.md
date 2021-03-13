---
title: printJob：start
description: 将打印作业提交到关联的打印机或 printerShare。 完成、中止或取消任何现有待定作业后，将打印该作业。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: dd264c395538ee3d77fe22829edca27a6d7ad4b1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775918"
---
# <a name="printjob-start"></a><span data-ttu-id="4b579-104">printJob：start</span><span class="sxs-lookup"><span data-stu-id="4b579-104">printJob: start</span></span>
<span data-ttu-id="4b579-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b579-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="4b579-106">将打印作业提交到关联的 [打印机或](../resources/printer.md) [printerShare](../resources/printershare.md)。</span><span class="sxs-lookup"><span data-stu-id="4b579-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="4b579-107">将在完成、中止或取消任何现有待定作业后打印该作业。</span><span class="sxs-lookup"><span data-stu-id="4b579-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b579-108">权限</span><span class="sxs-lookup"><span data-stu-id="4b579-108">Permissions</span></span>
<span data-ttu-id="4b579-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b579-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4b579-111">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据所使用的打印机还是 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 的权限。</span><span class="sxs-lookup"><span data-stu-id="4b579-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="4b579-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b579-112">Permission type</span></span> | <span data-ttu-id="4b579-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b579-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4b579-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b579-114">Delegated (work or school account)</span></span>| <span data-ttu-id="4b579-115">PrintJob.Create、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b579-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="4b579-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b579-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b579-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b579-117">Not Supported.</span></span>|
|<span data-ttu-id="4b579-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b579-118">Application</span></span>| <span data-ttu-id="4b579-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b579-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b579-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b579-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/jobs/{printJobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="4b579-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b579-121">Request headers</span></span>
|<span data-ttu-id="4b579-122">名称</span><span class="sxs-lookup"><span data-stu-id="4b579-122">Name</span></span>|<span data-ttu-id="4b579-123">说明</span><span class="sxs-lookup"><span data-stu-id="4b579-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4b579-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b579-124">Authorization</span></span>|<span data-ttu-id="4b579-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b579-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b579-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b579-127">Request body</span></span>
<span data-ttu-id="4b579-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b579-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b579-129">响应</span><span class="sxs-lookup"><span data-stu-id="4b579-129">Response</span></span>
<span data-ttu-id="4b579-130">如果成功，此方法在 `200 OK` 正文中返回 响应代码和 [printJobStatus](../resources/printjobstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b579-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b579-131">示例</span><span class="sxs-lookup"><span data-stu-id="4b579-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b579-132">请求</span><span class="sxs-lookup"><span data-stu-id="4b579-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4b579-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b579-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob_start"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs/{printJobId}/start
```
# <a name="c"></a>[<span data-ttu-id="4b579-134">C#</span><span class="sxs-lookup"><span data-stu-id="4b579-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b579-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b579-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b579-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b579-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b579-137">Java</span><span class="sxs-lookup"><span data-stu-id="4b579-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b579-138">响应</span><span class="sxs-lookup"><span data-stu-id="4b579-138">Response</span></span>
<span data-ttu-id="4b579-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4b579-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```

