---
title: 获取附件
description: 读取附加到事件、邮件、Outlook 任务或帖子的附件的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: 6759953148245935e5a2dc2b0825a7c55af18dc3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128874"
---
# <a name="get-attachment"></a><span data-ttu-id="9946e-103">获取附件</span><span class="sxs-lookup"><span data-stu-id="9946e-103">Get attachment</span></span>

<span data-ttu-id="9946e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9946e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="9946e-105">读取附加到用户事件、邮件[、Outlook](../resources/outlooktask.md)任务或组帖子的附件的属性、关系或[](../resources/event.md)原始[内容](../resources/post.md)。 [](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="9946e-105">Read the properties, relationships, or raw contents of an attachment that is attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md).</span></span> 

<span data-ttu-id="9946e-106">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="9946e-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="9946e-107">文件。</span><span class="sxs-lookup"><span data-stu-id="9946e-107">A file.</span></span> <span data-ttu-id="9946e-108">采用编程方式，这是 [fileAttachment](../resources/fileattachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="9946e-108">Programmatically, this is a [fileAttachment](../resources/fileattachment.md) resource.</span></span>
* <span data-ttu-id="9946e-109">Outlook 项目（联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="9946e-109">An Outlook item (contact, event or message).</span></span> <span data-ttu-id="9946e-110">采用编程方式，项目附件是 [itemAttachment](../resources/itemattachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="9946e-110">Programmatically, an item attachment is an [itemAttachment](../resources/itemattachment.md) resource.</span></span> <span data-ttu-id="9946e-111">可使用 `$expand` 来进一步获取该项的属性。</span><span class="sxs-lookup"><span data-stu-id="9946e-111">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="9946e-112">请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="9946e-112">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="9946e-113">指向存储在云中的文件的链接。</span><span class="sxs-lookup"><span data-stu-id="9946e-113">A link to a file stored in the cloud.</span></span> <span data-ttu-id="9946e-114">采用编程方式，这是 [referenceAttachment](../resources/referenceattachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="9946e-114">Programmatically, this is a [referenceAttachment](../resources/referenceattachment.md) resource.</span></span>

<span data-ttu-id="9946e-115">所有这些类型的附件都派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="9946e-115">All these types of attachments are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="9946e-116">获取文件或项目附件的原始内容</span><span class="sxs-lookup"><span data-stu-id="9946e-116">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="9946e-117">你可以附加路径段 `/$value` 以获取文件或项目附件的原始内容。</span><span class="sxs-lookup"><span data-stu-id="9946e-117">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="9946e-118">对于文件附件，内容类型基于其原始内容类型。</span><span class="sxs-lookup"><span data-stu-id="9946e-118">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="9946e-119">请参阅以下[示例](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="9946e-119">See an [example](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) below.</span></span>

<span data-ttu-id="9946e-120">对于作为[联系人](../resources/contact.md)、[事件](../resources/event.md)或[邮件](../resources/message.md)的项目附件，返回的原始内容为 MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="9946e-120">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="9946e-121">项目附件类型</span><span class="sxs-lookup"><span data-stu-id="9946e-121">Item attachment type</span></span>  | <span data-ttu-id="9946e-122">返回的原始内容</span><span class="sxs-lookup"><span data-stu-id="9946e-122">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="9946e-123">**联系人**</span><span class="sxs-lookup"><span data-stu-id="9946e-123">**contact**</span></span> | <span data-ttu-id="9946e-124">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="9946e-124">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="9946e-125">请参阅[示例](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="9946e-125">See [example](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="9946e-126">**事件**</span><span class="sxs-lookup"><span data-stu-id="9946e-126">**event**</span></span> | <span data-ttu-id="9946e-127">iCal MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="9946e-127">iCal MIME format.</span></span> <span data-ttu-id="9946e-128">请参阅[示例](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="9946e-128">See [example](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="9946e-129">**邮件**</span><span class="sxs-lookup"><span data-stu-id="9946e-129">**message**</span></span> | <span data-ttu-id="9946e-130">MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="9946e-130">MIME format.</span></span> <span data-ttu-id="9946e-131">请参阅[示例](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="9946e-131">See [example](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="9946e-132">尝试获取参考附件的 `$value` 时返回 HTTP 405。</span><span class="sxs-lookup"><span data-stu-id="9946e-132">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="9946e-133">权限</span><span class="sxs-lookup"><span data-stu-id="9946e-133">Permissions</span></span>

<span data-ttu-id="9946e-134">根据 **附件所附加到** 的资源 **(** 事件、邮件 **、outlookTask** 或 post) 以及请求的权限类型 (委派或应用程序) ，下表中指定的权限是调用此 API 所需的最小特权。</span><span class="sxs-lookup"><span data-stu-id="9946e-134">Depending on the resource (**event**, **message**, **outlookTask**, or **post**) that the attachment is attached to and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="9946e-135">若要了解详细信息，包括在选择更多特权之前的[注意事项](/graph/auth/auth-concepts#best-practices-for-requesting-permissions)，请在“[权限](/graph/permissions-reference)”中搜索以下权限。</span><span class="sxs-lookup"><span data-stu-id="9946e-135">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9946e-136">支持的资源</span><span class="sxs-lookup"><span data-stu-id="9946e-136">Supported resource</span></span> | <span data-ttu-id="9946e-137">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9946e-137">Delegated (work or school account)</span></span> | <span data-ttu-id="9946e-138">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9946e-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9946e-139">应用程序</span><span class="sxs-lookup"><span data-stu-id="9946e-139">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="9946e-140">事件</span><span class="sxs-lookup"><span data-stu-id="9946e-140">event</span></span>](../resources/event.md) | <span data-ttu-id="9946e-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9946e-141">Calendars.Read</span></span> | <span data-ttu-id="9946e-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9946e-142">Calendars.Read</span></span> | <span data-ttu-id="9946e-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9946e-143">Calendars.Read</span></span> |
| [<span data-ttu-id="9946e-144">邮件</span><span class="sxs-lookup"><span data-stu-id="9946e-144">message</span></span>](../resources/message.md) | <span data-ttu-id="9946e-145">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9946e-145">Mail.Read</span></span> | <span data-ttu-id="9946e-146">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9946e-146">Mail.Read</span></span> | <span data-ttu-id="9946e-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9946e-147">Mail.Read</span></span> |
| [<span data-ttu-id="9946e-148">outlookTask</span><span class="sxs-lookup"><span data-stu-id="9946e-148">outlookTask</span></span>](../resources/outlooktask.md) |  <span data-ttu-id="9946e-149">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="9946e-149">Tasks.Read</span></span> | <span data-ttu-id="9946e-150">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="9946e-150">Tasks.Read</span></span> | <span data-ttu-id="9946e-151">不支持</span><span class="sxs-lookup"><span data-stu-id="9946e-151">Not supported</span></span> |
| [<span data-ttu-id="9946e-152">帖子</span><span class="sxs-lookup"><span data-stu-id="9946e-152">post</span></span>](../resources/post.md) | <span data-ttu-id="9946e-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9946e-153">Group.Read.All</span></span> | <span data-ttu-id="9946e-154">不支持</span><span class="sxs-lookup"><span data-stu-id="9946e-154">Not supported</span></span> | <span data-ttu-id="9946e-155">不支持</span><span class="sxs-lookup"><span data-stu-id="9946e-155">Not supported</span></span> |


<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="9946e-156">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9946e-156">HTTP request</span></span>

<span data-ttu-id="9946e-157">此部分显示每个实体的 HTTP GET 请求语法， ([事件](../resources/event.md)、邮件[、Outlook](../resources/outlooktask.md)任务和支持附件) 发布[](../resources/post.md)消息： [](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="9946e-157">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), and [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="9946e-158">若要获取附件的属性和关系，请指定要索引到附件集合、附加到指定事件、邮件[、Outlook](../resources/outlooktask.md)任务或[](../resources/event.md)post[](../resources/message.md)实例的[附件](../resources/post.md)ID。</span><span class="sxs-lookup"><span data-stu-id="9946e-158">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="9946e-159">如果附件是文件或 Outlook 项目（联系人、事件或邮件），则可以通过将路径段 `/$value` 附加到请求 URL 来进一步获取附件的原始内容。</span><span class="sxs-lookup"><span data-stu-id="9946e-159">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="9946e-160">事件的 [附件](../resources/event.md)：</span><span class="sxs-lookup"><span data-stu-id="9946e-160">An attachment of an [event](../resources/event.md):</span></span>

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

<span data-ttu-id="9946e-161">用户 [邮箱中的](../resources/message.md) 邮件附件：</span><span class="sxs-lookup"><span data-stu-id="9946e-161">An attachment of a [message](../resources/message.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="9946e-162">用户邮箱 [中](../resources/message.md) 顶级 [mailFolder](../resources/mailfolder.md) 中包含的邮件附件：</span><span class="sxs-lookup"><span data-stu-id="9946e-162">An attachment of a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="9946e-163">用户邮箱 [中](../resources/message.md) [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的邮件附件：</span><span class="sxs-lookup"><span data-stu-id="9946e-163">An attachment of a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="9946e-164">前面的示例显示了一个嵌套级别，但邮件可以位于子级的子级中，等等。</span><span class="sxs-lookup"><span data-stu-id="9946e-164">The preceding example shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>

<span data-ttu-id="9946e-165">Outlook 任务的 [附件](../resources/outlooktask.md)：</span><span class="sxs-lookup"><span data-stu-id="9946e-165">An attachment of an [Outlook task](../resources/outlooktask.md):</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments/{id}
GET /users/{id}/outlook/tasks/{id}/attachments/{id}
GET /me/outlook/tasks/{id}/attachments/{id}/$value
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

<span data-ttu-id="9946e-166">属于组[对话](../resources/post.md)[的主题](../resources/conversationthread.md)中的帖子附件： [](../resources/conversation.md)</span><span class="sxs-lookup"><span data-stu-id="9946e-166">An attachment of a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9946e-167">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9946e-167">Optional query parameters</span></span>

<span data-ttu-id="9946e-168">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9946e-168">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9946e-169">请求标头</span><span class="sxs-lookup"><span data-stu-id="9946e-169">Request headers</span></span>

| <span data-ttu-id="9946e-170">名称</span><span class="sxs-lookup"><span data-stu-id="9946e-170">Name</span></span>       | <span data-ttu-id="9946e-171">类型</span><span class="sxs-lookup"><span data-stu-id="9946e-171">Type</span></span> | <span data-ttu-id="9946e-172">说明</span><span class="sxs-lookup"><span data-stu-id="9946e-172">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9946e-173">Authorization</span><span class="sxs-lookup"><span data-stu-id="9946e-173">Authorization</span></span>  | <span data-ttu-id="9946e-174">string</span><span class="sxs-lookup"><span data-stu-id="9946e-174">string</span></span>  | <span data-ttu-id="9946e-p109">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9946e-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9946e-177">请求正文</span><span class="sxs-lookup"><span data-stu-id="9946e-177">Request body</span></span>

<span data-ttu-id="9946e-178">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9946e-178">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9946e-179">响应</span><span class="sxs-lookup"><span data-stu-id="9946e-179">Response</span></span>

<span data-ttu-id="9946e-180">如果成功，GET 方法将返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9946e-180">If successful, the GET method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="9946e-181">如果要获取附件的属性和关系，则响应正文应包含 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9946e-181">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span>
<span data-ttu-id="9946e-182">返回附件类型的属性：[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)。</span><span class="sxs-lookup"><span data-stu-id="9946e-182">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

<span data-ttu-id="9946e-183">如果要获取文件或项目附件的原始内容，则响应正文应包含附件的原始值。</span><span class="sxs-lookup"><span data-stu-id="9946e-183">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="9946e-184">示例</span><span class="sxs-lookup"><span data-stu-id="9946e-184">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="9946e-185">示例 1：获取文件附件的属性</span><span class="sxs-lookup"><span data-stu-id="9946e-185">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="9946e-186">请求</span><span class="sxs-lookup"><span data-stu-id="9946e-186">Request</span></span>

<span data-ttu-id="9946e-187">下面是请求获取邮件上文件附件的属性的示例。</span><span class="sxs-lookup"><span data-stu-id="9946e-187">Here is an example of the request to get the properties of a file attachment on a message.</span></span>

# <a name="http"></a>[<span data-ttu-id="9946e-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="9946e-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment_beta",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="c"></a>[<span data-ttu-id="9946e-189">C#</span><span class="sxs-lookup"><span data-stu-id="9946e-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9946e-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9946e-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9946e-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9946e-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9946e-192">Java</span><span class="sxs-lookup"><span data-stu-id="9946e-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9946e-193">响应</span><span class="sxs-lookup"><span data-stu-id="9946e-193">Response</span></span>

<span data-ttu-id="9946e-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9946e-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="9946e-197">示例 2：获取项目附件的属性</span><span class="sxs-lookup"><span data-stu-id="9946e-197">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="9946e-198">请求</span><span class="sxs-lookup"><span data-stu-id="9946e-198">Request</span></span>

<span data-ttu-id="9946e-199">下一个示例演示如何在邮件上获取项目附件。</span><span class="sxs-lookup"><span data-stu-id="9946e-199">The next example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="9946e-200">返回 **itemAttachment** 的属性。</span><span class="sxs-lookup"><span data-stu-id="9946e-200">The properties of the **itemAttachment** are returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="9946e-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="9946e-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```
# <a name="c"></a>[<span data-ttu-id="9946e-202">C#</span><span class="sxs-lookup"><span data-stu-id="9946e-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9946e-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9946e-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9946e-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9946e-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9946e-205">Java</span><span class="sxs-lookup"><span data-stu-id="9946e-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9946e-206">响应</span><span class="sxs-lookup"><span data-stu-id="9946e-206">Response</span></span>
<span data-ttu-id="9946e-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9946e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="9946e-210">示例 3：展开并获取附加到邮件的项目的属性</span><span class="sxs-lookup"><span data-stu-id="9946e-210">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="9946e-211">请求</span><span class="sxs-lookup"><span data-stu-id="9946e-211">Request</span></span>

<span data-ttu-id="9946e-212">下一个示例演示如何使用 `$expand` 来获取附加到该邮件的项目（联系人、事件或邮件）的属性。</span><span class="sxs-lookup"><span data-stu-id="9946e-212">The next example shows how to use `$expand` to get the properties of the item (contact, event, or message) that is attached to the message.</span></span> <span data-ttu-id="9946e-213">在此示例中，该项目是一封邮件；还会返回该附加邮件的属性。</span><span class="sxs-lookup"><span data-stu-id="9946e-213">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="9946e-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="9946e-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```
# <a name="c"></a>[<span data-ttu-id="9946e-215">C#</span><span class="sxs-lookup"><span data-stu-id="9946e-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9946e-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9946e-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9946e-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9946e-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9946e-218">Java</span><span class="sxs-lookup"><span data-stu-id="9946e-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9946e-219">响应</span><span class="sxs-lookup"><span data-stu-id="9946e-219">Response</span></span>
<span data-ttu-id="9946e-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9946e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-4-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="9946e-223">示例 4：获取参考附件的属性</span><span class="sxs-lookup"><span data-stu-id="9946e-223">Example 4: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="9946e-224">请求</span><span class="sxs-lookup"><span data-stu-id="9946e-224">Request</span></span>

<span data-ttu-id="9946e-225">下面的示例展示了用于获取事件的参考附件的请求。</span><span class="sxs-lookup"><span data-stu-id="9946e-225">Here is an example of the request to get a reference attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="9946e-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="9946e-226">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGE1M88AADUv0uAAAG=","AAMkAGE1Mg72tgf7hJp0PICVGCc0g="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```
# <a name="c"></a>[<span data-ttu-id="9946e-227">C#</span><span class="sxs-lookup"><span data-stu-id="9946e-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9946e-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9946e-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9946e-229">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9946e-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9946e-230">Java</span><span class="sxs-lookup"><span data-stu-id="9946e-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9946e-231">响应</span><span class="sxs-lookup"><span data-stu-id="9946e-231">Response</span></span>
<span data-ttu-id="9946e-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9946e-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


### <a name="example-5-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="9946e-235">示例 5：获取邮件上的文件附件的原始内容</span><span class="sxs-lookup"><span data-stu-id="9946e-235">Example 5: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="9946e-236">请求</span><span class="sxs-lookup"><span data-stu-id="9946e-236">Request</span></span>

<span data-ttu-id="9946e-237">下面是请求获取已附加到邮件的 Word 文件原始内容的示例。</span><span class="sxs-lookup"><span data-stu-id="9946e-237">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="9946e-238">响应</span><span class="sxs-lookup"><span data-stu-id="9946e-238">Response</span></span>
<span data-ttu-id="9946e-239">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9946e-239">Here is an example of the response.</span></span> <span data-ttu-id="9946e-240">实际响应正文包含文件附件的原始字节，为简洁起见，此处为缩写。</span><span class="sxs-lookup"><span data-stu-id="9946e-240">The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="9946e-241">示例 6：获取邮件上的联系人附件的 MIME 原始内容</span><span class="sxs-lookup"><span data-stu-id="9946e-241">Example 6: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="9946e-242">请求</span><span class="sxs-lookup"><span data-stu-id="9946e-242">Request</span></span>

<span data-ttu-id="9946e-243">下面是请求获取已附加到邮件的联系人项目原始内容的示例。</span><span class="sxs-lookup"><span data-stu-id="9946e-243">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="9946e-244">响应</span><span class="sxs-lookup"><span data-stu-id="9946e-244">Response</span></span>
<span data-ttu-id="9946e-245">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9946e-245">Here is an example of the response.</span></span> 

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


### <a name="example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="9946e-246">示例 7：获取邮件上的事件附件的 MIME 原始内容</span><span class="sxs-lookup"><span data-stu-id="9946e-246">Example 7: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="9946e-247">请求</span><span class="sxs-lookup"><span data-stu-id="9946e-247">Request</span></span>

<span data-ttu-id="9946e-248">下面是请求获取已附加到邮件的事件原始内容的示例。</span><span class="sxs-lookup"><span data-stu-id="9946e-248">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="9946e-249">响应</span><span class="sxs-lookup"><span data-stu-id="9946e-249">Response</span></span>
<span data-ttu-id="9946e-250">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9946e-250">Here is an example of the response.</span></span> 

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


### <a name="example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="9946e-251">示例 8：获取邮件上的会议邀请项目附件的 MIME 原始内容</span><span class="sxs-lookup"><span data-stu-id="9946e-251">Example 8: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="9946e-252">请求</span><span class="sxs-lookup"><span data-stu-id="9946e-252">Request</span></span>

<span data-ttu-id="9946e-253">下面是请求获取已附加到邮件的会议邀请（[eventMessage](../resources/eventmessage.md) 类型）的原始内容的示例。</span><span class="sxs-lookup"><span data-stu-id="9946e-253">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="9946e-254">**eventMessage** 实体基于 **邮件** 类型。</span><span class="sxs-lookup"><span data-stu-id="9946e-254">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="9946e-255">响应</span><span class="sxs-lookup"><span data-stu-id="9946e-255">Response</span></span>
<span data-ttu-id="9946e-256">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9946e-256">Here is an example of the response.</span></span> 

<span data-ttu-id="9946e-257">响应正文包含 MIME 格式的 **eventMessage** 附件。</span><span class="sxs-lookup"><span data-stu-id="9946e-257">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="9946e-258">为简洁起见，已截断 **eventMessage** 的正文。</span><span class="sxs-lookup"><span data-stu-id="9946e-258">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="9946e-259">可通过实际调用返回完整的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="9946e-259">The full message body is returned from an actual call.</span></span>

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
