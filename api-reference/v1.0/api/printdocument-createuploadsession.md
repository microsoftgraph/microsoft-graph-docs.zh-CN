---
title: printDocument： createUploadSession
description: 创建上载会话以迭代上载 printDocument 的二进制文件范围。
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 164a5ca3bf6b2f53c3c5952d49f605493b4d9275
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080083"
---
# <a name="printdocument-createuploadsession"></a><span data-ttu-id="109de-103">printDocument： createUploadSession</span><span class="sxs-lookup"><span data-stu-id="109de-103">printDocument: createUploadSession</span></span>
<span data-ttu-id="109de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="109de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="109de-105">创建允许应用反复上载链接到打印文档的二进制文件范围的上载会话。</span><span class="sxs-lookup"><span data-stu-id="109de-105">Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.</span></span>

<span data-ttu-id="109de-106">作为响应的一部分，此操作返回可用于后续顺序查询的上载 `PUT` URL。</span><span class="sxs-lookup"><span data-stu-id="109de-106">As part of the response, this action returns an upload URL that can be used in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="109de-107">每个操作的请求头可用于指定要 `PUT` 上载的字节的确切范围。</span><span class="sxs-lookup"><span data-stu-id="109de-107">Request headers for each `PUT` operation can be used to specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="109de-108">这允许恢复传输，以防在上载过程中网络连接中断。</span><span class="sxs-lookup"><span data-stu-id="109de-108">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

><span data-ttu-id="109de-109">**注意**：只有在关联的打印作业上存在 [printTask](../resources/printTask.md) 状态（由请求应用创建的触发器启动）时，使用应用程序权限创建上载 `processing` 会话才能成功。</span><span class="sxs-lookup"><span data-stu-id="109de-109">**Note**: Creating an upload session using application permissions will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> <span data-ttu-id="109de-110">若要详细了解如何注册任务触发器，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="109de-110">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="109de-111">权限</span><span class="sxs-lookup"><span data-stu-id="109de-111">Permissions</span></span>
<span data-ttu-id="109de-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="109de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="109de-114">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据使用的打印机还是 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="109de-114">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

| <span data-ttu-id="109de-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="109de-115">Permission type</span></span>                        | <span data-ttu-id="109de-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="109de-116">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="109de-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="109de-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="109de-118">PrintJob.Create、PrintJob.ReadWrite、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="109de-118">PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="109de-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="109de-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="109de-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="109de-120">Not Supported.</span></span> |
| <span data-ttu-id="109de-121">Application</span><span class="sxs-lookup"><span data-stu-id="109de-121">Application</span></span>                            | <span data-ttu-id="109de-122">PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="109de-122">PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="109de-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="109de-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

<span data-ttu-id="109de-124">若要使用打印机创建上载 **会话**：</span><span class="sxs-lookup"><span data-stu-id="109de-124">To create an upload session using **printer**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

<span data-ttu-id="109de-125">若要使用 **printerShare (** 仅受委派权限支持，请) ：</span><span class="sxs-lookup"><span data-stu-id="109de-125">To create an upload session using **printerShare** (supported with delegated permissions only):</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="109de-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="109de-126">Request headers</span></span>
|<span data-ttu-id="109de-127">名称</span><span class="sxs-lookup"><span data-stu-id="109de-127">Name</span></span>|<span data-ttu-id="109de-128">说明</span><span class="sxs-lookup"><span data-stu-id="109de-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="109de-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="109de-129">Authorization</span></span>|<span data-ttu-id="109de-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="109de-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="109de-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="109de-132">Content-Type</span></span>|<span data-ttu-id="109de-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="109de-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="109de-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="109de-135">Request body</span></span>
<span data-ttu-id="109de-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="109de-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="109de-137">参数</span><span class="sxs-lookup"><span data-stu-id="109de-137">Parameter</span></span>    | <span data-ttu-id="109de-138">类型</span><span class="sxs-lookup"><span data-stu-id="109de-138">Type</span></span>        | <span data-ttu-id="109de-139">说明</span><span class="sxs-lookup"><span data-stu-id="109de-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="109de-140">properties</span><span class="sxs-lookup"><span data-stu-id="109de-140">properties</span></span>|[<span data-ttu-id="109de-141">printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="109de-141">printDocumentUploadProperties</span></span>](../resources/printDocumentUploadProperties.md)|<span data-ttu-id="109de-142">表示要上载的二进制文件的属性。</span><span class="sxs-lookup"><span data-stu-id="109de-142">Represents properties of the binary file to be uploaded.</span></span>|

<span data-ttu-id="109de-143">请求正文中 **contentType** 属性的值应受 printer/printerShare 支持。</span><span class="sxs-lookup"><span data-stu-id="109de-143">The value of the **contentType** property in the request body should be supported by the printer/printerShare.</span></span> <span data-ttu-id="109de-144">可以通过获取 [printer/printerShare 的 printerCapabilities](../resources/printercapabilities.md) 获取受支持的内容类型。</span><span class="sxs-lookup"><span data-stu-id="109de-144">You can get the supported content types by getting [printerCapabilities](../resources/printercapabilities.md) of the printer/printerShare.</span></span> 

<span data-ttu-id="109de-145">对于 **将 OXPS 转换为 PDF，** 你需要为支持 的 `application/oxps` printer/printerShare 传递为 `application/pdf` contentType。</span><span class="sxs-lookup"><span data-stu-id="109de-145">For **OXPS to PDF** conversion, you need to pass `application/oxps` as contentType for printer/printerShare that supports `application/pdf`.</span></span> <span data-ttu-id="109de-146">当满足以下所有条件 **时，通用** 打印会将 OXPS 转换为 **PDF：**</span><span class="sxs-lookup"><span data-stu-id="109de-146">Universal Print converts **OXPS to PDF**, when **all** the following conditions are met:</span></span> 
1.  <span data-ttu-id="109de-147">打印机/打印机共享在 `application/pdf` **printerCapabilities 中支持**。</span><span class="sxs-lookup"><span data-stu-id="109de-147">The printer/printer share supports `application/pdf` in **printerCapabilities**.</span></span> 
2.  <span data-ttu-id="109de-148">`application/oxps` **printerCapabilities 不支持打印机/打印机共享**。</span><span class="sxs-lookup"><span data-stu-id="109de-148">The printer/printer share does NOT support `application/oxps` in **printerCapabilities**.</span></span> 
3.  <span data-ttu-id="109de-149">请求正文中 **contentType** 属性的值为 `application/oxps` 。</span><span class="sxs-lookup"><span data-stu-id="109de-149">The value for the **contentType** property in the request body is `application/oxps`.</span></span>

## <a name="response"></a><span data-ttu-id="109de-150">响应</span><span class="sxs-lookup"><span data-stu-id="109de-150">Response</span></span>

<span data-ttu-id="109de-151">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 [uploadSession](../resources/uploadsession.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="109de-151">If successful, this method returns a `200 OK` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="109de-152">**注意**：作为 **uploadSession** 响应对象的一部分返回的 **uploadUrl** 属性是后续查询用于上载文件的字节范围的不透明 `PUT` URL。</span><span class="sxs-lookup"><span data-stu-id="109de-152">**Note**: The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="109de-153">它包含过期 `PUT` **expirationDateTime 的后续查询的适当身份验证令牌**。</span><span class="sxs-lookup"><span data-stu-id="109de-153">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="109de-154">不要更改此 URL。</span><span class="sxs-lookup"><span data-stu-id="109de-154">Do not change this URL.</span></span>

## <a name="examples"></a><span data-ttu-id="109de-155">示例</span><span class="sxs-lookup"><span data-stu-id="109de-155">Examples</span></span>

<span data-ttu-id="109de-156">以下示例演示如何创建可用于后续文件上载操作到指定 printDocument 的上载会话。</span><span class="sxs-lookup"><span data-stu-id="109de-156">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified printDocument.</span></span>

### <a name="request"></a><span data-ttu-id="109de-157">请求</span><span class="sxs-lookup"><span data-stu-id="109de-157">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="109de-158">响应</span><span class="sxs-lookup"><span data-stu-id="109de-158">Response</span></span>
<span data-ttu-id="109de-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="109de-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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

