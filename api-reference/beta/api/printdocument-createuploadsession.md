---
title: printDocument： createUploadSession
description: 创建上载会话以迭代上载 printDocument 的二进制文件范围。
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 55199e600be68562e256342e79f14a37cc669681
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766019"
---
# <a name="printdocument-createuploadsession"></a><span data-ttu-id="f5ab3-103">printDocument： createUploadSession</span><span class="sxs-lookup"><span data-stu-id="f5ab3-103">printDocument: createUploadSession</span></span>

<span data-ttu-id="f5ab3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5ab3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5ab3-105">创建允许应用反复上载链接到打印文档的二进制文件范围的上载会话。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-105">Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.</span></span>

<span data-ttu-id="f5ab3-106">作为响应的一部分，此操作返回可用于后续顺序查询的上载 `PUT` URL。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-106">As part of the response, this action returns an upload URL that can be used in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="f5ab3-107">每个操作的请求头可用于指定要 `PUT` 上载的字节的确切范围。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-107">Request headers for each `PUT` operation can be used to specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="f5ab3-108">这允许恢复传输，以防在上载过程中网络连接中断。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-108">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f5ab3-109">权限</span><span class="sxs-lookup"><span data-stu-id="f5ab3-109">Permissions</span></span>

<span data-ttu-id="f5ab3-110">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f5ab3-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
<span data-ttu-id="f5ab3-112">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据使用的打印机还是 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

| <span data-ttu-id="f5ab3-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5ab3-113">Permission type</span></span>                        | <span data-ttu-id="f5ab3-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5ab3-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f5ab3-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5ab3-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5ab3-116">PrintJob.Create、PrintJob.ReadWrite、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5ab3-116">PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="f5ab3-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5ab3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5ab3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-118">Not Supported.</span></span> |
| <span data-ttu-id="f5ab3-119">Application</span><span class="sxs-lookup"><span data-stu-id="f5ab3-119">Application</span></span>                            | <span data-ttu-id="f5ab3-120">PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5ab3-120">PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5ab3-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5ab3-121">HTTP request</span></span>

<span data-ttu-id="f5ab3-122">若要使用打印机创建上载 **会话**：</span><span class="sxs-lookup"><span data-stu-id="f5ab3-122">To create an upload session using **printer**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

<span data-ttu-id="f5ab3-123">使用 printerShare 创建 **上传会话：**</span><span class="sxs-lookup"><span data-stu-id="f5ab3-123">To create an upload session using **printerShare**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="f5ab3-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5ab3-124">Request headers</span></span>

| <span data-ttu-id="f5ab3-125">名称</span><span class="sxs-lookup"><span data-stu-id="f5ab3-125">Name</span></span>          | <span data-ttu-id="f5ab3-126">说明</span><span class="sxs-lookup"><span data-stu-id="f5ab3-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f5ab3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5ab3-127">Authorization</span></span> | <span data-ttu-id="f5ab3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5ab3-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="f5ab3-130">Content-type</span></span> | <span data-ttu-id="f5ab3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f5ab3-p104">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="f5ab3-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5ab3-133">Request body</span></span>

<span data-ttu-id="f5ab3-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f5ab3-135">参数</span><span class="sxs-lookup"><span data-stu-id="f5ab3-135">Parameter</span></span>    | <span data-ttu-id="f5ab3-136">类型</span><span class="sxs-lookup"><span data-stu-id="f5ab3-136">Type</span></span>        | <span data-ttu-id="f5ab3-137">说明</span><span class="sxs-lookup"><span data-stu-id="f5ab3-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f5ab3-138">properties</span><span class="sxs-lookup"><span data-stu-id="f5ab3-138">properties</span></span>|[<span data-ttu-id="f5ab3-139">printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="f5ab3-139">printDocumentUploadProperties</span></span>](../resources/printDocumentUploadProperties.md)|<span data-ttu-id="f5ab3-140">表示要上载的二进制文件的属性。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-140">Represents properties of the binary file to be uploaded.</span></span>|

<span data-ttu-id="f5ab3-141">请求正文中 **contentType** 属性的值应受 printer/printerShare 支持。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-141">The value of the **contentType** property in the request body should be supported by the printer/printerShare.</span></span> <span data-ttu-id="f5ab3-142">可以通过获取 [printer/printerShare 的 printerCapabilities](../resources/printercapabilities.md) 获取受支持的内容类型。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-142">You can get the supported content types by getting [printerCapabilities](../resources/printercapabilities.md) of the printer/printerShare.</span></span> 

<span data-ttu-id="f5ab3-143">对于 **将 OXPS 转换为 PDF，** 你需要为支持 的 `application/oxps` printer/printerShare 传递为 `application/pdf` contentType。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-143">For **OXPS to PDF** conversion, you need to pass `application/oxps` as contentType for printer/printerShare that supports `application/pdf`.</span></span> <span data-ttu-id="f5ab3-144">当满足以下所有条件 **时，通用** 打印会将 OXPS 转换为 **PDF：**</span><span class="sxs-lookup"><span data-stu-id="f5ab3-144">Universal Print converts **OXPS to PDF**, when **all** the following conditions are met:</span></span> 
1.  <span data-ttu-id="f5ab3-145">打印机/打印机共享在 `application/pdf` **printerCapabilities 中支持**。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-145">The printer/printer share supports `application/pdf` in **printerCapabilities**.</span></span> 
2.  <span data-ttu-id="f5ab3-146">`application/oxps` **printerCapabilities 不支持打印机/打印机共享**。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-146">The printer/printer share does NOT support `application/oxps` in **printerCapabilities**.</span></span> 
3.  <span data-ttu-id="f5ab3-147">请求正文中 **contentType** 属性的值为 `application/oxps` 。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-147">The value for the **contentType** property in the request body is `application/oxps`.</span></span>

## <a name="response"></a><span data-ttu-id="f5ab3-148">响应</span><span class="sxs-lookup"><span data-stu-id="f5ab3-148">Response</span></span>

<span data-ttu-id="f5ab3-149">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 [uploadSession](../resources/uploadsession.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-149">If successful, this method returns a `200 OK` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="f5ab3-150">**注意**：作为 **uploadSession** 响应对象的一部分返回的 **uploadUrl** 属性是后续查询用于上载文件的字节范围的不透明 `PUT` URL。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-150">**Note**: The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="f5ab3-151">它包含过期 `PUT` **expirationDateTime 的后续查询的适当身份验证令牌**。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-151">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="f5ab3-152">不要更改此 URL。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-152">Do not change this URL.</span></span>

## <a name="examples"></a><span data-ttu-id="f5ab3-153">示例</span><span class="sxs-lookup"><span data-stu-id="f5ab3-153">Examples</span></span>

<span data-ttu-id="f5ab3-154">以下示例演示如何创建可用于后续文件上载操作到指定 printDocument 的上载会话。</span><span class="sxs-lookup"><span data-stu-id="f5ab3-154">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified printDocument.</span></span>

### <a name="request"></a><span data-ttu-id="f5ab3-155">请求</span><span class="sxs-lookup"><span data-stu-id="f5ab3-155">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "printdocument_createuploadsession"
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

### <a name="response"></a><span data-ttu-id="f5ab3-156">响应</span><span class="sxs-lookup"><span data-stu-id="f5ab3-156">Response</span></span>

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
