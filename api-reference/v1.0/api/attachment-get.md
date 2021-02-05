---
title: 获取附件
description: '读取附加到事件的附件的属性和关系 '
localization_priority: Priority
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8ffd1ceec1d3dbdb7e30a059836b11cc8e5a0276
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092636"
---
# <a name="get-attachment"></a><span data-ttu-id="16bc2-103">获取附件</span><span class="sxs-lookup"><span data-stu-id="16bc2-103">Get attachment</span></span>

<span data-ttu-id="16bc2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16bc2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16bc2-105">阅读附加到用户[事件](../resources/event.md)、[邮件](../resources/message.md)或组[帖子](../resources/post.md)的附件的属性、关系或原始内容。</span><span class="sxs-lookup"><span data-stu-id="16bc2-105">Read the properties, relationships, or raw contents of an attachment that is attached to a user [event](../resources/event.md), [message](../resources/message.md), or group [post](../resources/post.md).</span></span> 

<span data-ttu-id="16bc2-106">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="16bc2-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="16bc2-107">文件。</span><span class="sxs-lookup"><span data-stu-id="16bc2-107">A file.</span></span> <span data-ttu-id="16bc2-108">采用编程方式，这是 [fileAttachment](../resources/fileattachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="16bc2-108">Programmatically, this is a [fileAttachment](../resources/fileattachment.md) resource.</span></span>
* <span data-ttu-id="16bc2-109">Outlook 项目（联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="16bc2-109">An Outlook item (contact, event or message).</span></span> <span data-ttu-id="16bc2-110">采用编程方式，项目附件是 [itemAttachment](../resources/itemattachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="16bc2-110">Programmatically, an item attachment is an [itemAttachment](../resources/itemattachment.md) resource.</span></span> <span data-ttu-id="16bc2-111">可使用 `$expand` 来进一步获取该项的属性。</span><span class="sxs-lookup"><span data-stu-id="16bc2-111">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="16bc2-112">请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="16bc2-112">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="16bc2-113">指向存储在云中的文件的链接。</span><span class="sxs-lookup"><span data-stu-id="16bc2-113">A link to a file stored in the cloud.</span></span> <span data-ttu-id="16bc2-114">采用编程方式，这是 [referenceAttachment](../resources/referenceattachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="16bc2-114">Programmatically, this is a [referenceAttachment](../resources/referenceattachment.md) resource.</span></span>

<span data-ttu-id="16bc2-115">所有这些类型的附件都派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="16bc2-115">All these types of attachments are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="16bc2-116">获取文件或项目附件的原始内容</span><span class="sxs-lookup"><span data-stu-id="16bc2-116">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="16bc2-117">你可以附加路径段 `/$value` 以获取文件或项目附件的原始内容。</span><span class="sxs-lookup"><span data-stu-id="16bc2-117">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="16bc2-118">对于文件附件，内容类型基于其原始内容类型。</span><span class="sxs-lookup"><span data-stu-id="16bc2-118">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="16bc2-119">请参阅以下[示例](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="16bc2-119">See an [example](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) below.</span></span>

<span data-ttu-id="16bc2-120">对于作为[联系人](../resources/contact.md)、[事件](../resources/event.md)或[邮件](../resources/message.md)的项目附件，返回的原始内容为 MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="16bc2-120">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="16bc2-121">项目附件类型</span><span class="sxs-lookup"><span data-stu-id="16bc2-121">Item attachment type</span></span>  | <span data-ttu-id="16bc2-122">返回的原始内容</span><span class="sxs-lookup"><span data-stu-id="16bc2-122">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="16bc2-123">**联系人**</span><span class="sxs-lookup"><span data-stu-id="16bc2-123">**contact**</span></span> | <span data-ttu-id="16bc2-124">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="16bc2-124">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="16bc2-125">请参阅[示例](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="16bc2-125">See [example](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="16bc2-126">**事件**</span><span class="sxs-lookup"><span data-stu-id="16bc2-126">**event**</span></span> | <span data-ttu-id="16bc2-127">iCal MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="16bc2-127">iCal MIME format.</span></span> <span data-ttu-id="16bc2-128">请参阅[示例](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="16bc2-128">See [example](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="16bc2-129">**邮件**</span><span class="sxs-lookup"><span data-stu-id="16bc2-129">**message**</span></span> | <span data-ttu-id="16bc2-130">MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="16bc2-130">MIME format.</span></span> <span data-ttu-id="16bc2-131">请参阅[示例](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message)。</span><span class="sxs-lookup"><span data-stu-id="16bc2-131">See [example](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="16bc2-132">尝试获取参考附件的 `$value` 时返回 HTTP 405。</span><span class="sxs-lookup"><span data-stu-id="16bc2-132">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="16bc2-133">权限</span><span class="sxs-lookup"><span data-stu-id="16bc2-133">Permissions</span></span>

<span data-ttu-id="16bc2-134">根据附件所附加到的资源（**事件**、**邮件** 或 **帖子**）和请求的权限类型（委派或应用程序），下表中指定的权限是调用此 API 所需的最低特权。</span><span class="sxs-lookup"><span data-stu-id="16bc2-134">Depending on the resource (**event**, **message**, or **post**) that the attachment is attached to and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="16bc2-135">若要了解详细信息，包括在选择更多特权之前的[注意事项](/graph/auth/auth-concepts#best-practices-for-requesting-permissions)，请在“[权限](/graph/permissions-reference)”中搜索以下权限。</span><span class="sxs-lookup"><span data-stu-id="16bc2-135">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16bc2-136">支持的资源</span><span class="sxs-lookup"><span data-stu-id="16bc2-136">Supported resource</span></span> | <span data-ttu-id="16bc2-137">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16bc2-137">Delegated (work or school account)</span></span> | <span data-ttu-id="16bc2-138">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16bc2-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16bc2-139">应用程序</span><span class="sxs-lookup"><span data-stu-id="16bc2-139">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="16bc2-140">事件</span><span class="sxs-lookup"><span data-stu-id="16bc2-140">event</span></span>](../resources/event.md) | <span data-ttu-id="16bc2-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="16bc2-141">Calendars.Read</span></span> | <span data-ttu-id="16bc2-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="16bc2-142">Calendars.Read</span></span> | <span data-ttu-id="16bc2-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="16bc2-143">Calendars.Read</span></span> |
| [<span data-ttu-id="16bc2-144">邮件</span><span class="sxs-lookup"><span data-stu-id="16bc2-144">message</span></span>](../resources/message.md) | <span data-ttu-id="16bc2-145">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="16bc2-145">Mail.Read</span></span> | <span data-ttu-id="16bc2-146">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="16bc2-146">Mail.Read</span></span> | <span data-ttu-id="16bc2-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="16bc2-147">Mail.Read</span></span> |
| [<span data-ttu-id="16bc2-148">帖子</span><span class="sxs-lookup"><span data-stu-id="16bc2-148">post</span></span>](../resources/post.md) | <span data-ttu-id="16bc2-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="16bc2-149">Group.Read.All</span></span> | <span data-ttu-id="16bc2-150">不支持</span><span class="sxs-lookup"><span data-stu-id="16bc2-150">Not supported</span></span> | <span data-ttu-id="16bc2-151">不支持</span><span class="sxs-lookup"><span data-stu-id="16bc2-151">Not supported</span></span> |


<!--
* If accessing attachments in group events or posts: Group.Read.All.
-->

## <a name="http-request"></a><span data-ttu-id="16bc2-152">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16bc2-152">HTTP request</span></span>
<span data-ttu-id="16bc2-153">此部分显示了支持附件的每个实体（[事件](../resources/event.md)、[邮件](../resources/message.md)和[帖子](../resources/post.md)）的 HTTP GET 请求语法：</span><span class="sxs-lookup"><span data-stu-id="16bc2-153">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), and [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="16bc2-154">若要获取附件的属性和关系，请指定要索引到 **附件** 集合的附件 ID，它已附加到指定的 [事件](../resources/event.md)、[邮件](../resources/message.md)或 [帖子](../resources/post.md)实例。</span><span class="sxs-lookup"><span data-stu-id="16bc2-154">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="16bc2-155">如果附件是文件或 Outlook 项目（联系人、事件或邮件），则可以通过将路径段 `/$value` 附加到请求 URL 来进一步获取附件的原始内容。</span><span class="sxs-lookup"><span data-stu-id="16bc2-155">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="16bc2-156">用户的默认[日历](../resources/calendar.md)中的[事件](../resources/event.md)附件。</span><span class="sxs-lookup"><span data-stu-id="16bc2-156">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}

GET /me/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}/$value
```

<span data-ttu-id="16bc2-157">指定的用户[日历](../resources/calendar.md)中的[事件](../resources/event.md)附件。</span><span class="sxs-lookup"><span data-stu-id="16bc2-157">Attachments for an [event](../resources/event.md) in the specified user [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendars/{id}/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}/$value
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
GET /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="16bc2-158">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="16bc2-158">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}/$value
```
<span data-ttu-id="16bc2-159">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="16bc2-159">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}/$value
```
<span data-ttu-id="16bc2-160">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="16bc2-160">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}

GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="16bc2-161">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="16bc2-161">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}

GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="16bc2-p109">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。 </span><span class="sxs-lookup"><span data-stu-id="16bc2-p109">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}

GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="16bc2-164">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="16bc2-164">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}

GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16bc2-165">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="16bc2-165">Optional query parameters</span></span>
<span data-ttu-id="16bc2-166">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="16bc2-166">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="16bc2-167">请求标头</span><span class="sxs-lookup"><span data-stu-id="16bc2-167">Request headers</span></span>
| <span data-ttu-id="16bc2-168">名称</span><span class="sxs-lookup"><span data-stu-id="16bc2-168">Name</span></span>       | <span data-ttu-id="16bc2-169">类型</span><span class="sxs-lookup"><span data-stu-id="16bc2-169">Type</span></span> | <span data-ttu-id="16bc2-170">说明</span><span class="sxs-lookup"><span data-stu-id="16bc2-170">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="16bc2-171">Authorization</span><span class="sxs-lookup"><span data-stu-id="16bc2-171">Authorization</span></span>  | <span data-ttu-id="16bc2-172">string</span><span class="sxs-lookup"><span data-stu-id="16bc2-172">string</span></span>  | <span data-ttu-id="16bc2-p110">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16bc2-p110">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16bc2-175">请求正文</span><span class="sxs-lookup"><span data-stu-id="16bc2-175">Request body</span></span>
<span data-ttu-id="16bc2-176">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16bc2-176">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16bc2-177">响应</span><span class="sxs-lookup"><span data-stu-id="16bc2-177">Response</span></span>

<span data-ttu-id="16bc2-178">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="16bc2-178">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="16bc2-179">如果要获取附件的属性和关系，则响应正文应包含 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="16bc2-179">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span> <span data-ttu-id="16bc2-180">返回附件类型的属性：[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)。</span><span class="sxs-lookup"><span data-stu-id="16bc2-180">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

<span data-ttu-id="16bc2-181">如果要获取文件或项目附件的原始内容，则响应正文应包含附件的原始值。</span><span class="sxs-lookup"><span data-stu-id="16bc2-181">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="16bc2-182">示例</span><span class="sxs-lookup"><span data-stu-id="16bc2-182">Examples</span></span> 

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="16bc2-183">示例 1：获取文件附件的属性</span><span class="sxs-lookup"><span data-stu-id="16bc2-183">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="16bc2-184">请求</span><span class="sxs-lookup"><span data-stu-id="16bc2-184">Request</span></span>

<span data-ttu-id="16bc2-185">下面的示例展示了用于获取事件的文件附件的请求。</span><span class="sxs-lookup"><span data-stu-id="16bc2-185">Here is an example of the request to get a file attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="16bc2-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="16bc2-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment_v1",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="c"></a>[<span data-ttu-id="16bc2-187">C#</span><span class="sxs-lookup"><span data-stu-id="16bc2-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16bc2-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16bc2-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16bc2-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16bc2-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16bc2-190">Java</span><span class="sxs-lookup"><span data-stu-id="16bc2-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="16bc2-191">响应</span><span class="sxs-lookup"><span data-stu-id="16bc2-191">Response</span></span>
<span data-ttu-id="16bc2-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16bc2-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_file_attachment_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKjAAA%3D')/attachments/$entity",
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
### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="16bc2-195">示例 2：获取项目附件的属性</span><span class="sxs-lookup"><span data-stu-id="16bc2-195">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="16bc2-196">请求</span><span class="sxs-lookup"><span data-stu-id="16bc2-196">Request</span></span>

<span data-ttu-id="16bc2-197">下一个示例演示如何在邮件上获取项目附件。</span><span class="sxs-lookup"><span data-stu-id="16bc2-197">The next example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="16bc2-198">返回 **itemAttachment** 的属性。</span><span class="sxs-lookup"><span data-stu-id="16bc2-198">The properties of the **itemAttachment** are returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="16bc2-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="16bc2-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_item_attachment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=
```
# <a name="c"></a>[<span data-ttu-id="16bc2-200">C#</span><span class="sxs-lookup"><span data-stu-id="16bc2-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16bc2-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16bc2-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16bc2-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16bc2-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16bc2-203">Java</span><span class="sxs-lookup"><span data-stu-id="16bc2-203">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="16bc2-204">响应</span><span class="sxs-lookup"><span data-stu-id="16bc2-204">Response</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="16bc2-205">示例 3：展开并获取附加到邮件的项目的属性</span><span class="sxs-lookup"><span data-stu-id="16bc2-205">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="16bc2-206">请求</span><span class="sxs-lookup"><span data-stu-id="16bc2-206">Request</span></span>
<span data-ttu-id="16bc2-207">下一个示例演示如何使用 `$expand` 来获取附加到该邮件的项目（联系人、事件或邮件）的属性。</span><span class="sxs-lookup"><span data-stu-id="16bc2-207">The next example shows how to use `$expand` to get the properties of the item (contact, event, or message) that is attached to the message.</span></span> <span data-ttu-id="16bc2-208">在此示例中，该项目是一封邮件；还会返回该附加邮件的属性。</span><span class="sxs-lookup"><span data-stu-id="16bc2-208">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="16bc2-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="16bc2-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_item_attachment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```
# <a name="c"></a>[<span data-ttu-id="16bc2-210">C#</span><span class="sxs-lookup"><span data-stu-id="16bc2-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16bc2-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16bc2-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16bc2-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16bc2-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16bc2-213">Java</span><span class="sxs-lookup"><span data-stu-id="16bc2-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="16bc2-214">响应</span><span class="sxs-lookup"><span data-stu-id="16bc2-214">Response</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
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
    ]
  }
}
```



### <a name="example-4-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="16bc2-215">示例 4：获取参考附件的属性</span><span class="sxs-lookup"><span data-stu-id="16bc2-215">Example 4: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="16bc2-216">请求</span><span class="sxs-lookup"><span data-stu-id="16bc2-216">Request</span></span>
<span data-ttu-id="16bc2-217">下面的示例展示了用于获取消息的参考附件的请求。</span><span class="sxs-lookup"><span data-stu-id="16bc2-217">Here is an example of the request to get a reference attachment on a message.</span></span>

# <a name="http"></a>[<span data-ttu-id="16bc2-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="16bc2-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGUzY5QKgAAA=","AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKgAAA=/attachments/AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=
```
# <a name="c"></a>[<span data-ttu-id="16bc2-219">C#</span><span class="sxs-lookup"><span data-stu-id="16bc2-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16bc2-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16bc2-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16bc2-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16bc2-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16bc2-222">Java</span><span class="sxs-lookup"><span data-stu-id="16bc2-222">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="16bc2-223">响应</span><span class="sxs-lookup"><span data-stu-id="16bc2-223">Response</span></span>
<span data-ttu-id="16bc2-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16bc2-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKgAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.referenceAttachment",
    "id": "AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=",
    "lastModifiedDateTime": "2019-04-02T02:58:11Z",
    "name": "Sales Invoice Template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 1060,
    "isInline": true
}
```

### <a name="example-5-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="16bc2-227">示例 5：获取邮件上的文件附件的原始内容</span><span class="sxs-lookup"><span data-stu-id="16bc2-227">Example 5: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="16bc2-228">请求</span><span class="sxs-lookup"><span data-stu-id="16bc2-228">Request</span></span>

<span data-ttu-id="16bc2-229">下面是请求获取已附加到邮件的 Word 文件原始内容的示例。</span><span class="sxs-lookup"><span data-stu-id="16bc2-229">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="16bc2-230">响应</span><span class="sxs-lookup"><span data-stu-id="16bc2-230">Response</span></span>
<span data-ttu-id="16bc2-231">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16bc2-231">Here is an example of the response.</span></span> <span data-ttu-id="16bc2-232">实际响应正文包含文件附件的原始字节，为简洁起见，此处为缩写。</span><span class="sxs-lookup"><span data-stu-id="16bc2-232">The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="16bc2-233">示例 6：获取邮件上的联系人附件的 MIME 原始内容</span><span class="sxs-lookup"><span data-stu-id="16bc2-233">Example 6: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="16bc2-234">请求</span><span class="sxs-lookup"><span data-stu-id="16bc2-234">Request</span></span>

<span data-ttu-id="16bc2-235">下面是请求获取已附加到邮件的联系人项目原始内容的示例。</span><span class="sxs-lookup"><span data-stu-id="16bc2-235">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="16bc2-236">响应</span><span class="sxs-lookup"><span data-stu-id="16bc2-236">Response</span></span>
<span data-ttu-id="16bc2-237">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16bc2-237">Here is an example of the response.</span></span> 

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


### <a name="example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="16bc2-238">示例 7：获取邮件上的事件附件的 MIME 原始内容</span><span class="sxs-lookup"><span data-stu-id="16bc2-238">Example 7: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="16bc2-239">请求</span><span class="sxs-lookup"><span data-stu-id="16bc2-239">Request</span></span>

<span data-ttu-id="16bc2-240">下面是请求获取已附加到邮件的事件原始内容的示例。</span><span class="sxs-lookup"><span data-stu-id="16bc2-240">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="16bc2-241">响应</span><span class="sxs-lookup"><span data-stu-id="16bc2-241">Response</span></span>
<span data-ttu-id="16bc2-242">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16bc2-242">Here is an example of the response.</span></span> 

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


### <a name="example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="16bc2-243">示例 8：获取邮件上的会议邀请项目附件的 MIME 原始内容</span><span class="sxs-lookup"><span data-stu-id="16bc2-243">Example 8: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="16bc2-244">请求</span><span class="sxs-lookup"><span data-stu-id="16bc2-244">Request</span></span>

<span data-ttu-id="16bc2-245">下面是请求获取已附加到邮件的会议邀请（[eventMessage](../resources/eventmessage.md) 类型）的原始内容的示例。</span><span class="sxs-lookup"><span data-stu-id="16bc2-245">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="16bc2-246">**eventMessage** 实体基于 **邮件** 类型。</span><span class="sxs-lookup"><span data-stu-id="16bc2-246">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="16bc2-247">响应</span><span class="sxs-lookup"><span data-stu-id="16bc2-247">Response</span></span>
<span data-ttu-id="16bc2-248">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16bc2-248">Here is an example of the response.</span></span> 

<span data-ttu-id="16bc2-249">响应正文包含 MIME 格式的 **eventMessage** 附件。</span><span class="sxs-lookup"><span data-stu-id="16bc2-249">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="16bc2-250">为简洁起见，已截断 **eventMessage** 的正文。</span><span class="sxs-lookup"><span data-stu-id="16bc2-250">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="16bc2-251">可通过实际调用返回完整的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="16bc2-251">The full message body is returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: get_and_expand_item_attachment/item:
      Property 'item' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
