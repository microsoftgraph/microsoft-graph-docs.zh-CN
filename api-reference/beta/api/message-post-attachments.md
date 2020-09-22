---
title: Add attachment
description: '使用此 API 可将附件添加到邮件中。 '
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 00eb01bf7ddc25c649cd5a36a0403984152fd7fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076909"
---
# <a name="add-attachment"></a><span data-ttu-id="eee58-103">添加附件</span><span class="sxs-lookup"><span data-stu-id="eee58-103">Add attachment</span></span>

<span data-ttu-id="eee58-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eee58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eee58-105">使用此 API 可将[附件](../resources/attachment.md)添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="eee58-105">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="eee58-106">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="eee58-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="eee58-107">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="eee58-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="eee58-108">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="eee58-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="eee58-109">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="eee58-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="eee58-110">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="eee58-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="eee58-111">您可以通过发布到现有 [邮件](../resources/message.md) 的附件集合，或在正在 [起草](../api/user-post-messages.md)的新邮件中添加附件，或 [在即时创建和发送](../api/user-sendmail.md)附件。</span><span class="sxs-lookup"><span data-stu-id="eee58-111">You can add an attachment to an existing [message](../resources/message.md) by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

><span data-ttu-id="eee58-112">**注意**：此操作限制了可以添加到 3 MB 以下的附件的大小。</span><span class="sxs-lookup"><span data-stu-id="eee58-112">**Note**: This operation limits the size of the attachment you can add to under 3 MB.</span></span>
>
> <span data-ttu-id="eee58-113">但是，如果您要附加到邮件的文件介于3MB 和150MB 之间，则可以 [创建上载会话](attachment-createuploadsession.md) 并以迭代方式上载要附加的文件的范围。</span><span class="sxs-lookup"><span data-stu-id="eee58-113">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="eee58-114">有关示例，请参阅 [将大型文件附加到 Outlook 邮件](/graph/outlook-large-attachments) 。</span><span class="sxs-lookup"><span data-stu-id="eee58-114">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>
## <a name="permissions"></a><span data-ttu-id="eee58-115">权限</span><span class="sxs-lookup"><span data-stu-id="eee58-115">Permissions</span></span>
<span data-ttu-id="eee58-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eee58-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eee58-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="eee58-118">Permission type</span></span>      | <span data-ttu-id="eee58-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eee58-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eee58-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eee58-120">Delegated (work or school account)</span></span> | <span data-ttu-id="eee58-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eee58-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eee58-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eee58-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eee58-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eee58-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eee58-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="eee58-124">Application</span></span> | <span data-ttu-id="eee58-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eee58-125">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eee58-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eee58-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="eee58-127">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="eee58-127">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="eee58-128">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="eee58-128">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="eee58-p103">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。 </span><span class="sxs-lookup"><span data-stu-id="eee58-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eee58-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="eee58-131">Request headers</span></span>
| <span data-ttu-id="eee58-132">名称</span><span class="sxs-lookup"><span data-stu-id="eee58-132">Name</span></span>       | <span data-ttu-id="eee58-133">类型</span><span class="sxs-lookup"><span data-stu-id="eee58-133">Type</span></span> | <span data-ttu-id="eee58-134">说明</span><span class="sxs-lookup"><span data-stu-id="eee58-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eee58-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="eee58-135">Authorization</span></span>  | <span data-ttu-id="eee58-136">string</span><span class="sxs-lookup"><span data-stu-id="eee58-136">string</span></span>  | <span data-ttu-id="eee58-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eee58-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eee58-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eee58-139">Content-Type</span></span> | <span data-ttu-id="eee58-140">string</span><span class="sxs-lookup"><span data-stu-id="eee58-140">string</span></span>  | <span data-ttu-id="eee58-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="eee58-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eee58-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="eee58-143">Request body</span></span>
<span data-ttu-id="eee58-144">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eee58-144">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eee58-145">响应</span><span class="sxs-lookup"><span data-stu-id="eee58-145">Response</span></span>

<span data-ttu-id="eee58-146">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [附件](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eee58-146">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="eee58-147">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="eee58-147">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="eee58-148">请求</span><span class="sxs-lookup"><span data-stu-id="eee58-148">Request</span></span>
<span data-ttu-id="eee58-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eee58-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eee58-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="eee58-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eee58-151">C#</span><span class="sxs-lookup"><span data-stu-id="eee58-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eee58-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eee58-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eee58-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eee58-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="eee58-154">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eee58-154">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="eee58-155">响应</span><span class="sxs-lookup"><span data-stu-id="eee58-155">Response</span></span>
<span data-ttu-id="eee58-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eee58-156">Here is an example of the response.</span></span> 
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

## <a name="example-item-attachment"></a><span data-ttu-id="eee58-157">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="eee58-157">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="eee58-158">请求</span><span class="sxs-lookup"><span data-stu-id="eee58-158">Request</span></span>
<span data-ttu-id="eee58-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eee58-159">Here is an example of the request.</span></span>

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


##### <a name="response"></a><span data-ttu-id="eee58-160">响应</span><span class="sxs-lookup"><span data-stu-id="eee58-160">Response</span></span>
<span data-ttu-id="eee58-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eee58-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="eee58-164">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="eee58-164">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="eee58-165">请求</span><span class="sxs-lookup"><span data-stu-id="eee58-165">Request</span></span>
<span data-ttu-id="eee58-166">下面的示例展示了向现有邮件添加引用附件的请求。</span><span class="sxs-lookup"><span data-stu-id="eee58-166">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="eee58-167">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="eee58-167">The attachment points to a folder on OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="eee58-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="eee58-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eee58-169">C#</span><span class="sxs-lookup"><span data-stu-id="eee58-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eee58-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eee58-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eee58-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eee58-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eee58-172">响应</span><span class="sxs-lookup"><span data-stu-id="eee58-172">Response</span></span>
<span data-ttu-id="eee58-173">下面的示例展示了完整的响应。</span><span class="sxs-lookup"><span data-stu-id="eee58-173">Here is an example of a full response.</span></span>
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


