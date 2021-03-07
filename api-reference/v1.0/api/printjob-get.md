---
title: 获取 printJob
description: 检索打印作业的属性和关系。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c97ffa869a14fbceedd0fc2e5b8f737792490d1c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517277"
---
# <a name="get-printjob"></a><span data-ttu-id="32fe0-103">获取 printJob</span><span class="sxs-lookup"><span data-stu-id="32fe0-103">Get printJob</span></span>
<span data-ttu-id="32fe0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32fe0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="32fe0-105">检索打印作业的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="32fe0-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="32fe0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="32fe0-106">Permissions</span></span>
<span data-ttu-id="32fe0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32fe0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="32fe0-109">除了以下权限外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据使用的打印机或 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="32fe0-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="32fe0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="32fe0-110">Permission type</span></span> | <span data-ttu-id="32fe0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32fe0-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="32fe0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32fe0-112">Delegated (work or school account)</span></span>| <span data-ttu-id="32fe0-113">PrintJob.ReadBasic、PrintJob.Read、PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32fe0-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="32fe0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32fe0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32fe0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="32fe0-115">Not Supported.</span></span>|
|<span data-ttu-id="32fe0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="32fe0-116">Application</span></span>| <span data-ttu-id="32fe0-117">PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32fe0-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32fe0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32fe0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="32fe0-119">若要从打印机获取作业，请：</span><span class="sxs-lookup"><span data-stu-id="32fe0-119">To get a job from a printer:</span></span>
```http
GET /print/printers/{id}/jobs/{id}
```

<span data-ttu-id="32fe0-120">若要从打印机共享获取作业，请：</span><span class="sxs-lookup"><span data-stu-id="32fe0-120">To get a job from a printer share:</span></span>
```http
GET /print/shares/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32fe0-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="32fe0-121">Optional query parameters</span></span>
<span data-ttu-id="32fe0-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="32fe0-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="32fe0-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="32fe0-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="32fe0-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="32fe0-124">Request headers</span></span>
|<span data-ttu-id="32fe0-125">名称</span><span class="sxs-lookup"><span data-stu-id="32fe0-125">Name</span></span>|<span data-ttu-id="32fe0-126">说明</span><span class="sxs-lookup"><span data-stu-id="32fe0-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="32fe0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="32fe0-127">Authorization</span></span>|<span data-ttu-id="32fe0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32fe0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32fe0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="32fe0-130">Request body</span></span>
<span data-ttu-id="32fe0-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="32fe0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32fe0-132">响应</span><span class="sxs-lookup"><span data-stu-id="32fe0-132">Response</span></span>

<span data-ttu-id="32fe0-133">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [printJob](../resources/printjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32fe0-133">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32fe0-134">示例</span><span class="sxs-lookup"><span data-stu-id="32fe0-134">Examples</span></span>

### <a name="example-1-get-print-job"></a><span data-ttu-id="32fe0-135">示例 1：获取打印作业</span><span class="sxs-lookup"><span data-stu-id="32fe0-135">Example 1: Get print job</span></span>

#### <a name="request"></a><span data-ttu-id="32fe0-136">请求</span><span class="sxs-lookup"><span data-stu-id="32fe0-136">Request</span></span>
<span data-ttu-id="32fe0-137">下面是请求获取打印作业元数据的示例。</span><span class="sxs-lookup"><span data-stu-id="32fe0-137">The following is an example of a request to get metadata for a print job.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}
```

#### <a name="response"></a><span data-ttu-id="32fe0-138">响应</span><span class="sxs-lookup"><span data-stu-id="32fe0-138">Response</span></span>
<span data-ttu-id="32fe0-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="32fe0-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false
}
```

### <a name="example-2-get-print-job-with-task-list"></a><span data-ttu-id="32fe0-140">示例 2：获取包含任务列表的打印作业</span><span class="sxs-lookup"><span data-stu-id="32fe0-140">Example 2: Get print job with task list</span></span>

#### <a name="request"></a><span data-ttu-id="32fe0-141">请求</span><span class="sxs-lookup"><span data-stu-id="32fe0-141">Request</span></span>
<span data-ttu-id="32fe0-142">下面是一个请求，请求获取打印作业以及针对打印[](../resources/printtask.md)作业执行或已执行的任何任务。</span><span class="sxs-lookup"><span data-stu-id="32fe0-142">The following is a request to get a print job and any [tasks](../resources/printtask.md) that are executing, or have executed, against it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=tasks
```

#### <a name="response"></a><span data-ttu-id="32fe0-143">响应</span><span class="sxs-lookup"><span data-stu-id="32fe0-143">Response</span></span>
<span data-ttu-id="32fe0-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="32fe0-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "tasks": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="32fe0-145">示例 3：获取打印作业及其关联的文档数据</span><span class="sxs-lookup"><span data-stu-id="32fe0-145">Example 3: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="32fe0-146">请求</span><span class="sxs-lookup"><span data-stu-id="32fe0-146">Request</span></span>
<span data-ttu-id="32fe0-147">下面是请求获取打印作业及其关联文档数据的示例。</span><span class="sxs-lookup"><span data-stu-id="32fe0-147">The following is an example of a request to get a print job and its associated document data.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=documents
```

#### <a name="response"></a><span data-ttu-id="32fe0-148">响应</span><span class="sxs-lookup"><span data-stu-id="32fe0-148">Response</span></span>
<span data-ttu-id="32fe0-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="32fe0-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "documents@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs('5182')/documents",
  "documents": [
    {
      "id": "ca96c367-c3ad-478a-bbce-fbd1cd856e73",
      "displayName": "",
      "contentType": "application/oxps",
      "size": 276604
    }
  ]
}
```
