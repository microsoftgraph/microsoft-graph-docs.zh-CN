---
title: 附件： createUploadSession
description: 创建上载会话以以迭代方式上载文件的范围，以便将文件附加到指定的邮件。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 006a0ac5428aeca18549f8f66863d7312c63750d
ms.sourcegitcommit: feebe30e62aa19ce5cb8e8338e043326e464ed9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991851"
---
# <a name="attachment-createuploadsession"></a><span data-ttu-id="ae7ab-103">附件： createUploadSession</span><span class="sxs-lookup"><span data-stu-id="ae7ab-103">attachment: createUploadSession</span></span>

<span data-ttu-id="ae7ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae7ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae7ab-105">创建一个允许应用程序以迭代方式上载文件范围的上载会话，以便将该文件附加到指定的 Outlook 项目。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-105">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified Outlook item.</span></span> <span data-ttu-id="ae7ab-106">项目可以是[消息](../resources/message.md)或[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-106">The item can be a [message](../resources/message.md) or [event](../resources/event.md).</span></span>

<span data-ttu-id="ae7ab-107">如果文件大小在 3 MB 到 150 MB 之间，则使用此方法附加文件。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-107">Use this approach to attach a file if the file size is between 3 MB and 150 MB.</span></span> <span data-ttu-id="ae7ab-108">若要附加小于 3 MB 的文件，请在 Outlook 项目`POST`的 "**附件**" 导航属性上执行操作;请参阅如何[为邮件](message-post-attachments.md)或[事件](event-post-attachments.md)执行此操作。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-108">To attach a file that's smaller than 3 MB, do a `POST` operation on the **attachments** navigation property of the Outlook item; see how to do this [for a message](message-post-attachments.md) or [for an event](event-post-attachments.md).</span></span> 

<span data-ttu-id="ae7ab-109">作为响应的一部分，此操作将返回可在后续顺序`PUT`查询中使用的上载 URL。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-109">As part of the response, this action returns an upload URL that you can use in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="ae7ab-110">每个`PUT`操作的请求标头允许您指定要上载的确切字节范围。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-110">Request headers for each `PUT` operation let you specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="ae7ab-111">这样，如果在上载过程中断开网络连接，则可以恢复传输。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-111">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

<span data-ttu-id="ae7ab-112">以下是使用上载会话将文件附加到 Outlook 项目的步骤：</span><span class="sxs-lookup"><span data-stu-id="ae7ab-112">The following are the steps to attach a file to an Outlook item using an upload session:</span></span>

1. <span data-ttu-id="ae7ab-113">创建上传会话。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-113">Create an upload session.</span></span>
2. <span data-ttu-id="ae7ab-114">在该上传会话中，以迭代方式上载字节的范围（每次最长为 4 MB），直到上载了文件的所有字节，并将该文件附加到指定的项目。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-114">Within that upload session, iteratively upload ranges of bytes (up to 4 MB each time) until all the bytes of the file have been uploaded, and the file is attached to the specified item.</span></span>
3. <span data-ttu-id="ae7ab-115">保存附件的 ID 以供将来访问。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-115">Save the ID for the attachment for future access.</span></span>
4. <span data-ttu-id="ae7ab-116">可选：删除上传会话。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-116">Optional: Delete the upload session.</span></span>

<span data-ttu-id="ae7ab-117">有关示例，请参阅[将大型文件附加到 Outlook 消息或事件](/graph/outlook-large-attachments)。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-117">See [attach large files to Outlook messages or events](/graph/outlook-large-attachments) for an example.</span></span>

> [!TIP]
> <span data-ttu-id="ae7ab-118">Exchange Online 允许管理员自定义 Office 365 邮箱的邮件大小限制，包括任何邮件附件。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-118">Exchange Online lets administrators customize the message size limit for Office 365 mailboxes,  including any message attachments.</span></span> <span data-ttu-id="ae7ab-119">默认情况下，此邮件大小限制为 35 MB。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-119">By default, this message size limit is 35 MB.</span></span> <span data-ttu-id="ae7ab-120">了解如何[自定义最大邮件大小](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb)，以支持大于租户默认限制的附件。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-120">Find out how to [customize the maximum message size](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) to support attachments larger than the default limit for your tenant.</span></span> 

> [!IMPORTANT] 
> <span data-ttu-id="ae7ab-121">如果要将大型文件附加到共享或委派邮箱中的邮件或事件，请注意[已知问题](/graph/known-issues#attaching-large-files-to-messages)。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-121">Be aware of a [known issue](/graph/known-issues#attaching-large-files-to-messages) if you're attaching a large file to a message or event in a shared or delegated mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae7ab-122">权限</span><span class="sxs-lookup"><span data-stu-id="ae7ab-122">Permissions</span></span>

<span data-ttu-id="ae7ab-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae7ab-125">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae7ab-125">Permission type</span></span>                        | <span data-ttu-id="ae7ab-126">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae7ab-126">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ae7ab-127">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae7ab-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae7ab-128">"日历"、"邮件"、"写"</span><span class="sxs-lookup"><span data-stu-id="ae7ab-128">Calendars.ReadWrite, Mail.ReadWrite</span></span> |
| <span data-ttu-id="ae7ab-129">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae7ab-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae7ab-130">"日历"、"邮件"、"写"</span><span class="sxs-lookup"><span data-stu-id="ae7ab-130">Calendars.ReadWrite, Mail.ReadWrite</span></span> |
| <span data-ttu-id="ae7ab-131">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae7ab-131">Application</span></span>                            | <span data-ttu-id="ae7ab-132">"日历"、"邮件"、"写"</span><span class="sxs-lookup"><span data-stu-id="ae7ab-132">Calendars.ReadWrite, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae7ab-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae7ab-133">HTTP request</span></span>

<span data-ttu-id="ae7ab-134">创建用于将文件附加到**事件**的上载会话：</span><span class="sxs-lookup"><span data-stu-id="ae7ab-134">To create an upload session for attaching a file to an **event**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
```

<span data-ttu-id="ae7ab-135">创建用于将文件附加到**邮件**的上载会话：</span><span class="sxs-lookup"><span data-stu-id="ae7ab-135">To create an upload session for attaching a file to a **message**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="ae7ab-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae7ab-136">Request headers</span></span>

| <span data-ttu-id="ae7ab-137">名称</span><span class="sxs-lookup"><span data-stu-id="ae7ab-137">Name</span></span>          | <span data-ttu-id="ae7ab-138">说明</span><span class="sxs-lookup"><span data-stu-id="ae7ab-138">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ae7ab-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae7ab-139">Authorization</span></span> | <span data-ttu-id="ae7ab-140">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ae7ab-140">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="ae7ab-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae7ab-141">Request body</span></span>

<span data-ttu-id="ae7ab-142">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ae7ab-143">参数</span><span class="sxs-lookup"><span data-stu-id="ae7ab-143">Parameter</span></span>    | <span data-ttu-id="ae7ab-144">类型</span><span class="sxs-lookup"><span data-stu-id="ae7ab-144">Type</span></span>        | <span data-ttu-id="ae7ab-145">说明</span><span class="sxs-lookup"><span data-stu-id="ae7ab-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ae7ab-146">AttachmentItem</span><span class="sxs-lookup"><span data-stu-id="ae7ab-146">AttachmentItem</span></span>|[<span data-ttu-id="ae7ab-147">attachmentItem</span><span class="sxs-lookup"><span data-stu-id="ae7ab-147">attachmentItem</span></span>](../resources/attachmentitem.md)|<span data-ttu-id="ae7ab-148">表示要上载和附加的项的属性。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-148">Represents attributes of the item to be uploaded and attached.</span></span> <span data-ttu-id="ae7ab-149">至少指定附件类型（`file`）、名称和文件大小。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-149">At minimum, specify the attachment type (`file`), a name, and the size of the file.</span></span>|

## <a name="response"></a><span data-ttu-id="ae7ab-150">响应</span><span class="sxs-lookup"><span data-stu-id="ae7ab-150">Response</span></span>

<span data-ttu-id="ae7ab-151">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[uploadSession](../resources/uploadsession.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-151">If successful, this method returns a `201 Created` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="ae7ab-152">**注意**：</span><span class="sxs-lookup"><span data-stu-id="ae7ab-152">**Note**:</span></span> 
>
><span data-ttu-id="ae7ab-153">作为**uploadSession** response 对象的一部分返回的**uploadUrl**属性是一个不透明的 URL， `PUT`用于随后的查询上传文件的字节范围。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-153">The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="ae7ab-154">它包含针对`PUT` **expirationDateTime**到期的后续查询的相应 auth 令牌。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-154">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="ae7ab-155">请勿自定义此 URL。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-155">Do not customize this URL.</span></span>
>
><span data-ttu-id="ae7ab-156">**NextExpectedRanges**属性指定要从中上载的下一个文件字节位置，例如`"NextExpectedRanges":["2097152"]`。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-156">The **nextExpectedRanges** property specifies the next file byte location to upload from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="ae7ab-157">必须按顺序上传文件中的字节。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-157">You must upload bytes in a file in order.</span></span>

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a><span data-ttu-id="ae7ab-158">示例</span><span class="sxs-lookup"><span data-stu-id="ae7ab-158">Examples</span></span>

<span data-ttu-id="ae7ab-159">下面的示例演示如何创建可在后续文件上载操作中用于指定邮件的上载会话。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-159">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified message.</span></span>

### <a name="request"></a><span data-ttu-id="ae7ab-160">请求</span><span class="sxs-lookup"><span data-stu-id="ae7ab-160">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="ae7ab-161">响应</span><span class="sxs-lookup"><span data-stu-id="ae7ab-161">Response</span></span>

> <span data-ttu-id="ae7ab-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ae7ab-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
