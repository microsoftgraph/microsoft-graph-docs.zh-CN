---
title: 获取 printJob
description: 检索打印作业的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 64d8d76a6c701210ad4556b2862b630b3dafb78c
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849114"
---
# <a name="get-printjob"></a><span data-ttu-id="848f5-103">获取 printJob</span><span class="sxs-lookup"><span data-stu-id="848f5-103">Get printJob</span></span>

<span data-ttu-id="848f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="848f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="848f5-105">检索打印作业的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="848f5-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="848f5-106">权限</span><span class="sxs-lookup"><span data-stu-id="848f5-106">Permissions</span></span>
<span data-ttu-id="848f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="848f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="848f5-109">除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且拥有授予 [获取打印机](printer-get.md) 或 [获取 printerShare](printershare-get.md) 访问权限的权限，具体取决于打印机或 printerShare 是否正在使用。</span><span class="sxs-lookup"><span data-stu-id="848f5-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="848f5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="848f5-110">Permission type</span></span> | <span data-ttu-id="848f5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="848f5-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="848f5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="848f5-112">Delegated (work or school account)</span></span>| <span data-ttu-id="848f5-113">PrintJob、PrintJob、user.readbasic.all、PrintJob、PrintJob、ReadWriteBasic、all、PrintJob、PrintJob、ReadWriteBasic、PrintJob、、、、all</span><span class="sxs-lookup"><span data-stu-id="848f5-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="848f5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="848f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="848f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="848f5-115">Not Supported.</span></span>|
|<span data-ttu-id="848f5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="848f5-116">Application</span></span>| <span data-ttu-id="848f5-117">PrintJob、PrintJob、PrintJob、all、all、All 和 All。</span><span class="sxs-lookup"><span data-stu-id="848f5-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="848f5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="848f5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="848f5-119">若要从打印机中获取作业，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="848f5-119">To get a job from a printer:</span></span>
```http
GET /print/printers/{id}/jobs/{id}
```

<span data-ttu-id="848f5-120">若要从打印机共享中获取作业，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="848f5-120">To get a job from a printer share:</span></span>
```http
GET /print/shares/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="848f5-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="848f5-121">Optional query parameters</span></span>
<span data-ttu-id="848f5-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="848f5-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="848f5-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="848f5-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="848f5-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="848f5-124">Request headers</span></span>
| <span data-ttu-id="848f5-125">名称</span><span class="sxs-lookup"><span data-stu-id="848f5-125">Name</span></span>      |<span data-ttu-id="848f5-126">说明</span><span class="sxs-lookup"><span data-stu-id="848f5-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="848f5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="848f5-127">Authorization</span></span> | <span data-ttu-id="848f5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="848f5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="848f5-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="848f5-130">Request body</span></span>
<span data-ttu-id="848f5-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="848f5-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="848f5-132">响应</span><span class="sxs-lookup"><span data-stu-id="848f5-132">Response</span></span>
<span data-ttu-id="848f5-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printJob](../resources/printjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="848f5-133">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="848f5-134">示例</span><span class="sxs-lookup"><span data-stu-id="848f5-134">Examples</span></span>

### <a name="example-1-get-print-job"></a><span data-ttu-id="848f5-135">示例1：获取打印作业</span><span class="sxs-lookup"><span data-stu-id="848f5-135">Example 1: Get print job</span></span>

#### <a name="request"></a><span data-ttu-id="848f5-136">请求</span><span class="sxs-lookup"><span data-stu-id="848f5-136">Request</span></span>
<span data-ttu-id="848f5-137">下面的示例演示了获取打印作业的元数据的请求。</span><span class="sxs-lookup"><span data-stu-id="848f5-137">The following is an example of a request to get metadata for a print job.</span></span>

# <a name="http"></a>[<span data-ttu-id="848f5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="848f5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182
```
# <a name="c"></a>[<span data-ttu-id="848f5-139">C#</span><span class="sxs-lookup"><span data-stu-id="848f5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="848f5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="848f5-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="848f5-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="848f5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="848f5-142">响应</span><span class="sxs-lookup"><span data-stu-id="848f5-142">Response</span></span>
<span data-ttu-id="848f5-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="848f5-143">The following is an example of the response.</span></span>
><span data-ttu-id="848f5-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="848f5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 408

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {},
  "status": {
    "processingState": "completed",
    "processingStateDescription": "The print job has completed successfully and no further processing will take place."
  }
}
```

### <a name="example-2-get-print-job-with-task-list"></a><span data-ttu-id="848f5-146">示例2：使用任务列表获取打印作业</span><span class="sxs-lookup"><span data-stu-id="848f5-146">Example 2: Get print job with task list</span></span>

#### <a name="request"></a><span data-ttu-id="848f5-147">请求</span><span class="sxs-lookup"><span data-stu-id="848f5-147">Request</span></span>
<span data-ttu-id="848f5-148">下面是一个请求，用于获取打印作业以及正在对其执行或已执行的任何 [任务](../resources/printtask.md) 。</span><span class="sxs-lookup"><span data-stu-id="848f5-148">The following is a request to get a print job and any [tasks](../resources/printtask.md) that are executing, or have executed, against it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182?$expand=tasks
```

#### <a name="response"></a><span data-ttu-id="848f5-149">响应</span><span class="sxs-lookup"><span data-stu-id="848f5-149">Response</span></span>
<span data-ttu-id="848f5-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="848f5-150">The following is an example of the response.</span></span>
><span data-ttu-id="848f5-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="848f5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 774

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs(tasks())/$entity",
  "id": "5182",
  "createdDateTime": "2020-06-30T17:18:52.3930472Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "processingState": "pendingHeld",
    "processingStateDescription": "The job is not a candidate for processing yet."
  },
  "tasks": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="848f5-153">示例3：获取打印作业及其关联的文档数据</span><span class="sxs-lookup"><span data-stu-id="848f5-153">Example 3: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="848f5-154">请求</span><span class="sxs-lookup"><span data-stu-id="848f5-154">Request</span></span>
<span data-ttu-id="848f5-155">下面的示例演示了获取打印作业及其关联的文档数据的请求。</span><span class="sxs-lookup"><span data-stu-id="848f5-155">The following is an example of a request to get a print job and its associated document data.</span></span>
# <a name="http"></a>[<span data-ttu-id="848f5-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="848f5-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216?$expand=documents
```
# <a name="c"></a>[<span data-ttu-id="848f5-157">C#</span><span class="sxs-lookup"><span data-stu-id="848f5-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withdocumentdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="848f5-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="848f5-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withdocumentdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="848f5-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="848f5-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withdocumentdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="848f5-160">响应</span><span class="sxs-lookup"><span data-stu-id="848f5-160">Response</span></span>
<span data-ttu-id="848f5-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="848f5-161">The following is an example of the response.</span></span>
><span data-ttu-id="848f5-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="848f5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1688

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('86b6d420-7e6b-4797-a05c-af4e56cd81bd')/jobs(documents())/$entity",
  "id": "31216",
  "createdDateTime": "2020-06-26T04:20:06.5715544Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "ipAddress": null,
    "userPrincipalName": "",
    "oDataType": null
  },
  "status": {
  "processingState": "aborted",
  "processingStateDescription": "The print job has been aborted by a user or the printer and no further processing will take place."
  },
  "documents@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('86b6d420-7e6b-4797-a05c-af4e56cd81bd')/jobs('31216')/documents",
  "documents": [
    {
      "id": "ca96c367-c3ad-478a-bbce-fbd1cd856e73",
      "displayName": "",
      "contentType": "application/oxps",
      "size": 276604,
      "configuration": {
        "quality": "medium",
        "dpi": 300,
        "feedDirection": null,
        "orientation": "landscape",
        "duplexMode": "oneSided",
        "copies": 2,
        "colorMode": "color",
        "inputBin": null,
        "outputBin": null,
        "mediaSize": null,
        "mediaType": null,
        "finishings": [],
        "pagesPerSheet": null,
        "multipageLayout": "clockwiseFromTopLeft",
        "collate": true,
        "scaling": null,
        "fitPdfToPage": null,
        "margin": null,
        "pageRanges": []
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


