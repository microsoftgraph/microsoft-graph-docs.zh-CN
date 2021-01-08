---
title: printJob： start
description: 将打印作业提交到关联的打印机或 printerShare。 完成、中止或取消任何现有待定作业后，将打印该作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: d2cb4a5413d592d170e31a882be93d900deca8c1
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784786"
---
# <a name="printjob-start"></a><span data-ttu-id="04d7d-104">printJob： start</span><span class="sxs-lookup"><span data-stu-id="04d7d-104">printJob: start</span></span>

<span data-ttu-id="04d7d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04d7d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04d7d-106">将打印作业提交到关联的[打印机](../resources/printer.md)或[printerShare。](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="04d7d-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="04d7d-107">将在完成、中止或取消任何现有待定作业后打印该作业。</span><span class="sxs-lookup"><span data-stu-id="04d7d-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="04d7d-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="04d7d-108">Permissions</span></span>
<span data-ttu-id="04d7d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04d7d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="04d7d-111">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据使用的打印机或 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 的权限。</span><span class="sxs-lookup"><span data-stu-id="04d7d-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="04d7d-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="04d7d-112">Permission type</span></span> | <span data-ttu-id="04d7d-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04d7d-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="04d7d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04d7d-114">Delegated (work or school account)</span></span>| <span data-ttu-id="04d7d-115">PrintJob.Create、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04d7d-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="04d7d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04d7d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04d7d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="04d7d-117">Not Supported.</span></span>|
|<span data-ttu-id="04d7d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="04d7d-118">Application</span></span>| <span data-ttu-id="04d7d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="04d7d-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04d7d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04d7d-120">HTTP request</span></span>
```http
POST /print/shares/{id}/jobs/{id}/start
```
## <a name="request-headers"></a><span data-ttu-id="04d7d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="04d7d-121">Request headers</span></span>
| <span data-ttu-id="04d7d-122">名称</span><span class="sxs-lookup"><span data-stu-id="04d7d-122">Name</span></span>          | <span data-ttu-id="04d7d-123">说明</span><span class="sxs-lookup"><span data-stu-id="04d7d-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="04d7d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="04d7d-124">Authorization</span></span> | <span data-ttu-id="04d7d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="04d7d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04d7d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="04d7d-127">Request body</span></span>

<span data-ttu-id="04d7d-128">不要提交此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="04d7d-128">Do not submit a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="04d7d-129">响应</span><span class="sxs-lookup"><span data-stu-id="04d7d-129">Response</span></span>
<span data-ttu-id="04d7d-130">如果成功，此方法在正文中 `200 OK` 返回响应代码和 [printJobStatus](../resources/printjobstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04d7d-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="04d7d-131">示例</span><span class="sxs-lookup"><span data-stu-id="04d7d-131">Example</span></span>
<span data-ttu-id="04d7d-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="04d7d-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="04d7d-133">请求</span><span class="sxs-lookup"><span data-stu-id="04d7d-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a><span data-ttu-id="04d7d-134">响应</span><span class="sxs-lookup"><span data-stu-id="04d7d-134">Response</span></span>
<span data-ttu-id="04d7d-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="04d7d-135">The following is an example of the response.</span></span> 
><span data-ttu-id="04d7d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="04d7d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


