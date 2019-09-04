---
title: 获取附件
description: 读取附加到事件、邮件、Outlook 任务或帖子的附件的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: de8243597044e2077c4b2a1b8b91f35d2b6eecca
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718959"
---
# <a name="get-attachment"></a><span data-ttu-id="4addc-103">获取附件</span><span class="sxs-lookup"><span data-stu-id="4addc-103">Get attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4addc-104">读取附加到用户[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[帖子](../resources/post.md)的附件的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4addc-104">Read the properties and relationships of an attachment, attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

<span data-ttu-id="4addc-105">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="4addc-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="4addc-106">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="4addc-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="4addc-107">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="4addc-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span> <span data-ttu-id="4addc-108">您可以使用`$expand`来进一步获取该项目的属性。</span><span class="sxs-lookup"><span data-stu-id="4addc-108">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="4addc-109">请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="4addc-109">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="4addc-110">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="4addc-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="4addc-111">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="4addc-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span>

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="4addc-112">获取文件或项目附件的原始内容</span><span class="sxs-lookup"><span data-stu-id="4addc-112">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="4addc-113">您可以追加路径段`/$value`以获取文件或项目附件的原始内容。</span><span class="sxs-lookup"><span data-stu-id="4addc-113">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="4addc-114">对于文件附件, 内容类型基于其原始内容类型。</span><span class="sxs-lookup"><span data-stu-id="4addc-114">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="4addc-115">请参阅以下[示例](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="4addc-115">See an [example](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) below.</span></span>

<span data-ttu-id="4addc-116">对于作为[联系人](../resources/contact.md)、[事件](../resources/event.md)或[邮件](../resources/message.md)的项目附件, 返回的原始内容为 MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="4addc-116">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="4addc-117">项目附件类型</span><span class="sxs-lookup"><span data-stu-id="4addc-117">Item attachment type</span></span>  | <span data-ttu-id="4addc-118">返回的原始内容</span><span class="sxs-lookup"><span data-stu-id="4addc-118">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4addc-119">**联系人**</span><span class="sxs-lookup"><span data-stu-id="4addc-119">**contact**</span></span> | <span data-ttu-id="4addc-120">[vCard](http://www.faqs.org/rfcs/rfc2426.html)MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="4addc-120">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="4addc-121">请参阅[示例](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="4addc-121">See [example](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="4addc-122">**事件**</span><span class="sxs-lookup"><span data-stu-id="4addc-122">**event**</span></span> | <span data-ttu-id="4addc-123">iCal MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="4addc-123">iCal MIME format.</span></span> <span data-ttu-id="4addc-124">请参阅[示例](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="4addc-124">See [example](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="4addc-125">**邮件**</span><span class="sxs-lookup"><span data-stu-id="4addc-125">**message**</span></span> | <span data-ttu-id="4addc-126">MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="4addc-126">MIME format.</span></span> <span data-ttu-id="4addc-127">请参阅[示例](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="4addc-127">See [example](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="4addc-128">尝试获取引用附件`$value`的尝试返回 HTTP 405。</span><span class="sxs-lookup"><span data-stu-id="4addc-128">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="4addc-129">权限</span><span class="sxs-lookup"><span data-stu-id="4addc-129">Permissions</span></span>

<span data-ttu-id="4addc-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4addc-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="4addc-132">如果访问邮件中的附件: Mail. Read</span><span class="sxs-lookup"><span data-stu-id="4addc-132">If accessing attachments in messages: Mail.Read</span></span>
* <span data-ttu-id="4addc-133">如果访问事件中的附件: "日历"。阅读</span><span class="sxs-lookup"><span data-stu-id="4addc-133">If accessing attachments in events: Calendars.Read</span></span>
* <span data-ttu-id="4addc-134">如果访问 Outlook 任务中的附件: Tasks. Read</span><span class="sxs-lookup"><span data-stu-id="4addc-134">If accessing attachments in Outlook tasks: Tasks.Read</span></span>
* <span data-ttu-id="4addc-135">如果访问组帖子中的附件: Group. All</span><span class="sxs-lookup"><span data-stu-id="4addc-135">If accessing attachments in group posts: Group.Read.All</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="4addc-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4addc-136">HTTP request</span></span>

<span data-ttu-id="4addc-137">本节显示支持附件的每个实体 ([事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[post](../resources/post.md)) 的 HTTP GET 请求语法:</span><span class="sxs-lookup"><span data-stu-id="4addc-137">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="4addc-138">若要获取附件的属性和关系, 请将附件 ID 指定为附加到指定[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[post](../resources/post.md)实例的**附件**集合中的索引。</span><span class="sxs-lookup"><span data-stu-id="4addc-138">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="4addc-139">如果附件是文件或 Outlook 项目 (联系人、事件或邮件), 您可以通过将路径段`/$value`追加到请求 URL 来进一步获取附件的原始内容。</span><span class="sxs-lookup"><span data-stu-id="4addc-139">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="4addc-140">[事件](../resources/event.md)的附件:</span><span class="sxs-lookup"><span data-stu-id="4addc-140">An attachment of an [event](../resources/event.md):</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
GET /me/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}/$value
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="4addc-141">用户邮箱中的[邮件](../resources/message.md)附件:</span><span class="sxs-lookup"><span data-stu-id="4addc-141">An attachment of a [message](../resources/message.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="4addc-142">在用户邮箱的顶级[mailFolder](../resources/mailfolder.md)中包含的[邮件](../resources/message.md)的附件:</span><span class="sxs-lookup"><span data-stu-id="4addc-142">An attachment of a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="4addc-143">包含在用户邮箱中的[mailFolder](../resources/mailfolder.md)的子文件夹中的[邮件](../resources/message.md)的附件:</span><span class="sxs-lookup"><span data-stu-id="4addc-143">An attachment of a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="4addc-144">上面的示例展示了一层嵌套, 但邮件可以位于子元素的子级中, 依此类推。</span><span class="sxs-lookup"><span data-stu-id="4addc-144">The preceding example shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>

<span data-ttu-id="4addc-145">[Outlook 任务](../resources/outlooktask.md)的附件:</span><span class="sxs-lookup"><span data-stu-id="4addc-145">An attachment of an [Outlook task](../resources/outlooktask.md):</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments/{id}
GET /users/{id}/outlook/tasks/{id}/attachments/{id}
GET /me/outlook/tasks/{id}/attachments/{id}/$value
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

<span data-ttu-id="4addc-146">在属于组[对话](../resources/conversation.md)的[线程](../resources/conversationthread.md)中的[帖子](../resources/post.md)的附件:</span><span class="sxs-lookup"><span data-stu-id="4addc-146">An attachment of a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4addc-147">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4addc-147">Optional query parameters</span></span>

<span data-ttu-id="4addc-148">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4addc-148">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4addc-149">请求标头</span><span class="sxs-lookup"><span data-stu-id="4addc-149">Request headers</span></span>

| <span data-ttu-id="4addc-150">名称</span><span class="sxs-lookup"><span data-stu-id="4addc-150">Name</span></span>       | <span data-ttu-id="4addc-151">类型</span><span class="sxs-lookup"><span data-stu-id="4addc-151">Type</span></span> | <span data-ttu-id="4addc-152">说明</span><span class="sxs-lookup"><span data-stu-id="4addc-152">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4addc-153">Authorization</span><span class="sxs-lookup"><span data-stu-id="4addc-153">Authorization</span></span>  | <span data-ttu-id="4addc-154">string</span><span class="sxs-lookup"><span data-stu-id="4addc-154">string</span></span>  | <span data-ttu-id="4addc-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4addc-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4addc-157">请求正文</span><span class="sxs-lookup"><span data-stu-id="4addc-157">Request body</span></span>

<span data-ttu-id="4addc-158">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4addc-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4addc-159">响应</span><span class="sxs-lookup"><span data-stu-id="4addc-159">Response</span></span>

<span data-ttu-id="4addc-160">如果成功, GET 方法将返回`200 OK`响应代码。</span><span class="sxs-lookup"><span data-stu-id="4addc-160">If successful, the GET method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="4addc-161">如果要获取附件的属性和关系, 响应正文包含[附件](../resources/attachment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4addc-161">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span>

<span data-ttu-id="4addc-162">如果要获取文件或项目附件的原始内容, 响应正文将包含附件的原始值。</span><span class="sxs-lookup"><span data-stu-id="4addc-162">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="4addc-163">示例</span><span class="sxs-lookup"><span data-stu-id="4addc-163">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="4addc-164">示例 1: 获取文件附件的属性</span><span class="sxs-lookup"><span data-stu-id="4addc-164">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4addc-165">请求</span><span class="sxs-lookup"><span data-stu-id="4addc-165">Request</span></span>

<span data-ttu-id="4addc-166">下面的示例展示了获取邮件的文件附件属性的请求。</span><span class="sxs-lookup"><span data-stu-id="4addc-166">Here is an example of the request to get the properties of a file attachment on a message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4addc-167">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4addc-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment_beta",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4addc-168">C#</span><span class="sxs-lookup"><span data-stu-id="4addc-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4addc-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4addc-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4addc-170">目标-C</span><span class="sxs-lookup"><span data-stu-id="4addc-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4addc-171">响应</span><span class="sxs-lookup"><span data-stu-id="4addc-171">Response</span></span>

<span data-ttu-id="4addc-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4addc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_file_attachment_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKjAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "id": "AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=",
    "lastModifiedDateTime": "2019-04-02T03:41:29Z",
    "name": "Draft sales invoice template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 13068,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "UEsDBBQABgAIAAAAIQ4AAAAA"
}
```

### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="4addc-175">示例 2: 获取项目附件的属性</span><span class="sxs-lookup"><span data-stu-id="4addc-175">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4addc-176">请求</span><span class="sxs-lookup"><span data-stu-id="4addc-176">Request</span></span>

<span data-ttu-id="4addc-177">第一个示例演示如何获取邮件的项目附件。</span><span class="sxs-lookup"><span data-stu-id="4addc-177">The first example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="4addc-178">返回**itemAttachment**的属性。</span><span class="sxs-lookup"><span data-stu-id="4addc-178">The properties of the **itemAttachment** are returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4addc-179">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4addc-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4addc-180">C#</span><span class="sxs-lookup"><span data-stu-id="4addc-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4addc-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4addc-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4addc-182">目标-C</span><span class="sxs-lookup"><span data-stu-id="4addc-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4addc-183">响应</span><span class="sxs-lookup"><span data-stu-id="4addc-183">Response</span></span>
<span data-ttu-id="4addc-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4addc-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1M-CJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="4addc-187">示例 3: 展开和获取附加到邮件的项目的属性</span><span class="sxs-lookup"><span data-stu-id="4addc-187">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="4addc-188">请求</span><span class="sxs-lookup"><span data-stu-id="4addc-188">Request</span></span>

<span data-ttu-id="4addc-189">下一个示例演示如何使用`$expand`来获取附加到邮件的项目 (事件、邮件、Outlook 任务或 post) 的属性。</span><span class="sxs-lookup"><span data-stu-id="4addc-189">The next example shows how to use `$expand` to get the properties of the item (event, message, Outlook task, or post) that is attached to the message.</span></span> <span data-ttu-id="4addc-190">在此示例中, 该项目是一条消息;此外, 还将返回该附加邮件的属性。</span><span class="sxs-lookup"><span data-stu-id="4addc-190">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4addc-191">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4addc-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4addc-192">C#</span><span class="sxs-lookup"><span data-stu-id="4addc-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4addc-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4addc-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4addc-194">目标-C</span><span class="sxs-lookup"><span data-stu-id="4addc-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4addc-195">响应</span><span class="sxs-lookup"><span data-stu-id="4addc-195">Response</span></span>
<span data-ttu-id="4addc-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4addc-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_and_expand_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
  "item":{
    "@odata.type":"#microsoft.graph.message",
    "id":"",
    "createdDateTime":"2017-07-21T00:20:41Z",
    "lastModifiedDateTime":"2017-07-21T00:20:34Z",
    "receivedDateTime":"2017-07-21T00:19:55Z",
    "sentDateTime":"2017-07-21T00:19:52Z",
    "hasAttachments":false,
    "internetMessageId":"<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
    "subject":"Reminder - please bring laptop",
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "conversationIndex":"AQHTAbcSwb41IIwGp0qstrYSZH+U7Q==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "body":{
      "contentType":"html",
      "content":"<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
    },
    "sender":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "from":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "toRecipients":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients":[
      {
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.onmicrosoft.com"
        }
      }
    ],
    "flag":{
      "flagStatus":"notFlagged"
    }
  }
}
```

### <a name="example-4-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="4addc-199">示例 4: 获取引用附件的属性</span><span class="sxs-lookup"><span data-stu-id="4addc-199">Example 4: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4addc-200">请求</span><span class="sxs-lookup"><span data-stu-id="4addc-200">Request</span></span>

<span data-ttu-id="4addc-201">下面的示例展示了用于获取事件的参考附件的请求。</span><span class="sxs-lookup"><span data-stu-id="4addc-201">Here is an example of the request to get a reference attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4addc-202">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4addc-202">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGE1M88AADUv0uAAAG=","AAMkAGE1Mg72tgf7hJp0PICVGCc0g="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4addc-203">C#</span><span class="sxs-lookup"><span data-stu-id="4addc-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4addc-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4addc-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4addc-205">目标-C</span><span class="sxs-lookup"><span data-stu-id="4addc-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4addc-206">响应</span><span class="sxs-lookup"><span data-stu-id="4addc-206">Response</span></span>
<span data-ttu-id="4addc-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4addc-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_reference_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
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


### <a name="example-5-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="4addc-210">示例 5: 获取邮件的文件附件的原始内容</span><span class="sxs-lookup"><span data-stu-id="4addc-210">Example 5: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="4addc-211">请求</span><span class="sxs-lookup"><span data-stu-id="4addc-211">Request</span></span>

<span data-ttu-id="4addc-212">下面的示例展示了获取已附加到邮件的 Word 文件的原始内容的请求。</span><span class="sxs-lookup"><span data-stu-id="4addc-212">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="4addc-213">响应</span><span class="sxs-lookup"><span data-stu-id="4addc-213">Response</span></span>
<span data-ttu-id="4addc-214">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4addc-214">Here is an example of the response.</span></span> <span data-ttu-id="4addc-215">实际的响应正文包括文件附件的原始字节, 在这里可缩写为简洁。</span><span class="sxs-lookup"><span data-stu-id="4addc-215">The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="4addc-216">示例 6: 获取邮件的联系人附件的 MIME 原始内容</span><span class="sxs-lookup"><span data-stu-id="4addc-216">Example 6: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="4addc-217">请求</span><span class="sxs-lookup"><span data-stu-id="4addc-217">Request</span></span>

<span data-ttu-id="4addc-218">下面的示例展示了获取已附加到邮件的联系人项目的原始内容的请求。</span><span class="sxs-lookup"><span data-stu-id="4addc-218">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="4addc-219">响应</span><span class="sxs-lookup"><span data-stu-id="4addc-219">Response</span></span>
<span data-ttu-id="4addc-220">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4addc-220">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCARD
PROFILE:VCARD
VERSION:3.0
MAILER:Microsoft Exchange
PRODID:Microsoft Exchange
FN:Alex Wilbur
N:Wilbur;Alex;;;
NOTE:Sunday\, June 10\, 2012 5:44 PM:\nGutter\, window cleaning\, pressure 
 washing\, roof debris blowing\n
ORG:Contoso;
CLASS:PUBLIC
ADR;TYPE=WORK,PREF:;;4567 Main St;Buffalo;NY;98052;United States of America
LABEL;TYPE=WORK,PREF:4567 Main St\nBuffalo\, NY 98052
ADR;TYPE=HOME:;;;;;;
ADR;TYPE=POSTAL:;;;;;;
TEL;TYPE=WORK:(425) 555-0100
TITLE:
X-MS-IMADDRESS:
REV;VALUE=DATE-TIME:2019-04-09T02:13:31,161Z
END:VCARD
```


### <a name="example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="4addc-221">示例 7: 获取邮件的事件附件的 MIME 原始内容</span><span class="sxs-lookup"><span data-stu-id="4addc-221">Example 7: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="4addc-222">请求</span><span class="sxs-lookup"><span data-stu-id="4addc-222">Request</span></span>

<span data-ttu-id="4addc-223">下面的示例展示了获取已附加到邮件的事件的原始内容的请求。</span><span class="sxs-lookup"><span data-stu-id="4addc-223">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="4addc-224">响应</span><span class="sxs-lookup"><span data-stu-id="4addc-224">Response</span></span>
<span data-ttu-id="4addc-225">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4addc-225">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCALENDAR
METHOD:PUBLISH
PRODID:Microsoft Exchange Server 2010
VERSION:2.0
BEGIN:VTIMEZONE
TZID:Pacific Standard Time
BEGIN:STANDARD
DTSTART:16010101T020000
TZOFFSETFROM:-0700
TZOFFSETTO:-0800
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=1SU;BYMONTH=11
END:STANDARD
BEGIN:DAYLIGHT
DTSTART:16010101T020000
TZOFFSETFROM:-0800
TZOFFSETTO:-0700
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=2SU;BYMONTH=3
END:DAYLIGHT
END:VTIMEZONE
BEGIN:VEVENT
ORGANIZER;CN=Adele Vance:MAILTO:adelev@contoso.com
ATTENDEE;ROLE=REQ-PARTICIPANT;PARTSTAT=NEEDS-ACTION;RSVP=TRUE;CN=Adele Vance:MAILTO:adelev@contoso.com
DESCRIPTION;LANGUAGE=en-US:\n
UID:040000008200
SUMMARY;LANGUAGE=en-US:Review Megan's docs
DTSTART;TZID=Pacific Standard Time:20190409T140000
DTEND;TZID=Pacific Standard Time:20190409T160000
CLASS:PUBLIC
PRIORITY:5
DTSTAMP:20190409T211833Z
TRANSP:OPAQUE
STATUS:CONFIRMED
SEQUENCE:0
LOCATION;LANGUAGE=en-US:
X-MICROSOFT-CDO-APPT-SEQUENCE:0
X-MICROSOFT-CDO-OWNERAPPTID:0
X-MICROSOFT-CDO-BUSYSTATUS:BUSY
X-MICROSOFT-CDO-INTENDEDSTATUS:BUSY
X-MICROSOFT-CDO-ALLDAYEVENT:FALSE
X-MICROSOFT-CDO-IMPORTANCE:1
X-MICROSOFT-CDO-INSTTYPE:0
X-MICROSOFT-DONOTFORWARDMEETING:FALSE
X-MICROSOFT-DISALLOW-COUNTER:FALSE
X-MICROSOFT-LOCATIONS:[]
BEGIN:VALARM
DESCRIPTION:REMINDER
TRIGGER;RELATED=START:-PT15M
ACTION:DISPLAY
END:VALARM
END:VEVENT
END:VCALENDAR
```


### <a name="example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="4addc-226">示例 8: 获取邮件上会议邀请项目附件的 MIME 原始内容</span><span class="sxs-lookup"><span data-stu-id="4addc-226">Example 8: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="4addc-227">请求</span><span class="sxs-lookup"><span data-stu-id="4addc-227">Request</span></span>

<span data-ttu-id="4addc-228">下面的示例展示了获取已附加到邮件的会议邀请 ( [eventMessage](../resources/eventmessage.md)类型) 的原始内容的请求。</span><span class="sxs-lookup"><span data-stu-id="4addc-228">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="4addc-229">**EventMessage**实体基于**邮件**类型。</span><span class="sxs-lookup"><span data-stu-id="4addc-229">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="4addc-230">响应</span><span class="sxs-lookup"><span data-stu-id="4addc-230">Response</span></span>
<span data-ttu-id="4addc-231">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4addc-231">Here is an example of the response.</span></span> 

<span data-ttu-id="4addc-232">响应正文包含 MIME 格式的**eventMessage**附件。</span><span class="sxs-lookup"><span data-stu-id="4addc-232">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="4addc-233">为简洁起见, **eventMessage**的正文将被截断。</span><span class="sxs-lookup"><span data-stu-id="4addc-233">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="4addc-234">实际调用会返回完整的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="4addc-234">The full message body is returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

From: Megan Bowen <MeganB@contoso.OnMicrosoft.com>
To: Adele Vance <AdeleV@contoso.OnMicrosoft.com>
Subject: Let's go for lunch
Thread-Topic: Let's go for lunch
Thread-Index: AdTPqxOmg4AXoJV960a1j5NrJCHYjA==
X-MS-Exchange-MessageSentRepresentingType: 1
Date: Thu, 28 Feb 2019 21:17:58 +0000
Message-ID:
    <CY4PR2201MB1046E9C83FC42478EF4EE283C9750@CY4PR2201MB1046.namprd22.prod.outlook.com>
Content-Language: en-US
X-MS-Has-Attach:
X-MS-Exchange-Organization-SCL: -1
X-MS-TNEF-Correlator:
X-MS-Exchange-Organization-RecordReviewCfmType: 0
Content-Type: multipart/alternative;
    boundary="_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_"
MIME-Version: 1.0

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/plain; charset="us-ascii"

Does mid month work for you?

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/html; charset="us-ascii"

<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=us-ascii">
</head>
<body>
Does mid month work for you?
</body>
</html>

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/calendar; charset="utf-8"; method=REQUEST
Content-Transfer-Encoding: base64

QkVHSU46VkNBTEVOREFSDQpNRVRIT0Q6UkVRVUVTVA0KUFJPRElEOk1pY3Jvc29mdCBFeGNoYW5n


--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_--
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
