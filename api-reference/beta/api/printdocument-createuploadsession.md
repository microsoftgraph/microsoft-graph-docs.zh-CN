---
title: printDocument：createUploadSession
description: 创建上载会话以迭代上载 printDocument 的二进制文件范围。
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 0dbb2a9101fbf5033d1c91f1254c6ea0ba00f6e4
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784836"
---
# <a name="printdocument-createuploadsession"></a><span data-ttu-id="374db-103">printDocument：createUploadSession</span><span class="sxs-lookup"><span data-stu-id="374db-103">printDocument: createUploadSession</span></span>

<span data-ttu-id="374db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="374db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="374db-105">创建允许应用迭代上载链接到打印文档的二进制文件范围的上载会话。</span><span class="sxs-lookup"><span data-stu-id="374db-105">Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.</span></span>

<span data-ttu-id="374db-106">作为响应的一部分，此操作返回可用于后续顺序查询的上载 `PUT` URL。</span><span class="sxs-lookup"><span data-stu-id="374db-106">As part of the response, this action returns an upload URL that can be used in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="374db-107">每个操作的请求标头可用于指定要上载的 `PUT` 字节的准确范围。</span><span class="sxs-lookup"><span data-stu-id="374db-107">Request headers for each `PUT` operation can be used to specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="374db-108">这允许恢复传输，以防在上载过程中网络连接中断。</span><span class="sxs-lookup"><span data-stu-id="374db-108">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="374db-109">权限</span><span class="sxs-lookup"><span data-stu-id="374db-109">Permissions</span></span>

<span data-ttu-id="374db-110">调用此 API 需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="374db-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="374db-111">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="374db-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
<span data-ttu-id="374db-112">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据使用的打印机或 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="374db-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

| <span data-ttu-id="374db-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="374db-113">Permission type</span></span>                        | <span data-ttu-id="374db-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="374db-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="374db-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="374db-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="374db-116">PrintJob.Create、PrintJob.ReadWrite、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="374db-116">PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="374db-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="374db-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="374db-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="374db-118">Not Supported.</span></span> |
| <span data-ttu-id="374db-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="374db-119">Application</span></span>                            | <span data-ttu-id="374db-120">PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="374db-120">PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="374db-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="374db-121">HTTP request</span></span>

<span data-ttu-id="374db-122">若要使用打印机创建上载 **会话**，</span><span class="sxs-lookup"><span data-stu-id="374db-122">To create an upload session using **printer**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

<span data-ttu-id="374db-123">若要使用 **printerShare 创建上载会话**：</span><span class="sxs-lookup"><span data-stu-id="374db-123">To create an upload session using **printerShare**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="374db-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="374db-124">Request headers</span></span>

| <span data-ttu-id="374db-125">名称</span><span class="sxs-lookup"><span data-stu-id="374db-125">Name</span></span>          | <span data-ttu-id="374db-126">说明</span><span class="sxs-lookup"><span data-stu-id="374db-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="374db-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="374db-127">Authorization</span></span> | <span data-ttu-id="374db-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="374db-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="374db-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="374db-130">Content-type</span></span> | <span data-ttu-id="374db-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="374db-p104">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="374db-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="374db-133">Request body</span></span>

<span data-ttu-id="374db-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="374db-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="374db-135">参数</span><span class="sxs-lookup"><span data-stu-id="374db-135">Parameter</span></span>    | <span data-ttu-id="374db-136">类型</span><span class="sxs-lookup"><span data-stu-id="374db-136">Type</span></span>        | <span data-ttu-id="374db-137">说明</span><span class="sxs-lookup"><span data-stu-id="374db-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="374db-138">properties</span><span class="sxs-lookup"><span data-stu-id="374db-138">properties</span></span>|[<span data-ttu-id="374db-139">printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="374db-139">printDocumentUploadProperties</span></span>](../resources/printDocumentUploadProperties.md)|<span data-ttu-id="374db-140">表示要上载的二进制文件的属性。</span><span class="sxs-lookup"><span data-stu-id="374db-140">Represents properties of the binary file to be uploaded.</span></span>|

<span data-ttu-id="374db-141">请求正文中 **contentType** 属性的值应受 printer/printerShare 支持。</span><span class="sxs-lookup"><span data-stu-id="374db-141">The value of the **contentType** property in the request body should be supported by the printer/printerShare.</span></span> <span data-ttu-id="374db-142">可以通过获取 [printer/printerShare 的 printerCapabilities](../resources/printercapabilities.md) 获取受支持的内容类型。</span><span class="sxs-lookup"><span data-stu-id="374db-142">You can get the supported content types by getting [printerCapabilities](../resources/printercapabilities.md) of the printer/printerShare.</span></span> 

<span data-ttu-id="374db-143">FOR **OXPS to PDF** conversion， you need to pass as `application/oxps` contentType for printer/printerShare that `application/pdf` supports.</span><span class="sxs-lookup"><span data-stu-id="374db-143">For **OXPS to PDF** conversion, you need to pass `application/oxps` as contentType for printer/printerShare that supports `application/pdf`.</span></span> <span data-ttu-id="374db-144">当满足以下所有条件时，通用打印会将OXPS 转换为 **PDF：**</span><span class="sxs-lookup"><span data-stu-id="374db-144">Universal Print converts **OXPS to PDF**, when **all** the following conditions are met:</span></span> 
1.  <span data-ttu-id="374db-145">打印机/打印机共享在 `application/pdf` **printerCapabilities 中支持**。</span><span class="sxs-lookup"><span data-stu-id="374db-145">The printer/printer share supports `application/pdf` in **printerCapabilities**.</span></span> 
2.  <span data-ttu-id="374db-146">打印机/打印机共享在 `application/oxps` **printerCapabilities 中不支持**。</span><span class="sxs-lookup"><span data-stu-id="374db-146">The printer/printer share does NOT support `application/oxps` in **printerCapabilities**.</span></span> 
3.  <span data-ttu-id="374db-147">请求正文中 **contentType** 属性的值为 `application/oxps` 。</span><span class="sxs-lookup"><span data-stu-id="374db-147">The value for the **contentType** property in the request body is `application/oxps`.</span></span>

## <a name="response"></a><span data-ttu-id="374db-148">响应</span><span class="sxs-lookup"><span data-stu-id="374db-148">Response</span></span>

<span data-ttu-id="374db-149">如果成功，此方法在响应正文中返回响应代码和新 `200 OK` [uploadSession](../resources/uploadsession.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="374db-149">If successful, this method returns a `200 OK` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="374db-150">**注意**：作为 **uploadSession** 响应对象的一部分返回的 **uploadUrl** 属性是后续查询的不透明 URL，用于上载文件的字节 `PUT` 范围。</span><span class="sxs-lookup"><span data-stu-id="374db-150">**Note**: The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="374db-151">它包含到期的 `PUT` **expirationDateTime** 后续查询的适当身份验证令牌。</span><span class="sxs-lookup"><span data-stu-id="374db-151">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="374db-152">不要更改此 URL。</span><span class="sxs-lookup"><span data-stu-id="374db-152">Do not change this URL.</span></span>

## <a name="examples"></a><span data-ttu-id="374db-153">示例</span><span class="sxs-lookup"><span data-stu-id="374db-153">Examples</span></span>

<span data-ttu-id="374db-154">以下示例演示如何创建可用于后续文件上载操作到指定 printDocument 的上载会话。</span><span class="sxs-lookup"><span data-stu-id="374db-154">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified printDocument.</span></span>

### <a name="request"></a><span data-ttu-id="374db-155">请求</span><span class="sxs-lookup"><span data-stu-id="374db-155">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="374db-156">响应</span><span class="sxs-lookup"><span data-stu-id="374db-156">Response</span></span>

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
