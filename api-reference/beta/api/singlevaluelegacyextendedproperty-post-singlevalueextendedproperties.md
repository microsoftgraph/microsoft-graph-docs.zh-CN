---
title: 创建单值扩展属性
description: '在新建或现有的资源实例中创建一个或多个单值扩展属性。 '
ms.openlocfilehash: c55ab01ecde214feb38857e8d77f83eb3bfbabc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043439"
---
# <a name="create-single-value-extended-property"></a><span data-ttu-id="d8c01-103">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="d8c01-103">Create single-value extended property</span></span>

> <span data-ttu-id="d8c01-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d8c01-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8c01-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d8c01-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8c01-106">在新建或现有的资源实例中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d8c01-106">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="d8c01-107">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="d8c01-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="d8c01-108">日历</span><span class="sxs-lookup"><span data-stu-id="d8c01-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="d8c01-109">联系人</span><span class="sxs-lookup"><span data-stu-id="d8c01-109">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="d8c01-110">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d8c01-110">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="d8c01-111">事件</span><span class="sxs-lookup"><span data-stu-id="d8c01-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="d8c01-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d8c01-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="d8c01-113">message</span><span class="sxs-lookup"><span data-stu-id="d8c01-113">message</span></span>](../resources/message.md)
- [<span data-ttu-id="d8c01-114">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="d8c01-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="d8c01-115">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="d8c01-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="d8c01-116">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="d8c01-116">As well as the following group resources:</span></span>

- <span data-ttu-id="d8c01-117">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="d8c01-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="d8c01-118">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="d8c01-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="d8c01-119">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="d8c01-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="d8c01-120">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="d8c01-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8c01-121">权限</span><span class="sxs-lookup"><span data-stu-id="d8c01-121">Permissions</span></span>
<span data-ttu-id="d8c01-122">正在根据资源创建中的扩展的属性和权限键入 （委派或应用程序） 您请求，至少要调用此 API 是下表中所指定的权限。</span><span class="sxs-lookup"><span data-stu-id="d8c01-122">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="d8c01-123">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8c01-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8c01-124">支持的资源</span><span class="sxs-lookup"><span data-stu-id="d8c01-124">Supported resource</span></span> | <span data-ttu-id="d8c01-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8c01-125">Delegated (work or school account)</span></span> | <span data-ttu-id="d8c01-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8c01-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8c01-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8c01-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="d8c01-128">日历</span><span class="sxs-lookup"><span data-stu-id="d8c01-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="d8c01-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-129">Calendars.ReadWrite</span></span> | <span data-ttu-id="d8c01-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-130">Calendars.ReadWrite</span></span> | <span data-ttu-id="d8c01-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-131">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="d8c01-132">联系人</span><span class="sxs-lookup"><span data-stu-id="d8c01-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="d8c01-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="d8c01-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="d8c01-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-135">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="d8c01-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d8c01-136">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="d8c01-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-137">Contacts.ReadWrite</span></span> | <span data-ttu-id="d8c01-138">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-138">Contacts.ReadWrite</span></span> | <span data-ttu-id="d8c01-139">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-139">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="d8c01-140">事件</span><span class="sxs-lookup"><span data-stu-id="d8c01-140">event</span></span>](../resources/event.md) | <span data-ttu-id="d8c01-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-141">Calendars.ReadWrite</span></span> | <span data-ttu-id="d8c01-142">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-142">Calendars.ReadWrite</span></span> |  <span data-ttu-id="d8c01-143">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-143">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="d8c01-144">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="d8c01-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="d8c01-145">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8c01-145">Group.ReadWrite.All</span></span> | <span data-ttu-id="d8c01-146">不支持</span><span class="sxs-lookup"><span data-stu-id="d8c01-146">Not supported</span></span> | <span data-ttu-id="d8c01-147">不支持</span><span class="sxs-lookup"><span data-stu-id="d8c01-147">Not supported</span></span> |
| <span data-ttu-id="d8c01-148">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="d8c01-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="d8c01-149">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8c01-149">Group.ReadWrite.All</span></span> | <span data-ttu-id="d8c01-150">不支持</span><span class="sxs-lookup"><span data-stu-id="d8c01-150">Not supported</span></span> | <span data-ttu-id="d8c01-151">不支持</span><span class="sxs-lookup"><span data-stu-id="d8c01-151">Not supported</span></span> |
| <span data-ttu-id="d8c01-152">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="d8c01-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="d8c01-153">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8c01-153">Group.ReadWrite.All</span></span> | <span data-ttu-id="d8c01-154">不支持</span><span class="sxs-lookup"><span data-stu-id="d8c01-154">Not supported</span></span> | <span data-ttu-id="d8c01-155">不支持</span><span class="sxs-lookup"><span data-stu-id="d8c01-155">Not supported</span></span> |
| [<span data-ttu-id="d8c01-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d8c01-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="d8c01-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-157">Mail.ReadWrite</span></span> | <span data-ttu-id="d8c01-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-158">Mail.ReadWrite</span></span> | <span data-ttu-id="d8c01-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-159">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="d8c01-160">邮件</span><span class="sxs-lookup"><span data-stu-id="d8c01-160">message</span></span>](../resources/message.md) | <span data-ttu-id="d8c01-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-161">Mail.ReadWrite</span></span> | <span data-ttu-id="d8c01-162">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-162">Mail.ReadWrite</span></span> | <span data-ttu-id="d8c01-163">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-163">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="d8c01-164">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="d8c01-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="d8c01-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="d8c01-166">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-166">Tasks.ReadWrite</span></span> | <span data-ttu-id="d8c01-167">不支持</span><span class="sxs-lookup"><span data-stu-id="d8c01-167">Not supported</span></span> |
| [<span data-ttu-id="d8c01-168">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="d8c01-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="d8c01-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="d8c01-170">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8c01-170">Tasks.ReadWrite</span></span> | <span data-ttu-id="d8c01-171">不支持</span><span class="sxs-lookup"><span data-stu-id="d8c01-171">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="d8c01-172">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8c01-172">HTTP request</span></span>
<span data-ttu-id="d8c01-173">可以在新建或现有的资源实例中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d8c01-173">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="d8c01-174">若要创建_新_资源实例中的一个或多个扩展的属性，使用相同的 REST 请求作为创建该实例，并在请求正文中包含的新资源实例_和扩展的属性_的属性。</span><span class="sxs-lookup"><span data-stu-id="d8c01-174">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="d8c01-175">注意一些资源，以多种方式支持创建。</span><span class="sxs-lookup"><span data-stu-id="d8c01-175">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="d8c01-176">有关创建这些资源实例的详细信息，请参阅创建[消息](../resources/message.md)、 [mailFolder](../api/user-post-mailfolders.md)、[事件](../api/user-post-events.md)、[日历](../api/user-post-calendars.md)、[联系人](../api/user-post-contacts.md)、 [contactFolder](../api/user-post-contactfolders.md)，相应主题[Outlook 任务](../resources/outlooktask.md)、 [Outlook 任务文件夹](../resources/outlooktaskfolder.md)，[组事件](../api/group-post-events.md)，并[组文章](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="d8c01-176">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="d8c01-177">以下是请求的语法。</span><span class="sxs-lookup"><span data-stu-id="d8c01-177">The following is the syntax of the requests.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
POST /me/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks

POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="d8c01-178">若要在现有资源实例中创建一个或多个扩展属性，请在请求中指定实例，并在请求正文中包括扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d8c01-178">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="d8c01-179">**注意**不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d8c01-179">**Note** You cannot create an extended property in an existing group post.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
PATCH /me/outlook/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}

PATCH /me/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d8c01-180">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8c01-180">Request headers</span></span>
| <span data-ttu-id="d8c01-181">名称</span><span class="sxs-lookup"><span data-stu-id="d8c01-181">Name</span></span>       | <span data-ttu-id="d8c01-182">值</span><span class="sxs-lookup"><span data-stu-id="d8c01-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d8c01-183">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8c01-183">Authorization</span></span> | <span data-ttu-id="d8c01-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8c01-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8c01-186">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8c01-186">Content-Type</span></span> | <span data-ttu-id="d8c01-187">application/json</span><span class="sxs-lookup"><span data-stu-id="d8c01-187">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8c01-188">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8c01-188">Request body</span></span>

<span data-ttu-id="d8c01-189">提供每个 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象在资源实例的 **singleValueExtendedProperties** 集合属性中的 JSON 正文。</span><span class="sxs-lookup"><span data-stu-id="d8c01-189">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="d8c01-190">**属性**</span><span class="sxs-lookup"><span data-stu-id="d8c01-190">**Property**</span></span>|<span data-ttu-id="d8c01-191">**类型**</span><span class="sxs-lookup"><span data-stu-id="d8c01-191">**Type**</span></span>|<span data-ttu-id="d8c01-192">**说明**</span><span class="sxs-lookup"><span data-stu-id="d8c01-192">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d8c01-193">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d8c01-193">singleValueExtendedProperties</span></span>|<span data-ttu-id="d8c01-194">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="d8c01-194">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d8c01-195">一个或多个单值扩展属性的数组。</span><span class="sxs-lookup"><span data-stu-id="d8c01-195">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="d8c01-196">id</span><span class="sxs-lookup"><span data-stu-id="d8c01-196">id</span></span>|<span data-ttu-id="d8c01-197">String</span><span class="sxs-lookup"><span data-stu-id="d8c01-197">String</span></span>|<span data-ttu-id="d8c01-p105">对于 **singleValueExtendedProperties** 集合中的每个属性，请指定此参数以标识属性。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="d8c01-p105">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="d8c01-202">值</span><span class="sxs-lookup"><span data-stu-id="d8c01-202">value</span></span>|<span data-ttu-id="d8c01-203">string</span><span class="sxs-lookup"><span data-stu-id="d8c01-203">string</span></span>|<span data-ttu-id="d8c01-p106">对于 **singleValueExtendedProperties** 集合中的每个属性，请指定属性值。必需。</span><span class="sxs-lookup"><span data-stu-id="d8c01-p106">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="d8c01-206">在_新的_资源实例中创建扩展属性时，除了新的 **singleValueExtendedProperties** 集合，请提供资源实例的 JSON 表示形式（即 [邮件](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md) 等）。</span><span class="sxs-lookup"><span data-stu-id="d8c01-206">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="d8c01-207">响应</span><span class="sxs-lookup"><span data-stu-id="d8c01-207">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="d8c01-208">响应代码</span><span class="sxs-lookup"><span data-stu-id="d8c01-208">Response code</span></span>
<span data-ttu-id="d8c01-209">在新建资源实例中成功创建扩展属性的操作返回 `201 Created`（在新的组帖子中除外），根据所用的方法，该操作可以返回 `200 OK` 或 `202 Accepted`。</span><span class="sxs-lookup"><span data-stu-id="d8c01-209">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="d8c01-210">在现有的资源实例中，成功的创建操作返回 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="d8c01-210">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="d8c01-211">响应正文</span><span class="sxs-lookup"><span data-stu-id="d8c01-211">Response body</span></span>

<span data-ttu-id="d8c01-p107">创建扩展属性时，该响应只包括新建或现有的实例，但不包括新的扩展属性。若要查看新创建的扩展属性，请 [获取通过扩展属性扩展的实例](../api/singlevaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="d8c01-p107">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="d8c01-214">通过回复线程或帖子在_新建_[组帖子](../resources/post.md)中创建扩展属性时，响应仅包括响应代码，但不包括新帖子或扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d8c01-214">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="d8c01-215">示例</span><span class="sxs-lookup"><span data-stu-id="d8c01-215">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d8c01-216">请求 1</span><span class="sxs-lookup"><span data-stu-id="d8c01-216">Request 1</span></span>

<span data-ttu-id="d8c01-p108">第一个示例在相同的 POST 操作中创建一个新事件和一个单值扩展属性。除了通常要包括的新事件的属性，请求正文还包括 **singleValueExtendedProperties** 集合，该集合包含一个单值扩展属性和以下属性：</span><span class="sxs-lookup"><span data-stu-id="d8c01-p108">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>

- <span data-ttu-id="d8c01-219">**id** 将属性类型指定为 `String`、GUID 和名为 `Fun` 的属性。</span><span class="sxs-lookup"><span data-stu-id="d8c01-219">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="d8c01-220">**value** 将 `Food` 指定为 `Fun` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="d8c01-220">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/events
Content-Type: application/json

{
  "subject": "Celebrate Thanksgiving",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together!"
  },
  "start": {
      "dateTime": "2015-11-26T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-26T23:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    }
  ],
  "singleValueExtendedProperties": [
     {
           "id":"String {66f5a359-4659-4830-9070-00040ec6ac6e} Name Fun",
           "value":"Food"
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="d8c01-221">响应 1</span><span class="sxs-lookup"><span data-stu-id="d8c01-221">Response 1</span></span>

<span data-ttu-id="d8c01-p109">成功的响应由 `HTTP 201 Created` 响应代码表示，并在响应正文中包括新事件，类似于 [仅创建事件](../api/user-post-events.md) 中的响应。该响应不包括任何新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d8c01-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="d8c01-224">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的事件](../api/singlevaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="d8c01-224">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="d8c01-225">请求 2</span><span class="sxs-lookup"><span data-stu-id="d8c01-225">Request 2</span></span>

<span data-ttu-id="d8c01-p110">第二个示例为指定的现有邮件创建一个单值扩展属性。扩展属性是 **singleValueExtendedProperties** 数组中的唯一元素。请求正文包括扩展属性的以下参数：</span><span class="sxs-lookup"><span data-stu-id="d8c01-p110">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="d8c01-229">**id** 将属性类型指定为 `String`、GUID 和名为 `Color` 的属性。</span><span class="sxs-lookup"><span data-stu-id="d8c01-229">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="d8c01-230">**value** 将 `Green` 指定为 `Color` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="d8c01-230">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')

Content-Type: application/json

{
  "singleValueExtendedProperties": [
      {
         "id":"String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
         "value":"Green"
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="d8c01-231">响应 2</span><span class="sxs-lookup"><span data-stu-id="d8c01-231">Response 2</span></span>

<span data-ttu-id="d8c01-p111">成功的响应由 `HTTP 200 OK` 响应代码表示，并在响应正文中包括指定的邮件，类似于 [更新邮件](../api/message-update.md) 中的响应。该响应不包括新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d8c01-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="d8c01-234">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的邮件](../api/singlevaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="d8c01-234">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

