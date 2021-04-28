---
title: Add attachment
description: '使用此 API 可将附件添加到邮件中。 '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0d282afb127dba1222f208d0660e6ff584c22834
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052234"
---
# <a name="add-attachment"></a><span data-ttu-id="e439c-103">添加附件</span><span class="sxs-lookup"><span data-stu-id="e439c-103">Add attachment</span></span>

<span data-ttu-id="e439c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e439c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e439c-105">使用此 API 可将[附件](../resources/attachment.md)添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="e439c-105">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="e439c-106">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="e439c-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="e439c-107">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="e439c-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="e439c-108">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="e439c-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="e439c-109">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="e439c-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="e439c-110">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="e439c-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="e439c-111">通过发布到邮件附件集合，你可以把附件添加到现有邮件，也可以把附件添加到 [正在创建和发送的邮件](../api/user-sendmail.md)。</span><span class="sxs-lookup"><span data-stu-id="e439c-111">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="e439c-112">此操作将可添加到的附件的大小限制在 3 MB 以下。</span><span class="sxs-lookup"><span data-stu-id="e439c-112">This operation limits the size of the attachment you can add to under 3 MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="e439c-113">权限</span><span class="sxs-lookup"><span data-stu-id="e439c-113">Permissions</span></span>
<span data-ttu-id="e439c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e439c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e439c-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="e439c-116">Permission type</span></span>      | <span data-ttu-id="e439c-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e439c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e439c-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e439c-118">Delegated (work or school account)</span></span> | <span data-ttu-id="e439c-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e439c-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e439c-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e439c-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e439c-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e439c-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e439c-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="e439c-122">Application</span></span> | <span data-ttu-id="e439c-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e439c-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e439c-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e439c-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="e439c-125">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="e439c-125">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="e439c-126">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="e439c-126">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="e439c-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。 </span><span class="sxs-lookup"><span data-stu-id="e439c-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e439c-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="e439c-129">Request headers</span></span>
| <span data-ttu-id="e439c-130">名称</span><span class="sxs-lookup"><span data-stu-id="e439c-130">Name</span></span>       | <span data-ttu-id="e439c-131">类型</span><span class="sxs-lookup"><span data-stu-id="e439c-131">Type</span></span> | <span data-ttu-id="e439c-132">说明</span><span class="sxs-lookup"><span data-stu-id="e439c-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e439c-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="e439c-133">Authorization</span></span>  | <span data-ttu-id="e439c-134">string</span><span class="sxs-lookup"><span data-stu-id="e439c-134">string</span></span>  | <span data-ttu-id="e439c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e439c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e439c-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e439c-137">Content-Type</span></span> | <span data-ttu-id="e439c-138">string</span><span class="sxs-lookup"><span data-stu-id="e439c-138">string</span></span>  | <span data-ttu-id="e439c-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="e439c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e439c-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="e439c-141">Request body</span></span>
<span data-ttu-id="e439c-142">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e439c-142">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e439c-143">响应</span><span class="sxs-lookup"><span data-stu-id="e439c-143">Response</span></span>

<span data-ttu-id="e439c-144">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e439c-144">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="e439c-145">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="e439c-145">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="e439c-146">请求</span><span class="sxs-lookup"><span data-stu-id="e439c-146">Request</span></span>
<span data-ttu-id="e439c-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e439c-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e439c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e439c-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_file_attachment_from_message_v1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "R0lGODdhEAYEAA7"
}
```
# <a name="c"></a>[<span data-ttu-id="e439c-149">C#</span><span class="sxs-lookup"><span data-stu-id="e439c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e439c-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e439c-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e439c-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e439c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e439c-152">Java</span><span class="sxs-lookup"><span data-stu-id="e439c-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-message-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e439c-153">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e439c-153">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e439c-154">响应</span><span class="sxs-lookup"><span data-stu-id="e439c-154">Response</span></span>
<span data-ttu-id="e439c-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e439c-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_message_v1",
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
    "contentBytes": "R0lGODdhEAYEAA7"
}

```

## <a name="example-item-attachment"></a><span data-ttu-id="e439c-156">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="e439c-156">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="e439c-157">请求</span><span class="sxs-lookup"><span data-stu-id="e439c-157">Request</span></span>
<span data-ttu-id="e439c-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e439c-158">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "create_item_attachment_from_message_v1"
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


##### <a name="response"></a><span data-ttu-id="e439c-159">响应</span><span class="sxs-lookup"><span data-stu-id="e439c-159">Response</span></span>
<span data-ttu-id="e439c-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e439c-160">Here is an example of the response.</span></span> <span data-ttu-id="e439c-161">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e439c-161">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_message_v1",
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
  ]
}-->

