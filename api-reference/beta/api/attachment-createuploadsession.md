---
title: 附件： createUploadSession
description: 创建上载会话以以迭代方式上载文件的范围，以便将文件附加到指定的邮件。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6bfdc379a8eb7857e4871ad13a6be47e87a2fe6e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43368016"
---
# <a name="attachment-createuploadsession"></a><span data-ttu-id="029ed-103">附件： createUploadSession</span><span class="sxs-lookup"><span data-stu-id="029ed-103">attachment: createUploadSession</span></span>

<span data-ttu-id="029ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="029ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="029ed-105">创建一个允许应用程序以迭代方式上载文件范围的上载会话，以便将文件附加到指定的[邮件](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="029ed-105">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified [message](../resources/message.md).</span></span>

<span data-ttu-id="029ed-106">当文件大小介于 3 MB 和 150 MB 之间时，使用此方法可将文件附加到**邮件**。</span><span class="sxs-lookup"><span data-stu-id="029ed-106">Use this approach to attach a file to a **message** when the file size is between 3 MB and 150 MB.</span></span> <span data-ttu-id="029ed-107">若要附加小于 3 MB 的文件，请[在 "附件" 导航属性上进行发布](message-post-attachments.md)。</span><span class="sxs-lookup"><span data-stu-id="029ed-107">To attach a file that's smaller than 3 MB,  [POST on the attachments navigation property](message-post-attachments.md).</span></span> 

<span data-ttu-id="029ed-108">作为响应的一部分，此操作将返回可在后续顺序`PUT`查询中使用的上载 URL。</span><span class="sxs-lookup"><span data-stu-id="029ed-108">As part of the response, this action returns an upload URL that you can use in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="029ed-109">每个`PUT`操作的请求标头允许您指定要上载的确切字节范围。</span><span class="sxs-lookup"><span data-stu-id="029ed-109">Request headers for each `PUT` operation let you specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="029ed-110">这样，如果在上载过程中断开网络连接，则可以恢复传输。</span><span class="sxs-lookup"><span data-stu-id="029ed-110">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

<span data-ttu-id="029ed-111">以下是使用上传会话附加文件的步骤：</span><span class="sxs-lookup"><span data-stu-id="029ed-111">The following are the steps to attach a file using an upload session:</span></span>

1. <span data-ttu-id="029ed-112">创建上传会话</span><span class="sxs-lookup"><span data-stu-id="029ed-112">Create an upload session</span></span>
2. <span data-ttu-id="029ed-113">在该上传会话中，以迭代方式上载字节范围（每次最长 4 MB），直到上载了文件的所有字节，并将文件附加到指定的邮件</span><span class="sxs-lookup"><span data-stu-id="029ed-113">Within that upload session, iteratively upload ranges of bytes (up to 4 MB each time) until all the bytes of the file have been uploaded, and the file is attached to the specified message</span></span>
3. <span data-ttu-id="029ed-114">保存附件的 ID 以供将来访问</span><span class="sxs-lookup"><span data-stu-id="029ed-114">Save the ID for the attachment for future access</span></span>
4. <span data-ttu-id="029ed-115">可选：删除上传会话</span><span class="sxs-lookup"><span data-stu-id="029ed-115">Optional: Delete the upload session</span></span> 

<span data-ttu-id="029ed-116">有关示例，请参阅[将大型文件附加到 Outlook 邮件](/graph/outlook-large-attachments)。</span><span class="sxs-lookup"><span data-stu-id="029ed-116">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

> [!TIP]
> <span data-ttu-id="029ed-117">Exchange Online 允许管理员自定义 Office 365 邮箱的邮件大小限制，包括任何邮件附件。</span><span class="sxs-lookup"><span data-stu-id="029ed-117">Exchange Online lets administrators customize the message size limit for Office 365 mailboxes,  including any message attachments.</span></span> <span data-ttu-id="029ed-118">默认情况下，此邮件大小限制为 35 MB。</span><span class="sxs-lookup"><span data-stu-id="029ed-118">By default, this message size limit is 35 MB.</span></span> <span data-ttu-id="029ed-119">了解如何[自定义最大邮件大小](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb)，以支持大于租户默认限制的附件。</span><span class="sxs-lookup"><span data-stu-id="029ed-119">Find out how to [customize the maximum message size](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) to support attachments larger than the default limit for your tenant.</span></span> 

> [!IMPORTANT] 
> <span data-ttu-id="029ed-120">如果要附加到共享或委派邮箱中的邮件，请注意[已知问题](/graph/known-issues#attaching-large-files-to-messages)。</span><span class="sxs-lookup"><span data-stu-id="029ed-120">Be aware of a [known issue](/graph/known-issues#attaching-large-files-to-messages) if you're attaching to a message in a shared or delegated mailbox.</span></span>


## <a name="permissions"></a><span data-ttu-id="029ed-121">权限</span><span class="sxs-lookup"><span data-stu-id="029ed-121">Permissions</span></span>

<span data-ttu-id="029ed-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="029ed-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="029ed-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="029ed-124">Permission type</span></span>                        | <span data-ttu-id="029ed-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="029ed-125">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="029ed-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="029ed-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="029ed-127">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="029ed-127">Mail.ReadWrite</span></span> |
| <span data-ttu-id="029ed-128">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="029ed-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="029ed-129">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="029ed-129">Mail.ReadWrite</span></span> |
| <span data-ttu-id="029ed-130">应用程序</span><span class="sxs-lookup"><span data-stu-id="029ed-130">Application</span></span>                            | <span data-ttu-id="029ed-131">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="029ed-131">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="029ed-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="029ed-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="029ed-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="029ed-133">Request headers</span></span>

| <span data-ttu-id="029ed-134">名称</span><span class="sxs-lookup"><span data-stu-id="029ed-134">Name</span></span>          | <span data-ttu-id="029ed-135">说明</span><span class="sxs-lookup"><span data-stu-id="029ed-135">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="029ed-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="029ed-136">Authorization</span></span> | <span data-ttu-id="029ed-137">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="029ed-137">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="029ed-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="029ed-138">Request body</span></span>

<span data-ttu-id="029ed-139">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="029ed-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="029ed-140">参数</span><span class="sxs-lookup"><span data-stu-id="029ed-140">Parameter</span></span>    | <span data-ttu-id="029ed-141">类型</span><span class="sxs-lookup"><span data-stu-id="029ed-141">Type</span></span>        | <span data-ttu-id="029ed-142">说明</span><span class="sxs-lookup"><span data-stu-id="029ed-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="029ed-143">AttachmentItem</span><span class="sxs-lookup"><span data-stu-id="029ed-143">AttachmentItem</span></span>|[<span data-ttu-id="029ed-144">attachmentItem</span><span class="sxs-lookup"><span data-stu-id="029ed-144">attachmentItem</span></span>](../resources/attachmentitem.md)|<span data-ttu-id="029ed-145">表示要上载和附加的项的属性。</span><span class="sxs-lookup"><span data-stu-id="029ed-145">Represents attributes of the item to be uploaded and attached.</span></span> <span data-ttu-id="029ed-146">至少指定附件类型（`file`）、名称和文件大小。</span><span class="sxs-lookup"><span data-stu-id="029ed-146">At minimum, specify the attachment type (`file`), a name, and the size of the file.</span></span>|

## <a name="response"></a><span data-ttu-id="029ed-147">响应</span><span class="sxs-lookup"><span data-stu-id="029ed-147">Response</span></span>

<span data-ttu-id="029ed-148">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[uploadSession](../resources/uploadsession.md)对象。</span><span class="sxs-lookup"><span data-stu-id="029ed-148">If successful, this method returns a `201 Created` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="029ed-149">**注意**：</span><span class="sxs-lookup"><span data-stu-id="029ed-149">**Note**:</span></span> 
>
><span data-ttu-id="029ed-150">作为**uploadSession** response 对象的一部分返回的**uploadUrl**属性是一个不透明的 URL， `PUT`用于随后的查询上传文件的字节范围。</span><span class="sxs-lookup"><span data-stu-id="029ed-150">The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="029ed-151">它包含针对`PUT` **expirationDateTime**到期的后续查询的相应 auth 令牌。</span><span class="sxs-lookup"><span data-stu-id="029ed-151">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="029ed-152">请勿自定义此 URL。</span><span class="sxs-lookup"><span data-stu-id="029ed-152">Do not customize this URL.</span></span>
>
><span data-ttu-id="029ed-153">**NextExpectedRanges**属性指定要从中上载的下一个文件字节位置，例如`"NextExpectedRanges":["2097152"]`。</span><span class="sxs-lookup"><span data-stu-id="029ed-153">The **nextExpectedRanges** property specifies the next file byte location to upload from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="029ed-154">必须按顺序上传文件中的字节。</span><span class="sxs-lookup"><span data-stu-id="029ed-154">You must upload bytes in a file in order.</span></span>

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a><span data-ttu-id="029ed-155">示例</span><span class="sxs-lookup"><span data-stu-id="029ed-155">Examples</span></span>

<span data-ttu-id="029ed-156">下面的示例演示如何创建可在后续文件上载操作中使用的上载会话。</span><span class="sxs-lookup"><span data-stu-id="029ed-156">The following example shows how to create an upload session that you can use in subsequent file upload operations.</span></span>

### <a name="request"></a><span data-ttu-id="029ed-157">请求</span><span class="sxs-lookup"><span data-stu-id="029ed-157">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="029ed-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="029ed-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession",
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
# <a name="c"></a>[<span data-ttu-id="029ed-159">C#</span><span class="sxs-lookup"><span data-stu-id="029ed-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="029ed-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="029ed-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="029ed-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="029ed-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="029ed-162">响应</span><span class="sxs-lookup"><span data-stu-id="029ed-162">Response</span></span>

> <span data-ttu-id="029ed-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="029ed-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0uAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
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
