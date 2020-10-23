---
title: printDocument： createUploadSession
description: 创建一个上载会话，以以迭代方式上载 printDocument 的二进制文件的范围。
localization_priority: Normal
author: nilakhan
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 47043b64806cfa9ef3a66026a60b84ae11112168
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704942"
---
# <a name="printdocument-createuploadsession"></a><span data-ttu-id="77046-103">printDocument： createUploadSession</span><span class="sxs-lookup"><span data-stu-id="77046-103">printDocument: createUploadSession</span></span>

<span data-ttu-id="77046-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77046-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77046-105">创建一个上载会话，该会话允许应用程序以迭代方式上载链接到打印文档的二进制文件的范围。</span><span class="sxs-lookup"><span data-stu-id="77046-105">Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.</span></span>

<span data-ttu-id="77046-106">作为响应的一部分，此操作将返回可在后续顺序查询中使用的上载 URL `PUT` 。</span><span class="sxs-lookup"><span data-stu-id="77046-106">As part of the response, this action returns an upload URL that can be used in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="77046-107">每个操作的请求标头 `PUT` 可用于指定要上载的确切字节范围。</span><span class="sxs-lookup"><span data-stu-id="77046-107">Request headers for each `PUT` operation can be used to specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="77046-108">这样，如果在上载过程中断开网络连接，则可以恢复传输。</span><span class="sxs-lookup"><span data-stu-id="77046-108">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="77046-109">权限</span><span class="sxs-lookup"><span data-stu-id="77046-109">Permissions</span></span>

<span data-ttu-id="77046-110">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="77046-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="77046-111">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77046-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
<span data-ttu-id="77046-112">除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且拥有授予 [获取打印机](printer-get.md) 或 [获取 printerShare](printershare-get.md) 访问权限的权限，具体取决于打印机或 printerShare 是否正在使用。</span><span class="sxs-lookup"><span data-stu-id="77046-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

| <span data-ttu-id="77046-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="77046-113">Permission type</span></span>                        | <span data-ttu-id="77046-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77046-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="77046-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77046-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="77046-116">PrintJob，PrintJob。</span><span class="sxs-lookup"><span data-stu-id="77046-116">PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="77046-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77046-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77046-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="77046-118">Not Supported.</span></span> |
| <span data-ttu-id="77046-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="77046-119">Application</span></span>                            | <span data-ttu-id="77046-120">PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77046-120">PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77046-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77046-121">HTTP request</span></span>

<span data-ttu-id="77046-122">若要使用 **打印机**创建上载会话，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="77046-122">To create an upload session using **printer**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

<span data-ttu-id="77046-123">使用 **printerShare**创建上传会话的步骤：</span><span class="sxs-lookup"><span data-stu-id="77046-123">To create an upload session using **printerShare**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="77046-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="77046-124">Request headers</span></span>

| <span data-ttu-id="77046-125">名称</span><span class="sxs-lookup"><span data-stu-id="77046-125">Name</span></span>          | <span data-ttu-id="77046-126">说明</span><span class="sxs-lookup"><span data-stu-id="77046-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="77046-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="77046-127">Authorization</span></span> | <span data-ttu-id="77046-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77046-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77046-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="77046-130">Content-type</span></span> | <span data-ttu-id="77046-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="77046-p104">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="77046-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="77046-133">Request body</span></span>

<span data-ttu-id="77046-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="77046-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="77046-135">参数</span><span class="sxs-lookup"><span data-stu-id="77046-135">Parameter</span></span>    | <span data-ttu-id="77046-136">类型</span><span class="sxs-lookup"><span data-stu-id="77046-136">Type</span></span>        | <span data-ttu-id="77046-137">说明</span><span class="sxs-lookup"><span data-stu-id="77046-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77046-138">properties</span><span class="sxs-lookup"><span data-stu-id="77046-138">properties</span></span>|[<span data-ttu-id="77046-139">printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="77046-139">printDocumentUploadProperties</span></span>](../resources/printDocumentUploadProperties.md)|<span data-ttu-id="77046-140">表示要上载的二进制文件的属性。</span><span class="sxs-lookup"><span data-stu-id="77046-140">Represents properties of the binary file to be uploaded.</span></span>|

## <a name="response"></a><span data-ttu-id="77046-141">响应</span><span class="sxs-lookup"><span data-stu-id="77046-141">Response</span></span>

<span data-ttu-id="77046-142">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和新的 [uploadSession](../resources/uploadsession.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77046-142">If successful, this method returns a `200 OK` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="77046-143">**注意**：作为**uploadSession** response 对象的一部分返回的**uploadUrl**属性是一个不透明的 URL，用于随后的 `PUT` 查询，用于上传文件的字节范围。</span><span class="sxs-lookup"><span data-stu-id="77046-143">**Note**: The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="77046-144">它包含针对 ExpirationDateTime 到期的后续查询的相应 auth 令牌 `PUT` 。 **expirationDateTime**</span><span class="sxs-lookup"><span data-stu-id="77046-144">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="77046-145">请勿更改此 URL。</span><span class="sxs-lookup"><span data-stu-id="77046-145">Do not change this URL.</span></span>

## <a name="examples"></a><span data-ttu-id="77046-146">示例</span><span class="sxs-lookup"><span data-stu-id="77046-146">Examples</span></span>

<span data-ttu-id="77046-147">下面的示例演示如何创建可在后续文件上载操作中用于指定 printDocument 的上载会话。</span><span class="sxs-lookup"><span data-stu-id="77046-147">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified printDocument.</span></span>

### <a name="request"></a><span data-ttu-id="77046-148">请求</span><span class="sxs-lookup"><span data-stu-id="77046-148">Request</span></span>

<!-- {
  "blockType": "request",
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/1c879027-5120-4aaf-954a-ebfd509a3bcc/jobs/46207/documents/9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7/createUploadSession
Content-type: application/json

{
  "properties": {
    "documentName": "TestFile.pdf",
    "contentType": "application/pdf", 
    "size": 4533322
  }
}
```

### <a name="response"></a><span data-ttu-id="77046-149">响应</span><span class="sxs-lookup"><span data-stu-id="77046-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}",
    "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
    "nextExpectedRanges": [
        "0-4533321"
    ]
}
```
