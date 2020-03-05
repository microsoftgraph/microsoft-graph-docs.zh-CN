---
title: Add attachment
description: 创建组帖子时添加附件。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 62fe2fdc347c7c74eaedd57e844978ea87c2f275
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455462"
---
# <a name="add-attachment"></a><span data-ttu-id="8d910-103">添加附件</span><span class="sxs-lookup"><span data-stu-id="8d910-103">Add attachment</span></span>

<span data-ttu-id="8d910-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8d910-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d910-105">创建组帖子时添加[附件](../resources/attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="8d910-105">Add an [attachment](../resources/attachment.md) when creating a group post.</span></span> 

<span data-ttu-id="8d910-106">此操作将限制可添加到 4 MB 以下的附件的大小。</span><span class="sxs-lookup"><span data-stu-id="8d910-106">This operation limits the size of the attachment you can add to under 4 MB.</span></span>

<span data-ttu-id="8d910-107">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="8d910-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="8d910-108">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="8d910-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="8d910-109">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="8d910-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="8d910-110">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="8d910-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="8d910-111">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="8d910-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8d910-112">权限</span><span class="sxs-lookup"><span data-stu-id="8d910-112">Permissions</span></span>
<span data-ttu-id="8d910-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d910-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d910-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d910-115">Permission type</span></span>      | <span data-ttu-id="8d910-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d910-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d910-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d910-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8d910-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d910-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8d910-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d910-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d910-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d910-120">Not supported.</span></span>    |
|<span data-ttu-id="8d910-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d910-121">Application</span></span> | <span data-ttu-id="8d910-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d910-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d910-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d910-123">HTTP request</span></span>
<span data-ttu-id="8d910-124">在组的[conversationThread](../resources/conversationthread.md)中创建[帖子](../resources/post.md)时包含附件。</span><span class="sxs-lookup"><span data-stu-id="8d910-124">Include an attachment when creating a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="8d910-125">指定父[对话](../resources/conversation.md)是可选的。</span><span class="sxs-lookup"><span data-stu-id="8d910-125">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="8d910-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d910-126">Request headers</span></span>
| <span data-ttu-id="8d910-127">标头</span><span class="sxs-lookup"><span data-stu-id="8d910-127">Header</span></span>       | <span data-ttu-id="8d910-128">值</span><span class="sxs-lookup"><span data-stu-id="8d910-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d910-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d910-129">Authorization</span></span>  | <span data-ttu-id="8d910-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d910-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d910-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d910-132">Request body</span></span>
<span data-ttu-id="8d910-133">在请求正文中，提供包含**post**参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8d910-133">In the request body, provide a JSON object that includes a **post** parameter.</span></span>

| <span data-ttu-id="8d910-134">参数</span><span class="sxs-lookup"><span data-stu-id="8d910-134">Parameter</span></span>    | <span data-ttu-id="8d910-135">类型</span><span class="sxs-lookup"><span data-stu-id="8d910-135">Type</span></span>   |<span data-ttu-id="8d910-136">说明</span><span class="sxs-lookup"><span data-stu-id="8d910-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d910-137">帖子</span><span class="sxs-lookup"><span data-stu-id="8d910-137">post</span></span>|[<span data-ttu-id="8d910-138">帖子</span><span class="sxs-lookup"><span data-stu-id="8d910-138">post</span></span>](../resources/post.md)|<span data-ttu-id="8d910-139">要答复的新帖子，其中包含[附件](../resources/attachment.md)集合中的一个或多个附件。</span><span class="sxs-lookup"><span data-stu-id="8d910-139">The new post that is being replied with, which includes one or more attachments in an [attachment](../resources/attachment.md) collection.</span></span>|

## <a name="response"></a><span data-ttu-id="8d910-140">响应</span><span class="sxs-lookup"><span data-stu-id="8d910-140">Response</span></span>

<span data-ttu-id="8d910-p104">如果成功，此方法返回 `202 Accepted` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="8d910-p104">If successful, this method returns `202 Accepted` response code. It does not return a response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d910-143">示例</span><span class="sxs-lookup"><span data-stu-id="8d910-143">Examples</span></span>
### <a name="example-1-include-a-file-attachment"></a><span data-ttu-id="8d910-144">示例1：包含文件附件</span><span class="sxs-lookup"><span data-stu-id="8d910-144">Example 1: Include a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="8d910-145">请求</span><span class="sxs-lookup"><span data-stu-id="8d910-145">Request</span></span>
<span data-ttu-id="8d910-146">下面的示例展示了在创建帖子时将文件作为附件包含的一个请求。</span><span class="sxs-lookup"><span data-stu-id="8d910-146">Here is an example of a request that includes a file as an attachment when creating a post.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d910-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d910-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8d910-148">C#</span><span class="sxs-lookup"><span data-stu-id="8d910-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d910-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d910-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d910-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d910-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8d910-151">响应</span><span class="sxs-lookup"><span data-stu-id="8d910-151">Response</span></span>
<span data-ttu-id="8d910-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8d910-152">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
```

### <a name="example-2-include-an-item-attachment"></a><span data-ttu-id="8d910-153">示例2：包含项目附件</span><span class="sxs-lookup"><span data-stu-id="8d910-153">Example 2: Include an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="8d910-154">请求</span><span class="sxs-lookup"><span data-stu-id="8d910-154">Request</span></span>
<span data-ttu-id="8d910-155">下面的示例展示了在创建帖子时将事件作为附件包含的一个请求。</span><span class="sxs-lookup"><span data-stu-id="8d910-155">Here is an example of a request that includes an event as an attachment when creating a post.</span></span>

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


#### <a name="response"></a><span data-ttu-id="8d910-156">响应</span><span class="sxs-lookup"><span data-stu-id="8d910-156">Response</span></span>
<span data-ttu-id="8d910-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8d910-157">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-include-a-reference-attachment"></a><span data-ttu-id="8d910-158">示例3：包含引用附件</span><span class="sxs-lookup"><span data-stu-id="8d910-158">Example 3: Include a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="8d910-159">请求</span><span class="sxs-lookup"><span data-stu-id="8d910-159">Request</span></span>
<span data-ttu-id="8d910-160">下面的示例展示了在创建帖子时包含参考附件的请求。</span><span class="sxs-lookup"><span data-stu-id="8d910-160">Here is an example of a request that includes a reference attachment when creating a post.</span></span>
<span data-ttu-id="8d910-161">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="8d910-161">The attachment points to a folder on OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d910-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d910-162">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="8d910-163">C#</span><span class="sxs-lookup"><span data-stu-id="8d910-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d910-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d910-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d910-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d910-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d910-166">响应</span><span class="sxs-lookup"><span data-stu-id="8d910-166">Response</span></span>
<span data-ttu-id="8d910-167">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8d910-167">Here is an example of the response.</span></span>
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
