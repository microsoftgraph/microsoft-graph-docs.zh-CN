---
title: 将大文件附加到 Outlook 邮件或事件
description: 可选择两种方法中的一种来将文件附加到邮件或事件，具体取决于文件的大小。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 5e8bce4043816fd6d5e454c6e4671bf8b3c6b448
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44052421"
---
# <a name="attach-large-files-to-outlook-messages-or-events"></a><span data-ttu-id="31fca-103">将大文件附加到 Outlook 邮件或事件</span><span class="sxs-lookup"><span data-stu-id="31fca-103">Attach large files to Outlook messages or events</span></span>

<span data-ttu-id="31fca-104">使用 Microsoft Graph API，可将最大 150 MB 的文件附加到 Outlook [邮件](/graph/api/resources/message?view=graph-rest-1.0)或 [事件](/graph/api/resources/event?view=graph-rest-1.0)项目。</span><span class="sxs-lookup"><span data-stu-id="31fca-104">Using the Microsoft Graph API, you can attach files up to 150 MB to an Outlook [message](/graph/api/resources/message?view=graph-rest-1.0) or [event](/graph/api/resources/event?view=graph-rest-1.0) item.</span></span> <span data-ttu-id="31fca-105">根据文件大小，选择以下两种方法之一来附加文件：</span><span class="sxs-lookup"><span data-stu-id="31fca-105">Depending on the file size, choose one of two ways to attach the file:</span></span>
- <span data-ttu-id="31fca-106">如果文件大小小于 3 MB，应该针对 Outlook 项的**附件**导航属性执行单个 POST；了解如何针对[邮件](/graph/api/message-post-attachments?view=graph-rest-1.0)或[事件](/graph/api/event-post-attachments?view=graph-rest-1.0)执行此操作。</span><span class="sxs-lookup"><span data-stu-id="31fca-106">If the file size is under 3 MB, do a single POST on the **attachments** navigation property of the Outlook item; see how to do this [for a message](/graph/api/message-post-attachments?view=graph-rest-1.0) or [for an event](/graph/api/event-post-attachments?view=graph-rest-1.0).</span></span> <span data-ttu-id="31fca-107">成功的 `POST` 响应包括文件附件的 ID。</span><span class="sxs-lookup"><span data-stu-id="31fca-107">The successful `POST` response includes the ID of the file attachment.</span></span>
- <span data-ttu-id="31fca-108">如果文件大小介于 3MB 和 150MB 之间，则创建一个上传会话，并以迭代的方式使用 `PUT` 来上传文件的字节范围，直到完整的文件上传完毕。</span><span class="sxs-lookup"><span data-stu-id="31fca-108">If the file size is between 3MB and 150MB, create an upload session, and iteratively use `PUT` to upload ranges of bytes of the file until you have uploaded the entire file.</span></span> <span data-ttu-id="31fca-109">最后一个成功 `PUT` 响应中的标头包括带附件 ID 的 URL。</span><span class="sxs-lookup"><span data-stu-id="31fca-109">A header in the final successful `PUT` response includes a URL with the attachment ID.</span></span>

<span data-ttu-id="31fca-110">若要将多个文件附加到邮件，请根据每个文件的文件大小，选择相应的方法，并单独附加文件。</span><span class="sxs-lookup"><span data-stu-id="31fca-110">To attach multiple files to a message, choose the approach for each file based on its file size and attach the files individually.</span></span>

<span data-ttu-id="31fca-111">本文逐步介绍了第二种方法，创建并使用上传会话来添加大型文件附件（大小超过 3 MB）至 Outlook 项。</span><span class="sxs-lookup"><span data-stu-id="31fca-111">This article illustrates the second approach step by step, creating and using an upload session to add a large file attachment (of size over 3MB) to an Outlook item.</span></span> <span data-ttu-id="31fca-112">各步显示相应的邮件或事件代码。</span><span class="sxs-lookup"><span data-stu-id="31fca-112">Each step shows the corresponding code for a message and for an event.</span></span> <span data-ttu-id="31fca-113">成功上传整个文件后，文章显示获取含有文件附件 ID 的响应标头，随后显示使用附件 ID 来获取原始附件内容或附件元数据。</span><span class="sxs-lookup"><span data-stu-id="31fca-113">Upon successfully uploading the entire file, the article shows getting a response header that contains an ID for the file attachment, and then using that attachment ID to get the raw attachment content or attachment metadata.</span></span> 

> [!IMPORTANT] 
> <span data-ttu-id="31fca-114">如果要将大文件附加到共享或委派邮箱中的邮件或事件，请注意一个[已知问题](known-issues.md#attaching-large-files-to-messages)。</span><span class="sxs-lookup"><span data-stu-id="31fca-114">Be aware of a [known issue](known-issues.md#attaching-large-files-to-messages) if you're attaching large files to a message or event in a shared or delegated mailbox.</span></span>

## <a name="step-1-create-an-upload-session"></a><span data-ttu-id="31fca-115">第 1 步：创建上传会话</span><span class="sxs-lookup"><span data-stu-id="31fca-115">Step 1: Create an upload session</span></span>

<span data-ttu-id="31fca-116">[创建上传会话](/graph/api/attachment-createuploadsession?view=graph-rest-1.0)，将文件附加到邮件或事件。</span><span class="sxs-lookup"><span data-stu-id="31fca-116">[Create an upload session](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) to attach a file to a message or event.</span></span> <span data-ttu-id="31fca-117">在输入参数 **AttachmentItem** 中指定文件。</span><span class="sxs-lookup"><span data-stu-id="31fca-117">Specify the file in the input parameter **AttachmentItem**.</span></span>

<span data-ttu-id="31fca-118">成功的操作返回 `HTTP 201 Created` 和新的 [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-1.0) 实例，其中包含可在后续 `PUT` 操作中用于上传文件各部分的非跳转 URL。</span><span class="sxs-lookup"><span data-stu-id="31fca-118">A successful operation returns `HTTP 201 Created` and a new [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-1.0) instance, which contains an opaque URL that you can use in subsequent `PUT` operations to upload portions of the file.</span></span> <span data-ttu-id="31fca-119">**uploadSession** 提供一个临时存储位置，在此位置保存文件字节数，直到完整文件上传完毕。</span><span class="sxs-lookup"><span data-stu-id="31fca-119">The **uploadSession** provides a temporary storage location where the bytes of the file are saved until you have uploaded the complete file.</span></span>

<span data-ttu-id="31fca-120">请务必请求 `Mail.ReadWrite` 权限，以为邮件创建 **uploadSession**，并为事件创建 `Calendars.ReadWrite`。</span><span class="sxs-lookup"><span data-stu-id="31fca-120">Make sure to request `Mail.ReadWrite` permission to create the **uploadSession** for a message, and `Calendars.ReadWrite` for an event.</span></span> <span data-ttu-id="31fca-121">新的 **uploadSession** 的 **uploadUrl** 属性中返回的非跳转 URL 经过预身份验证，包含针对 `https://outlook.office.com` 域中后续 `PUT` 查询的相应授权令牌。</span><span class="sxs-lookup"><span data-stu-id="31fca-121">The opaque URL, returned in the **uploadUrl** property of the new **uploadSession**, is pre-authenticated and contains the appropriate authorization token for subsequent `PUT` queries in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="31fca-122">该令牌会在 **expirationDateTime** 过期。</span><span class="sxs-lookup"><span data-stu-id="31fca-122">That token expires by **expirationDateTime**.</span></span> <span data-ttu-id="31fca-123">请勿自定义 `PUT` 操作的此 URL。</span><span class="sxs-lookup"><span data-stu-id="31fca-123">Do not customize this URL for the `PUT` operations.</span></span>

<span data-ttu-id="31fca-124">响应中的 **uploadSession** 对象还包含 **nextExpectedRanges** 属性，这指示初始上传开始位置应该为 0 字节。</span><span class="sxs-lookup"><span data-stu-id="31fca-124">The **uploadSession** object in the response also includes the **nextExpectedRanges** property, which indicates the initial upload starting location should be byte 0.</span></span>

### <a name="example-create-an-upload-session-for-a-message"></a><span data-ttu-id="31fca-125">示例：创建邮件的上传会话</span><span class="sxs-lookup"><span data-stu-id="31fca-125">Example: create an upload session for a message</span></span>

#### <a name="request"></a><span data-ttu-id="31fca-126">请求</span><span class="sxs-lookup"><span data-stu-id="31fca-126">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="31fca-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="31fca-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession_message",
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
# <a name="c"></a>[<span data-ttu-id="31fca-128">C#</span><span class="sxs-lookup"><span data-stu-id="31fca-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31fca-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31fca-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31fca-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31fca-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="31fca-131">响应</span><span class="sxs-lookup"><span data-stu-id="31fca-131">Response</span></span>
<span data-ttu-id="31fca-132">下列示例响应显示为邮件返回的 **uploadSession** 资源。</span><span class="sxs-lookup"><span data-stu-id="31fca-132">The following example response shows the **uploadSession** resource returned for the message.</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession_message",
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

### <a name="example-create-an-upload-session-for-an-event"></a><span data-ttu-id="31fca-133">示例：创建事件的上传会话</span><span class="sxs-lookup"><span data-stu-id="31fca-133">Example: create an upload session for an event</span></span>
#### <a name="request"></a><span data-ttu-id="31fca-134">请求</span><span class="sxs-lookup"><span data-stu-id="31fca-134">Request</span></span> 


# <a name="http"></a>[<span data-ttu-id="31fca-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="31fca-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession_event",
  "sampleKeys": ["AAMkADU5CCmSAAA="]
}-->
```http
POST https://graph.microsoft.com/beta/me/events/AAMkADU5CCmSAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```
# <a name="c"></a>[<span data-ttu-id="31fca-136">C#</span><span class="sxs-lookup"><span data-stu-id="31fca-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31fca-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31fca-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31fca-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31fca-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="31fca-139">响应</span><span class="sxs-lookup"><span data-stu-id="31fca-139">Response</span></span>
<span data-ttu-id="31fca-140">下列示例响应显示为shi'jian事件返回的 **uploadSession** 资源。</span><span class="sxs-lookup"><span data-stu-id="31fca-140">The following example response shows the **uploadSession** resource returned for the event.</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw",
    "expirationDateTime": "2020-02-22T02:46:56.7410786Z",
    "nextExpectedRanges": [
        "0-"
    ]
}

```


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a><span data-ttu-id="31fca-141">步骤 2：使用上传会话上传文件的字节范围</span><span class="sxs-lookup"><span data-stu-id="31fca-141">Step 2: Use the upload session to upload a range of bytes of the file</span></span>

<span data-ttu-id="31fca-142">如果要上传文件或文件的一部分，在 **uploadSession** 资源 **uploadUrl** 属性中，对第 1 步返回的 URL 进行 `PUT` 请求。</span><span class="sxs-lookup"><span data-stu-id="31fca-142">To upload the file, or a portion of the file, make a `PUT` request to the URL returned in step 1 in the **uploadUrl** property of the **uploadSession** resource.</span></span> <span data-ttu-id="31fca-143">可上传整个文件，或将文件拆分为多个字节范围。</span><span class="sxs-lookup"><span data-stu-id="31fca-143">You can upload the entire file, or split the file into multiple byte ranges.</span></span> <span data-ttu-id="31fca-144">为获得更好的性能，请保持每个字节范围小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="31fca-144">For better performance, keep each byte range less than 4 MB.</span></span>

<span data-ttu-id="31fca-145">按如下所述指定请求标头和请求正文。</span><span class="sxs-lookup"><span data-stu-id="31fca-145">Specify request headers and request body as described below.</span></span>

### <a name="request-headers"></a><span data-ttu-id="31fca-146">请求标头</span><span class="sxs-lookup"><span data-stu-id="31fca-146">Request headers</span></span>

| <span data-ttu-id="31fca-147">名称</span><span class="sxs-lookup"><span data-stu-id="31fca-147">Name</span></span>       | <span data-ttu-id="31fca-148">类型</span><span class="sxs-lookup"><span data-stu-id="31fca-148">Type</span></span> | <span data-ttu-id="31fca-149">说明</span><span class="sxs-lookup"><span data-stu-id="31fca-149">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="31fca-150">Content-Length</span><span class="sxs-lookup"><span data-stu-id="31fca-150">Content-Length</span></span> | <span data-ttu-id="31fca-151">Int32</span><span class="sxs-lookup"><span data-stu-id="31fca-151">Int32</span></span> | <span data-ttu-id="31fca-152">此操作中上传的字节数。</span><span class="sxs-lookup"><span data-stu-id="31fca-152">The number of bytes being uploaded in this operation.</span></span> <span data-ttu-id="31fca-153">为获得更好的性能，请将每个 `PUT` 操作的字节数的上限限制为 4 MB。</span><span class="sxs-lookup"><span data-stu-id="31fca-153">For better performance, keep the upper limit of the number of bytes for each `PUT` operation to 4 MB.</span></span> <span data-ttu-id="31fca-154">必填。</span><span class="sxs-lookup"><span data-stu-id="31fca-154">Required.</span></span> |
| <span data-ttu-id="31fca-155">Content-Range</span><span class="sxs-lookup"><span data-stu-id="31fca-155">Content-Range</span></span> | <span data-ttu-id="31fca-156">字符串</span><span class="sxs-lookup"><span data-stu-id="31fca-156">String</span></span> | <span data-ttu-id="31fca-157">此操作中要上传的文件的从 0 开始的字节范围，格式为 `bytes {start}-{end}/{total}`。</span><span class="sxs-lookup"><span data-stu-id="31fca-157">The 0-based byte range of the file being uploaded in this operation, expressed in the format `bytes {start}-{end}/{total}`.</span></span> <span data-ttu-id="31fca-158">必填。</span><span class="sxs-lookup"><span data-stu-id="31fca-158">Required.</span></span> |
| <span data-ttu-id="31fca-159">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31fca-159">Content-Type</span></span> | <span data-ttu-id="31fca-160">String</span><span class="sxs-lookup"><span data-stu-id="31fca-160">String</span></span>  | <span data-ttu-id="31fca-161">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="31fca-161">The MIME type.</span></span> <span data-ttu-id="31fca-162">指定 `application/octet-stream`。</span><span class="sxs-lookup"><span data-stu-id="31fca-162">Specify `application/octet-stream`.</span></span> <span data-ttu-id="31fca-163">必填。</span><span class="sxs-lookup"><span data-stu-id="31fca-163">Required.</span></span> |

<span data-ttu-id="31fca-164">请勿指定 `Authorization` 请求标头。</span><span class="sxs-lookup"><span data-stu-id="31fca-164">Do not specify an `Authorization` request header.</span></span> <span data-ttu-id="31fca-165">`PUT` 查询使用 **uploadUrl** 属性中预身份验证的 URL，该属性允许访问 `https://outlook.office.com` 域。</span><span class="sxs-lookup"><span data-stu-id="31fca-165">The `PUT` query uses a pre-authenticated URL from the **uploadUrl** property, that allows access to the `https://outlook.office.com` domain.</span></span>

### <a name="request-body"></a><span data-ttu-id="31fca-166">请求正文</span><span class="sxs-lookup"><span data-stu-id="31fca-166">Request body</span></span>

<span data-ttu-id="31fca-167">指定要附加的文件的实际字节数，它们位于由 `Content-Range` 请求标头指定的位置范围内。</span><span class="sxs-lookup"><span data-stu-id="31fca-167">Specify the actual bytes of the file to be attached, that are in the location range specified by the `Content-Range` request header.</span></span>

### <a name="response"></a><span data-ttu-id="31fca-168">响应</span><span class="sxs-lookup"><span data-stu-id="31fca-168">Response</span></span>
<span data-ttu-id="31fca-169">成功的上传将返回 `HTTP 200 OK` 和 **uploadSession** 对象。</span><span class="sxs-lookup"><span data-stu-id="31fca-169">A successful upload returns `HTTP 200 OK` and an **uploadSession** object.</span></span> <span data-ttu-id="31fca-170">请注意响应对象中的以下项：</span><span class="sxs-lookup"><span data-stu-id="31fca-170">Note the following in the response object:</span></span>

- <span data-ttu-id="31fca-171">**ExpirationDateTime** 属性指示 **uploadUrl** 属性值中嵌入的身份验证令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="31fca-171">The **ExpirationDateTime** property indicates the expiration date/time for the auth token embedded in the **uploadUrl** property value.</span></span> <span data-ttu-id="31fca-172">此到期日期/时间与步骤 1 中由初始 **uploadSession** 返回的值相同。</span><span class="sxs-lookup"><span data-stu-id="31fca-172">This expiration date/time remains the same as returned by the initial **uploadSession** in step 1.</span></span>
- <span data-ttu-id="31fca-173">**NextExpectedRanges** 指定上传开始的下一个字节位置，例如 `"NextExpectedRanges":["2097152"]`。</span><span class="sxs-lookup"><span data-stu-id="31fca-173">The **NextExpectedRanges** specifies the next byte location to start uploading from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="31fca-174">必须按顺序上传文件中的字节。</span><span class="sxs-lookup"><span data-stu-id="31fca-174">You must upload bytes in a file in order.</span></span>
<!-- The **NextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"NextExpectedRanges":["2097152"]`.
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"NextExpectedRanges":["1998457-2097094"]`.
-->
- <span data-ttu-id="31fca-175">**uploadUrl** 属性不会显式返回，因为上传会话的所有 `PUT` 操作使用创建会话时返回的同一 URL（步骤 1）。</span><span class="sxs-lookup"><span data-stu-id="31fca-175">The **uploadUrl** property is not explicitly returned, because all `PUT` operations of an upload session use the same URL returned when creating the session (step 1).</span></span>

### <a name="example-first-upload-to-the-message"></a><span data-ttu-id="31fca-176">示例：首先上传至消息</span><span class="sxs-lookup"><span data-stu-id="31fca-176">Example: first upload to the message</span></span>
#### <a name="request"></a><span data-ttu-id="31fca-177">请求</span><span class="sxs-lookup"><span data-stu-id="31fca-177">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="31fca-178">响应</span><span class="sxs-lookup"><span data-stu-id="31fca-178">Response</span></span>

<span data-ttu-id="31fca-179">下列示例响应在 **NextExpectedRanges** 属性中显示服务器预期的下一字节范围的起点。</span><span class="sxs-lookup"><span data-stu-id="31fca-179">The following example response shows in the **NextExpectedRanges** property the start of the next byte range that the server expects.</span></span>
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

### <a name="example-first-upload-to-the-event"></a><span data-ttu-id="31fca-180">示例：首先上传至事件</span><span class="sxs-lookup"><span data-stu-id="31fca-180">Example: first upload to the event</span></span>
#### <a name="request"></a><span data-ttu-id="31fca-181">请求</span><span class="sxs-lookup"><span data-stu-id="31fca-181">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

#### <a name="response"></a><span data-ttu-id="31fca-182">响应</span><span class="sxs-lookup"><span data-stu-id="31fca-182">Response</span></span>

<span data-ttu-id="31fca-183">下列示例响应在 **NextExpectedRanges** 属性中显示服务器预期的下一字节范围的起点。</span><span class="sxs-lookup"><span data-stu-id="31fca-183">The following example response shows in the **NextExpectedRanges** property the start of the next byte range that the server expects.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://outlook.office.com/api/beta/$metadata#Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69%4098a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA%3D')/AttachmentSessions/$entity",
    "ExpirationDateTime":"2020-02-22T02:46:56.7410786Z",
    "NextExpectedRanges":["2097152"]
}
```


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a><span data-ttu-id="31fca-184">步骤 3：继续上传字节范围，直至完整文件上传完毕</span><span class="sxs-lookup"><span data-stu-id="31fca-184">Step 3: Continue uploading byte ranges until the entire file has been uploaded</span></span>

<span data-ttu-id="31fca-185">执行步骤 2 中的初始上传后，在会话的到期日期/时间前，使用步骤 2 中所述的 `PUT` 请求，继续上传文件中剩余的部分。</span><span class="sxs-lookup"><span data-stu-id="31fca-185">Following the initial upload in step 2, continue to upload the remaining portion of the file, using a similar `PUT` request as described in step 2, before you reach the expiration date/time for the session.</span></span> <span data-ttu-id="31fca-186">使用 **NextExpectedRanges** 集合确定要上传的下一个字节范围的开头。</span><span class="sxs-lookup"><span data-stu-id="31fca-186">Use the **NextExpectedRanges** collection to determine where to start the next byte range to upload.</span></span> <span data-ttu-id="31fca-187">可能会发现指定了多个范围，这些范围指明了服务器尚未收到的文件部分。</span><span class="sxs-lookup"><span data-stu-id="31fca-187">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="31fca-188">如果需要恢复中断的传输，并且客户端不能确定服务的状态，这个方法很有用。</span><span class="sxs-lookup"><span data-stu-id="31fca-188">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="31fca-189">成功上传文件的最后一个字节后，最终 `PUT` 操作返回 `HTTP 201 Created` 以及指示 `https://outlook.office.com` 域中文件附件 URL 的 `Location` 标头。</span><span class="sxs-lookup"><span data-stu-id="31fca-189">Once the last byte of the file has been successfully uploaded, the final `PUT` operation returns `HTTP 201 Created` and a `Location` header that indicates the URL to the file attachment in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="31fca-190">可从 URL 获取附件 ID 并将其保存供以后使用。</span><span class="sxs-lookup"><span data-stu-id="31fca-190">You can get the attachment ID from the URL and save it for later use.</span></span> <span data-ttu-id="31fca-191">可以使用该 ID [获取附件的元数据](/graph/api/attachment-get?view=graph-rest-1.0)，或使用 Microsoft Graph 终结点[将附件从 Outlook 项中删除](/graph/api/attachment-delete?view=graph-rest-1.0)，具体取决于你的场景。</span><span class="sxs-lookup"><span data-stu-id="31fca-191">Depending on your scenario, you can use that ID to [get the metadata of the attachment](/graph/api/attachment-get?view=graph-rest-1.0), or [remove the attachment from the Outlook item](/graph/api/attachment-delete?view=graph-rest-1.0) using the Microsoft Graph endpoint.</span></span>

<span data-ttu-id="31fca-192">下列示例显示在此处理步骤中上传最后的文件字节范围至邮件和事件。</span><span class="sxs-lookup"><span data-stu-id="31fca-192">The following examples show uploading the last byte range of the file to the message and to the event in the preceding steps.</span></span>

### <a name="example-final-upload-to-the-message"></a><span data-ttu-id="31fca-193">示例：最后上传至消息</span><span class="sxs-lookup"><span data-stu-id="31fca-193">Example: final upload to the message</span></span>
#### <a name="request"></a><span data-ttu-id="31fca-194">请求</span><span class="sxs-lookup"><span data-stu-id="31fca-194">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="31fca-195">响应</span><span class="sxs-lookup"><span data-stu-id="31fca-195">Response</span></span>
<span data-ttu-id="31fca-196">下列示例显示可保存附件 ID（`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`）以供随后使用的 `Location` 响应标头。</span><span class="sxs-lookup"><span data-stu-id="31fca-196">The following example response shows a `Location` response header from which you can save the attachment ID (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) for later use.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

### <a name="example-final-upload-to-the-event"></a><span data-ttu-id="31fca-197">示例：最后上传至事件</span><span class="sxs-lookup"><span data-stu-id="31fca-197">Example: final upload to the event</span></span>
#### <a name="request"></a><span data-ttu-id="31fca-198">请求</span><span class="sxs-lookup"><span data-stu-id="31fca-198">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

#### <a name="response"></a><span data-ttu-id="31fca-199">响应</span><span class="sxs-lookup"><span data-stu-id="31fca-199">Response</span></span>
<span data-ttu-id="31fca-200">下列示例显示可保存附件 ID（`AAMkADU5CCmSAAANZAlYPeyQByv7Y=`）以供随后使用的 `Location` 响应标头。</span><span class="sxs-lookup"><span data-stu-id="31fca-200">The following example response shows a `Location` response header from which you can save the attachment ID (`AAMkADU5CCmSAAANZAlYPeyQByv7Y=`) for later use.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/beta/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-outlook-item"></a><span data-ttu-id="31fca-201">步骤 4（可选）：从 Outlook 项中获取文件附件</span><span class="sxs-lookup"><span data-stu-id="31fca-201">Step 4 (optional): Get the file attachment from the Outlook item</span></span>

<span data-ttu-id="31fca-202">和往常一样，从 Outlook 项中[获取附件](/graph/api/attachment-get?view=graph-rest-1.0)在理论上并不受附件大小限制。</span><span class="sxs-lookup"><span data-stu-id="31fca-202">As always, [getting an attachment](/graph/api/attachment-get?view=graph-rest-1.0) from an Outlook item is not technically limited by attachment size.</span></span>

<span data-ttu-id="31fca-203">但是，获取采用 base64 编码格式的大文件附件会影响 API 性能。</span><span class="sxs-lookup"><span data-stu-id="31fca-203">However, getting a large file attachment in base64-encoded format affects API performance.</span></span> <span data-ttu-id="31fca-204">如果需要大型附件：</span><span class="sxs-lookup"><span data-stu-id="31fca-204">If you expect a large attachment:</span></span>

- <span data-ttu-id="31fca-205">作为获取采用 base64 格式的附件内容的替代方法，可以[获取文件附件的元数据](/graph/api/attachment-get?view=graph-rest-1.0#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="31fca-205">As an alternative to getting the attachment content in base64 format, you can [get the raw data of the file attachment](/graph/api/attachment-get?view=graph-rest-1.0#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message).</span></span>
- <span data-ttu-id="31fca-206">要[获取文件附件的元数据](/graph/api/attachment-get?view=graph-rest-1.0#example-1-get-the-properties-of-a-file-attachment)，可以附加 `$select` 参数以仅包含所需的元数据属性，排除返回采用 base64 格式的文件附件的 **contentBytes** 属性。</span><span class="sxs-lookup"><span data-stu-id="31fca-206">To [get the metadata of the file attachment](/graph/api/attachment-get?view=graph-rest-1.0#example-1-get-the-properties-of-a-file-attachment), append a `$select` parameter to include only those metadata properties you want, excluding the **contentBytes** property which returns the file attachment in base64 format.</span></span>

### <a name="example-get-the-raw-file-attached-to-the-event"></a><span data-ttu-id="31fca-207">示例：获取附加到事件的原始文件</span><span class="sxs-lookup"><span data-stu-id="31fca-207">Example: Get the raw file attached to the event</span></span>
<span data-ttu-id="31fca-208">按照事件示例和使用上一步 `Location` 标头中返回的附件 ID，下一示例请求显示使用 `$value` 参数获取附件的原始内容数据。</span><span class="sxs-lookup"><span data-stu-id="31fca-208">Following the event example and using the attachment ID returned in the `Location` header of the previous step, the next example request shows using a `$value` parameter to get the attachment raw content data.</span></span>

#### <a name="request"></a><span data-ttu-id="31fca-209">请求</span><span class="sxs-lookup"><span data-stu-id="31fca-209">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "walkthrough_get_attachment_raw",
  "sampleKeys": ["d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32", "AAMkADU5CCmSAAA=", "AAMkADU5CCmSAAANZAlYPeyQByv7Y="]
}-->
```http
GET https://graph.microsoft.com/beta/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')/$value
```

#### <a name="response"></a><span data-ttu-id="31fca-210">响应</span><span class="sxs-lookup"><span data-stu-id="31fca-210">Response</span></span>

<!-- {
  "blockType": "ignored",
  "name": "walkthrough_get_attachment_raw",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
content-length: 3483322
Content-type: image/jpeg

{Raw bytes of the file}
```


### <a name="example-get-the-metadata-of-the-file-attached-to-the-message"></a><span data-ttu-id="31fca-211">示例：获取邮件附加的文件的元数据</span><span class="sxs-lookup"><span data-stu-id="31fca-211">Example: Get the metadata of the file attached to the message</span></span>
<span data-ttu-id="31fca-212">按照邮件示例，下一示例请求显示使用 `$select` 参数来获取有关邮件的文件附件的部分元数据，不包括 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="31fca-212">Following the message example, the next example request shows using a `$select` parameter to get some of the metadata of a file attachment on a message, excluding **contentBytes**.</span></span>

#### <a name="request"></a><span data-ttu-id="31fca-213">请求</span><span class="sxs-lookup"><span data-stu-id="31fca-213">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment_metadata",
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline
```

#### <a name="response"></a><span data-ttu-id="31fca-214">响应</span><span class="sxs-lookup"><span data-stu-id="31fca-214">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_get_attachment_metadata",
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


## <a name="alternative-cancel-the-upload-session"></a><span data-ttu-id="31fca-215">替代方法：取消上传会话</span><span class="sxs-lookup"><span data-stu-id="31fca-215">Alternative: Cancel the upload session</span></span>

<span data-ttu-id="31fca-216">在上传会话到期之前的任何时间，如果必须取消上传，可使用同一初始非跳转 URL 来删除上传会话。</span><span class="sxs-lookup"><span data-stu-id="31fca-216">At any point of time before the upload session expires, if you have to cancel the upload, you can use the same initial opaque URL to delete the upload session.</span></span> <span data-ttu-id="31fca-217">成功的操作将返回 `HTTP 204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="31fca-217">A successful operation returns `HTTP 204 No Content`.</span></span>

### <a name="example-cancel-the-upload-session-for-the-message"></a><span data-ttu-id="31fca-218">示例：取消邮件的上传会话</span><span class="sxs-lookup"><span data-stu-id="31fca-218">Example: cancel the upload session for the message</span></span>

#### <a name="request"></a><span data-ttu-id="31fca-219">请求</span><span class="sxs-lookup"><span data-stu-id="31fca-219">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

#### <a name="response"></a><span data-ttu-id="31fca-220">响应</span><span class="sxs-lookup"><span data-stu-id="31fca-220">Response</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```
## <a name="errors"></a><span data-ttu-id="31fca-221">错误</span><span class="sxs-lookup"><span data-stu-id="31fca-221">Errors</span></span>

### <a name="errorattachmentsizeshouldnotbelessthanminimumsize"></a><span data-ttu-id="31fca-222">ErrorAttachmentSizeShouldNotBeLessThanMinimumSize</span><span class="sxs-lookup"><span data-stu-id="31fca-222">ErrorAttachmentSizeShouldNotBeLessThanMinimumSize</span></span>

<span data-ttu-id="31fca-223">尝试[创建上传会话](/graph/api/attachment-createuploadsession?view=graph-rest-1.0)以附加小于 3 MB 的文件时返回此错误。</span><span class="sxs-lookup"><span data-stu-id="31fca-223">This error is returned when attempting to [create an upload session](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) to attach a file smaller than 3 MB.</span></span> <span data-ttu-id="31fca-224">如果文件大小小于 3 MB，则应该针对[邮件](/graph/api/message-post-attachments?view=graph-rest-1.0)或[事件](/graph/api/event-post-attachments?view=graph-rest-1.0)的**附件**导航属性执行单个 POST。</span><span class="sxs-lookup"><span data-stu-id="31fca-224">If the file size is under 3 MB, you should do a single POST on the **attachments** navigation property [of the message](/graph/api/message-post-attachments?view=graph-rest-1.0) or [of the event](/graph/api/event-post-attachments?view=graph-rest-1.0).</span></span> <span data-ttu-id="31fca-225">成功的 `POST` 响应包括附加到邮件的文件的 ID。</span><span class="sxs-lookup"><span data-stu-id="31fca-225">The successful `POST` response includes the ID of the file attached to the message.</span></span>

