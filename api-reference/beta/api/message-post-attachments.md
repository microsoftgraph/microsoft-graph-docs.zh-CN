---
title: Add attachment
description: '使用此 API 可将附件添加到邮件中。 '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 61776660883cdcf9ea8d6122e2e84c5b63505935
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131171"
---
# <a name="add-attachment"></a><span data-ttu-id="39cf9-103">添加附件</span><span class="sxs-lookup"><span data-stu-id="39cf9-103">Add attachment</span></span>

<span data-ttu-id="39cf9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39cf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39cf9-105">使用此 API 可将[附件](../resources/attachment.md)添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="39cf9-105">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="39cf9-106">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="39cf9-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="39cf9-107">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="39cf9-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="39cf9-108">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="39cf9-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="39cf9-109">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="39cf9-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="39cf9-110">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="39cf9-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="39cf9-111">可以通过发布到现有邮件的附件集合或[](../resources/message.md)正在草稿、创建和发送的新邮件添加[附件](../api/user-sendmail.md)。 [](../api/user-post-messages.md)</span><span class="sxs-lookup"><span data-stu-id="39cf9-111">You can add an attachment to an existing [message](../resources/message.md) by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

><span data-ttu-id="39cf9-112">**注意**：此操作将可添加到的附件大小限制在 3 MB 以下。</span><span class="sxs-lookup"><span data-stu-id="39cf9-112">**Note**: This operation limits the size of the attachment you can add to under 3 MB.</span></span>
>
> <span data-ttu-id="39cf9-113">但是，如果要将介于 3MB 到 150MB 之间的文件附加到邮件，可以创建上载会话并反复[](attachment-createuploadsession.md)上载文件范围以附加它。</span><span class="sxs-lookup"><span data-stu-id="39cf9-113">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="39cf9-114">有关 [示例，请参阅将大文件附加到 Outlook](/graph/outlook-large-attachments) 邮件。</span><span class="sxs-lookup"><span data-stu-id="39cf9-114">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>
## <a name="permissions"></a><span data-ttu-id="39cf9-115">权限</span><span class="sxs-lookup"><span data-stu-id="39cf9-115">Permissions</span></span>
<span data-ttu-id="39cf9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39cf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39cf9-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="39cf9-118">Permission type</span></span>      | <span data-ttu-id="39cf9-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39cf9-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39cf9-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39cf9-120">Delegated (work or school account)</span></span> | <span data-ttu-id="39cf9-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39cf9-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="39cf9-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39cf9-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39cf9-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39cf9-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="39cf9-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="39cf9-124">Application</span></span> | <span data-ttu-id="39cf9-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39cf9-125">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="39cf9-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39cf9-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="39cf9-127">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="39cf9-127">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="39cf9-128">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="39cf9-128">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="39cf9-p103">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。 </span><span class="sxs-lookup"><span data-stu-id="39cf9-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="39cf9-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="39cf9-131">Request headers</span></span>
| <span data-ttu-id="39cf9-132">名称</span><span class="sxs-lookup"><span data-stu-id="39cf9-132">Name</span></span>       | <span data-ttu-id="39cf9-133">类型</span><span class="sxs-lookup"><span data-stu-id="39cf9-133">Type</span></span> | <span data-ttu-id="39cf9-134">说明</span><span class="sxs-lookup"><span data-stu-id="39cf9-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="39cf9-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="39cf9-135">Authorization</span></span>  | <span data-ttu-id="39cf9-136">string</span><span class="sxs-lookup"><span data-stu-id="39cf9-136">string</span></span>  | <span data-ttu-id="39cf9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39cf9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39cf9-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39cf9-139">Content-Type</span></span> | <span data-ttu-id="39cf9-140">string</span><span class="sxs-lookup"><span data-stu-id="39cf9-140">string</span></span>  | <span data-ttu-id="39cf9-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="39cf9-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39cf9-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="39cf9-143">Request body</span></span>
<span data-ttu-id="39cf9-144">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39cf9-144">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="39cf9-145">响应</span><span class="sxs-lookup"><span data-stu-id="39cf9-145">Response</span></span>

<span data-ttu-id="39cf9-146">如果成功，此方法在 `201 Created` 响应正文中返回响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39cf9-146">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="39cf9-147">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="39cf9-147">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="39cf9-148">请求</span><span class="sxs-lookup"><span data-stu-id="39cf9-148">Request</span></span>
<span data-ttu-id="39cf9-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39cf9-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39cf9-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="39cf9-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_message_beta"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "a0b1c76de9f7="
}
```
# <a name="c"></a>[<span data-ttu-id="39cf9-151">C#</span><span class="sxs-lookup"><span data-stu-id="39cf9-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39cf9-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39cf9-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39cf9-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39cf9-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39cf9-154">Java</span><span class="sxs-lookup"><span data-stu-id="39cf9-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-message-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="39cf9-155">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39cf9-155">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="39cf9-156">响应</span><span class="sxs-lookup"><span data-stu-id="39cf9-156">Response</span></span>
<span data-ttu-id="39cf9-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="39cf9-157">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_message_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 202

{
    "id": "AAMkADNkN2R",
    "lastModifiedDateTime": "2017-01-26T08:48:28Z",
    "name": "smile",
    "contentType": "image/gif",
    "size": 1008,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "a0b1c76de9f7="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="39cf9-158">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="39cf9-158">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="39cf9-159">请求</span><span class="sxs-lookup"><span data-stu-id="39cf9-159">Request</span></span>
<span data-ttu-id="39cf9-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39cf9-160">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_message_beta"
}-->

```
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event", 
  "item": {
    "@odata.type": "microsoft.graph.event",
    "subject": "Discuss gifts for children",
    "body": {
      "contentType": "HTML",
      "content": "Let's look for funding!"
    },
    "start": {
      "dateTime": "2016-12-02T18:00:00",
      "timeZone": "Pacific Standard Time"
    },
    "end": {
      "dateTime": "2016-12-02T19:00:00",
      "timeZone": "Pacific Standard Time"
    }
  }
}

```


##### <a name="response"></a><span data-ttu-id="39cf9-161">响应</span><span class="sxs-lookup"><span data-stu-id="39cf9-161">Response</span></span>
<span data-ttu-id="39cf9-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="39cf9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_message_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "id":"AAMkADNkNJp5JVnQIe9r0=",
  "lastModifiedDateTime":"2016-12-01T22:27:13Z",
  "name":"Holiday event",
  "contentType":null,
  "size":2473,
  "isInline":false
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="39cf9-165">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="39cf9-165">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="39cf9-166">请求</span><span class="sxs-lookup"><span data-stu-id="39cf9-166">Request</span></span>
<span data-ttu-id="39cf9-167">下面是向现有邮件添加引用附件的请求示例。</span><span class="sxs-lookup"><span data-stu-id="39cf9-167">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="39cf9-168">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="39cf9-168">The attachment points to a folder on OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="39cf9-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="39cf9-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_message",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/me/messages/AAMkAGE1M88AADUv0uFAAA=/attachments
Content-type: application/json
Content-length: 319

{ 
    "@odata.type": "#microsoft.graph.referenceAttachment", 
    "name": "Personal pictures", 
    "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
    "providerType": "oneDriveConsumer", 
    "permission": "Edit", 
    "isFolder": "True" 
} 
```
# <a name="c"></a>[<span data-ttu-id="39cf9-170">C#</span><span class="sxs-lookup"><span data-stu-id="39cf9-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39cf9-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39cf9-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39cf9-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39cf9-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39cf9-173">Java</span><span class="sxs-lookup"><span data-stu-id="39cf9-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-reference-attachment-from-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="39cf9-174">响应</span><span class="sxs-lookup"><span data-stu-id="39cf9-174">Response</span></span>
<span data-ttu-id="39cf9-175">下面是完整响应的示例。</span><span class="sxs-lookup"><span data-stu-id="39cf9-175">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_reference_attachment_from_message",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/messages/AAMkAGE1M88AADUv0uFAAA%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PICVGCc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->


