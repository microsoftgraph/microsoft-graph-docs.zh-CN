---
title: Add attachment
description: '使用此 API 可将附件添加到邮件中。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3be39ef1160b2947c3f2efb2b1a5f926143aae23
ms.sourcegitcommit: 36066afdced00f32838a03747d3e7760fc43683a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36453146"
---
# <a name="add-attachment"></a><span data-ttu-id="6fc45-103">Add attachment</span><span class="sxs-lookup"><span data-stu-id="6fc45-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fc45-104">使用此 API 可将[附件](../resources/attachment.md)添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="6fc45-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="6fc45-105">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="6fc45-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="6fc45-106">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="6fc45-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="6fc45-107">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="6fc45-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="6fc45-108">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="6fc45-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="6fc45-109">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="6fc45-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="6fc45-110">您可以通过发布到现有邮件的附件集合, 或在正在[起草](../api/user-post-messages.md)的新邮件中添加附件, 或[在即时创建和发送](../api/user-sendmail.md)附件。</span><span class="sxs-lookup"><span data-stu-id="6fc45-110">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="6fc45-111">由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="6fc45-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="6fc45-112">权限</span><span class="sxs-lookup"><span data-stu-id="6fc45-112">Permissions</span></span>
<span data-ttu-id="6fc45-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fc45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fc45-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fc45-115">Permission type</span></span>      | <span data-ttu-id="6fc45-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fc45-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fc45-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fc45-117">Delegated (work or school account)</span></span> | <span data-ttu-id="6fc45-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fc45-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6fc45-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fc45-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fc45-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fc45-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6fc45-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fc45-121">Application</span></span> | <span data-ttu-id="6fc45-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fc45-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fc45-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fc45-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="6fc45-124">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="6fc45-124">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="6fc45-125">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="6fc45-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="6fc45-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="6fc45-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6fc45-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fc45-128">Request headers</span></span>
| <span data-ttu-id="6fc45-129">名称</span><span class="sxs-lookup"><span data-stu-id="6fc45-129">Name</span></span>       | <span data-ttu-id="6fc45-130">类型</span><span class="sxs-lookup"><span data-stu-id="6fc45-130">Type</span></span> | <span data-ttu-id="6fc45-131">说明</span><span class="sxs-lookup"><span data-stu-id="6fc45-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6fc45-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fc45-132">Authorization</span></span>  | <span data-ttu-id="6fc45-133">string</span><span class="sxs-lookup"><span data-stu-id="6fc45-133">string</span></span>  | <span data-ttu-id="6fc45-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fc45-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6fc45-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6fc45-136">Content-Type</span></span> | <span data-ttu-id="6fc45-137">string</span><span class="sxs-lookup"><span data-stu-id="6fc45-137">string</span></span>  | <span data-ttu-id="6fc45-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="6fc45-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fc45-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fc45-140">Request body</span></span>
<span data-ttu-id="6fc45-141">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fc45-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6fc45-142">响应</span><span class="sxs-lookup"><span data-stu-id="6fc45-142">Response</span></span>

<span data-ttu-id="6fc45-143">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[附件](../resources/attachment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6fc45-143">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="6fc45-144">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="6fc45-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="6fc45-145">请求</span><span class="sxs-lookup"><span data-stu-id="6fc45-145">Request</span></span>
<span data-ttu-id="6fc45-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fc45-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6fc45-147">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6fc45-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6fc45-148">C#</span><span class="sxs-lookup"><span data-stu-id="6fc45-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fc45-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fc45-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6fc45-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="6fc45-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="6fc45-151">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fc45-151">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6fc45-152">响应</span><span class="sxs-lookup"><span data-stu-id="6fc45-152">Response</span></span>
<span data-ttu-id="6fc45-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6fc45-153">Here is an example of the response.</span></span> 
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

## <a name="example-item-attachment"></a><span data-ttu-id="6fc45-154">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="6fc45-154">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="6fc45-155">请求</span><span class="sxs-lookup"><span data-stu-id="6fc45-155">Request</span></span>
<span data-ttu-id="6fc45-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fc45-156">Here is an example of the request.</span></span>

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


##### <a name="response"></a><span data-ttu-id="6fc45-157">响应</span><span class="sxs-lookup"><span data-stu-id="6fc45-157">Response</span></span>
<span data-ttu-id="6fc45-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6fc45-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="6fc45-161">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="6fc45-161">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="6fc45-162">请求</span><span class="sxs-lookup"><span data-stu-id="6fc45-162">Request</span></span>
<span data-ttu-id="6fc45-163">下面的示例展示了向现有邮件添加引用附件的请求。</span><span class="sxs-lookup"><span data-stu-id="6fc45-163">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="6fc45-164">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="6fc45-164">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6fc45-165">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6fc45-165">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6fc45-166">C#</span><span class="sxs-lookup"><span data-stu-id="6fc45-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fc45-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fc45-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6fc45-168">目标-C</span><span class="sxs-lookup"><span data-stu-id="6fc45-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6fc45-169">响应</span><span class="sxs-lookup"><span data-stu-id="6fc45-169">Response</span></span>
<span data-ttu-id="6fc45-170">下面的示例展示了完整的响应。</span><span class="sxs-lookup"><span data-stu-id="6fc45-170">Here is an example of a full response.</span></span>
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
