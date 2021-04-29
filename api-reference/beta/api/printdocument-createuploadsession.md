---
title: printDocument： createUploadSession
description: 创建上载会话以迭代上载 printDocument 的二进制文件范围。
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7f565aacff1cf656f0697f5564763f40341981f7
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080678"
---
# <a name="printdocument-createuploadsession"></a><span data-ttu-id="9584e-103">printDocument： createUploadSession</span><span class="sxs-lookup"><span data-stu-id="9584e-103">printDocument: createUploadSession</span></span>

<span data-ttu-id="9584e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9584e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9584e-105">创建允许应用反复上载链接到打印文档的二进制文件范围的上载会话。</span><span class="sxs-lookup"><span data-stu-id="9584e-105">Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.</span></span>

<span data-ttu-id="9584e-106">作为响应的一部分，此操作返回可用于后续顺序查询的上载 `PUT` URL。</span><span class="sxs-lookup"><span data-stu-id="9584e-106">As part of the response, this action returns an upload URL that can be used in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="9584e-107">每个操作的请求头可用于指定要 `PUT` 上载的字节的确切范围。</span><span class="sxs-lookup"><span data-stu-id="9584e-107">Request headers for each `PUT` operation can be used to specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="9584e-108">这允许恢复传输，以防在上载过程中网络连接中断。</span><span class="sxs-lookup"><span data-stu-id="9584e-108">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

><span data-ttu-id="9584e-109">**注意**：只有在关联的打印作业上存在 [printTask](../resources/printTask.md) 状态（由请求应用创建的触发器启动）时，使用应用程序权限创建上载 `processing` 会话才能成功。</span><span class="sxs-lookup"><span data-stu-id="9584e-109">**Note**: Creating an upload session using application permissions will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> <span data-ttu-id="9584e-110">若要详细了解如何注册任务触发器，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="9584e-110">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="9584e-111">权限</span><span class="sxs-lookup"><span data-stu-id="9584e-111">Permissions</span></span>

<span data-ttu-id="9584e-112">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="9584e-112">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9584e-113">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9584e-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
<span data-ttu-id="9584e-114">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据使用的打印机还是 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="9584e-114">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

| <span data-ttu-id="9584e-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="9584e-115">Permission type</span></span>                        | <span data-ttu-id="9584e-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9584e-116">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9584e-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9584e-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="9584e-118">PrintJob.Create、PrintJob.ReadWrite、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9584e-118">PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="9584e-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9584e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9584e-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="9584e-120">Not Supported.</span></span> |
| <span data-ttu-id="9584e-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="9584e-121">Application</span></span>                            | <span data-ttu-id="9584e-122">PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9584e-122">PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9584e-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9584e-123">HTTP request</span></span>

<span data-ttu-id="9584e-124">若要使用打印机创建上载 **会话**：</span><span class="sxs-lookup"><span data-stu-id="9584e-124">To create an upload session using **printer**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

<span data-ttu-id="9584e-125">若要使用 **printerShare (** 仅受委派权限支持，请) ：</span><span class="sxs-lookup"><span data-stu-id="9584e-125">To create an upload session using **printerShare** (supported with delegated permissions only):</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="9584e-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="9584e-126">Request headers</span></span>

| <span data-ttu-id="9584e-127">名称</span><span class="sxs-lookup"><span data-stu-id="9584e-127">Name</span></span>          | <span data-ttu-id="9584e-128">说明</span><span class="sxs-lookup"><span data-stu-id="9584e-128">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9584e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="9584e-129">Authorization</span></span> | <span data-ttu-id="9584e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9584e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9584e-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="9584e-132">Content-type</span></span> | <span data-ttu-id="9584e-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9584e-p105">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="9584e-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="9584e-135">Request body</span></span>

<span data-ttu-id="9584e-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9584e-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9584e-137">参数</span><span class="sxs-lookup"><span data-stu-id="9584e-137">Parameter</span></span>    | <span data-ttu-id="9584e-138">类型</span><span class="sxs-lookup"><span data-stu-id="9584e-138">Type</span></span>        | <span data-ttu-id="9584e-139">说明</span><span class="sxs-lookup"><span data-stu-id="9584e-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9584e-140">properties</span><span class="sxs-lookup"><span data-stu-id="9584e-140">properties</span></span>|[<span data-ttu-id="9584e-141">printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="9584e-141">printDocumentUploadProperties</span></span>](../resources/printDocumentUploadProperties.md)|<span data-ttu-id="9584e-142">表示要上载的二进制文件的属性。</span><span class="sxs-lookup"><span data-stu-id="9584e-142">Represents properties of the binary file to be uploaded.</span></span>|

<span data-ttu-id="9584e-143">请求正文中 **contentType** 属性的值应受 printer/printerShare 支持。</span><span class="sxs-lookup"><span data-stu-id="9584e-143">The value of the **contentType** property in the request body should be supported by the printer/printerShare.</span></span> <span data-ttu-id="9584e-144">可以通过获取 [printer/printerShare 的 printerCapabilities](../resources/printercapabilities.md) 获取受支持的内容类型。</span><span class="sxs-lookup"><span data-stu-id="9584e-144">You can get the supported content types by getting [printerCapabilities](../resources/printercapabilities.md) of the printer/printerShare.</span></span> 

<span data-ttu-id="9584e-145">对于 **将 OXPS 转换为 PDF，** 你需要为支持 的 `application/oxps` printer/printerShare 传递为 `application/pdf` contentType。</span><span class="sxs-lookup"><span data-stu-id="9584e-145">For **OXPS to PDF** conversion, you need to pass `application/oxps` as contentType for printer/printerShare that supports `application/pdf`.</span></span> <span data-ttu-id="9584e-146">当满足以下所有条件 **时，通用** 打印会将 OXPS 转换为 **PDF：**</span><span class="sxs-lookup"><span data-stu-id="9584e-146">Universal Print converts **OXPS to PDF**, when **all** the following conditions are met:</span></span> 
1.  <span data-ttu-id="9584e-147">打印机/打印机共享在 `application/pdf` **printerCapabilities 中支持**。</span><span class="sxs-lookup"><span data-stu-id="9584e-147">The printer/printer share supports `application/pdf` in **printerCapabilities**.</span></span> 
2.  <span data-ttu-id="9584e-148">`application/oxps` **printerCapabilities 不支持打印机/打印机共享**。</span><span class="sxs-lookup"><span data-stu-id="9584e-148">The printer/printer share does NOT support `application/oxps` in **printerCapabilities**.</span></span> 
3.  <span data-ttu-id="9584e-149">请求正文中 **contentType** 属性的值为 `application/oxps` 。</span><span class="sxs-lookup"><span data-stu-id="9584e-149">The value for the **contentType** property in the request body is `application/oxps`.</span></span>

## <a name="response"></a><span data-ttu-id="9584e-150">响应</span><span class="sxs-lookup"><span data-stu-id="9584e-150">Response</span></span>

<span data-ttu-id="9584e-151">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 [uploadSession](../resources/uploadsession.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9584e-151">If successful, this method returns a `200 OK` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="9584e-152">**注意**：作为 **uploadSession** 响应对象的一部分返回的 **uploadUrl** 属性是后续查询用于上载文件的字节范围的不透明 `PUT` URL。</span><span class="sxs-lookup"><span data-stu-id="9584e-152">**Note**: The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="9584e-153">它包含过期 `PUT` **expirationDateTime 的后续查询的适当身份验证令牌**。</span><span class="sxs-lookup"><span data-stu-id="9584e-153">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="9584e-154">不要更改此 URL。</span><span class="sxs-lookup"><span data-stu-id="9584e-154">Do not change this URL.</span></span>

## <a name="examples"></a><span data-ttu-id="9584e-155">示例</span><span class="sxs-lookup"><span data-stu-id="9584e-155">Examples</span></span>

<span data-ttu-id="9584e-156">以下示例演示如何创建可用于后续文件上载操作到指定 printDocument 的上载会话。</span><span class="sxs-lookup"><span data-stu-id="9584e-156">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified printDocument.</span></span>

### <a name="request"></a><span data-ttu-id="9584e-157">请求</span><span class="sxs-lookup"><span data-stu-id="9584e-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9584e-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="9584e-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9584e-159">C#</span><span class="sxs-lookup"><span data-stu-id="9584e-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printdocument-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9584e-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9584e-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printdocument-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9584e-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9584e-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printdocument-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9584e-162">Java</span><span class="sxs-lookup"><span data-stu-id="9584e-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printdocument-createuploadsession-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9584e-163">响应</span><span class="sxs-lookup"><span data-stu-id="9584e-163">Response</span></span>

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
