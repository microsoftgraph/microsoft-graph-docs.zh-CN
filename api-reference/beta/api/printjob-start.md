---
title: printJob：start
description: 将打印作业提交到关联的打印机或 printerShare。 完成、中止或取消任何现有待定作业后，将打印该作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 288e3b8cfcd1458f7d71c8fb43ae57ac97237e56
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049875"
---
# <a name="printjob-start"></a><span data-ttu-id="d3945-104">printJob：start</span><span class="sxs-lookup"><span data-stu-id="d3945-104">printJob: start</span></span>

<span data-ttu-id="d3945-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3945-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3945-106">将打印作业提交到关联的 [打印机或](../resources/printer.md) [printerShare](../resources/printershare.md)。</span><span class="sxs-lookup"><span data-stu-id="d3945-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="d3945-107">将在完成、中止或取消任何现有待定作业后打印该作业。</span><span class="sxs-lookup"><span data-stu-id="d3945-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3945-108">权限</span><span class="sxs-lookup"><span data-stu-id="d3945-108">Permissions</span></span>
<span data-ttu-id="d3945-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3945-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d3945-111">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据所使用的打印机还是 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 的权限。</span><span class="sxs-lookup"><span data-stu-id="d3945-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="d3945-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3945-112">Permission type</span></span> | <span data-ttu-id="d3945-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3945-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d3945-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3945-114">Delegated (work or school account)</span></span>| <span data-ttu-id="d3945-115">PrintJob.Create、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3945-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="d3945-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3945-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3945-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3945-117">Not Supported.</span></span>|
|<span data-ttu-id="d3945-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3945-118">Application</span></span>| <span data-ttu-id="d3945-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3945-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3945-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3945-120">HTTP request</span></span>
```http
POST /print/shares/{id}/jobs/{id}/start
```
## <a name="request-headers"></a><span data-ttu-id="d3945-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3945-121">Request headers</span></span>
| <span data-ttu-id="d3945-122">名称</span><span class="sxs-lookup"><span data-stu-id="d3945-122">Name</span></span>          | <span data-ttu-id="d3945-123">说明</span><span class="sxs-lookup"><span data-stu-id="d3945-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d3945-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3945-124">Authorization</span></span> | <span data-ttu-id="d3945-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d3945-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3945-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3945-127">Request body</span></span>

<span data-ttu-id="d3945-128">请勿提交此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3945-128">Do not submit a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="d3945-129">响应</span><span class="sxs-lookup"><span data-stu-id="d3945-129">Response</span></span>
<span data-ttu-id="d3945-130">如果成功，此方法在 `200 OK` 正文中返回 响应代码和 [printJobStatus](../resources/printjobstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3945-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="d3945-131">示例</span><span class="sxs-lookup"><span data-stu-id="d3945-131">Example</span></span>
<span data-ttu-id="d3945-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d3945-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d3945-133">请求</span><span class="sxs-lookup"><span data-stu-id="d3945-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a><span data-ttu-id="d3945-134">响应</span><span class="sxs-lookup"><span data-stu-id="d3945-134">Response</span></span>
<span data-ttu-id="d3945-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d3945-135">The following is an example of the response.</span></span> 
><span data-ttu-id="d3945-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d3945-136">**Note:** The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


