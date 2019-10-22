---
title: 附件： createUploadSession
description: 创建上载会话以以迭代方式上载文件的范围，以便将文件附加到指定的邮件。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 116b73b53689c01e346568b6b5d67e56fb31b283
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621603"
---
# <a name="attachment-createuploadsession"></a><span data-ttu-id="7f005-103">附件： createUploadSession</span><span class="sxs-lookup"><span data-stu-id="7f005-103">attachment: createUploadSession</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f005-104">创建一个允许应用程序以迭代方式上载文件范围的上载会话，以便将文件附加到指定的[邮件](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="7f005-104">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified [message](../resources/message.md).</span></span>

<span data-ttu-id="7f005-105">使用此方法可以将3MB 和150MB 之间的大小的文件附加到**邮件**。</span><span class="sxs-lookup"><span data-stu-id="7f005-105">Use this approach to attach files of sizes between 3MB and 150MB to a **message**.</span></span> <span data-ttu-id="7f005-106">若要在4MB 下附加大小的文件，只需[在 "附件" 导航属性上进行发布](message-post-attachments.md)即可。</span><span class="sxs-lookup"><span data-stu-id="7f005-106">To attach files of sizes under 4MB, simply [POST on the attachments navigation property](message-post-attachments.md).</span></span> 

<span data-ttu-id="7f005-107">作为响应的一部分，此操作将返回可在后续顺序`PUT`查询中使用的上载 URL。</span><span class="sxs-lookup"><span data-stu-id="7f005-107">As part of the response, this action returns an upload URL that you can use in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="7f005-108">每个`PUT`操作的请求标头允许您指定要上载的确切字节范围。</span><span class="sxs-lookup"><span data-stu-id="7f005-108">Request headers for each `PUT` operation let you specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="7f005-109">这样，如果在上载过程中断开网络连接，则可以恢复传输。</span><span class="sxs-lookup"><span data-stu-id="7f005-109">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

<span data-ttu-id="7f005-110">以下是使用上传会话附加文件的步骤：</span><span class="sxs-lookup"><span data-stu-id="7f005-110">The following are the steps to attach a file using an upload session:</span></span>

1. <span data-ttu-id="7f005-111">创建上传会话</span><span class="sxs-lookup"><span data-stu-id="7f005-111">Create an upload session</span></span>
2. <span data-ttu-id="7f005-112">在该上传会话中，以迭代方式上载字节范围（每次最长 4 MB），直到上载了文件的所有字节，并将文件附加到指定的邮件</span><span class="sxs-lookup"><span data-stu-id="7f005-112">Within that upload session, iteratively upload ranges of bytes (up to 4 MB each time) until all the bytes of the file have been uploaded, and the file is attached to the specified message</span></span>
3. <span data-ttu-id="7f005-113">保存附件的 ID 以供将来访问</span><span class="sxs-lookup"><span data-stu-id="7f005-113">Save the ID for the attachment for future access</span></span>
4. <span data-ttu-id="7f005-114">可选：删除上传会话</span><span class="sxs-lookup"><span data-stu-id="7f005-114">Optional: Delete the upload session</span></span> 

<span data-ttu-id="7f005-115">有关示例，请参阅[将大型文件附加到 Outlook 邮件](/graph/outlook-large-attachments)。</span><span class="sxs-lookup"><span data-stu-id="7f005-115">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>


## <a name="permissions"></a><span data-ttu-id="7f005-116">权限</span><span class="sxs-lookup"><span data-stu-id="7f005-116">Permissions</span></span>

<span data-ttu-id="7f005-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f005-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f005-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f005-119">Permission type</span></span>                        | <span data-ttu-id="7f005-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f005-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7f005-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f005-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f005-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f005-122">Mail.ReadWrite</span></span> |
| <span data-ttu-id="7f005-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f005-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f005-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f005-124">Mail.ReadWrite</span></span> |
| <span data-ttu-id="7f005-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f005-125">Application</span></span>                            | <span data-ttu-id="7f005-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f005-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f005-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f005-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="7f005-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f005-128">Request headers</span></span>

| <span data-ttu-id="7f005-129">名称</span><span class="sxs-lookup"><span data-stu-id="7f005-129">Name</span></span>          | <span data-ttu-id="7f005-130">说明</span><span class="sxs-lookup"><span data-stu-id="7f005-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7f005-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f005-131">Authorization</span></span> | <span data-ttu-id="7f005-132">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7f005-132">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="7f005-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f005-133">Request body</span></span>

<span data-ttu-id="7f005-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7f005-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7f005-135">参数</span><span class="sxs-lookup"><span data-stu-id="7f005-135">Parameter</span></span>    | <span data-ttu-id="7f005-136">类型</span><span class="sxs-lookup"><span data-stu-id="7f005-136">Type</span></span>        | <span data-ttu-id="7f005-137">说明</span><span class="sxs-lookup"><span data-stu-id="7f005-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7f005-138">AttachmentItem</span><span class="sxs-lookup"><span data-stu-id="7f005-138">AttachmentItem</span></span>|[<span data-ttu-id="7f005-139">attachmentItem</span><span class="sxs-lookup"><span data-stu-id="7f005-139">attachmentItem</span></span>](../resources/attachmentitem.md)|<span data-ttu-id="7f005-140">表示要上载和附加的项的属性。</span><span class="sxs-lookup"><span data-stu-id="7f005-140">Represents attributes of the item to be uploaded and attached.</span></span> <span data-ttu-id="7f005-141">至少指定附件类型（`file`）、名称和文件大小。</span><span class="sxs-lookup"><span data-stu-id="7f005-141">At minimum, specify the attachment type (`file`), a name, and the size of the file.</span></span>|

## <a name="response"></a><span data-ttu-id="7f005-142">响应</span><span class="sxs-lookup"><span data-stu-id="7f005-142">Response</span></span>

<span data-ttu-id="7f005-143">如果成功，此方法在`201, Created`响应正文中返回响应代码和新的[uploadSession](../resources/uploadsession.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7f005-143">If successful, this method returns `201, Created` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="7f005-144">**注意**：</span><span class="sxs-lookup"><span data-stu-id="7f005-144">**Note**:</span></span> 
>
><span data-ttu-id="7f005-145">作为**uploadSession** response 对象的一部分返回的**uploadUrl**属性是一个不透明的 URL， `PUT`用于随后的查询上传文件的字节范围。</span><span class="sxs-lookup"><span data-stu-id="7f005-145">The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="7f005-146">它包含针对`PUT` **expirationDateTime**到期的后续查询的相应 auth 令牌。</span><span class="sxs-lookup"><span data-stu-id="7f005-146">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="7f005-147">请勿自定义此 URL。</span><span class="sxs-lookup"><span data-stu-id="7f005-147">Do not customize this URL.</span></span>
>
><span data-ttu-id="7f005-148">**NextExpectedRanges**属性指定要从中上载的下一个文件字节位置，例如`"NextExpectedRanges":["2097152"]`。</span><span class="sxs-lookup"><span data-stu-id="7f005-148">The **nextExpectedRanges** property specifies the next file byte location to upload from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="7f005-149">您必须按顺序将字节上载到文件中。</span><span class="sxs-lookup"><span data-stu-id="7f005-149">You must upload bytes in a file in order.</span></span>

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a><span data-ttu-id="7f005-150">示例</span><span class="sxs-lookup"><span data-stu-id="7f005-150">Examples</span></span>

<span data-ttu-id="7f005-151">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7f005-151">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="7f005-152">请求</span><span class="sxs-lookup"><span data-stu-id="7f005-152">Request</span></span>

<span data-ttu-id="7f005-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7f005-153">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f005-154">响应</span><span class="sxs-lookup"><span data-stu-id="7f005-154">Response</span></span>

<span data-ttu-id="7f005-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7f005-155">The following is an example of the response.</span></span>

> <span data-ttu-id="7f005-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7f005-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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