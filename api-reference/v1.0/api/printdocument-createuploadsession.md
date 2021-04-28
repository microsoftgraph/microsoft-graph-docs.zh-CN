---
title: printDocument： createUploadSession
description: 创建上载会话以迭代上载 printDocument 的二进制文件范围。
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c72144dc8b4aa39a87b1c8785ba61e69dab16c37
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067213"
---
# <a name="printdocument-createuploadsession"></a><span data-ttu-id="98cea-103">printDocument： createUploadSession</span><span class="sxs-lookup"><span data-stu-id="98cea-103">printDocument: createUploadSession</span></span>
<span data-ttu-id="98cea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98cea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="98cea-105">创建允许应用反复上载链接到打印文档的二进制文件范围的上载会话。</span><span class="sxs-lookup"><span data-stu-id="98cea-105">Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.</span></span>

<span data-ttu-id="98cea-106">作为响应的一部分，此操作返回可用于后续顺序查询的上载 `PUT` URL。</span><span class="sxs-lookup"><span data-stu-id="98cea-106">As part of the response, this action returns an upload URL that can be used in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="98cea-107">每个操作的请求头可用于指定要 `PUT` 上载的字节的确切范围。</span><span class="sxs-lookup"><span data-stu-id="98cea-107">Request headers for each `PUT` operation can be used to specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="98cea-108">这允许恢复传输，以防在上载过程中网络连接中断。</span><span class="sxs-lookup"><span data-stu-id="98cea-108">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="98cea-109">权限</span><span class="sxs-lookup"><span data-stu-id="98cea-109">Permissions</span></span>
<span data-ttu-id="98cea-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98cea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="98cea-112">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据使用的打印机还是 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="98cea-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

| <span data-ttu-id="98cea-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="98cea-113">Permission type</span></span>                        | <span data-ttu-id="98cea-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98cea-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="98cea-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98cea-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="98cea-116">PrintJob.Create、PrintJob.ReadWrite、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98cea-116">PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="98cea-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98cea-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98cea-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="98cea-118">Not Supported.</span></span> |
| <span data-ttu-id="98cea-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="98cea-119">Application</span></span>                            | <span data-ttu-id="98cea-120">PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98cea-120">PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98cea-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98cea-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

<span data-ttu-id="98cea-122">若要使用打印机创建上载 **会话**：</span><span class="sxs-lookup"><span data-stu-id="98cea-122">To create an upload session using **printer**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

<span data-ttu-id="98cea-123">使用 printerShare 创建 **上传会话：**</span><span class="sxs-lookup"><span data-stu-id="98cea-123">To create an upload session using **printerShare**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="98cea-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="98cea-124">Request headers</span></span>
|<span data-ttu-id="98cea-125">名称</span><span class="sxs-lookup"><span data-stu-id="98cea-125">Name</span></span>|<span data-ttu-id="98cea-126">说明</span><span class="sxs-lookup"><span data-stu-id="98cea-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="98cea-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="98cea-127">Authorization</span></span>|<span data-ttu-id="98cea-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98cea-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="98cea-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="98cea-130">Content-Type</span></span>|<span data-ttu-id="98cea-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="98cea-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98cea-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="98cea-133">Request body</span></span>
<span data-ttu-id="98cea-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="98cea-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="98cea-135">参数</span><span class="sxs-lookup"><span data-stu-id="98cea-135">Parameter</span></span>    | <span data-ttu-id="98cea-136">类型</span><span class="sxs-lookup"><span data-stu-id="98cea-136">Type</span></span>        | <span data-ttu-id="98cea-137">说明</span><span class="sxs-lookup"><span data-stu-id="98cea-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="98cea-138">properties</span><span class="sxs-lookup"><span data-stu-id="98cea-138">properties</span></span>|[<span data-ttu-id="98cea-139">printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="98cea-139">printDocumentUploadProperties</span></span>](../resources/printDocumentUploadProperties.md)|<span data-ttu-id="98cea-140">表示要上载的二进制文件的属性。</span><span class="sxs-lookup"><span data-stu-id="98cea-140">Represents properties of the binary file to be uploaded.</span></span>|

<span data-ttu-id="98cea-141">请求正文中 **contentType** 属性的值应受 printer/printerShare 支持。</span><span class="sxs-lookup"><span data-stu-id="98cea-141">The value of the **contentType** property in the request body should be supported by the printer/printerShare.</span></span> <span data-ttu-id="98cea-142">可以通过获取 [printer/printerShare 的 printerCapabilities](../resources/printercapabilities.md) 获取受支持的内容类型。</span><span class="sxs-lookup"><span data-stu-id="98cea-142">You can get the supported content types by getting [printerCapabilities](../resources/printercapabilities.md) of the printer/printerShare.</span></span> 

<span data-ttu-id="98cea-143">对于 **将 OXPS 转换为 PDF，** 你需要为支持 的 `application/oxps` printer/printerShare 传递为 `application/pdf` contentType。</span><span class="sxs-lookup"><span data-stu-id="98cea-143">For **OXPS to PDF** conversion, you need to pass `application/oxps` as contentType for printer/printerShare that supports `application/pdf`.</span></span> <span data-ttu-id="98cea-144">当满足以下所有条件 **时，通用** 打印会将 OXPS 转换为 **PDF：**</span><span class="sxs-lookup"><span data-stu-id="98cea-144">Universal Print converts **OXPS to PDF**, when **all** the following conditions are met:</span></span> 
1.  <span data-ttu-id="98cea-145">打印机/打印机共享在 `application/pdf` **printerCapabilities 中支持**。</span><span class="sxs-lookup"><span data-stu-id="98cea-145">The printer/printer share supports `application/pdf` in **printerCapabilities**.</span></span> 
2.  <span data-ttu-id="98cea-146">`application/oxps` **printerCapabilities 不支持打印机/打印机共享**。</span><span class="sxs-lookup"><span data-stu-id="98cea-146">The printer/printer share does NOT support `application/oxps` in **printerCapabilities**.</span></span> 
3.  <span data-ttu-id="98cea-147">请求正文中 **contentType** 属性的值为 `application/oxps` 。</span><span class="sxs-lookup"><span data-stu-id="98cea-147">The value for the **contentType** property in the request body is `application/oxps`.</span></span>

## <a name="response"></a><span data-ttu-id="98cea-148">响应</span><span class="sxs-lookup"><span data-stu-id="98cea-148">Response</span></span>

<span data-ttu-id="98cea-149">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 [uploadSession](../resources/uploadsession.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98cea-149">If successful, this method returns a `200 OK` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="98cea-150">**注意**：作为 **uploadSession** 响应对象的一部分返回的 **uploadUrl** 属性是后续查询用于上载文件的字节范围的不透明 `PUT` URL。</span><span class="sxs-lookup"><span data-stu-id="98cea-150">**Note**: The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="98cea-151">它包含过期 `PUT` **expirationDateTime 的后续查询的适当身份验证令牌**。</span><span class="sxs-lookup"><span data-stu-id="98cea-151">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="98cea-152">不要更改此 URL。</span><span class="sxs-lookup"><span data-stu-id="98cea-152">Do not change this URL.</span></span>

## <a name="examples"></a><span data-ttu-id="98cea-153">示例</span><span class="sxs-lookup"><span data-stu-id="98cea-153">Examples</span></span>

<span data-ttu-id="98cea-154">以下示例演示如何创建可用于后续文件上载操作到指定 printDocument 的上载会话。</span><span class="sxs-lookup"><span data-stu-id="98cea-154">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified printDocument.</span></span>

### <a name="request"></a><span data-ttu-id="98cea-155">请求</span><span class="sxs-lookup"><span data-stu-id="98cea-155">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printdocument_createuploadsession"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/createUploadSession
Content-Type: application/json
Content-length: 96

{
  "properties": {
    "documentName": "TestFile.pdf",
    "contentType": "application/pdf", 
    "size": 4533322
  }
}
```


### <a name="response"></a><span data-ttu-id="98cea-156">响应</span><span class="sxs-lookup"><span data-stu-id="98cea-156">Response</span></span>
<span data-ttu-id="98cea-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="98cea-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}",
    "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
    "nextExpectedRanges": [
        "0-4533321"
    ]
}
```

