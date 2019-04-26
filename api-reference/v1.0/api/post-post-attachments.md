---
title: Add attachment
description: 使用此 API 将 附件 添加到帖子。 由于存在
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: b2b1c619e40fa915b079f97a6efb444981b28709
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576288"
---
# <a name="add-attachment"></a><span data-ttu-id="87a01-104">Add attachment</span><span class="sxs-lookup"><span data-stu-id="87a01-104">Add attachment</span></span>

<span data-ttu-id="87a01-p102">使用此 API 将 [附件](../resources/attachment.md) 添加到帖子。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="87a01-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="87a01-107">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="87a01-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="87a01-108">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="87a01-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="87a01-109">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="87a01-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="87a01-110">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="87a01-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="87a01-111">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="87a01-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="87a01-112">权限</span><span class="sxs-lookup"><span data-stu-id="87a01-112">Permissions</span></span>
<span data-ttu-id="87a01-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87a01-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87a01-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="87a01-115">Permission type</span></span>      | <span data-ttu-id="87a01-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87a01-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87a01-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87a01-117">Delegated (work or school account)</span></span> | <span data-ttu-id="87a01-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87a01-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="87a01-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87a01-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87a01-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="87a01-120">Not supported.</span></span>    |
|<span data-ttu-id="87a01-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="87a01-121">Application</span></span> | <span data-ttu-id="87a01-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87a01-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87a01-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87a01-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="87a01-124">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="87a01-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="87a01-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="87a01-125">Request headers</span></span>
| <span data-ttu-id="87a01-126">标头</span><span class="sxs-lookup"><span data-stu-id="87a01-126">Header</span></span>       | <span data-ttu-id="87a01-127">值</span><span class="sxs-lookup"><span data-stu-id="87a01-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87a01-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="87a01-128">Authorization</span></span>  | <span data-ttu-id="87a01-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="87a01-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87a01-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="87a01-131">Request body</span></span>
<span data-ttu-id="87a01-132">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87a01-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="87a01-133">响应</span><span class="sxs-lookup"><span data-stu-id="87a01-133">Response</span></span>

<span data-ttu-id="87a01-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="87a01-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="87a01-135">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="87a01-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="87a01-136">请求</span><span class="sxs-lookup"><span data-stu-id="87a01-136">Request</span></span>
<span data-ttu-id="87a01-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="87a01-137">Here is an example of the request.</span></span>
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

<span data-ttu-id="87a01-138">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87a01-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="87a01-139">响应</span><span class="sxs-lookup"><span data-stu-id="87a01-139">Response</span></span>
<span data-ttu-id="87a01-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="87a01-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="87a01-143">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="87a01-143">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="87a01-144">请求</span><span class="sxs-lookup"><span data-stu-id="87a01-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
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

##### <a name="response"></a><span data-ttu-id="87a01-145">响应</span><span class="sxs-lookup"><span data-stu-id="87a01-145">Response</span></span>
<span data-ttu-id="87a01-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="87a01-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
