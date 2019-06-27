---
title: Add attachment
description: 使用此 API 将 附件 添加到帖子。 自此处起
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 16b054b093a90f6017c073c77b5656ea56c8bbc3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275185"
---
# <a name="add-attachment"></a><span data-ttu-id="dab7c-104">Add attachment</span><span class="sxs-lookup"><span data-stu-id="dab7c-104">Add attachment</span></span>

<span data-ttu-id="dab7c-p102">使用此 API 将 [附件](../resources/attachment.md) 添加到帖子。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="dab7c-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="dab7c-107">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="dab7c-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="dab7c-108">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="dab7c-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="dab7c-109">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="dab7c-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="dab7c-110">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="dab7c-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="dab7c-111">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="dab7c-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="dab7c-112">权限</span><span class="sxs-lookup"><span data-stu-id="dab7c-112">Permissions</span></span>
<span data-ttu-id="dab7c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dab7c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dab7c-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="dab7c-115">Permission type</span></span>      | <span data-ttu-id="dab7c-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dab7c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dab7c-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dab7c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="dab7c-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dab7c-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dab7c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dab7c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dab7c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="dab7c-120">Not supported.</span></span>    |
|<span data-ttu-id="dab7c-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="dab7c-121">Application</span></span> | <span data-ttu-id="dab7c-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dab7c-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dab7c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dab7c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="dab7c-124">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="dab7c-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="dab7c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="dab7c-125">Request headers</span></span>
| <span data-ttu-id="dab7c-126">标头</span><span class="sxs-lookup"><span data-stu-id="dab7c-126">Header</span></span>       | <span data-ttu-id="dab7c-127">值</span><span class="sxs-lookup"><span data-stu-id="dab7c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dab7c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="dab7c-128">Authorization</span></span>  | <span data-ttu-id="dab7c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dab7c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dab7c-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="dab7c-131">Request body</span></span>
<span data-ttu-id="dab7c-132">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dab7c-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dab7c-133">响应</span><span class="sxs-lookup"><span data-stu-id="dab7c-133">Response</span></span>

<span data-ttu-id="dab7c-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dab7c-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="dab7c-135">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="dab7c-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="dab7c-136">请求</span><span class="sxs-lookup"><span data-stu-id="dab7c-136">Request</span></span>
<span data-ttu-id="dab7c-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dab7c-137">Here is an example of the request.</span></span>
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

<span data-ttu-id="dab7c-138">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dab7c-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="dab7c-139">响应</span><span class="sxs-lookup"><span data-stu-id="dab7c-139">Response</span></span>
<span data-ttu-id="dab7c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dab7c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="dab7c-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dab7c-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dab7c-144">C#</span><span class="sxs-lookup"><span data-stu-id="dab7c-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dab7c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="dab7c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dab7c-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="dab7c-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="dab7c-147">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="dab7c-147">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="dab7c-148">请求</span><span class="sxs-lookup"><span data-stu-id="dab7c-148">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="dab7c-149">响应</span><span class="sxs-lookup"><span data-stu-id="dab7c-149">Response</span></span>
<span data-ttu-id="dab7c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dab7c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
