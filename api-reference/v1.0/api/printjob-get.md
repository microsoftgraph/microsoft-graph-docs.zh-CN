---
title: 获取 printJob
description: 检索打印作业的属性和关系。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 976624807ab6cbf8a104790665c481e3f54f9750
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776002"
---
# <a name="get-printjob"></a><span data-ttu-id="44358-103">获取 printJob</span><span class="sxs-lookup"><span data-stu-id="44358-103">Get printJob</span></span>
<span data-ttu-id="44358-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44358-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="44358-105">检索打印作业的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="44358-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="44358-106">权限</span><span class="sxs-lookup"><span data-stu-id="44358-106">Permissions</span></span>
<span data-ttu-id="44358-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="44358-109">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据使用的打印机还是 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="44358-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="44358-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="44358-110">Permission type</span></span> | <span data-ttu-id="44358-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44358-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="44358-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44358-112">Delegated (work or school account)</span></span>| <span data-ttu-id="44358-113">PrintJob.ReadBasic、PrintJob.Read、PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44358-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="44358-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44358-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44358-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="44358-115">Not Supported.</span></span>|
|<span data-ttu-id="44358-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="44358-116">Application</span></span>| <span data-ttu-id="44358-117">PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44358-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44358-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44358-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="44358-119">从打印机获取作业：</span><span class="sxs-lookup"><span data-stu-id="44358-119">To get a job from a printer:</span></span>
```http
GET /print/printers/{id}/jobs/{id}
```

<span data-ttu-id="44358-120">从打印机共享获取作业：</span><span class="sxs-lookup"><span data-stu-id="44358-120">To get a job from a printer share:</span></span>
```http
GET /print/shares/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44358-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="44358-121">Optional query parameters</span></span>
<span data-ttu-id="44358-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="44358-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="44358-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="44358-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="44358-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="44358-124">Request headers</span></span>
|<span data-ttu-id="44358-125">名称</span><span class="sxs-lookup"><span data-stu-id="44358-125">Name</span></span>|<span data-ttu-id="44358-126">说明</span><span class="sxs-lookup"><span data-stu-id="44358-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="44358-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="44358-127">Authorization</span></span>|<span data-ttu-id="44358-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44358-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44358-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="44358-130">Request body</span></span>
<span data-ttu-id="44358-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="44358-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44358-132">响应</span><span class="sxs-lookup"><span data-stu-id="44358-132">Response</span></span>

<span data-ttu-id="44358-133">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printJob](../resources/printjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44358-133">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44358-134">示例</span><span class="sxs-lookup"><span data-stu-id="44358-134">Examples</span></span>

### <a name="example-1-get-print-job"></a><span data-ttu-id="44358-135">示例 1：获取打印作业</span><span class="sxs-lookup"><span data-stu-id="44358-135">Example 1: Get print job</span></span>

#### <a name="request"></a><span data-ttu-id="44358-136">请求</span><span class="sxs-lookup"><span data-stu-id="44358-136">Request</span></span>
<span data-ttu-id="44358-137">下面是请求获取打印作业的元数据的示例。</span><span class="sxs-lookup"><span data-stu-id="44358-137">The following is an example of a request to get metadata for a print job.</span></span>


# <a name="http"></a>[<span data-ttu-id="44358-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="44358-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}
```
# <a name="c"></a>[<span data-ttu-id="44358-139">C#</span><span class="sxs-lookup"><span data-stu-id="44358-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44358-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44358-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44358-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44358-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44358-142">Java</span><span class="sxs-lookup"><span data-stu-id="44358-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44358-143">响应</span><span class="sxs-lookup"><span data-stu-id="44358-143">Response</span></span>
<span data-ttu-id="44358-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="44358-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-print-job-with-task-list"></a><span data-ttu-id="44358-145">示例 2：获取包含任务列表的打印作业</span><span class="sxs-lookup"><span data-stu-id="44358-145">Example 2: Get print job with task list</span></span>

#### <a name="request"></a><span data-ttu-id="44358-146">请求</span><span class="sxs-lookup"><span data-stu-id="44358-146">Request</span></span>
<span data-ttu-id="44358-147">下面是一个请求，请求获取打印作业以及针对打印[](../resources/printtask.md)作业执行或已执行的任何任务。</span><span class="sxs-lookup"><span data-stu-id="44358-147">The following is a request to get a print job and any [tasks](../resources/printtask.md) that are executing, or have executed, against it.</span></span>


# <a name="http"></a>[<span data-ttu-id="44358-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="44358-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=tasks
```
# <a name="c"></a>[<span data-ttu-id="44358-149">C#</span><span class="sxs-lookup"><span data-stu-id="44358-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withtasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44358-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44358-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withtasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44358-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44358-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withtasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44358-152">Java</span><span class="sxs-lookup"><span data-stu-id="44358-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-withtasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44358-153">响应</span><span class="sxs-lookup"><span data-stu-id="44358-153">Response</span></span>
<span data-ttu-id="44358-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="44358-154">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="44358-155">示例 3：获取打印作业及其关联的文档数据</span><span class="sxs-lookup"><span data-stu-id="44358-155">Example 3: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="44358-156">请求</span><span class="sxs-lookup"><span data-stu-id="44358-156">Request</span></span>
<span data-ttu-id="44358-157">下面是请求获取打印作业及其关联文档数据的示例。</span><span class="sxs-lookup"><span data-stu-id="44358-157">The following is an example of a request to get a print job and its associated document data.</span></span>


# <a name="http"></a>[<span data-ttu-id="44358-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="44358-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=documents
```
# <a name="c"></a>[<span data-ttu-id="44358-159">C#</span><span class="sxs-lookup"><span data-stu-id="44358-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withdocumentdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44358-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44358-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withdocumentdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44358-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44358-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withdocumentdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44358-162">Java</span><span class="sxs-lookup"><span data-stu-id="44358-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-withdocumentdata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44358-163">响应</span><span class="sxs-lookup"><span data-stu-id="44358-163">Response</span></span>
<span data-ttu-id="44358-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="44358-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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
