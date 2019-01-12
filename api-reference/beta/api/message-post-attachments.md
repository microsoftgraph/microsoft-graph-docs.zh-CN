---
title: Add attachment
description: '使用此 API 可将附件添加到邮件中。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fc24c0a444c07dc8fb8e33814498fe5454b1b3fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991900"
---
# <a name="add-attachment"></a><span data-ttu-id="bcdc5-103">Add attachment</span><span class="sxs-lookup"><span data-stu-id="bcdc5-103">Add attachment</span></span>

> <span data-ttu-id="bcdc5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bcdc5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bcdc5-106">使用此 API 可将[附件](../resources/attachment.md)添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-106">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="bcdc5-107">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="bcdc5-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="bcdc5-108">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="bcdc5-109">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="bcdc5-110">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="bcdc5-111">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="bcdc5-112">您可以通过其 attachments 集合，向其投递添加到现有邮件附件或到新邮件的正在[绘制](../api/user-post-messages.md)，或[创建和发送即时](../api/user-sendmail.md)。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-112">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="bcdc5-113">由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-113">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="bcdc5-114">权限</span><span class="sxs-lookup"><span data-stu-id="bcdc5-114">Permissions</span></span>
<span data-ttu-id="bcdc5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcdc5-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="bcdc5-117">Permission type</span></span>      | <span data-ttu-id="bcdc5-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bcdc5-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcdc5-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bcdc5-119">Delegated (work or school account)</span></span> | <span data-ttu-id="bcdc5-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcdc5-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bcdc5-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bcdc5-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcdc5-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcdc5-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bcdc5-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="bcdc5-123">Application</span></span> | <span data-ttu-id="bcdc5-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcdc5-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcdc5-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bcdc5-125">HTTP request</span></span>
<span data-ttu-id="bcdc5-126"><!-- { "blockType": "ignored" } -->[邮件](../resources/message.md)用户的邮箱中的附件。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-126"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="bcdc5-127">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-127">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="bcdc5-p103">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bcdc5-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="bcdc5-130">Request headers</span></span>
| <span data-ttu-id="bcdc5-131">名称</span><span class="sxs-lookup"><span data-stu-id="bcdc5-131">Name</span></span>       | <span data-ttu-id="bcdc5-132">类型</span><span class="sxs-lookup"><span data-stu-id="bcdc5-132">Type</span></span> | <span data-ttu-id="bcdc5-133">说明</span><span class="sxs-lookup"><span data-stu-id="bcdc5-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bcdc5-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcdc5-134">Authorization</span></span>  | <span data-ttu-id="bcdc5-135">string</span><span class="sxs-lookup"><span data-stu-id="bcdc5-135">string</span></span>  | <span data-ttu-id="bcdc5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bcdc5-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bcdc5-138">Content-Type</span></span> | <span data-ttu-id="bcdc5-139">string</span><span class="sxs-lookup"><span data-stu-id="bcdc5-139">string</span></span>  | <span data-ttu-id="bcdc5-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcdc5-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="bcdc5-142">Request body</span></span>
<span data-ttu-id="bcdc5-143">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-143">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bcdc5-144">响应</span><span class="sxs-lookup"><span data-stu-id="bcdc5-144">Response</span></span>

<span data-ttu-id="bcdc5-145">如果成功，此方法返回`201 Created`响应代码和响应正文中的[Attachment](../resources/attachment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-145">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="bcdc5-146">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="bcdc5-146">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="bcdc5-147">请求</span><span class="sxs-lookup"><span data-stu-id="bcdc5-147">Request</span></span>
<span data-ttu-id="bcdc5-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "R0lGODdhEAYEAA7"
}
```

<span data-ttu-id="bcdc5-149">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-149">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bcdc5-150">响应</span><span class="sxs-lookup"><span data-stu-id="bcdc5-150">Response</span></span>
<span data-ttu-id="bcdc5-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
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
    "contentBytes": "R0lGODdhEAYEAA7"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="bcdc5-152">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="bcdc5-152">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="bcdc5-153">请求</span><span class="sxs-lookup"><span data-stu-id="bcdc5-153">Request</span></span>
<span data-ttu-id="bcdc5-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_message"
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

##### <a name="response"></a><span data-ttu-id="bcdc5-155">响应</span><span class="sxs-lookup"><span data-stu-id="bcdc5-155">Response</span></span>
<span data-ttu-id="bcdc5-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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

## <a name="example-reference-attachment"></a><span data-ttu-id="bcdc5-159">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="bcdc5-159">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="bcdc5-160">请求</span><span class="sxs-lookup"><span data-stu-id="bcdc5-160">Request</span></span>
<span data-ttu-id="bcdc5-161">下面是请求的添加到现有邮件引用附件的示例。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-161">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="bcdc5-162">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-162">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="bcdc5-163">响应</span><span class="sxs-lookup"><span data-stu-id="bcdc5-163">Response</span></span>
<span data-ttu-id="bcdc5-164">下面是响应的完整的一个示例。</span><span class="sxs-lookup"><span data-stu-id="bcdc5-164">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
