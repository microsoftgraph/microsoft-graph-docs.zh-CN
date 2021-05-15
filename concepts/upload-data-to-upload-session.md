---
title: 使用 Microsoft Graph 通用打印 API 上载文档
description: 通用打印是一种新式打印解决方案，组织可以使用它通过 Microsoft 云服务来管理自己的打印基础设施。
author: nilakhan
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: bd34071caf8d428847693be86eb7082e7f80e99c
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473260"
---
# <a name="upload-documents-using-the-microsoft-graph-universal-print-api"></a><span data-ttu-id="04d88-103">使用 Microsoft Graph 通用打印 API 上载文档</span><span class="sxs-lookup"><span data-stu-id="04d88-103">Upload documents using the Microsoft Graph Universal Print API</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../api-reference/includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="04d88-104">若要使用 Microsoft Graph 中的通用打印 API 打印文档，你需要 [创建一个打印作业](/graph/api/printershare-post-jobs)、上传文档，然后 [启动打印作业](/graph/api/printjob-start)。</span><span class="sxs-lookup"><span data-stu-id="04d88-104">To print a document using the Universal Print API in Microsoft Graph, you [create a print job](/graph/api/printershare-post-jobs), upload a document, and then [start the print job](/graph/api/printjob-start).</span></span> <span data-ttu-id="04d88-105">本文介绍了如何上传文档，首先需要 [创建一个上载会话](/graph/api/printdocument-createuploadsession)。</span><span class="sxs-lookup"><span data-stu-id="04d88-105">This article describes how to upload a document, which starts with [creating an upload session](/graph/api/printdocument-createuploadsession).</span></span>

<span data-ttu-id="04d88-106">若要上传文件或文件的一部分，你的应用可以对在 **createUploadSession** 响应中收到的 **uploadUrl** 值发出 PUT 请求。</span><span class="sxs-lookup"><span data-stu-id="04d88-106">To upload a file, or a portion of a file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="04d88-107">可以上传整个文件，也可以将文件拆分为多个字节范围，只要任意给定请求中的最大字节数小于 10 MB 即可。</span><span class="sxs-lookup"><span data-stu-id="04d88-107">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 10 MB.</span></span>

<span data-ttu-id="04d88-108">可按任意顺序上传文件的片段，并且最多可并行上传四个并发请求。</span><span class="sxs-lookup"><span data-stu-id="04d88-108">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="04d88-109">上传文档的所有二进制片段时，二进制文件将链接到 **printDocument**。</span><span class="sxs-lookup"><span data-stu-id="04d88-109">When all the binary segments of a document are uploaded, the binary file is linked to the **printDocument**.</span></span>

## <a name="http-request"></a><span data-ttu-id="04d88-110">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04d88-110">HTTP request</span></span>

<span data-ttu-id="04d88-111">向 **createUploadSession** 响应中收到的 **uploadUrl** 值发出 PUT 请求。</span><span class="sxs-lookup"><span data-stu-id="04d88-111">Make a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="04d88-112">请求标头</span><span class="sxs-lookup"><span data-stu-id="04d88-112">Request headers</span></span>
| <span data-ttu-id="04d88-113">名称</span><span class="sxs-lookup"><span data-stu-id="04d88-113">Name</span></span>          | <span data-ttu-id="04d88-114">说明</span><span class="sxs-lookup"><span data-stu-id="04d88-114">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="04d88-115">Content-Range</span><span class="sxs-lookup"><span data-stu-id="04d88-115">Content-Range</span></span> | <span data-ttu-id="04d88-116">bytes {startByteIndex}-{endByteIndex}‬/{documentSizeInBytes}。</span><span class="sxs-lookup"><span data-stu-id="04d88-116">bytes {startByteIndex}-{endByteIndex}‬/{documentSizeInBytes}.</span></span> <span data-ttu-id="04d88-117">必填。</span><span class="sxs-lookup"><span data-stu-id="04d88-117">Required.</span></span>|
| <span data-ttu-id="04d88-118">Content-Length</span><span class="sxs-lookup"><span data-stu-id="04d88-118">Content-Length</span></span> | <span data-ttu-id="04d88-119">需要 {contentLength}。</span><span class="sxs-lookup"><span data-stu-id="04d88-119">{contentLength}‬ Required.</span></span>|

### <a name="request-body"></a><span data-ttu-id="04d88-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="04d88-120">Request body</span></span>
<span data-ttu-id="04d88-121">请求正文是一个二进制 blob，其中包含在 `Content-Range` 标头中指定为 **非独占** 字节范围的文档的字节数。</span><span class="sxs-lookup"><span data-stu-id="04d88-121">The request body is a binary blob containing the bytes of the document that are specified as an **inclusive** byte range in the `Content-Range` header.</span></span> 

### <a name="example"></a><span data-ttu-id="04d88-122">示例</span><span class="sxs-lookup"><span data-stu-id="04d88-122">Example</span></span>

```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Range: bytes=0-72796/4533322
Content-Length: 72797

<bytes 0-72796 of the file>

```

<span data-ttu-id="04d88-123">此处的 0 和 72796 是文件段的开始索引和结束索引，而 4533322 则是文档的大小。</span><span class="sxs-lookup"><span data-stu-id="04d88-123">Here, 0 and 72796 are the start and end indexes of the file segment and 4533322 is the size of document.</span></span>
## <a name="http-response"></a><span data-ttu-id="04d88-124">HTTP 响应</span><span class="sxs-lookup"><span data-stu-id="04d88-124">HTTP response</span></span>

<span data-ttu-id="04d88-125">当此请求完成时，如果还需要上传其他字节范围，服务器将会返回 `202 Accepted` 作为响应。</span><span class="sxs-lookup"><span data-stu-id="04d88-125">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": ["72797-4533321"]
}
```

<span data-ttu-id="04d88-126">应用可以使用 **nextExpectedRanges** 值来确定开始上传下一字节范围的位置。</span><span class="sxs-lookup"><span data-stu-id="04d88-126">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span> <span data-ttu-id="04d88-127">可能会发现指定的多个范围，这些范围指明了服务器尚未收到的文件部分。</span><span class="sxs-lookup"><span data-stu-id="04d88-127">You might see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="04d88-128">**nextExpectedRanges** 属性指示尚未收到的文件的范围，而不是应用应上传文件的方式。</span><span class="sxs-lookup"><span data-stu-id="04d88-128">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": [
  "72797-72897",
  "78929-4533322"
  ]
}
```

### <a name="remarks"></a><span data-ttu-id="04d88-129">备注</span><span class="sxs-lookup"><span data-stu-id="04d88-129">Remarks</span></span>

* <span data-ttu-id="04d88-130">如果因客户端发送了服务器已接收的片段导致失败，服务器将响应 `HTTP 416 Requested Range Not Satisfiable`。</span><span class="sxs-lookup"><span data-stu-id="04d88-130">On failures, when the client sends a fragment the server has already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`.</span></span> 
  <span data-ttu-id="04d88-131">可以[请求获取上传状态](#get-the-upload-session)，以获取缺少范围的更详细列表。</span><span class="sxs-lookup"><span data-stu-id="04d88-131">You can [request upload status](#get-the-upload-session) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="04d88-132">在进行 `PUT` 调用时添加 `Authorizatio`n 标头可能会导致 `HTTP 401 Unauthorized` 响应。</span><span class="sxs-lookup"><span data-stu-id="04d88-132">Including the `Authorizatio`n header when making the `PUT` call might result in an `HTTP 401 Unauthorized` response.</span></span> <span data-ttu-id="04d88-133">授权标头和持有者令牌只应在创建上传会话时发送。</span><span class="sxs-lookup"><span data-stu-id="04d88-133">The Authorization header and bearer token should only be sent when creating the upload session.</span></span> <span data-ttu-id="04d88-134">将数据上传到上传会话时，不应将其包含在内。</span><span class="sxs-lookup"><span data-stu-id="04d88-134">It should be not be included when uploading data to the upload session.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="04d88-135">完成文件</span><span class="sxs-lookup"><span data-stu-id="04d88-135">Completing a file</span></span>

<span data-ttu-id="04d88-136">接收文件的最后一个字节范围时，服务器将响应 `HTTP 201 Created`。</span><span class="sxs-lookup"><span data-stu-id="04d88-136">When the last byte range of a file is received, the server will respond with an `HTTP 201 Created`.</span></span> <span data-ttu-id="04d88-137">响应正文中还将包括关联 **printDocument** 的属性集。</span><span class="sxs-lookup"><span data-stu-id="04d88-137">The response body will also include the property set for the associated **printDocument**.</span></span>

### <a name="request"></a><span data-ttu-id="04d88-138">请求</span><span class="sxs-lookup"><span data-stu-id="04d88-138">Request</span></span>
<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "printjob.readwrite" } -->
```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Length: 10
Content-Range: bytes 4533312-4533321/4533322

<final bytes of the file>
```

### <a name="response"></a><span data-ttu-id="04d88-139">响应</span><span class="sxs-lookup"><span data-stu-id="04d88-139">Response</span></span>
<!-- { "blockType": "response", "@odata.type": "microsoft.graph.printDocument", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
   "id": "9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7",
   "documentName": "TestFile.pdf",
   "contentType": "application/pdf", 
   "size": 4533322
}
```

><span data-ttu-id="04d88-140">**注意：** 文档上传完成后，上传会话将会删除。</span><span class="sxs-lookup"><span data-stu-id="04d88-140">**Note:** The upload session is deleted after the document upload is complete.</span></span>

## <a name="get-the-upload-session"></a><span data-ttu-id="04d88-141">获取上传会话</span><span class="sxs-lookup"><span data-stu-id="04d88-141">Get the upload session</span></span>

<span data-ttu-id="04d88-142">若要获取上传会话，请将 GET 请求发送到上传 URL。</span><span class="sxs-lookup"><span data-stu-id="04d88-142">To get the upload session, send a GET request to the upload URL.</span></span> 

### <a name="request"></a><span data-ttu-id="04d88-143">请求</span><span class="sxs-lookup"><span data-stu-id="04d88-143">Request</span></span>
<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```http
GET https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a><span data-ttu-id="04d88-144">响应</span><span class="sxs-lookup"><span data-stu-id="04d88-144">Response</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": [
  "72797-72897",
  "78929-4533322"
  ]
}
```
## <a name="code-examples-create-upload-session-and-upload-documents"></a><span data-ttu-id="04d88-145">代码示例：创建上传会话和上传文档</span><span class="sxs-lookup"><span data-stu-id="04d88-145">Code examples: Create upload session and upload documents</span></span>
 
# <a name="c"></a>[<span data-ttu-id="04d88-146">C#</span><span class="sxs-lookup"><span data-stu-id="04d88-146">C#</span></span>](#tab/csharp)

```csharp

            GraphServiceClient graphClient = new GraphServiceClient( authProvider );

            var properties = new PrintDocumentUploadProperties
            {
                DocumentName = "TestFile.pdf",
                ContentType = "application/pdf",
                Size = 4533322
            };

            var uploadSession = await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"].Documents["{printDocument-id}"]
                .CreateUploadSession(properties)
                .Request()
                .PostAsync()

            // if using Graph SDK, maxSliceSize should in multiples of 320 KiB
            int maxSliceSize = 320 * 1024;
            var fileUploadTask =
                new LargeFileUploadTask<PrintDocument>(uploadSession, fileStream, maxSliceSize);

            // Create a callback that is invoked after each slice is uploaded
            IProgress<long> progress = new Progress<long>(prog =>
            {
                Console.WriteLine($"Uploaded {prog} bytes of {fileStream.Length} bytes");
            });

            // Upload the file

            var uploadResult = await fileUploadTask.UploadAsync(progress);
```

# <a name="javascript"></a>[<span data-ttu-id="04d88-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04d88-147">JavaScript</span></span>](#tab/javascript)

```javascript

    const options = {
      authProvider,
    };
    const client = Client.init(options);
   
   const fileName = "test.txt";
    const file = fs.readFileSync(`./${fileName}`);
    const stats = fs.statSync(`./${fileName}`);
    const requestUrl ="https://graph.microsoft.com/v1.0/print/shares/{id}/jobs/{id}/documents/{id}/createuploadsession"
    const payload = {
        "properties": {
            "documentName": fileName,
            "contentType": "application/pdf",
            "size": stats.size
        }
    }
    const uploadSession = await LargeFileUploadTask.createUploadSession(client, requestUrl, payload);

    const fileObject = {
        content: file,
        name: fileName,
        size: stats.size
    };

    const task = new LargeFileUploadTask(client, fileObject, uploadSession);

    const uploadResponse = await task.upload();
```
---

## <a name="cancel-the-upload-session"></a><span data-ttu-id="04d88-148">取消上传会话</span><span class="sxs-lookup"><span data-stu-id="04d88-148">Cancel the upload session</span></span>

<span data-ttu-id="04d88-p109">若要取消上传会话，请将 DELETE 请求发送到上传 URL。应在上传中止（例如，如果用户取消传输）的情况下使用此方法。</span><span class="sxs-lookup"><span data-stu-id="04d88-p109">To cancel an upload session, send a DELETE request to the upload URL. This should be used in scenarios where the upload is aborted; for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="04d88-151">**expirationDateTime** 通过后，系统将自动清理临时文件及其随附的上载会话。</span><span class="sxs-lookup"><span data-stu-id="04d88-151">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>

### <a name="request"></a><span data-ttu-id="04d88-152">请求</span><span class="sxs-lookup"><span data-stu-id="04d88-152">Request</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "printjob.readwrite" } -->

```http
DELETE https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a><span data-ttu-id="04d88-153">响应</span><span class="sxs-lookup"><span data-stu-id="04d88-153">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
