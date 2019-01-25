---
title: Add attachment
description: '使用此 API 可将附件添加到邮件中。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 56693a04d6f0579d043b4d745fe53ae61536b82e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510090"
---
# <a name="add-attachment"></a><span data-ttu-id="8b10e-103">Add attachment</span><span class="sxs-lookup"><span data-stu-id="8b10e-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b10e-104">使用此 API 可将[附件](../resources/attachment.md)添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="8b10e-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="8b10e-105">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="8b10e-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="8b10e-106">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="8b10e-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="8b10e-107">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="8b10e-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="8b10e-108">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="8b10e-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="8b10e-109">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="8b10e-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="8b10e-110">您可以通过其 attachments 集合，向其投递添加到现有邮件附件或到新邮件的正在[绘制](../api/user-post-messages.md)，或[创建和发送即时](../api/user-sendmail.md)。</span><span class="sxs-lookup"><span data-stu-id="8b10e-110">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="8b10e-111">由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="8b10e-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b10e-112">权限</span><span class="sxs-lookup"><span data-stu-id="8b10e-112">Permissions</span></span>
<span data-ttu-id="8b10e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b10e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b10e-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b10e-115">Permission type</span></span>      | <span data-ttu-id="8b10e-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b10e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b10e-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b10e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8b10e-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b10e-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8b10e-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b10e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b10e-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b10e-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8b10e-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b10e-121">Application</span></span> | <span data-ttu-id="8b10e-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b10e-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b10e-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b10e-123">HTTP request</span></span>
<span data-ttu-id="8b10e-124"><!-- { "blockType": "ignored" } -->[邮件](../resources/message.md)用户的邮箱中的附件。</span><span class="sxs-lookup"><span data-stu-id="8b10e-124"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="8b10e-125">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="8b10e-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="8b10e-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="8b10e-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8b10e-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b10e-128">Request headers</span></span>
| <span data-ttu-id="8b10e-129">名称</span><span class="sxs-lookup"><span data-stu-id="8b10e-129">Name</span></span>       | <span data-ttu-id="8b10e-130">类型</span><span class="sxs-lookup"><span data-stu-id="8b10e-130">Type</span></span> | <span data-ttu-id="8b10e-131">说明</span><span class="sxs-lookup"><span data-stu-id="8b10e-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8b10e-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b10e-132">Authorization</span></span>  | <span data-ttu-id="8b10e-133">string</span><span class="sxs-lookup"><span data-stu-id="8b10e-133">string</span></span>  | <span data-ttu-id="8b10e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b10e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b10e-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b10e-136">Content-Type</span></span> | <span data-ttu-id="8b10e-137">string</span><span class="sxs-lookup"><span data-stu-id="8b10e-137">string</span></span>  | <span data-ttu-id="8b10e-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="8b10e-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b10e-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b10e-140">Request body</span></span>
<span data-ttu-id="8b10e-141">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b10e-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8b10e-142">响应</span><span class="sxs-lookup"><span data-stu-id="8b10e-142">Response</span></span>

<span data-ttu-id="8b10e-143">如果成功，此方法返回`201 Created`响应代码和响应正文中的[Attachment](../resources/attachment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8b10e-143">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="8b10e-144">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="8b10e-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="8b10e-145">请求</span><span class="sxs-lookup"><span data-stu-id="8b10e-145">Request</span></span>
<span data-ttu-id="8b10e-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8b10e-146">Here is an example of the request.</span></span>
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

<span data-ttu-id="8b10e-147">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b10e-147">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8b10e-148">响应</span><span class="sxs-lookup"><span data-stu-id="8b10e-148">Response</span></span>
<span data-ttu-id="8b10e-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8b10e-149">Here is an example of the response.</span></span> 
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

## <a name="example-item-attachment"></a><span data-ttu-id="8b10e-150">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="8b10e-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="8b10e-151">请求</span><span class="sxs-lookup"><span data-stu-id="8b10e-151">Request</span></span>
<span data-ttu-id="8b10e-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8b10e-152">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8b10e-153">响应</span><span class="sxs-lookup"><span data-stu-id="8b10e-153">Response</span></span>
<span data-ttu-id="8b10e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8b10e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="8b10e-157">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="8b10e-157">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="8b10e-158">请求</span><span class="sxs-lookup"><span data-stu-id="8b10e-158">Request</span></span>
<span data-ttu-id="8b10e-159">下面是请求的添加到现有邮件引用附件的示例。</span><span class="sxs-lookup"><span data-stu-id="8b10e-159">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="8b10e-160">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="8b10e-160">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8b10e-161">响应</span><span class="sxs-lookup"><span data-stu-id="8b10e-161">Response</span></span>
<span data-ttu-id="8b10e-162">下面是响应的完整的一个示例。</span><span class="sxs-lookup"><span data-stu-id="8b10e-162">Here is an example of a full response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
