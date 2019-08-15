---
title: Add attachment
description: 使用此 API 将 附件 添加到帖子。 自此处起
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 611489e63c36a922f3eabd3a595680565151ab6f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412906"
---
# <a name="add-attachment"></a><span data-ttu-id="0a689-104">Add attachment</span><span class="sxs-lookup"><span data-stu-id="0a689-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a689-p102">使用此 API 将 [附件](../resources/attachment.md) 添加到帖子。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="0a689-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="0a689-107">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="0a689-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="0a689-108">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="0a689-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="0a689-109">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="0a689-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="0a689-110">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="0a689-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="0a689-111">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="0a689-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0a689-112">权限</span><span class="sxs-lookup"><span data-stu-id="0a689-112">Permissions</span></span>
<span data-ttu-id="0a689-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a689-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a689-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a689-115">Permission type</span></span>      | <span data-ttu-id="0a689-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a689-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a689-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a689-117">Delegated (work or school account)</span></span> | <span data-ttu-id="0a689-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a689-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a689-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a689-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a689-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a689-120">Not supported.</span></span>    |
|<span data-ttu-id="0a689-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a689-121">Application</span></span> | <span data-ttu-id="0a689-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a689-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a689-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a689-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0a689-124">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="0a689-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="0a689-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a689-125">Request headers</span></span>
| <span data-ttu-id="0a689-126">标头</span><span class="sxs-lookup"><span data-stu-id="0a689-126">Header</span></span>       | <span data-ttu-id="0a689-127">值</span><span class="sxs-lookup"><span data-stu-id="0a689-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a689-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a689-128">Authorization</span></span>  | <span data-ttu-id="0a689-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a689-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a689-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a689-131">Request body</span></span>
<span data-ttu-id="0a689-132">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a689-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0a689-133">响应</span><span class="sxs-lookup"><span data-stu-id="0a689-133">Response</span></span>

<span data-ttu-id="0a689-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0a689-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="0a689-135">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="0a689-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="0a689-136">请求</span><span class="sxs-lookup"><span data-stu-id="0a689-136">Request</span></span>
<span data-ttu-id="0a689-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a689-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a689-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0a689-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a689-139">C#</span><span class="sxs-lookup"><span data-stu-id="0a689-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a689-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a689-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a689-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="0a689-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="0a689-142">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a689-142">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="0a689-143">响应</span><span class="sxs-lookup"><span data-stu-id="0a689-143">Response</span></span>
<span data-ttu-id="0a689-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a689-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="0a689-147">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="0a689-147">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="0a689-148">请求</span><span class="sxs-lookup"><span data-stu-id="0a689-148">Request</span></span>

<!-- { "blockType": "ignored" } -->

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


##### <a name="response"></a><span data-ttu-id="0a689-149">响应</span><span class="sxs-lookup"><span data-stu-id="0a689-149">Response</span></span>
<span data-ttu-id="0a689-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a689-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="0a689-153">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="0a689-153">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="0a689-154">请求</span><span class="sxs-lookup"><span data-stu-id="0a689-154">Request</span></span>
<span data-ttu-id="0a689-155">下面的示例展示了向现有帖子添加引用附件的请求。</span><span class="sxs-lookup"><span data-stu-id="0a689-155">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="0a689-156">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="0a689-156">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a689-157">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0a689-157">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a689-158">C#</span><span class="sxs-lookup"><span data-stu-id="0a689-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a689-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a689-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a689-160">目标-C</span><span class="sxs-lookup"><span data-stu-id="0a689-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0a689-161">响应</span><span class="sxs-lookup"><span data-stu-id="0a689-161">Response</span></span>
<span data-ttu-id="0a689-162">下面的示例展示了完整的响应。</span><span class="sxs-lookup"><span data-stu-id="0a689-162">Here is an example of a full response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
