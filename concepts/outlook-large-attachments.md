---
title: 将大文件附加到 Outlook 邮件
description: 可选择两种方法中的一种来将文件附加到邮件，具体取决于文件的大小。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 74cc6ad4af5d649ca480c7b708b0716062e8d36a
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953604"
---
# <a name="attach-large-files-to-outlook-messages-as-attachments-preview"></a><span data-ttu-id="19fbf-103">将大文件作为附件附加到 Outlook 邮件（预览）</span><span class="sxs-lookup"><span data-stu-id="19fbf-103">Attach large files to Outlook messages as attachments (preview)</span></span>

<span data-ttu-id="19fbf-104">可选择两种方法中的一种来将文件附加到[邮件](/graph/api/resources/message?view=graph-rest-beta)，具体取决于文件的大小：</span><span class="sxs-lookup"><span data-stu-id="19fbf-104">Depending on the size of the file, you can choose one of two ways to attach a file to a [message](/graph/api/resources/message?view=graph-rest-beta):</span></span>

- <span data-ttu-id="19fbf-105">如果文件大小小于 4 MB，则可以[针对邮件的附件导航属性执行单个 POST](/graph/api/message-post-attachments?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="19fbf-105">If the file size is under 4 MB, you can do a single [POST on the attachments navigation property of the message](/graph/api/message-post-attachments?view=graph-rest-beta).</span></span> <span data-ttu-id="19fbf-106">成功的 `POST` 响应包括附加到邮件的文件的 ID。</span><span class="sxs-lookup"><span data-stu-id="19fbf-106">The successful `POST` response includes the ID of the file attached to the message.</span></span>
- <span data-ttu-id="19fbf-107">如果文件大小介于 3MB 和 150MB 之间，则创建一个上传会话，并以迭代的方式使用 `PUT` 来上传文件的字节范围，直到完整的文件上传完毕。</span><span class="sxs-lookup"><span data-stu-id="19fbf-107">If the file size is between 3MB and 150MB, create an upload session, and iteratively use `PUT` to upload ranges of bytes of the file until you have uploaded the entire file.</span></span> <span data-ttu-id="19fbf-108">最后一个成功 `PUT` 响应中的标头包括带附件 ID 的 URL。</span><span class="sxs-lookup"><span data-stu-id="19fbf-108">A header in the final successful `PUT` response includes a URL with the attachment ID.</span></span>

<span data-ttu-id="19fbf-109">本文使用一个示例来阐释第二种方法。</span><span class="sxs-lookup"><span data-stu-id="19fbf-109">This article uses an example to illustrate the second approach.</span></span> <span data-ttu-id="19fbf-110">该示例创建并使用上传会话，将大文件附件（大小超过 3MB）添加到特定邮件。</span><span class="sxs-lookup"><span data-stu-id="19fbf-110">The example creates and uses an upload session to add a large file attachment (of size over 3MB) to a specific message.</span></span> <span data-ttu-id="19fbf-111">成功上传整个文件时，它会获取一个 URL，其中包含文件附件的 ID，可用于执行其他操作，如获取文件附件元数据。</span><span class="sxs-lookup"><span data-stu-id="19fbf-111">Upon successfully uploading the entire file, it gets a URL that contains an ID for the file attachment, with which it can do other operations such as getting the file attachment metadata.</span></span>

## <a name="step-1-create-an-upload-session"></a><span data-ttu-id="19fbf-112">第 1 步：创建上传会话</span><span class="sxs-lookup"><span data-stu-id="19fbf-112">Step 1: Create an upload session</span></span>

<span data-ttu-id="19fbf-113">[创建上传会话](/graph/api/attachment-createuploadsession?view=graph-rest-beta)，将文件附加到邮件。</span><span class="sxs-lookup"><span data-stu-id="19fbf-113">[Create an upload session](/graph/api/attachment-createuploadsession?view=graph-rest-beta) to attach a file to a message.</span></span> <span data-ttu-id="19fbf-114">在输入参数 **AttachmentItem** 中指定文件。</span><span class="sxs-lookup"><span data-stu-id="19fbf-114">Specify the file in the input parameter **AttachmentItem**.</span></span>

<span data-ttu-id="19fbf-115">成功的操作返回 `HTTP 201 Created` 和新的 [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-beta) 实例，其中包含可在后续 `PUT` 操作中用于上传文件各部分的非跳转 URL。</span><span class="sxs-lookup"><span data-stu-id="19fbf-115">A successful operation returns `HTTP 201 Created` and a new [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-beta) instance, which contains an opaque URL that you can use in subsequent `PUT` operations to upload portions of the file.</span></span> <span data-ttu-id="19fbf-116">**uploadSession** 提供一个临时存储位置，在此位置保存文件字节数，直到完整文件上传完毕。</span><span class="sxs-lookup"><span data-stu-id="19fbf-116">The **uploadSession** provides a temporary storage location where the bytes of the file are saved until you have uploaded the complete file.</span></span>

<span data-ttu-id="19fbf-117">请务必请求 `Mail.ReadWrite` 权限以创建 **uploadSession**。</span><span class="sxs-lookup"><span data-stu-id="19fbf-117">Make sure to request `Mail.ReadWrite` permission to create the **uploadSession**.</span></span> <span data-ttu-id="19fbf-118">新的 **uploadSession** 的 **uploadUrl** 属性中返回的非跳转 URL 经过预身份验证，包含针对 `https://outlook.office.com` 域中后续 `PUT` 查询的相应授权令牌。</span><span class="sxs-lookup"><span data-stu-id="19fbf-118">The opaque URL, returned in the **uploadUrl** property of the new **uploadSession**, is pre-authenticated and contains the appropriate authorization token for subsequent `PUT` queries in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="19fbf-119">该令牌会在 **expirationDateTime** 过期。</span><span class="sxs-lookup"><span data-stu-id="19fbf-119">That token expires by **expirationDateTime**.</span></span> <span data-ttu-id="19fbf-120">请勿自定义 `PUT` 操作的此 URL。</span><span class="sxs-lookup"><span data-stu-id="19fbf-120">Do not customize this URL for the `PUT` operations.</span></span>

<span data-ttu-id="19fbf-121">响应中的 **uploadSession** 对象还包含 **nextExpectedRanges** 属性，这指示初始上传开始位置应该为 0 字节。</span><span class="sxs-lookup"><span data-stu-id="19fbf-121">The **uploadSession** object in the response also includes the **nextExpectedRanges** property, which indicates the initial upload starting location should be byte 0.</span></span>

### <a name="example-request-create-an-upload-session"></a><span data-ttu-id="19fbf-122">示例请求：创建上传会话</span><span class="sxs-lookup"><span data-stu-id="19fbf-122">Example request: create an upload session</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="19fbf-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="19fbf-123">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19fbf-124">C#</span><span class="sxs-lookup"><span data-stu-id="19fbf-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19fbf-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19fbf-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19fbf-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19fbf-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="example-response-get-an-uploadsession-object"></a><span data-ttu-id="19fbf-127">示例响应：获取 uploadSession 对象</span><span class="sxs-lookup"><span data-stu-id="19fbf-127">Example response: get an uploadSession object</span></span>
<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a><span data-ttu-id="19fbf-128">步骤 2：使用上传会话上传文件的字节范围</span><span class="sxs-lookup"><span data-stu-id="19fbf-128">Step 2: Use the upload session to upload a range of bytes of the file</span></span>

<span data-ttu-id="19fbf-129">要上传文件或文件的一部分，请向作为步骤 1 中 **uploadSession** 一部分返回的 **uploadUrl** 属性发出 `PUT` 请求。</span><span class="sxs-lookup"><span data-stu-id="19fbf-129">To upload the file, or a portion of the file, make a `PUT` request to the **uploadUrl** property value returned as part of the **uploadSession** in step 1.</span></span> <span data-ttu-id="19fbf-130">可上传整个文件，或将文件拆分为多个字节范围。</span><span class="sxs-lookup"><span data-stu-id="19fbf-130">You can upload the entire file, or split the file into multiple byte ranges.</span></span> <span data-ttu-id="19fbf-131">为获得更好的性能，请保持每个字节范围小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="19fbf-131">For better performance, keep each byte range less than 4 MB.</span></span>

<span data-ttu-id="19fbf-132">按如下所述指定请求标头和请求正文。</span><span class="sxs-lookup"><span data-stu-id="19fbf-132">Specify request headers and request body as described below.</span></span>

### <a name="request-headers"></a><span data-ttu-id="19fbf-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="19fbf-133">Request headers</span></span>

| <span data-ttu-id="19fbf-134">名称</span><span class="sxs-lookup"><span data-stu-id="19fbf-134">Name</span></span>       | <span data-ttu-id="19fbf-135">类型</span><span class="sxs-lookup"><span data-stu-id="19fbf-135">Type</span></span> | <span data-ttu-id="19fbf-136">说明</span><span class="sxs-lookup"><span data-stu-id="19fbf-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="19fbf-137">Content-Length</span><span class="sxs-lookup"><span data-stu-id="19fbf-137">Content-Length</span></span> | <span data-ttu-id="19fbf-138">Int32</span><span class="sxs-lookup"><span data-stu-id="19fbf-138">Int32</span></span> | <span data-ttu-id="19fbf-139">此操作中上传的字节数。</span><span class="sxs-lookup"><span data-stu-id="19fbf-139">The number of bytes being uploaded in this operation.</span></span> <span data-ttu-id="19fbf-140">为获得更好的性能，请将每个 `PUT` 操作的字节数的上限限制为 4 MB。</span><span class="sxs-lookup"><span data-stu-id="19fbf-140">For better performance, keep the upper limit of the number of bytes for each `PUT` operation to 4 MB.</span></span> <span data-ttu-id="19fbf-141">必填。</span><span class="sxs-lookup"><span data-stu-id="19fbf-141">Required.</span></span> |
| <span data-ttu-id="19fbf-142">Content-Range</span><span class="sxs-lookup"><span data-stu-id="19fbf-142">Content-Range</span></span> | <span data-ttu-id="19fbf-143">字符串</span><span class="sxs-lookup"><span data-stu-id="19fbf-143">String</span></span> | <span data-ttu-id="19fbf-144">此操作中要上传的文件的从 0 开始的字节范围，格式为 `bytes {start}-{end}/{total}`。</span><span class="sxs-lookup"><span data-stu-id="19fbf-144">The 0-based byte range of the file being uploaded in this operation, expressed in the format `bytes {start}-{end}/{total}`.</span></span> <span data-ttu-id="19fbf-145">必填。</span><span class="sxs-lookup"><span data-stu-id="19fbf-145">Required.</span></span> |
| <span data-ttu-id="19fbf-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19fbf-146">Content-Type</span></span> | <span data-ttu-id="19fbf-147">String</span><span class="sxs-lookup"><span data-stu-id="19fbf-147">String</span></span>  | <span data-ttu-id="19fbf-148">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="19fbf-148">The MIME type.</span></span> <span data-ttu-id="19fbf-149">指定 `application/octet-stream`。</span><span class="sxs-lookup"><span data-stu-id="19fbf-149">Specify `application/octet-stream`.</span></span> <span data-ttu-id="19fbf-150">必填。</span><span class="sxs-lookup"><span data-stu-id="19fbf-150">Required.</span></span> |

<span data-ttu-id="19fbf-151">请勿指定 `Authorization` 请求标头。</span><span class="sxs-lookup"><span data-stu-id="19fbf-151">Do not specify an `Authorization` request header.</span></span> <span data-ttu-id="19fbf-152">`PUT` 查询使用 **uploadUrl** 属性中预身份验证的 URL，该属性允许访问 `https://outlook.office.com` 域。</span><span class="sxs-lookup"><span data-stu-id="19fbf-152">The `PUT` query uses a pre-authenticated URL from the **uploadUrl** property, that allows access to the `https://outlook.office.com` domain.</span></span>

### <a name="request-body"></a><span data-ttu-id="19fbf-153">请求正文</span><span class="sxs-lookup"><span data-stu-id="19fbf-153">Request body</span></span>

<span data-ttu-id="19fbf-154">指定要附加的文件的实际字节数，它们位于由 `Content-Range` 请求标头指定的位置范围内。</span><span class="sxs-lookup"><span data-stu-id="19fbf-154">Specify the actual bytes of the file to be attached, that are in the location range specified by the `Content-Range` request header.</span></span>

### <a name="response"></a><span data-ttu-id="19fbf-155">响应</span><span class="sxs-lookup"><span data-stu-id="19fbf-155">Response</span></span>
<span data-ttu-id="19fbf-156">成功的上传将返回 `HTTP 200 OK` 和 **uploadSession** 对象。</span><span class="sxs-lookup"><span data-stu-id="19fbf-156">A successful upload returns `HTTP 200 OK` and an **uploadSession** object.</span></span> <span data-ttu-id="19fbf-157">请注意响应对象中的以下项：</span><span class="sxs-lookup"><span data-stu-id="19fbf-157">Note the following in the response object:</span></span>

- <span data-ttu-id="19fbf-158">**ExpirationDateTime** 属性指示 **uploadUrl** 属性值中嵌入的身份验证令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="19fbf-158">The **ExpirationDateTime** property indicates the expiration date/time for the auth token embedded in the **uploadUrl** property value.</span></span> <span data-ttu-id="19fbf-159">此到期日期/时间与步骤 1 中由初始 **uploadSession** 返回的值相同。</span><span class="sxs-lookup"><span data-stu-id="19fbf-159">This expiration date/time remains the same as returned by the initial **uploadSession** in step 1.</span></span>
- <span data-ttu-id="19fbf-160">**NextExpectedRanges** 指定上传开始的下一个字节位置，例如 `"NextExpectedRanges":["2097152"]`。</span><span class="sxs-lookup"><span data-stu-id="19fbf-160">The **NextExpectedRanges** specifies the next byte location to start uploading from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="19fbf-161">必须按顺序上传文件中的字节。</span><span class="sxs-lookup"><span data-stu-id="19fbf-161">You must upload bytes in a file in order.</span></span>
<!-- The **NextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"NextExpectedRanges":["2097152"]`.
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"NextExpectedRanges":["1998457-2097094"]`.
-->
- <span data-ttu-id="19fbf-162">**uploadUrl** 属性不会显式返回，因为上传会话的所有 `PUT` 操作使用创建会话时返回的同一 URL（步骤 1）。</span><span class="sxs-lookup"><span data-stu-id="19fbf-162">The **uploadUrl** property is not explicitly returned, because all `PUT` operations of an upload session use the same URL returned when creating the session (step 1).</span></span>

### <a name="example-request-first-upload"></a><span data-ttu-id="19fbf-163">示例请求：第一次上传</span><span class="sxs-lookup"><span data-stu-id="19fbf-163">Example request: first upload</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

### <a name="example-response-get-the-start-of-the-next-byte-range-that-the-server-expects"></a><span data-ttu-id="19fbf-164">示例响应：获取服务器需要的下一个字节范围的开头</span><span class="sxs-lookup"><span data-stu-id="19fbf-164">Example response: get the start of the next byte range that the server expects</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://outlook.office.com/api/beta/$metadata#Users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA%3D')/AttachmentSessions/$entity",
  "ExpirationDateTime":"2019-09-25T01:09:30.7671707Z",
  "NextExpectedRanges":["2097152"]
}
```


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a><span data-ttu-id="19fbf-165">步骤 3：继续上传字节范围，直至完整文件上传完毕</span><span class="sxs-lookup"><span data-stu-id="19fbf-165">Step 3: Continue uploading byte ranges until the entire file has been uploaded</span></span>

<span data-ttu-id="19fbf-166">执行步骤 2 中的初始上传后，在会话的到期日期/时间前，使用步骤 2 中所述的 `PUT` 请求，继续上传文件中剩余的部分。</span><span class="sxs-lookup"><span data-stu-id="19fbf-166">Following the initial upload in step 2, continue to upload the remaining portion of the file, using a similar `PUT` request as described in step 2, before you reach the expiration date/time for the session.</span></span> <span data-ttu-id="19fbf-167">使用 **NextExpectedRanges** 集合确定要上传的下一个字节范围的开头。</span><span class="sxs-lookup"><span data-stu-id="19fbf-167">Use the **NextExpectedRanges** collection to determine where to start the next byte range to upload.</span></span> <span data-ttu-id="19fbf-168">可能会发现指定了多个范围，这些范围指明了服务器尚未收到的文件部分。</span><span class="sxs-lookup"><span data-stu-id="19fbf-168">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="19fbf-169">如果需要恢复中断的传输，并且客户端不能确定服务的状态，这个方法很有用。</span><span class="sxs-lookup"><span data-stu-id="19fbf-169">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="19fbf-170">成功上传文件的最后一个字节后，最终 `PUT` 操作返回 `HTTP 201 Created` 以及指示 `https://outlook.office.com` 域中文件附件 URL 的 `Location` 标头。</span><span class="sxs-lookup"><span data-stu-id="19fbf-170">Once the last byte of the file has been successfully uploaded, the final `PUT` operation returns `HTTP 201 Created` and a `Location` header that indicates the URL to the file attachment in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="19fbf-171">可从 URL 获取附件 ID 并将其保存供以后使用。</span><span class="sxs-lookup"><span data-stu-id="19fbf-171">You can get the attachment ID from the URL and save it for later use.</span></span> <span data-ttu-id="19fbf-172">可以使用该 ID [获取附件的元数据](/graph/api/attachment-get?view=graph-rest-beta)，或使用 Microsoft Graph 终结点[将附件从邮件中删除](/graph/api/attachment-delete?view=graph-rest-beta)，具体取决于你的场景。</span><span class="sxs-lookup"><span data-stu-id="19fbf-172">Depending on your scneario, you can use that ID to [get the metadata of the attachment](/graph/api/attachment-get?view=graph-rest-beta), or [remove the attachment from the message](/graph/api/attachment-delete?view=graph-rest-beta) using the Microsoft Graph endpoint.</span></span>

<span data-ttu-id="19fbf-173">以下示例显示上传文件的最后一个字节范围。</span><span class="sxs-lookup"><span data-stu-id="19fbf-173">The following example shows uploading the last byte range of the file.</span></span>

### <a name="example-request-final-upload"></a><span data-ttu-id="19fbf-174">示例请求：最后一次上传</span><span class="sxs-lookup"><span data-stu-id="19fbf-174">Example request: final upload</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

### <a name="example-response-get-the-location-response-header-to-save-the-attachment-id"></a><span data-ttu-id="19fbf-175">示例响应：获取位置响应标头以保存附件 ID</span><span class="sxs-lookup"><span data-stu-id="19fbf-175">Example response: get the Location response header to save the attachment ID</span></span>

<span data-ttu-id="19fbf-176">通过 `Location` 响应标头指定的 URL，保存附件 ID (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) 以便日后使用。</span><span class="sxs-lookup"><span data-stu-id="19fbf-176">From the URL specified by the `Location` response header, save the attachment ID (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) for later use.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-message"></a><span data-ttu-id="19fbf-177">步骤 4（可选）：从邮件中获取文件附件</span><span class="sxs-lookup"><span data-stu-id="19fbf-177">Step 4 (optional): Get the file attachment from the message</span></span>

<span data-ttu-id="19fbf-178">和往常一样，从邮件中[获取附件](/graph/api/attachment-get?view=graph-rest-beta)在理论上并不受附件大小限制。</span><span class="sxs-lookup"><span data-stu-id="19fbf-178">As always, [getting an attachment](/graph/api/attachment-get?view=graph-rest-beta) from a message is not technically limited by attachment size.</span></span>

<span data-ttu-id="19fbf-179">但是，获取采用 base64 编码格式的大文件附件会影响 API 性能。</span><span class="sxs-lookup"><span data-stu-id="19fbf-179">However, getting a large file attachment in base64-encoded format affects API performance.</span></span> <span data-ttu-id="19fbf-180">如果需要大型附件：</span><span class="sxs-lookup"><span data-stu-id="19fbf-180">If you expect a large attachment:</span></span>

- <span data-ttu-id="19fbf-181">作为获取采用 base64 格式的附件内容的替代方法，可以[获取文件附件的元数据](/graph/api/attachment-get#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="19fbf-181">As an alternative to getting the attachment content in base64 format, you can [get the raw data of the file attachment](/graph/api/attachment-get#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="19fbf-182">要[获取文件附件的元数据](/graph/api/attachment-get?view=graph-rest-beta#example-1-get-the-properties-of-a-file-attachment)，可以附加 `$select` 参数以仅包含所需的元数据属性，排除返回采用 base64 格式的文件附件的 **contentBytes** 属性。</span><span class="sxs-lookup"><span data-stu-id="19fbf-182">To [get the metadata of the file attachment](/graph/api/attachment-get?view=graph-rest-beta#example-1-get-the-properties-of-a-file-attachment), append a `$select` parameter to include only those metadata properties you want, excluding the **contentBytes** property which returns the file attachment in base64 format.</span></span>

### <a name="example-request-get-the-file-attachment-metadata"></a><span data-ttu-id="19fbf-183">示例请求：获取文件附件元数据</span><span class="sxs-lookup"><span data-stu-id="19fbf-183">Example request: get the file attachment metadata</span></span>

<span data-ttu-id="19fbf-184">下面的示例显示发件人使用 `$select` 参数获取邮件中文件附件的所有元数据，除了 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="19fbf-184">The following example shows the sender using a `$select` parameter to get all the metadata of a file attachment on a message, except **contentBytes**.</span></span>

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment",
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline
```

### <a name="example-response"></a><span data-ttu-id="19fbf-185">示例响应</span><span class="sxs-lookup"><span data-stu-id="19fbf-185">Example response</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_get_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/messages('AAMkADI5MAAIT3drCAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "@odata.mediaContentType": "image/jpeg",
    "id": "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=",
    "lastModifiedDateTime": "2019-09-24T23:27:43Z",
    "name": "flower",
    "contentType": "image/jpeg",
    "size": 3640066,
    "isInline": false
}
```

## <a name="alternative-cancel-the-upload-session"></a><span data-ttu-id="19fbf-186">替代方法：取消上传会话</span><span class="sxs-lookup"><span data-stu-id="19fbf-186">Alternative: Cancel the upload session</span></span>

<span data-ttu-id="19fbf-187">在上传会话到期之前的任何时间，如果必须取消上传，可使用同一初始非跳转 URL 来删除上传会话。</span><span class="sxs-lookup"><span data-stu-id="19fbf-187">At any point of time before the upload session expires, if you have to cancel the upload, you can use the same initial opaque URL to delete the upload session.</span></span> <span data-ttu-id="19fbf-188">成功的操作将返回 `HTTP 204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="19fbf-188">A successful operation returns `HTTP 204 No Content`.</span></span>

### <a name="example-request-cancel-an-upload-session"></a><span data-ttu-id="19fbf-189">示例请求：取消上传会话</span><span class="sxs-lookup"><span data-stu-id="19fbf-189">Example request: cancel an upload session</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

### <a name="example-response"></a><span data-ttu-id="19fbf-190">示例响应</span><span class="sxs-lookup"><span data-stu-id="19fbf-190">Example response</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```


