# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="a98b0-101">通过上载会话上载大文件</span><span class="sxs-lookup"><span data-stu-id="a98b0-101">Upload large files with an upload session</span></span>

<span data-ttu-id="a98b0-p101">通过创建上传会话，使应用可以上传最大大小的文件。上传会话使应用可以在连续的 API 请求中上传多个范围的文件，这样一来，如果在上传过程中连接断开，应用也可以继续传输文件。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p101">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequental API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="a98b0-104">若要使用上传会话上传文件，请执行以下两个步骤：</span><span class="sxs-lookup"><span data-stu-id="a98b0-104">To upload a file using an upload session, there are two steps:</span></span>

1. [<span data-ttu-id="a98b0-105">创建上载会话</span><span class="sxs-lookup"><span data-stu-id="a98b0-105">Create an upload session</span></span>](#create-an-upload-session)
2. [<span data-ttu-id="a98b0-106">将字节上传到上传会话</span><span class="sxs-lookup"><span data-stu-id="a98b0-106">Upload bytes to the upload session</span></span>](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a><span data-ttu-id="a98b0-107">权限</span><span class="sxs-lookup"><span data-stu-id="a98b0-107">Permissions</span></span>
<span data-ttu-id="a98b0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a98b0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a98b0-110">Permission type</span></span>      | <span data-ttu-id="a98b0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a98b0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a98b0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a98b0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a98b0-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a98b0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a98b0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a98b0-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a98b0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a98b0-116">Application</span></span> | <span data-ttu-id="a98b0-117">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-117">Sites.ReadWrite.All</span></span> |

> <span data-ttu-id="a98b0-p103">**注意**：此 API 尚不支持 Files.ReadWrite.All 应用程序权限。即将规划提供完全支持。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p103">**Note**: The Files.ReadWrite.All application permission is not yet supported on this API. Full support is planned soon.</span></span> 

## <a name="create-an-upload-session"></a><span data-ttu-id="a98b0-120">创建上载会话</span><span class="sxs-lookup"><span data-stu-id="a98b0-120">Create an upload session</span></span>

<span data-ttu-id="a98b0-p104">要开始上载大文件，你的应用程序必须先请求新的上载会话。这可以创建一个临时存储位置，在上载完成之前保存文件字节数。上载最后一个字节后，上载会话即完成，最终文件会出现在目标文件夹中。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p104">To begin a large file upload, your app must first request a new upload session. This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded. Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>

### <a name="http-request"></a><span data-ttu-id="a98b0-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a98b0-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root:/{path-to-item}:/createUploadSession
POST /me/drive/items/{parent-item-id}:/{filename}:/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="a98b0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a98b0-125">Request body</span></span>
<span data-ttu-id="a98b0-p105">不需要请求正文。但是，你可以指定请求正文，以便提供与正在上载的文件有关的其他数据。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p105">No request body is required. However, you can specify a request body to provide additional data about the file being uploaded.</span></span>

<span data-ttu-id="a98b0-128">例如，要控制是否已获得文件名的行为，可以在请求正文中指定冲突行为属性。</span><span class="sxs-lookup"><span data-stu-id="a98b0-128">For example, to control the behavior if the filename is already taken, you can specify the conflict behavior property in the body of the request.</span></span>

```json
{
    "item": {
        "@microsoft.graph.conflictBehavior": "rename"
    }
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="a98b0-129">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="a98b0-129">Optional request headers</span></span>

| <span data-ttu-id="a98b0-130">名称</span><span class="sxs-lookup"><span data-stu-id="a98b0-130">Name</span></span>       | <span data-ttu-id="a98b0-131">值</span><span class="sxs-lookup"><span data-stu-id="a98b0-131">Value</span></span> | <span data-ttu-id="a98b0-132">说明</span><span class="sxs-lookup"><span data-stu-id="a98b0-132">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a98b0-133">*if-match*</span><span class="sxs-lookup"><span data-stu-id="a98b0-133">*if-match*</span></span> | <span data-ttu-id="a98b0-134">etag</span><span class="sxs-lookup"><span data-stu-id="a98b0-134">etag</span></span>  | <span data-ttu-id="a98b0-135">如果包含此请求标头，且提供的 eTag（或 cTag）与项目中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 错误响应。</span><span class="sxs-lookup"><span data-stu-id="a98b0-135">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` errr response is returned.</span></span> |

### <a name="response"></a><span data-ttu-id="a98b0-136">响应</span><span class="sxs-lookup"><span data-stu-id="a98b0-136">Response</span></span>
<span data-ttu-id="a98b0-137">对此请求的响应将提供新建 [uploadSession](../resources/uploadsession.md) 的详细信息，其中包括用于上载部分文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="a98b0-137">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

### <a name="example"></a><span data-ttu-id="a98b0-138">示例</span><span class="sxs-lookup"><span data-stu-id="a98b0-138">Example</span></span>

<!-- {
  "blockType": "request",
  "name": "driveItem_createUploadSession"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createUploadSession
```

##### <a name="response"></a><span data-ttu-id="a98b0-139">响应</span><span class="sxs-lookup"><span data-stu-id="a98b0-139">Response</span></span> 

<span data-ttu-id="a98b0-140">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a98b0-140">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://tenant-my.sharepoint.com/alkjl1kjklna",
  "expirationDateTime": "2020-08-24T10:58:00Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="a98b0-141">将字节上传到上传会话</span><span class="sxs-lookup"><span data-stu-id="a98b0-141">Upload bytes to the upload session</span></span>

<span data-ttu-id="a98b0-p106">若要上载文件或文件的一部分，你的应用程序可以对在 **createUploadSession** 响应中收到的 **uploadUrl** 值创建 PUT 请求。你可以上载整个文件，也可以将文件拆分为多个片段，只要任意给定请求的最大字节数少于 60 MiB 即可。必须按顺序上载文件的片段。不按顺序上载文件的片段将导致错误。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p106">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response. You can upload the entire file, or split the file into fragments, as long as the maximum bytes in any given request is less than 60 MiB. The fragments of the file must be uploaded sequentally in order. Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="a98b0-p107">**注意：**如果应用程序将一个文件拆分成多个片段，则每个片段的大小**必须**是 320 KiB 的倍数。如果使用的片断大小不能被 320 整除，会导致在提交某些文件时出错。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p107">**Note:** If your app splits a file into multiple fragments, the size of each fragment **MUST** be a multiple of 320 KiB. Using a fragment size that does not divide evenly by 320 will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="a98b0-148">示例</span><span class="sxs-lookup"><span data-stu-id="a98b0-148">Example</span></span>

<span data-ttu-id="a98b0-p108">本示例将上载 128 字节大小的文件中的前 26 个字节。**Content-Length** 标头指定当前请求的大小。**Content-Range** 标头指定此请求表示的整个文件中的字节范围。必须先知道文件的总长度，然后才可以上载文件的第一个片段。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p108">This example is uploading the first 26 bytes of a 128 byte file. The **Content-Length** header specifies the size of the current request. The **Content-Range** header indicates the range of bytes in the overall file that this request represents. The total length of the file must be known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="a98b0-p109">**重要说明：**应用程序必须确保 **Content-Range** 标头中指定的文件总大小对于所有的请求都相同。如果某片段声明有不同的文件大小，则请求将失败。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p109">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests. If a fragment declares a different file size, the request will fail.</span></span>

##### <a name="response"></a><span data-ttu-id="a98b0-155">响应</span><span class="sxs-lookup"><span data-stu-id="a98b0-155">Response</span></span>

<span data-ttu-id="a98b0-156">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a98b0-156">The following example shows the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="a98b0-p110">应用程序可以使用 **nextExpectedRanges** 值来确定开始上载下一片段的位置。你可能会看到指定的多个范围，指示服务器尚未收到的文件部分。如果需要恢复中断的传输，并且客户端不能确定服务的状态，这个方法很有用。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p110">Your app can use the **nextExpectedRanges** value to determine where to start the next fragment. You may see multiple ranges specified, indicating parts of the file that the server has not yet received. This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="a98b0-p111">始终都应根据以下最佳实践确定片段大小。请勿假定 **nextExpectedRanges** 将返回大小范围正确的上载片段。**nextExpectedRanges** 属性指定尚未收到的文件的范围，而不是上载文件的方式。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p111">You should always determine the fragment size according to the best practices below. Do not assume that **nextExpectedRanges** will return reanges of proper size for an upload fragment. The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how you should upload the file.</span></span>

<span data-ttu-id="a98b0-163">**注意：**</span><span class="sxs-lookup"><span data-stu-id="a98b0-163">**Notes:**</span></span>

* <span data-ttu-id="a98b0-164">`nextExpectedRanges` 属性不会总是列出所有缺少的范围。</span><span class="sxs-lookup"><span data-stu-id="a98b0-164">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="a98b0-p112">成功写入片段时，它将返回下一个开始范围（例如，"523-"）。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p112">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="a98b0-p113">如果因客户端发送了服务器已接收的片段导致失败，服务器将响应 `HTTP 416 Requested Range Not Satisfiable`。可以 [请求上载状态](#resuming-an-in-progress-upload) 以获取缺少范围的详细列表。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p113">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="a98b0-p114">在发出 `PUT` 调用时添加授权标头可能会导致 `HTTP 401 Unauthorized` 响应。只能在第一步中发出 `POST` 时发送授权标头和持有者令牌。不得在发出 `PUT` 时添加授权标头。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p114">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authorization header and bearer token should only be sent when issuing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>   


## <a name="completing-a-file"></a><span data-ttu-id="a98b0-172">完成文件</span><span class="sxs-lookup"><span data-stu-id="a98b0-172">Completing a file</span></span>

<span data-ttu-id="a98b0-p115">接收最后一个文件片段后，服务器将响应 `HTTP 201 Created` 或 `HTTP 200 OK`。响应正文还将包括 **driveItem** 的默认属性集，用来表示已完成的文件。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p115">When the last fragment of a file is received the server will response with an `HTTP 201 Created` or `HTTP 200 OK`. The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-final", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 21
Content-Range: bytes 101-127/128

<final bytes of the file>
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```
<span data-ttu-id="a98b0-175">**注意：**为使文档清晰起见，该项目的响应被截断。</span><span class="sxs-lookup"><span data-stu-id="a98b0-175">**Note:** The item response is truncated for documentation clarity.</span></span>

## <a name="cancel-an-upload-session"></a><span data-ttu-id="a98b0-176">取消上载会话</span><span class="sxs-lookup"><span data-stu-id="a98b0-176">Cancel an upload session</span></span>

<span data-ttu-id="a98b0-p116">若要取消上载会话，请将 DELETE 请求发送到上载 URL。这会清理用来保留以前上载的数据的临时文件。应在上载中止（例如，如果用户取消传输）的情况下使用上述方法。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p116">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="a98b0-180">**expirationDateTime** 通过后，系统将自动清理临时文件及其随附的上载会话。</span><span class="sxs-lookup"><span data-stu-id="a98b0-180">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>

### <a name="example"></a><span data-ttu-id="a98b0-181">示例</span><span class="sxs-lookup"><span data-stu-id="a98b0-181">Example</span></span>

<span data-ttu-id="a98b0-182">DELETE 请求将立即使上载会话过期，并删除以前上载的所有字节。</span><span class="sxs-lookup"><span data-stu-id="a98b0-182">The DELETE request will immedately expire the upload session and remove any previously uploaded bytes.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->
```http
DELETE https://tenant-my.sharepoint.com/alkjl1kjklna
```

##### <a name="response"></a><span data-ttu-id="a98b0-183">响应</span><span class="sxs-lookup"><span data-stu-id="a98b0-183">Response</span></span> 

<span data-ttu-id="a98b0-184">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a98b0-184">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="a98b0-185">继续正在进行的上传</span><span class="sxs-lookup"><span data-stu-id="a98b0-185">Resuming an in-progress upload</span></span>

<span data-ttu-id="a98b0-p117">如果上载请求在完成前断开或失败，将忽略该请求中的所有字节。如果应用程序与服务之间的连接断开，可能会发生这种情况。如果发生这种情况，应用程序仍可以继续传输以前完成的文件片段。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p117">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="a98b0-189">若要查找以前已接收的字节范围，应用程序可以请求上载会话的状态。</span><span class="sxs-lookup"><span data-stu-id="a98b0-189">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="a98b0-190">示例</span><span class="sxs-lookup"><span data-stu-id="a98b0-190">Example</span></span>
<span data-ttu-id="a98b0-191">通过向 `uploadUrl` 发送 GET 请求来查询上载状态。</span><span class="sxs-lookup"><span data-stu-id="a98b0-191">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->
```
GET https://tenant-my.sharepoint.com/alkjl1kjklna
```

<span data-ttu-id="a98b0-192">服务器将用需要上载的缺失字节范围的列表和上载会话的过期时间进行响应。</span><span class="sxs-lookup"><span data-stu-id="a98b0-192">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 200 OK

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="a98b0-193">上载剩余数据</span><span class="sxs-lookup"><span data-stu-id="a98b0-193">Upload remaining data</span></span>
<span data-ttu-id="a98b0-194">现在，你的应用程序已经知道开始上载的位置，请按照 [将字节上载到上载会话](#upload-bytes-to-the-upload-session) 中的步骤继续上载。</span><span class="sxs-lookup"><span data-stu-id="a98b0-194">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>


## <a name="best-practices"></a><span data-ttu-id="a98b0-195">最佳实践</span><span class="sxs-lookup"><span data-stu-id="a98b0-195">Best practices</span></span>

* <span data-ttu-id="a98b0-196">继续或重试由于连接中断或任意 5xx 错误而失败的上载，包括：</span><span class="sxs-lookup"><span data-stu-id="a98b0-196">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="a98b0-197">如果在继续或重试上载请求时返回任意 5xx 服务器错误，请使用指数退避战略。</span><span class="sxs-lookup"><span data-stu-id="a98b0-197">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="a98b0-198">对于其他错误，不应使用指数退避战略，而应限制尝试重试的次数。</span><span class="sxs-lookup"><span data-stu-id="a98b0-198">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="a98b0-199">通过重新开始整个上载继续上载时，请处理 `404 Not Found` 错误。</span><span class="sxs-lookup"><span data-stu-id="a98b0-199">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span>
* <span data-ttu-id="a98b0-200">对大于 10 MiB（10 \* 1024 \* 1024 字节）的文件使用可恢复文件传输。</span><span class="sxs-lookup"><span data-stu-id="a98b0-200">Use resumable file transfers for files larger than 10 MiB (10 \* 1024 \* 1024 bytes).</span></span>
* <span data-ttu-id="a98b0-p118">最佳的文件片段大小是 10 MiB，可以实现稳定高速连接。对于速度较慢或不可靠的连接，较小的文件片段大小可能会给你带来更好的结果。建议使用的片段大小为 5-10 MiB 之间。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p118">A fragment size of 10 MiB for stable high speed connections is optimal. For slower or less reliable connections you may get better results from a smaller fragment size. The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="a98b0-p119">使用 320 KiB（320 \* 1024 字节）倍数的文件片段大小。如果使用的片段大小不是 320 KiB 的倍数，可能会在上载最后一个文件片段后导致大文件传输失败。</span><span class="sxs-lookup"><span data-stu-id="a98b0-p119">Use a fragment size that is a multiple of 320 KiB (320 \* 1024 bytes). Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last fragment is uploaded.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
