---
title: Add attachment
description: '使用此 API 可将附件添加到邮件中。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1b68777b98a3f956b0032318070531db2bf9c627
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276788"
---
# <a name="add-attachment"></a><span data-ttu-id="16b0a-103">Add attachment</span><span class="sxs-lookup"><span data-stu-id="16b0a-103">Add attachment</span></span>

<span data-ttu-id="16b0a-104">使用此 API 可将[附件](../resources/attachment.md)添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="16b0a-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="16b0a-105">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="16b0a-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="16b0a-106">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="16b0a-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="16b0a-107">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="16b0a-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="16b0a-108">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="16b0a-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="16b0a-109">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="16b0a-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="16b0a-110">通过发布到邮件附件集合，你可以把附件添加到现有邮件，也可以把附件添加到 [正在创建和发送的邮件](../api/user-sendmail.md)。</span><span class="sxs-lookup"><span data-stu-id="16b0a-110">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="16b0a-111">由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="16b0a-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="16b0a-112">权限</span><span class="sxs-lookup"><span data-stu-id="16b0a-112">Permissions</span></span>
<span data-ttu-id="16b0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16b0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16b0a-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="16b0a-115">Permission type</span></span>      | <span data-ttu-id="16b0a-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16b0a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16b0a-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16b0a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="16b0a-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16b0a-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="16b0a-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16b0a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16b0a-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16b0a-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="16b0a-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="16b0a-121">Application</span></span> | <span data-ttu-id="16b0a-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16b0a-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="16b0a-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16b0a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="16b0a-124">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="16b0a-124">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="16b0a-125">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="16b0a-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="16b0a-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="16b0a-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="16b0a-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="16b0a-128">Request headers</span></span>
| <span data-ttu-id="16b0a-129">名称</span><span class="sxs-lookup"><span data-stu-id="16b0a-129">Name</span></span>       | <span data-ttu-id="16b0a-130">类型</span><span class="sxs-lookup"><span data-stu-id="16b0a-130">Type</span></span> | <span data-ttu-id="16b0a-131">说明</span><span class="sxs-lookup"><span data-stu-id="16b0a-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16b0a-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="16b0a-132">Authorization</span></span>  | <span data-ttu-id="16b0a-133">string</span><span class="sxs-lookup"><span data-stu-id="16b0a-133">string</span></span>  | <span data-ttu-id="16b0a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16b0a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16b0a-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16b0a-136">Content-Type</span></span> | <span data-ttu-id="16b0a-137">string</span><span class="sxs-lookup"><span data-stu-id="16b0a-137">string</span></span>  | <span data-ttu-id="16b0a-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="16b0a-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16b0a-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="16b0a-140">Request body</span></span>
<span data-ttu-id="16b0a-141">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16b0a-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="16b0a-142">响应</span><span class="sxs-lookup"><span data-stu-id="16b0a-142">Response</span></span>

<span data-ttu-id="16b0a-143">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="16b0a-143">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="16b0a-144">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="16b0a-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="16b0a-145">请求</span><span class="sxs-lookup"><span data-stu-id="16b0a-145">Request</span></span>
<span data-ttu-id="16b0a-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16b0a-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "base64R0lGODdhEAYEAA7"
}
```

<span data-ttu-id="16b0a-147">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16b0a-147">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="16b0a-148">响应</span><span class="sxs-lookup"><span data-stu-id="16b0a-148">Response</span></span>
<span data-ttu-id="16b0a-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16b0a-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP 201 Created
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
    "contentBytes": "base64R0lGODdhEAYEAA7"
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="16b0a-150">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="16b0a-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="16b0a-151">C#</span><span class="sxs-lookup"><span data-stu-id="16b0a-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16b0a-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="16b0a-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="16b0a-153">目标-C</span><span class="sxs-lookup"><span data-stu-id="16b0a-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="16b0a-154">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="16b0a-154">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="16b0a-155">请求</span><span class="sxs-lookup"><span data-stu-id="16b0a-155">Request</span></span>
<span data-ttu-id="16b0a-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16b0a-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_item_attachment_from_message"
}-->

```
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
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

##### <a name="response"></a><span data-ttu-id="16b0a-157">响应</span><span class="sxs-lookup"><span data-stu-id="16b0a-157">Response</span></span>
<span data-ttu-id="16b0a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16b0a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
