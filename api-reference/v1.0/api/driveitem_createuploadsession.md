---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "可恢复的文件上传"
ms.openlocfilehash: 39aee7121483e423c4adbd910c80e1ca059c685a
ms.sourcegitcommit: e9b5d370a1d9a03d908dc430994d6a196b1345b4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/11/2017
---
# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="18582-102">通过上传会话上传大文件</span><span class="sxs-lookup"><span data-stu-id="18582-102">Upload large files with an upload session</span></span>

<span data-ttu-id="18582-p101">通过创建上传会话，使应用可以上传最大大小的文件。上传会话使应用可以在连续的 API 请求中上传多个范围的文件，这样一来，如果在上传过程中连接断开，应用也可以继续传输文件。</span><span class="sxs-lookup"><span data-stu-id="18582-p101">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequential API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="18582-105">若要使用上传会话上传文件，请执行以下两个步骤：</span><span class="sxs-lookup"><span data-stu-id="18582-105">To upload a file using an upload session, there are two steps:</span></span>

1. [<span data-ttu-id="18582-106">创建上载会话</span><span class="sxs-lookup"><span data-stu-id="18582-106">Create an upload session</span></span>](#create-an-upload-session)
2. [<span data-ttu-id="18582-107">将字节上传到上传会话</span><span class="sxs-lookup"><span data-stu-id="18582-107">Upload bytes to the upload session</span></span>](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a><span data-ttu-id="18582-108">权限</span><span class="sxs-lookup"><span data-stu-id="18582-108">Permissions</span></span>

<span data-ttu-id="18582-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="18582-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="18582-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="18582-111">Permission type</span></span>      | <span data-ttu-id="18582-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18582-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18582-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18582-113">Delegated (work or school account)</span></span> | <span data-ttu-id="18582-114">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18582-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="18582-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18582-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18582-116">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18582-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="18582-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="18582-117">Application</span></span> | <span data-ttu-id="18582-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18582-118">Sites.ReadWrite.All</span></span> |

## <a name="create-an-upload-session"></a><span data-ttu-id="18582-119">创建上传会话</span><span class="sxs-lookup"><span data-stu-id="18582-119">Create an upload session</span></span>

<span data-ttu-id="18582-p103">要开始上载大文件，你的应用程序必须先请求新的上载会话。这可以创建一个临时存储位置，在上载完成之前保存文件字节数。上载最后一个字节后，上载会话即完成，最终文件会出现在目标文件夹中。</span><span class="sxs-lookup"><span data-stu-id="18582-p103">To begin a large file upload, your app must first request a new upload session. This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded. Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>

### <a name="http-request"></a><span data-ttu-id="18582-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18582-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="18582-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="18582-124">Request body</span></span>

<span data-ttu-id="18582-p104">不需要请求正文。但是，你可以指定请求正文，以便提供与正在上载的文件有关的其他数据。</span><span class="sxs-lookup"><span data-stu-id="18582-p104">No request body is required. However, you can specify a request body to provide additional data about the file being uploaded.</span></span>

<span data-ttu-id="18582-127">例如，要控制是否已获得文件名的行为，可以在请求正文中指定冲突行为属性。</span><span class="sxs-lookup"><span data-stu-id="18582-127">For example, to control the behavior if the filename is already taken, you can specify the conflict behavior property in the body of the request.</span></span>

<!-- { "blockType": "ignored" } -->
```json
{
    "item": {
        "@microsoft.graph.conflictBehavior": "rename"
    }
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="18582-128">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="18582-128">Optional request headers</span></span>

| <span data-ttu-id="18582-129">名称</span><span class="sxs-lookup"><span data-stu-id="18582-129">Name</span></span>       | <span data-ttu-id="18582-130">值</span><span class="sxs-lookup"><span data-stu-id="18582-130">Value</span></span> | <span data-ttu-id="18582-131">说明</span><span class="sxs-lookup"><span data-stu-id="18582-131">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="18582-132">*if-match*</span><span class="sxs-lookup"><span data-stu-id="18582-132">*if-match*</span></span> | <span data-ttu-id="18582-133">etag</span><span class="sxs-lookup"><span data-stu-id="18582-133">etag</span></span>  | <span data-ttu-id="18582-134">如果包含此请求标头，且提供的 eTag（或 cTag）与项目中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 错误响应。</span><span class="sxs-lookup"><span data-stu-id="18582-134">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` errr response is returned.</span></span> |

### <a name="request"></a><span data-ttu-id="18582-135">请求</span><span class="sxs-lookup"><span data-stu-id="18582-135">Request</span></span>

<span data-ttu-id="18582-136">对此请求的响应将提供新建 [uploadSession](../resources/uploadsession.md) 的详细信息，其中包括用于上载部分文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="18582-136">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

<!-- { "blockType": "request", "name": "upload-fragment-create-session", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drive/root:/{item-path}:/createUploadSession
Content-Type: application/json

{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename",
    "name": "largefile.dat"
  }
}
```

### <a name="response"></a><span data-ttu-id="18582-137">响应</span><span class="sxs-lookup"><span data-stu-id="18582-137">Response</span></span>

<span data-ttu-id="18582-138">如果成功，此请求的响应将详细说明应将其余请求作为 [UploadSession](../resources/uploadSession.md) 资源发送到哪里。</span><span class="sxs-lookup"><span data-stu-id="18582-138">The response to this request, if successful, will provide the details for where the remainder of the requests should be sent as an [UploadSession](../resources/uploadSession.md) resource.</span></span>

<span data-ttu-id="18582-139">此资源详细说明了应将文件的字节范围上传到哪里以及上传会话何时到期。</span><span class="sxs-lookup"><span data-stu-id="18582-139">This resource provides details about where the byte range of the file should be uploaded and when the upload session expires.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession",
       "optionalProperties": [ "nextExpectedRanges" ]  } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z"
}
```

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="18582-140">将字节上传到上传会话</span><span class="sxs-lookup"><span data-stu-id="18582-140">Upload bytes to the upload session</span></span>

<span data-ttu-id="18582-141">若要上传文件或文件的一部分，你的应用可以对在 **createUploadSession** 响应中收到的 **uploadUrl** 值创建 PUT 请求。</span><span class="sxs-lookup"><span data-stu-id="18582-141">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="18582-142">可以上传整个文件，也可以将文件拆分为多个字节范围，只要任意给定请求的最大字节数少于 60 MiB 即可。</span><span class="sxs-lookup"><span data-stu-id="18582-142">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 60 MiB.</span></span>

<span data-ttu-id="18582-143">必须按顺序上传文件的片段。</span><span class="sxs-lookup"><span data-stu-id="18582-143">The fragments of the file must be uploaded sequentally in order.</span></span>
<span data-ttu-id="18582-144">不按顺序上载文件的片段将导致错误。</span><span class="sxs-lookup"><span data-stu-id="18582-144">Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="18582-145">**注意：**如果应用将一个文件拆分为多个字节范围，则每个字节范围的大小**必须**是 320 KiB（327,680 个字节）的倍数。</span><span class="sxs-lookup"><span data-stu-id="18582-145">**Note:** If your app splits a file into multiple byte ranges, the size of each byte range **MUST** be a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="18582-146">如果使用的片断大小不能被 320 KiB 整除，会导致在提交某些文件时出错。</span><span class="sxs-lookup"><span data-stu-id="18582-146">Using a fragment size that does not divide evenly by 320 KiB will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="18582-147">示例</span><span class="sxs-lookup"><span data-stu-id="18582-147">Example</span></span>

<span data-ttu-id="18582-148">在本示例中，应用将上传 128 字节大小的文件中的前 26 个字节。</span><span class="sxs-lookup"><span data-stu-id="18582-148">In this example, the app is uploading the first 26 bytes of a 128 byte file.</span></span>

* <span data-ttu-id="18582-149">**Content-Length** 标头指定当前请求的大小。</span><span class="sxs-lookup"><span data-stu-id="18582-149">The **Content-Length** header specifies the size of the current request.</span></span>
* <span data-ttu-id="18582-150">**Content-Range** 标头指示此请求表示的整个文件中的字节范围。</span><span class="sxs-lookup"><span data-stu-id="18582-150">The **Content-Range** header indicates the range of bytes in the overall file that this request represents.</span></span>
* <span data-ttu-id="18582-151">要先知道文件的总长度，然后才可以上传文件的第一个片段。</span><span class="sxs-lookup"><span data-stu-id="18582-151">The total length of the file is known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="18582-152">**重要说明：**应用必须确保 **Content-Range** 标头中指定的文件总大小对于所有的请求都相同。</span><span class="sxs-lookup"><span data-stu-id="18582-152">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests.</span></span>
<span data-ttu-id="18582-153">如果某字节范围声明有不同的文件大小，则请求将失败。</span><span class="sxs-lookup"><span data-stu-id="18582-153">If a byte range declares a different file size, the request will fail.</span></span>

### <a name="response"></a><span data-ttu-id="18582-154">响应</span><span class="sxs-lookup"><span data-stu-id="18582-154">Response</span></span>

<span data-ttu-id="18582-155">当此请求完成时，如果还需要上传其他字节范围，服务器将会返回 `202 Accepted` 作为响应。</span><span class="sxs-lookup"><span data-stu-id="18582-155">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="18582-156">应用可以使用 **nextExpectedRanges** 值来确定开始上传下一字节范围的位置。</span><span class="sxs-lookup"><span data-stu-id="18582-156">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span>
<span data-ttu-id="18582-157">可能会发现指定了多个范围，这些范围指明了服务器尚未收到的文件部分。</span><span class="sxs-lookup"><span data-stu-id="18582-157">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="18582-158">如果需要恢复中断的传输，并且客户端不能确定服务的状态，这个方法很有用。</span><span class="sxs-lookup"><span data-stu-id="18582-158">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="18582-159">始终都应根据以下最佳实践确定字节范围大小。</span><span class="sxs-lookup"><span data-stu-id="18582-159">You should always determine the size of your byte ranges according to the best practices below.</span></span> <span data-ttu-id="18582-160">请勿假定 **nextExpectedRanges** 将返回大小范围正确的上传字节范围。</span><span class="sxs-lookup"><span data-stu-id="18582-160">Do not assume that **nextExpectedRanges** will return reanges of proper size for a byte range to upload.</span></span>
<span data-ttu-id="18582-161">**nextExpectedRanges** 属性指示尚未收到的文件的范围，而不是应用应上传文件的方式。</span><span class="sxs-lookup"><span data-stu-id="18582-161">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": [
  "12345-55232",
  "77829-99375"
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="18582-162">备注</span><span class="sxs-lookup"><span data-stu-id="18582-162">Remarks</span></span>

* <span data-ttu-id="18582-163">`nextExpectedRanges` 属性不会总是列出所有缺少的范围。</span><span class="sxs-lookup"><span data-stu-id="18582-163">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="18582-p111">成功写入片段时，它将返回下一个开始范围（例如，"523-"）。</span><span class="sxs-lookup"><span data-stu-id="18582-p111">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="18582-p112">如果因客户端发送了服务器已接收的片段导致失败，服务器将响应 `HTTP 416 Requested Range Not Satisfiable`。可以 [请求上载状态](#resuming-an-in-progress-upload) 以获取缺少范围的详细列表。</span><span class="sxs-lookup"><span data-stu-id="18582-p112">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="18582-p113">在发出 `PUT` 调用时添加授权标头可能会导致 `HTTP 401 Unauthorized` 响应。只能在第一步中发出 `POST` 时发送授权标头和持有者令牌。不得在发出 `PUT` 时添加授权标头。</span><span class="sxs-lookup"><span data-stu-id="18582-p113">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authorization header and bearer token should only be sent when issuing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="18582-171">完成文件</span><span class="sxs-lookup"><span data-stu-id="18582-171">Completing a file</span></span>

<span data-ttu-id="18582-172">接收最后一个文件字节范围后，服务器将响应 `HTTP 201 Created` 或 `HTTP 200 OK`。</span><span class="sxs-lookup"><span data-stu-id="18582-172">When the last byte range of a file is received the server will response with an `HTTP 201 Created` or `HTTP 200 OK`.</span></span>
<span data-ttu-id="18582-173">响应正文还会包括 **driveItem** 的默认属性集，用来表示已完成的文件。</span><span class="sxs-lookup"><span data-stu-id="18582-173">The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-final", "scopes": "files.readwrite" } -->

```
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
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

## <a name="handling-upload-conflicts"></a><span data-ttu-id="18582-174">处理上传冲突</span><span class="sxs-lookup"><span data-stu-id="18582-174">Handling upload conflicts</span></span>

<span data-ttu-id="18582-175">如果在文件上传后发生冲突（例如，在上传会话期间创建了同名的项），则会在最后一个字节范围上传时返回错误。</span><span class="sxs-lookup"><span data-stu-id="18582-175">If a conflict occurs after the file is uploaded (for example, an item with the same name was created during the upload session), an error is returned when the last byte range is uploaded.</span></span>

```http
HTTP/1.1 409 Conflict
Content-Type: application/json

{
  "error":
  {
    "code": "upload_name_conflict",
    "message": "Another file exists with the same name as the uploaded session. You can redirect the upload session to use a new filename by calling PUT with the new metadata and @microsoft.graph.sourceUrl attribute.",
  }
}
```

## <a name="cancel-the-upload-session"></a><span data-ttu-id="18582-176">取消上传会话</span><span class="sxs-lookup"><span data-stu-id="18582-176">Cancel the upload session</span></span>

<span data-ttu-id="18582-p115">若要取消上载会话，请将 DELETE 请求发送到上载 URL。这会清理用来保留以前上载的数据的临时文件。应在上载中止（例如，如果用户取消传输）的情况下使用上述方法。</span><span class="sxs-lookup"><span data-stu-id="18582-p115">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="18582-180">**expirationDateTime** 通过后，系统将自动清理临时文件及其随附的上传会话。</span><span class="sxs-lookup"><span data-stu-id="18582-180">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>
<span data-ttu-id="18582-181">有效期过后可能不会立即删除临时文件。</span><span class="sxs-lookup"><span data-stu-id="18582-181">Temporary files may not be deleted immedately after the expiration time has elapsed.</span></span>

### <a name="request"></a><span data-ttu-id="18582-182">请求</span><span class="sxs-lookup"><span data-stu-id="18582-182">Request</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a><span data-ttu-id="18582-183">响应</span><span class="sxs-lookup"><span data-stu-id="18582-183">Response</span></span>

<span data-ttu-id="18582-184">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="18582-184">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="18582-185">继续正在进行的上传</span><span class="sxs-lookup"><span data-stu-id="18582-185">Resuming an in-progress upload</span></span>

<span data-ttu-id="18582-p117">如果上载请求在完成前断开或失败，将忽略该请求中的所有字节。如果应用程序与服务之间的连接断开，可能会发生这种情况。如果发生这种情况，应用程序仍可以继续传输以前完成的文件片段。</span><span class="sxs-lookup"><span data-stu-id="18582-p117">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="18582-189">若要查找以前已接收的字节范围，应用程序可以请求上载会话的状态。</span><span class="sxs-lookup"><span data-stu-id="18582-189">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="18582-190">示例</span><span class="sxs-lookup"><span data-stu-id="18582-190">Example</span></span>

<span data-ttu-id="18582-191">通过向 `uploadUrl` 发送 GET 请求来查询上载状态。</span><span class="sxs-lookup"><span data-stu-id="18582-191">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

<span data-ttu-id="18582-192">服务器将用需要上载的缺失字节范围的列表和上载会话的过期时间进行响应。</span><span class="sxs-lookup"><span data-stu-id="18582-192">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="18582-193">上载剩余数据</span><span class="sxs-lookup"><span data-stu-id="18582-193">Upload remaining data</span></span>

<span data-ttu-id="18582-194">现在，你的应用程序已经知道开始上载的位置，请按照 [将字节上载到上载会话](#upload-bytes-to-the-upload-session) 中的步骤继续上载。</span><span class="sxs-lookup"><span data-stu-id="18582-194">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>

## <a name="handle-upload-errors"></a><span data-ttu-id="18582-195">处理上传错误</span><span class="sxs-lookup"><span data-stu-id="18582-195">Handle upload errors</span></span>

<span data-ttu-id="18582-196">在上传文件的最后一个字节范围时，可能会出现错误。</span><span class="sxs-lookup"><span data-stu-id="18582-196">When the last byte range of a file is uploaded, it is possible for an error to occur.</span></span> <span data-ttu-id="18582-197">这可能是由于名称冲突或超出配额限制所致。</span><span class="sxs-lookup"><span data-stu-id="18582-197">This can be due to a name conflict or quota limitation being exceeded.</span></span>
<span data-ttu-id="18582-198">将保留未到期的上传会话，这允许应用通过显式提交上传会话来恢复上传。</span><span class="sxs-lookup"><span data-stu-id="18582-198">The upload session will be preserved until the expiration time, which allows your app to recover the upload by explicitly committing the upload session.</span></span>

<span data-ttu-id="18582-199">若要显式提交上传会话，应用必须使用将用来提交上传会话的新 **driveItem** 资源发出 PUT 请求。</span><span class="sxs-lookup"><span data-stu-id="18582-199">To explicitly commit the upload session, your app must make a PUT request with a new **driveItem** resource that will be used when committing the upload session.</span></span>
<span data-ttu-id="18582-200">此新请求应纠正生成原始上传错误的错误根源。</span><span class="sxs-lookup"><span data-stu-id="18582-200">This new request should correct the source of error that generated the original upload error.</span></span>

<span data-ttu-id="18582-201">若要指示应用提交现有上传会话，PUT 请求必须包含 `@microsoft.graph.sourceUrl` 属性以及上传会话 URL 的值。</span><span class="sxs-lookup"><span data-stu-id="18582-201">To indicate that your app is committing an existing upload session, the PUT request must include the `@microsoft.graph.sourceUrl` property with the value of your upload session URL.</span></span>

<!-- { "blockType": "ignored", "name": "explicit-upload-commit", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/{path_to_parent}
Content-Type: application/json
If-Match: {etag or ctag}

{
  "name": "largefile_2.vhd",
  "@microsoft.graph.conflictBehavior": "rename",
  "@microsoft.graph.sourceUrl": "{upload session URL}"
}
```

<span data-ttu-id="18582-202">**注意：**可以在此调用中正常使用 `@microsoft.graph.conflictBehavior` 和 `if-match` 头。</span><span class="sxs-lookup"><span data-stu-id="18582-202">**Note:** You can use the `@microsoft.graph.conflictBehavior` and `if-match` headers as expected in this call.</span></span>

### <a name="http-response"></a><span data-ttu-id="18582-203">HTTP 响应</span><span class="sxs-lookup"><span data-stu-id="18582-203">HTTP response</span></span>

<span data-ttu-id="18582-204">如果可以使用新的元数据提交文件，将返回 `HTTP 201 Created` 或 `HTTP 200 OK` 响应，其中包含已上传文件的项元数据。</span><span class="sxs-lookup"><span data-stu-id="18582-204">If the file can be committed using the new metadata, an `HTTP 201 Created` or `HTTP 200 OK` response will be returned with the Item metadata for the uploaded file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

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

## <a name="best-practices"></a><span data-ttu-id="18582-205">最佳做法</span><span class="sxs-lookup"><span data-stu-id="18582-205">Best practices</span></span>

* <span data-ttu-id="18582-206">继续或重试由于连接中断或任意 5xx 错误而失败的上载，包括：</span><span class="sxs-lookup"><span data-stu-id="18582-206">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="18582-207">如果在继续或重试上载请求时返回任意 5xx 服务器错误，请使用指数退避战略。</span><span class="sxs-lookup"><span data-stu-id="18582-207">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="18582-208">对于其他错误，不应使用指数退避战略，而应限制尝试重试的次数。</span><span class="sxs-lookup"><span data-stu-id="18582-208">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="18582-209">通过重新开始整个上传继续上传时，请处理 `404 Not Found` 错误。</span><span class="sxs-lookup"><span data-stu-id="18582-209">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span> <span data-ttu-id="18582-210">这表示上传会话不再存在。</span><span class="sxs-lookup"><span data-stu-id="18582-210">This indicates the upload session no longer exists.</span></span>
* <span data-ttu-id="18582-211">对大于 10 MiB（10,485,760 个字节）的文件使用可恢复文件传输。</span><span class="sxs-lookup"><span data-stu-id="18582-211">Use resumable file transfers for files larger than 10 MiB (10,485,760 bytes).</span></span>
* <span data-ttu-id="18582-212">最佳的字节范围大小是 10 MiB，可以实现稳定高速连接。</span><span class="sxs-lookup"><span data-stu-id="18582-212">A byte range size of 10 MiB for stable high speed connections is optimal.</span></span> <span data-ttu-id="18582-213">对于速度较慢或不可靠的连接，较小的文件片段大小可能会给你带来更好的结果。</span><span class="sxs-lookup"><span data-stu-id="18582-213">For slower or less reliable connections you may get better results from a smaller fragment size.</span></span> <span data-ttu-id="18582-214">建议使用的片段大小为 5-10 MiB 之间。</span><span class="sxs-lookup"><span data-stu-id="18582-214">The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="18582-215">使用 320 KiB（327,680 个字节）倍数的字节范围大小。</span><span class="sxs-lookup"><span data-stu-id="18582-215">Use a byte range size that is a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="18582-216">如果使用的片段大小不是 320 KiB 的倍数，可能会在上传最后一个字节范围后导致大文件传输失败。</span><span class="sxs-lookup"><span data-stu-id="18582-216">Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last byte range is uploaded.</span></span>

## <a name="error-responses"></a><span data-ttu-id="18582-217">错误响应</span><span class="sxs-lookup"><span data-stu-id="18582-217">Error responses</span></span>

<span data-ttu-id="18582-218">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="18582-218">See the [Error Responses][error-response] topic for details about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "section": "documentation"
} -->
