---
title: 使用 Microsoft Graph 通用打印 API 上载文档
description: 通用打印是一种新式打印解决方案，组织可以使用它通过 Microsoft 云服务来管理自己的打印基础设施。
author: nilakhan
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: 78f876cdd2269dac9f9b68915f59d9ae2dd0b51d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265810"
---
# <a name="upload-documents-using-the-microsoft-graph-universal-print-api"></a>使用 Microsoft Graph 通用打印 API 上载文档

[!INCLUDE [cloudprinting-pricing-disclaimer](../api-reference/includes/cloudprinting-pricing-disclaimer.md)]

若要使用 Microsoft Graph 中的通用打印 API 打印文档，你需要 [创建一个打印作业](/graph/api/printershare-post-jobs)、上传文档，然后 [启动打印作业](/graph/api/printjob-start)。 本文介绍了如何上传文档，首先需要 [创建一个上载会话](/graph/api/printdocument-createuploadsession)。

若要上传文件或文件的一部分，你的应用可以对在 **createUploadSession** 响应中收到的 **uploadUrl** 值发出 PUT 请求。
可以上传整个文件，也可以将文件拆分为多个字节范围，只要任意给定请求中的最大字节数小于 10 MB 即可。

可按任意顺序上传文件的片段，并且最多可并行上传四个并发请求。 上传文档的所有二进制片段时，二进制文件将链接到 **printDocument**。

## <a name="http-request"></a>HTTP 请求

向 **createUploadSession** 响应中收到的 **uploadUrl** 值发出 PUT 请求。

### <a name="request-headers"></a>请求标头
| 名称          | 说明   |
|:--------------|:--------------|
| Content-Range | bytes {startByteIndex}-{endByteIndex}‬/{documentSizeInBytes}。 必填。|
| Content-Length | 需要 {contentLength}。|

### <a name="request-body"></a>请求正文
请求正文是一个二进制 blob，其中包含在 `Content-Range` 标头中指定为 **非独占** 字节范围的文档的字节数。 

### <a name="example"></a>示例

```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Range: bytes=0-72796/4533322
Content-Length: 72797

<bytes 0-72796 of the file>

```

此处的 0 和 72796 是文件段的开始索引和结束索引，而 4533322 则是文档的大小。
## <a name="http-response"></a>HTTP 响应

当此请求完成时，如果还需要上传其他字节范围，服务器将会返回 `202 Accepted` 作为响应。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": ["72797-4533321"]
}
```

应用可以使用 **nextExpectedRanges** 值来确定开始上传下一字节范围的位置。 可能会发现指定的多个范围，这些范围指明了服务器尚未收到的文件部分。 **nextExpectedRanges** 属性指示尚未收到的文件的范围，而不是应用应上传文件的方式。

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

### <a name="remarks"></a>备注

* 如果因客户端发送服务器已接收的片段导致失败，服务器将响应 `HTTP 416 Requested Range Not Satisfiable`。可以 [请求上载状态](#get-the-upload-session) 以获取缺少范围的详细列表。
* 在进行 `PUT` 调用时添加 `Authorizatio`n 标头可能会导致 `HTTP 401 Unauthorized` 响应。 授权标头和持有者令牌只应在创建上传会话时发送。 将数据上传到上传会话时，不应将其包含在内。

## <a name="completing-a-file"></a>完成文件

接收文件的最后一个字节范围时，服务器将响应 `HTTP 201 Created`。 响应正文中还将包括关联 **printDocument** 的属性集。

### <a name="request"></a>请求
<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "printjob.readwrite" } -->
```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Length: 10
Content-Range: bytes 4533312-4533321/4533322

<final bytes of the file>
```

### <a name="response"></a>响应
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

>**注意：** 文档上传完成后，上传会话将会删除。

## <a name="get-the-upload-session"></a>获取上传会话

若要获取上传会话，请将 GET 请求发送到上传 URL。 

### <a name="request"></a>请求
<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```http
GET https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a>响应

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
## <a name="code-examples-create-upload-session-and-upload-documents"></a>代码示例：创建上传会话和上传文档
 
# <a name="c"></a>[C#](#tab/csharp)

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

# <a name="javascript"></a>[JavaScript](#tab/javascript)

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

    // Create FileUpload object. 
    /* Note:
     * As alternatives to using a javascript `File` object to create a `FileUpload`, 
     * you can use a `ReadStream` object to create a `StreamUpload`.
     * const readStream = fs.createReadStream(`./test/sample_files/${fileName}`);
     * const fileObject = new StreamUpload(readStream, fileName, totalsize);
     * OR
     * you can also create a custom implementation of the `FileObject` interface.
     * FileUpload and StreamUpload classes are available in 3.0.0 version of the Microsoft Graph JS client library.
     */
    const fileObject = new FileUpload(file, file.name, file.size);
     
    // Create LargeFileUploadTask object and start the upload() task
    const task = new LargeFileUploadTask(client, fileObject, uploadSession);
    const uploadResponse = await task.upload();
```
---

## <a name="cancel-the-upload-session"></a>取消上传会话

若要取消上传会话，请将 DELETE 请求发送到上传 URL。应在上传中止（例如，如果用户取消传输）的情况下使用此方法。

**expirationDateTime** 通过后，系统将自动清理临时文件及其随附的上载会话。

### <a name="request"></a>请求

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "printjob.readwrite" } -->

```http
DELETE https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a>响应

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
