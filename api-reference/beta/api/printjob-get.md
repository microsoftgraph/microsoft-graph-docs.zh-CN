---
title: 获取 printJob
description: 检索打印作业的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 07744f37598c1bb32750bdf3697ca025182faaaa
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674209"
---
# <a name="get-printjob"></a><span data-ttu-id="67615-103">获取 printJob</span><span class="sxs-lookup"><span data-stu-id="67615-103">Get printJob</span></span>

<span data-ttu-id="67615-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67615-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67615-105">检索打印作业的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="67615-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="67615-106">权限</span><span class="sxs-lookup"><span data-stu-id="67615-106">Permissions</span></span>
<span data-ttu-id="67615-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67615-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="67615-109">除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且具有授予 [获取打印机](printer-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="67615-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="67615-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="67615-110">Permission type</span></span> | <span data-ttu-id="67615-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67615-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="67615-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67615-112">Delegated (work or school account)</span></span>| <span data-ttu-id="67615-113">PrintJob、PrintJob、user.readbasic.all、PrintJob、PrintJob、ReadWriteBasic、all、PrintJob、PrintJob、ReadWriteBasic、PrintJob、、、、all</span><span class="sxs-lookup"><span data-stu-id="67615-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="67615-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67615-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67615-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="67615-115">Not Supported.</span></span>|
|<span data-ttu-id="67615-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="67615-116">Application</span></span>| <span data-ttu-id="67615-117">PrintJob、PrintJob、PrintJob、all、all、All 和 All。</span><span class="sxs-lookup"><span data-stu-id="67615-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67615-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67615-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="67615-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="67615-119">Optional query parameters</span></span>
<span data-ttu-id="67615-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="67615-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="67615-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="67615-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="67615-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="67615-122">Request headers</span></span>
| <span data-ttu-id="67615-123">名称</span><span class="sxs-lookup"><span data-stu-id="67615-123">Name</span></span>      |<span data-ttu-id="67615-124">说明</span><span class="sxs-lookup"><span data-stu-id="67615-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="67615-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="67615-125">Authorization</span></span> | <span data-ttu-id="67615-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67615-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67615-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="67615-128">Request body</span></span>
<span data-ttu-id="67615-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="67615-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="67615-130">响应</span><span class="sxs-lookup"><span data-stu-id="67615-130">Response</span></span>
<span data-ttu-id="67615-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printJob](../resources/printjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="67615-131">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="67615-132">示例</span><span class="sxs-lookup"><span data-stu-id="67615-132">Examples</span></span>

### <a name="example-1-get-print-job"></a><span data-ttu-id="67615-133">示例1：获取打印作业</span><span class="sxs-lookup"><span data-stu-id="67615-133">Example 1: Get print job</span></span>

#### <a name="request"></a><span data-ttu-id="67615-134">请求</span><span class="sxs-lookup"><span data-stu-id="67615-134">Request</span></span>
<span data-ttu-id="67615-135">下面的示例演示了获取打印作业的元数据的请求。</span><span class="sxs-lookup"><span data-stu-id="67615-135">The following is an example of a request to get metadata for a print job.</span></span>

# <a name="http"></a>[<span data-ttu-id="67615-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="67615-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182
```
# <a name="c"></a>[<span data-ttu-id="67615-137">C#</span><span class="sxs-lookup"><span data-stu-id="67615-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67615-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67615-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67615-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67615-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="67615-140">响应</span><span class="sxs-lookup"><span data-stu-id="67615-140">Response</span></span>
<span data-ttu-id="67615-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67615-141">The following is an example of the response.</span></span>
><span data-ttu-id="67615-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="67615-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-print-job-with-task-list"></a><span data-ttu-id="67615-144">示例2：使用任务列表获取打印作业</span><span class="sxs-lookup"><span data-stu-id="67615-144">Example 2: Get print job with task list</span></span>

#### <a name="request"></a><span data-ttu-id="67615-145">请求</span><span class="sxs-lookup"><span data-stu-id="67615-145">Request</span></span>
<span data-ttu-id="67615-146">下面是一个请求，用于获取打印作业以及正在对其执行或已执行的任何 [任务](../resources/printtask.md) 。</span><span class="sxs-lookup"><span data-stu-id="67615-146">The following is a request to get a print job and any [tasks](../resources/printtask.md) that are executing, or have executed, against it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182?$expand=tasks
```

#### <a name="response"></a><span data-ttu-id="67615-147">响应</span><span class="sxs-lookup"><span data-stu-id="67615-147">Response</span></span>
<span data-ttu-id="67615-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67615-148">The following is an example of the response.</span></span>
><span data-ttu-id="67615-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="67615-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="67615-151">示例3：获取打印作业及其关联的文档数据</span><span class="sxs-lookup"><span data-stu-id="67615-151">Example 3: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="67615-152">请求</span><span class="sxs-lookup"><span data-stu-id="67615-152">Request</span></span>
<span data-ttu-id="67615-153">下面的示例演示了获取打印作业及其关联的文档数据的请求。</span><span class="sxs-lookup"><span data-stu-id="67615-153">The following is an example of a request to get a print job and its associated document data.</span></span>
# <a name="http"></a>[<span data-ttu-id="67615-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="67615-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216?$expand=documents
```
# <a name="c"></a>[<span data-ttu-id="67615-155">C#</span><span class="sxs-lookup"><span data-stu-id="67615-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withdocumentdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67615-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67615-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withdocumentdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67615-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67615-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withdocumentdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="67615-158">响应</span><span class="sxs-lookup"><span data-stu-id="67615-158">Response</span></span>
<span data-ttu-id="67615-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67615-159">The following is an example of the response.</span></span>
><span data-ttu-id="67615-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="67615-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
