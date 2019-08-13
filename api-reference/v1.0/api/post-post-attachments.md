---
title: Add attachment
description: 使用此 API 将 附件 添加到帖子。 自此处起
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b24e224b65b50a6754efaba35a131765b875e855
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375721"
---
# <a name="add-attachment"></a><span data-ttu-id="019ce-104">Add attachment</span><span class="sxs-lookup"><span data-stu-id="019ce-104">Add attachment</span></span>

<span data-ttu-id="019ce-p102">使用此 API 将 [附件](../resources/attachment.md) 添加到帖子。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="019ce-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="019ce-107">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="019ce-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="019ce-108">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="019ce-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="019ce-109">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="019ce-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="019ce-110">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="019ce-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="019ce-111">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="019ce-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="019ce-112">权限</span><span class="sxs-lookup"><span data-stu-id="019ce-112">Permissions</span></span>
<span data-ttu-id="019ce-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="019ce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="019ce-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="019ce-115">Permission type</span></span>      | <span data-ttu-id="019ce-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="019ce-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="019ce-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="019ce-117">Delegated (work or school account)</span></span> | <span data-ttu-id="019ce-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="019ce-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="019ce-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="019ce-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="019ce-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="019ce-120">Not supported.</span></span>    |
|<span data-ttu-id="019ce-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="019ce-121">Application</span></span> | <span data-ttu-id="019ce-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="019ce-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="019ce-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="019ce-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="019ce-124">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="019ce-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="019ce-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="019ce-125">Request headers</span></span>
| <span data-ttu-id="019ce-126">标头</span><span class="sxs-lookup"><span data-stu-id="019ce-126">Header</span></span>       | <span data-ttu-id="019ce-127">值</span><span class="sxs-lookup"><span data-stu-id="019ce-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="019ce-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="019ce-128">Authorization</span></span>  | <span data-ttu-id="019ce-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="019ce-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="019ce-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="019ce-131">Request body</span></span>
<span data-ttu-id="019ce-132">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="019ce-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="019ce-133">响应</span><span class="sxs-lookup"><span data-stu-id="019ce-133">Response</span></span>

<span data-ttu-id="019ce-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="019ce-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="019ce-135">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="019ce-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="019ce-136">请求</span><span class="sxs-lookup"><span data-stu-id="019ce-136">Request</span></span>
<span data-ttu-id="019ce-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="019ce-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="019ce-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="019ce-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "base64-contentBytes-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="019ce-139">C#</span><span class="sxs-lookup"><span data-stu-id="019ce-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="019ce-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="019ce-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="019ce-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="019ce-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="019ce-142">Java</span><span class="sxs-lookup"><span data-stu-id="019ce-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="019ce-143">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="019ce-143">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="019ce-144">响应</span><span class="sxs-lookup"><span data-stu-id="019ce-144">Response</span></span>
<span data-ttu-id="019ce-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="019ce-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="019ce-148">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="019ce-148">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="019ce-149">请求</span><span class="sxs-lookup"><span data-stu-id="019ce-149">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```


##### <a name="response"></a><span data-ttu-id="019ce-150">响应</span><span class="sxs-lookup"><span data-stu-id="019ce-150">Response</span></span>
<span data-ttu-id="019ce-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="019ce-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
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
