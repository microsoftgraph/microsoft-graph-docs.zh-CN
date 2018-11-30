---
title: Add attachment
description: 使用此 API 向帖子添加附件。 相那里
ms.openlocfilehash: 38126f015d19890a9a1f08d458f05505faa09e9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042719"
---
# <a name="add-attachment"></a><span data-ttu-id="9e351-104">Add attachment</span><span class="sxs-lookup"><span data-stu-id="9e351-104">Add attachment</span></span>

> <span data-ttu-id="9e351-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9e351-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e351-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9e351-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e351-p103">使用此 API 将 [附件](../resources/attachment.md) 添加到帖子。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="9e351-p103">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="9e351-109">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="9e351-109">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="9e351-110">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="9e351-110">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="9e351-111">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="9e351-111">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="9e351-112">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="9e351-112">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="9e351-113">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="9e351-113">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9e351-114">权限</span><span class="sxs-lookup"><span data-stu-id="9e351-114">Permissions</span></span>
<span data-ttu-id="9e351-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e351-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e351-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e351-117">Permission type</span></span>      | <span data-ttu-id="9e351-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e351-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e351-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e351-119">Delegated (work or school account)</span></span> | <span data-ttu-id="9e351-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e351-120">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9e351-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e351-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e351-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e351-122">Not supported.</span></span>    |
|<span data-ttu-id="9e351-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e351-123">Application</span></span> | <span data-ttu-id="9e351-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e351-124">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e351-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e351-125">HTTP request</span></span>
<span data-ttu-id="9e351-126"><!-- { "blockType": "ignored" } -->[发布](../resources/post.md)[线程](../resources/conversationthread.md)属于组的[对话](../resources/conversation.md)中的附件。</span><span class="sxs-lookup"><span data-stu-id="9e351-126"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="9e351-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e351-127">Request headers</span></span>
| <span data-ttu-id="9e351-128">标头</span><span class="sxs-lookup"><span data-stu-id="9e351-128">Header</span></span>       | <span data-ttu-id="9e351-129">值</span><span class="sxs-lookup"><span data-stu-id="9e351-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9e351-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e351-130">Authorization</span></span>  | <span data-ttu-id="9e351-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9e351-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9e351-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e351-133">Request body</span></span>
<span data-ttu-id="9e351-134">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e351-134">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9e351-135">响应</span><span class="sxs-lookup"><span data-stu-id="9e351-135">Response</span></span>

<span data-ttu-id="9e351-136">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e351-136">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="9e351-137">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="9e351-137">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9e351-138">请求</span><span class="sxs-lookup"><span data-stu-id="9e351-138">Request</span></span>
<span data-ttu-id="9e351-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e351-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="9e351-140">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e351-140">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="9e351-141">响应</span><span class="sxs-lookup"><span data-stu-id="9e351-141">Response</span></span>
<span data-ttu-id="9e351-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e351-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="9e351-145">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="9e351-145">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9e351-146">请求</span><span class="sxs-lookup"><span data-stu-id="9e351-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="9e351-147">响应</span><span class="sxs-lookup"><span data-stu-id="9e351-147">Response</span></span>
<span data-ttu-id="9e351-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e351-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```


## <a name="example-reference-attachment"></a><span data-ttu-id="9e351-151">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="9e351-151">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9e351-152">请求</span><span class="sxs-lookup"><span data-stu-id="9e351-152">Request</span></span>
<span data-ttu-id="9e351-153">下面是请求的添加到现有张贴内容的引用附件的示例。</span><span class="sxs-lookup"><span data-stu-id="9e351-153">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="9e351-154">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="9e351-154">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_post",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments
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

##### <a name="response"></a><span data-ttu-id="9e351-155">响应</span><span class="sxs-lookup"><span data-stu-id="9e351-155">Response</span></span>
<span data-ttu-id="9e351-156">下面是响应的完整的一个示例。</span><span class="sxs-lookup"><span data-stu-id="9e351-156">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments/$entity",
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
