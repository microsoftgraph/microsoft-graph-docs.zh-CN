---
title: attachment： createUploadSession
description: 创建上载会话以迭代上载文件的范围，以便将文件附加到指定消息。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8475327164c92ee0720a2236ca41294e6b8ff472
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051625"
---
# <a name="attachment-createuploadsession"></a><span data-ttu-id="4491d-103">attachment： createUploadSession</span><span class="sxs-lookup"><span data-stu-id="4491d-103">attachment: createUploadSession</span></span>

<span data-ttu-id="4491d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4491d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4491d-105">创建允许应用迭代上载文件范围的上载会话，以便将文件附加到指定的Outlook项。</span><span class="sxs-lookup"><span data-stu-id="4491d-105">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified Outlook item.</span></span> <span data-ttu-id="4491d-106">项目可以是消息[或](../resources/message.md)[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="4491d-106">The item can be a [message](../resources/message.md) or [event](../resources/event.md).</span></span>

<span data-ttu-id="4491d-107">如果文件大小在 3 MB 到 150 MB 之间，则使用该方法附加文件。</span><span class="sxs-lookup"><span data-stu-id="4491d-107">Use this approach to attach a file if the file size is between 3 MB and 150 MB.</span></span> <span data-ttu-id="4491d-108">若要附加小于 3 MB 的文件，请对 Outlook 项目的附件导航属性执行一个操作;请参阅如何为邮件或 `POST` [事件执行该操作](event-post-attachments.md)。  [](message-post-attachments.md)</span><span class="sxs-lookup"><span data-stu-id="4491d-108">To attach a file that's smaller than 3 MB, do a `POST` operation on the **attachments** navigation property of the Outlook item; see how to do this [for a message](message-post-attachments.md) or [for an event](event-post-attachments.md).</span></span> 

<span data-ttu-id="4491d-109">作为响应的一部分，此操作返回可用于后续顺序查询的上载 `PUT` URL。</span><span class="sxs-lookup"><span data-stu-id="4491d-109">As part of the response, this action returns an upload URL that you can use in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="4491d-110">通过每个操作的请求 `PUT` 标头，可以指定要上载的字节的准确范围。</span><span class="sxs-lookup"><span data-stu-id="4491d-110">Request headers for each `PUT` operation let you specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="4491d-111">这允许恢复传输，以防在上载过程中网络连接中断。</span><span class="sxs-lookup"><span data-stu-id="4491d-111">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

<span data-ttu-id="4491d-112">以下是使用上载会话将文件附加到Outlook项的步骤：</span><span class="sxs-lookup"><span data-stu-id="4491d-112">The following are the steps to attach a file to an Outlook item using an upload session:</span></span>

1. <span data-ttu-id="4491d-113">创建上载会话。</span><span class="sxs-lookup"><span data-stu-id="4491d-113">Create an upload session.</span></span>
2. <span data-ttu-id="4491d-114">在此上载会话中，每次) 以迭代方式上载字节范围 (最多上载 4 MB，直到上载文件的所有字节，并且文件附加到指定项。</span><span class="sxs-lookup"><span data-stu-id="4491d-114">Within that upload session, iteratively upload ranges of bytes (up to 4 MB each time) until all the bytes of the file have been uploaded, and the file is attached to the specified item.</span></span>
3. <span data-ttu-id="4491d-115">保存附件的 ID，供将来访问。</span><span class="sxs-lookup"><span data-stu-id="4491d-115">Save the ID for the attachment for future access.</span></span>
4. <span data-ttu-id="4491d-116">可选：删除上载会话。</span><span class="sxs-lookup"><span data-stu-id="4491d-116">Optional: Delete the upload session.</span></span>

<span data-ttu-id="4491d-117">有关[示例，请参阅Outlook大文件附加到邮件](/graph/outlook-large-attachments)或事件。</span><span class="sxs-lookup"><span data-stu-id="4491d-117">See [attach large files to Outlook messages or events](/graph/outlook-large-attachments) for an example.</span></span>

> [!TIP]
> <span data-ttu-id="4491d-118">Exchange Online管理员可自定义邮箱的邮件大小Microsoft 365，包括任何邮件附件。</span><span class="sxs-lookup"><span data-stu-id="4491d-118">Exchange Online lets administrators customize the message size limit for Microsoft 365 mailboxes,  including any message attachments.</span></span> <span data-ttu-id="4491d-119">默认情况下，此邮件大小限制为 35 MB。</span><span class="sxs-lookup"><span data-stu-id="4491d-119">By default, this message size limit is 35 MB.</span></span> <span data-ttu-id="4491d-120">了解如何自定义 [最大邮件大小](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) 以支持大于租户默认限制的附件。</span><span class="sxs-lookup"><span data-stu-id="4491d-120">Find out how to [customize the maximum message size](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) to support attachments larger than the default limit for your tenant.</span></span> 

> [!IMPORTANT] 
> <span data-ttu-id="4491d-121">如果将大文件 [附加到](/graph/known-issues#attaching-large-files-to-messages) 共享或委派邮箱中的邮件或事件，请注意已知问题。</span><span class="sxs-lookup"><span data-stu-id="4491d-121">Be aware of a [known issue](/graph/known-issues#attaching-large-files-to-messages) if you're attaching a large file to a message or event in a shared or delegated mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="4491d-122">权限</span><span class="sxs-lookup"><span data-stu-id="4491d-122">Permissions</span></span>

<span data-ttu-id="4491d-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4491d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4491d-125">权限类型</span><span class="sxs-lookup"><span data-stu-id="4491d-125">Permission type</span></span>                        | <span data-ttu-id="4491d-126">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4491d-126">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4491d-127">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4491d-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="4491d-128">Calendars.ReadWrite、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4491d-128">Calendars.ReadWrite, Mail.ReadWrite</span></span> |
| <span data-ttu-id="4491d-129">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4491d-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4491d-130">Calendars.ReadWrite、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4491d-130">Calendars.ReadWrite, Mail.ReadWrite</span></span> |
| <span data-ttu-id="4491d-131">应用程序</span><span class="sxs-lookup"><span data-stu-id="4491d-131">Application</span></span>                            | <span data-ttu-id="4491d-132">Calendars.ReadWrite、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4491d-132">Calendars.ReadWrite, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4491d-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4491d-133">HTTP request</span></span>

<span data-ttu-id="4491d-134">若要创建上传会话以将文件附加到 **事件**：</span><span class="sxs-lookup"><span data-stu-id="4491d-134">To create an upload session for attaching a file to an **event**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
```

<span data-ttu-id="4491d-135">若要创建用于将文件附加到邮件的上载 **会话：**</span><span class="sxs-lookup"><span data-stu-id="4491d-135">To create an upload session for attaching a file to a **message**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="4491d-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="4491d-136">Request headers</span></span>

| <span data-ttu-id="4491d-137">名称</span><span class="sxs-lookup"><span data-stu-id="4491d-137">Name</span></span>          | <span data-ttu-id="4491d-138">说明</span><span class="sxs-lookup"><span data-stu-id="4491d-138">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4491d-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="4491d-139">Authorization</span></span> | <span data-ttu-id="4491d-140">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="4491d-140">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="4491d-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="4491d-141">Request body</span></span>

<span data-ttu-id="4491d-142">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4491d-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4491d-143">参数</span><span class="sxs-lookup"><span data-stu-id="4491d-143">Parameter</span></span>    | <span data-ttu-id="4491d-144">类型</span><span class="sxs-lookup"><span data-stu-id="4491d-144">Type</span></span>        | <span data-ttu-id="4491d-145">说明</span><span class="sxs-lookup"><span data-stu-id="4491d-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4491d-146">AttachmentItem</span><span class="sxs-lookup"><span data-stu-id="4491d-146">AttachmentItem</span></span>|[<span data-ttu-id="4491d-147">attachmentItem</span><span class="sxs-lookup"><span data-stu-id="4491d-147">attachmentItem</span></span>](../resources/attachmentitem.md)|<span data-ttu-id="4491d-148">表示要上载和附加的项目的属性。</span><span class="sxs-lookup"><span data-stu-id="4491d-148">Represents attributes of the item to be uploaded and attached.</span></span> <span data-ttu-id="4491d-149">至少应指定附件 `file` () 、名称和文件大小。</span><span class="sxs-lookup"><span data-stu-id="4491d-149">At minimum, specify the attachment type (`file`), a name, and the size of the file.</span></span>|

## <a name="response"></a><span data-ttu-id="4491d-150">响应</span><span class="sxs-lookup"><span data-stu-id="4491d-150">Response</span></span>

<span data-ttu-id="4491d-151">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和新 [uploadSession](../resources/uploadsession.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4491d-151">If successful, this method returns a `201 Created` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="4491d-152">**注意**：</span><span class="sxs-lookup"><span data-stu-id="4491d-152">**Note**:</span></span> 
>
><span data-ttu-id="4491d-153">作为 **uploadSession** 响应对象的一部分返回的 **uploadUrl** 属性是后续查询用于上载文件的字节范围的不透明 `PUT` URL。</span><span class="sxs-lookup"><span data-stu-id="4491d-153">The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="4491d-154">它包含过期 `PUT` **expirationDateTime 的后续查询的适当身份验证令牌**。</span><span class="sxs-lookup"><span data-stu-id="4491d-154">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="4491d-155">不自定义此 URL。</span><span class="sxs-lookup"><span data-stu-id="4491d-155">Do not customize this URL.</span></span>
>
><span data-ttu-id="4491d-156">**nextExpectedRanges** 属性指定要上载的下一个文件字节位置，例如， `"NextExpectedRanges":["2097152"]` 。</span><span class="sxs-lookup"><span data-stu-id="4491d-156">The **nextExpectedRanges** property specifies the next file byte location to upload from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="4491d-157">必须按顺序上传文件中的字节。</span><span class="sxs-lookup"><span data-stu-id="4491d-157">You must upload bytes in a file in order.</span></span>

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a><span data-ttu-id="4491d-158">示例</span><span class="sxs-lookup"><span data-stu-id="4491d-158">Examples</span></span>

<span data-ttu-id="4491d-159">以下示例演示如何创建可用于后续文件上载操作到指定邮件的上载会话。</span><span class="sxs-lookup"><span data-stu-id="4491d-159">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified message.</span></span>

### <a name="request"></a><span data-ttu-id="4491d-160">请求</span><span class="sxs-lookup"><span data-stu-id="4491d-160">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4491d-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="4491d-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower", 
    "size": 3483322
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4491d-162">C#</span><span class="sxs-lookup"><span data-stu-id="4491d-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4491d-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4491d-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4491d-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4491d-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4491d-165">Java</span><span class="sxs-lookup"><span data-stu-id="4491d-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/attachment-createuploadsession-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4491d-166">响应</span><span class="sxs-lookup"><span data-stu-id="4491d-166">Response</span></span>

> <span data-ttu-id="4491d-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4491d-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "attachment_createuploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0uAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment: createUploadSession",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

