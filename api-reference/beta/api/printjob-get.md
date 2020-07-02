---
title: 获取 printJob
description: 检索打印作业的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c634c4679cf65a8e723e55a4b0b9c39298a764b3
ms.sourcegitcommit: 9f1e02ab486a2c3e0a128e5d36f46cebe4961581
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2020
ms.locfileid: "45024425"
---
# <a name="get-printjob"></a><span data-ttu-id="ce5eb-103">获取 printJob</span><span class="sxs-lookup"><span data-stu-id="ce5eb-103">Get printJob</span></span>

<span data-ttu-id="ce5eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce5eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce5eb-105">检索打印作业的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce5eb-106">权限</span><span class="sxs-lookup"><span data-stu-id="ce5eb-106">Permissions</span></span>
<span data-ttu-id="ce5eb-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ce5eb-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ce5eb-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce5eb-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ce5eb-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="ce5eb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce5eb-110">Permission type</span></span> | <span data-ttu-id="ce5eb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce5eb-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ce5eb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce5eb-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ce5eb-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="ce5eb-113">Users.Read.All</span></span> |
|<span data-ttu-id="ce5eb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce5eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce5eb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-115">Not Supported.</span></span>|
|<span data-ttu-id="ce5eb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce5eb-116">Application</span></span>|<span data-ttu-id="ce5eb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce5eb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce5eb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce5eb-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ce5eb-119">Optional query parameters</span></span>
<span data-ttu-id="ce5eb-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ce5eb-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce5eb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce5eb-122">Request headers</span></span>
| <span data-ttu-id="ce5eb-123">名称</span><span class="sxs-lookup"><span data-stu-id="ce5eb-123">Name</span></span>      |<span data-ttu-id="ce5eb-124">说明</span><span class="sxs-lookup"><span data-stu-id="ce5eb-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce5eb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce5eb-125">Authorization</span></span> | <span data-ttu-id="ce5eb-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="ce5eb-126">Bearer {token}.</span></span> <span data-ttu-id="ce5eb-127">Required.</span><span class="sxs-lookup"><span data-stu-id="ce5eb-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce5eb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce5eb-128">Request body</span></span>
<span data-ttu-id="ce5eb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ce5eb-130">响应</span><span class="sxs-lookup"><span data-stu-id="ce5eb-130">Response</span></span>
<span data-ttu-id="ce5eb-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[printJob](../resources/printjob.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-131">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="ce5eb-132">示例</span><span class="sxs-lookup"><span data-stu-id="ce5eb-132">Examples</span></span>

### <a name="example-1-get-a-print-job"></a><span data-ttu-id="ce5eb-133">示例1：获取打印作业</span><span class="sxs-lookup"><span data-stu-id="ce5eb-133">Example 1: Get a print job</span></span>

#### <a name="request"></a><span data-ttu-id="ce5eb-134">请求</span><span class="sxs-lookup"><span data-stu-id="ce5eb-134">Request</span></span>
<span data-ttu-id="ce5eb-135">下面的示例演示了获取打印作业的请求。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-135">The following is an example of a request to get a print job.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce5eb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce5eb-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}
```
# <a name="c"></a>[<span data-ttu-id="ce5eb-137">C#</span><span class="sxs-lookup"><span data-stu-id="ce5eb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce5eb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce5eb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce5eb-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce5eb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ce5eb-140">响应</span><span class="sxs-lookup"><span data-stu-id="ce5eb-140">Response</span></span>
<span data-ttu-id="ce5eb-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-141">The following is an example of the response.</span></span>
><span data-ttu-id="ce5eb-142">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="ce5eb-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ce5eb-143">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ce5eb-143">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="ce5eb-144">示例2：获取打印作业及其关联的文档数据</span><span class="sxs-lookup"><span data-stu-id="ce5eb-144">Example 2: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="ce5eb-145">请求</span><span class="sxs-lookup"><span data-stu-id="ce5eb-145">Request</span></span>
<span data-ttu-id="ce5eb-146">下面的示例演示了获取打印作业及其关联的文档数据的请求。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-146">The following is an example of a request to get a print job and its associated document data.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce5eb-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce5eb-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216?$expand=documents
```

---

#### <a name="response"></a><span data-ttu-id="ce5eb-148">响应</span><span class="sxs-lookup"><span data-stu-id="ce5eb-148">Response</span></span>
<span data-ttu-id="ce5eb-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ce5eb-149">The following is an example of the response.</span></span>
><span data-ttu-id="ce5eb-150">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="ce5eb-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ce5eb-151">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ce5eb-151">All the properties will be returned from an actual call.</span></span>
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
