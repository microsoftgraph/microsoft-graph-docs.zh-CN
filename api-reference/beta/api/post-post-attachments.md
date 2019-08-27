---
title: Add attachment
description: 创建组帖子时添加附件。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 425b3f8c3fa744c33defc7790ede0871ff60fef2
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633536"
---
# <a name="add-attachment"></a><span data-ttu-id="debbb-103">添加附件</span><span class="sxs-lookup"><span data-stu-id="debbb-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="debbb-104">创建组帖子时添加[附件](../resources/attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="debbb-104">Add an [attachment](../resources/attachment.md) when creating a group post.</span></span> 

<span data-ttu-id="debbb-105">由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="debbb-105">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="debbb-106">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="debbb-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="debbb-107">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="debbb-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="debbb-108">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="debbb-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="debbb-109">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="debbb-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="debbb-110">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="debbb-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="debbb-111">权限</span><span class="sxs-lookup"><span data-stu-id="debbb-111">Permissions</span></span>
<span data-ttu-id="debbb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="debbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="debbb-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="debbb-114">Permission type</span></span>      | <span data-ttu-id="debbb-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="debbb-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="debbb-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="debbb-116">Delegated (work or school account)</span></span> | <span data-ttu-id="debbb-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="debbb-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="debbb-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="debbb-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="debbb-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="debbb-119">Not supported.</span></span>    |
|<span data-ttu-id="debbb-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="debbb-120">Application</span></span> | <span data-ttu-id="debbb-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="debbb-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="debbb-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="debbb-122">HTTP request</span></span>
<span data-ttu-id="debbb-123">在组的[conversationThread](../resources/conversationthread.md)中创建[帖子](../resources/post.md)时包含附件。</span><span class="sxs-lookup"><span data-stu-id="debbb-123">Include an attachment when creating a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="debbb-124">指定父[对话](../resources/conversation.md)是可选的。</span><span class="sxs-lookup"><span data-stu-id="debbb-124">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="debbb-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="debbb-125">Request headers</span></span>
| <span data-ttu-id="debbb-126">标头</span><span class="sxs-lookup"><span data-stu-id="debbb-126">Header</span></span>       | <span data-ttu-id="debbb-127">值</span><span class="sxs-lookup"><span data-stu-id="debbb-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="debbb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="debbb-128">Authorization</span></span>  | <span data-ttu-id="debbb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="debbb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="debbb-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="debbb-131">Request body</span></span>
<span data-ttu-id="debbb-132">在请求正文中, 提供包含**post**参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="debbb-132">In the request body, provide a JSON object that includes a **post** parameter.</span></span>

| <span data-ttu-id="debbb-133">参数</span><span class="sxs-lookup"><span data-stu-id="debbb-133">Parameter</span></span>    | <span data-ttu-id="debbb-134">类型</span><span class="sxs-lookup"><span data-stu-id="debbb-134">Type</span></span>   |<span data-ttu-id="debbb-135">说明</span><span class="sxs-lookup"><span data-stu-id="debbb-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="debbb-136">帖子</span><span class="sxs-lookup"><span data-stu-id="debbb-136">post</span></span>|[<span data-ttu-id="debbb-137">帖子</span><span class="sxs-lookup"><span data-stu-id="debbb-137">post</span></span>](../resources/post.md)|<span data-ttu-id="debbb-138">要答复的新帖子, 其中包含[附件](../resources/attachment.md)集合中的一个或多个附件。</span><span class="sxs-lookup"><span data-stu-id="debbb-138">The new post that is being replied with, which includes one or more attachments in an [attachment](../resources/attachment.md) collection.</span></span>|

## <a name="response"></a><span data-ttu-id="debbb-139">响应</span><span class="sxs-lookup"><span data-stu-id="debbb-139">Response</span></span>

<span data-ttu-id="debbb-p104">如果成功，此方法返回 `202 Accepted` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="debbb-p104">If successful, this method returns `202 Accepted` response code. It does not return a response body.</span></span>

## <a name="examples"></a><span data-ttu-id="debbb-142">示例</span><span class="sxs-lookup"><span data-stu-id="debbb-142">Examples</span></span>
### <a name="example-1-include-a-file-attachment"></a><span data-ttu-id="debbb-143">示例 1: 包含文件附件</span><span class="sxs-lookup"><span data-stu-id="debbb-143">Example 1: Include a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="debbb-144">请求</span><span class="sxs-lookup"><span data-stu-id="debbb-144">Request</span></span>
<span data-ttu-id="debbb-145">下面的示例展示了在创建帖子时将文件作为附件包含的一个请求。</span><span class="sxs-lookup"><span data-stu-id="debbb-145">Here is an example of a request that includes a file as an attachment when creating a post.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="debbb-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="debbb-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "text",
      "content": "Which quarter does that file cover? See my attachment."
    },
    "attachments": [{
      "@odata.type": "#microsoft.graph.fileAttachment",
      "name": "Another file as attachment",
      "contentBytes": "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu"
    } ]
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="debbb-147">C#</span><span class="sxs-lookup"><span data-stu-id="debbb-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="debbb-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="debbb-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="debbb-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="debbb-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="debbb-150">响应</span><span class="sxs-lookup"><span data-stu-id="debbb-150">Response</span></span>
<span data-ttu-id="debbb-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="debbb-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
```

### <a name="example-2-include-an-item-attachment"></a><span data-ttu-id="debbb-152">示例 2: 包含项目附件</span><span class="sxs-lookup"><span data-stu-id="debbb-152">Example 2: Include an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="debbb-153">请求</span><span class="sxs-lookup"><span data-stu-id="debbb-153">Request</span></span>
<span data-ttu-id="debbb-154">下面的示例展示了在创建帖子时将事件作为附件包含的一个请求。</span><span class="sxs-lookup"><span data-stu-id="debbb-154">Here is an example of a request that includes an event as an attachment when creating a post.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "text",
      "content": "I attached an event."
    },
    "attachments": [{
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
              "dateTime": "2019-12-02T18:00:00",
              "timeZone": "Pacific Standard Time"
          },
          "end": {
              "dateTime": "2019-12-02T19:00:00",
              "timeZone": "Pacific Standard Time"
          }
      }
    } ]
  }
}
```


#### <a name="response"></a><span data-ttu-id="debbb-155">响应</span><span class="sxs-lookup"><span data-stu-id="debbb-155">Response</span></span>
<span data-ttu-id="debbb-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="debbb-156">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-include-a-reference-attachment"></a><span data-ttu-id="debbb-157">示例 3: 包含引用附件</span><span class="sxs-lookup"><span data-stu-id="debbb-157">Example 3: Include a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="debbb-158">请求</span><span class="sxs-lookup"><span data-stu-id="debbb-158">Request</span></span>
<span data-ttu-id="debbb-159">下面的示例展示了在创建帖子时包含参考附件的请求。</span><span class="sxs-lookup"><span data-stu-id="debbb-159">Here is an example of a request that includes a reference attachment when creating a post.</span></span>
<span data-ttu-id="debbb-160">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="debbb-160">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="debbb-161">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="debbb-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "text",
      "content": "I attached a reference to a file on OneDrive."
    },
    "attachments": [{
      "@odata.type": "#microsoft.graph.referenceAttachment", 
      "name": "Personal pictures", 
      "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
      "providerType": "oneDriveConsumer", 
      "permission": "Edit", 
      "isFolder": "True"
    } ]
  }
}
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="debbb-162">C#</span><span class="sxs-lookup"><span data-stu-id="debbb-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="debbb-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="debbb-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="debbb-164">目标-C</span><span class="sxs-lookup"><span data-stu-id="debbb-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="debbb-165">响应</span><span class="sxs-lookup"><span data-stu-id="debbb-165">Response</span></span>
<span data-ttu-id="debbb-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="debbb-166">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_reference_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
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
