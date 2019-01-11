---
title: 创建多值扩展属性
description: '在新建或现有的资源实例中创建一个或多个多值扩展属性。 '
localization_priority: Normal
ms.openlocfilehash: 54be6f428ac5d7b604093fdad3a03b48b89243a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863047"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="20d47-103">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="20d47-103">Create multi-value extended property</span></span>

> <span data-ttu-id="20d47-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="20d47-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20d47-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="20d47-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="20d47-106">在新建或现有的资源实例中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="20d47-106">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="20d47-107">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="20d47-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="20d47-108">日历</span><span class="sxs-lookup"><span data-stu-id="20d47-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="20d47-109">联系人</span><span class="sxs-lookup"><span data-stu-id="20d47-109">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="20d47-110">contactFolder</span><span class="sxs-lookup"><span data-stu-id="20d47-110">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="20d47-111">事件</span><span class="sxs-lookup"><span data-stu-id="20d47-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="20d47-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="20d47-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="20d47-113">message</span><span class="sxs-lookup"><span data-stu-id="20d47-113">message</span></span>](../resources/message.md)
- [<span data-ttu-id="20d47-114">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="20d47-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="20d47-115">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="20d47-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="20d47-116">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="20d47-116">As well as the following group resources:</span></span>

- <span data-ttu-id="20d47-117">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="20d47-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="20d47-118">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="20d47-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="20d47-119">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="20d47-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="20d47-120">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="20d47-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="20d47-121">权限</span><span class="sxs-lookup"><span data-stu-id="20d47-121">Permissions</span></span>
<span data-ttu-id="20d47-122">正在根据资源创建中的扩展的属性和权限键入 （委派或应用程序） 您请求，至少要调用此 API 是下表中所指定的权限。</span><span class="sxs-lookup"><span data-stu-id="20d47-122">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="20d47-123">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20d47-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20d47-124">支持的资源</span><span class="sxs-lookup"><span data-stu-id="20d47-124">Supported resource</span></span> | <span data-ttu-id="20d47-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20d47-125">Delegated (work or school account)</span></span> | <span data-ttu-id="20d47-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20d47-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20d47-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="20d47-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="20d47-128">日历</span><span class="sxs-lookup"><span data-stu-id="20d47-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="20d47-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-129">Calendars.ReadWrite</span></span> | <span data-ttu-id="20d47-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-130">Calendars.ReadWrite</span></span> | <span data-ttu-id="20d47-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-131">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="20d47-132">联系人</span><span class="sxs-lookup"><span data-stu-id="20d47-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="20d47-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="20d47-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="20d47-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-135">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="20d47-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="20d47-136">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="20d47-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-137">Contacts.ReadWrite</span></span> | <span data-ttu-id="20d47-138">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-138">Contacts.ReadWrite</span></span> | <span data-ttu-id="20d47-139">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-139">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="20d47-140">事件</span><span class="sxs-lookup"><span data-stu-id="20d47-140">event</span></span>](../resources/event.md) | <span data-ttu-id="20d47-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-141">Calendars.ReadWrite</span></span> | <span data-ttu-id="20d47-142">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-142">Calendars.ReadWrite</span></span> |  <span data-ttu-id="20d47-143">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-143">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="20d47-144">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="20d47-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="20d47-145">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d47-145">Group.ReadWrite.All</span></span> | <span data-ttu-id="20d47-146">不支持</span><span class="sxs-lookup"><span data-stu-id="20d47-146">Not supported</span></span> | <span data-ttu-id="20d47-147">不支持</span><span class="sxs-lookup"><span data-stu-id="20d47-147">Not supported</span></span> |
| <span data-ttu-id="20d47-148">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="20d47-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="20d47-149">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d47-149">Group.ReadWrite.All</span></span> | <span data-ttu-id="20d47-150">不支持</span><span class="sxs-lookup"><span data-stu-id="20d47-150">Not supported</span></span> | <span data-ttu-id="20d47-151">不支持</span><span class="sxs-lookup"><span data-stu-id="20d47-151">Not supported</span></span> |
| <span data-ttu-id="20d47-152">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="20d47-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="20d47-153">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d47-153">Group.ReadWrite.All</span></span> | <span data-ttu-id="20d47-154">不支持</span><span class="sxs-lookup"><span data-stu-id="20d47-154">Not supported</span></span> | <span data-ttu-id="20d47-155">不支持</span><span class="sxs-lookup"><span data-stu-id="20d47-155">Not supported</span></span> |
| [<span data-ttu-id="20d47-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="20d47-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="20d47-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-157">Mail.ReadWrite</span></span> | <span data-ttu-id="20d47-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-158">Mail.ReadWrite</span></span> | <span data-ttu-id="20d47-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-159">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="20d47-160">邮件</span><span class="sxs-lookup"><span data-stu-id="20d47-160">message</span></span>](../resources/message.md) | <span data-ttu-id="20d47-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-161">Mail.ReadWrite</span></span> | <span data-ttu-id="20d47-162">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-162">Mail.ReadWrite</span></span> | <span data-ttu-id="20d47-163">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-163">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="20d47-164">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="20d47-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="20d47-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="20d47-166">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-166">Tasks.ReadWrite</span></span> | <span data-ttu-id="20d47-167">不支持</span><span class="sxs-lookup"><span data-stu-id="20d47-167">Not supported</span></span> |
| [<span data-ttu-id="20d47-168">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="20d47-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="20d47-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="20d47-170">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d47-170">Tasks.ReadWrite</span></span> | <span data-ttu-id="20d47-171">不支持</span><span class="sxs-lookup"><span data-stu-id="20d47-171">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="20d47-172">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20d47-172">HTTP request</span></span>
<span data-ttu-id="20d47-173">可以在新建或现有的资源实例中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="20d47-173">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="20d47-174">若要创建_新_资源实例中的一个或多个扩展的属性，使用相同的 REST 请求作为创建该实例，并在请求正文中包含的新资源实例_和扩展的属性_的属性。</span><span class="sxs-lookup"><span data-stu-id="20d47-174">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="20d47-175">注意一些资源，以多种方式支持创建。</span><span class="sxs-lookup"><span data-stu-id="20d47-175">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="20d47-176">有关创建这些资源实例的详细信息，请参阅创建[消息](../resources/message.md)、 [mailFolder](../api/user-post-mailfolders.md)、[事件](../api/user-post-events.md)、[日历](../api/user-post-calendars.md)、[联系人](../api/user-post-contacts.md)、 [contactFolder](../api/user-post-contactfolders.md)，相应主题[Outlook 任务](../resources/outlooktask.md)、 [Outlook 任务文件夹](../resources/outlooktaskfolder.md)，[组事件](../api/group-post-events.md)，并[组文章](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="20d47-176">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="20d47-177">以下是请求的语法。</span><span class="sxs-lookup"><span data-stu-id="20d47-177">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="20d47-178">若要在现有资源实例中创建一个或多个扩展属性，请在请求中指定实例，并在请求正文中包括扩展属性。</span><span class="sxs-lookup"><span data-stu-id="20d47-178">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="20d47-179">**注意**不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="20d47-179">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="20d47-180">请求标头</span><span class="sxs-lookup"><span data-stu-id="20d47-180">Request headers</span></span>
| <span data-ttu-id="20d47-181">名称</span><span class="sxs-lookup"><span data-stu-id="20d47-181">Name</span></span>       | <span data-ttu-id="20d47-182">值</span><span class="sxs-lookup"><span data-stu-id="20d47-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="20d47-183">Authorization</span><span class="sxs-lookup"><span data-stu-id="20d47-183">Authorization</span></span> | <span data-ttu-id="20d47-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20d47-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20d47-186">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20d47-186">Content-Type</span></span> | <span data-ttu-id="20d47-187">application/json</span><span class="sxs-lookup"><span data-stu-id="20d47-187">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="20d47-188">请求正文</span><span class="sxs-lookup"><span data-stu-id="20d47-188">Request body</span></span>

<span data-ttu-id="20d47-189">提供每个 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象在资源实例的 **multiValueExtendedProperties** 集合属性中的 JSON 正文。</span><span class="sxs-lookup"><span data-stu-id="20d47-189">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="20d47-190">**属性**</span><span class="sxs-lookup"><span data-stu-id="20d47-190">**Property**</span></span>|<span data-ttu-id="20d47-191">**类型**</span><span class="sxs-lookup"><span data-stu-id="20d47-191">**Type**</span></span>|<span data-ttu-id="20d47-192">**说明**</span><span class="sxs-lookup"><span data-stu-id="20d47-192">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="20d47-193">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="20d47-193">multiValueExtendedProperties</span></span>|<span data-ttu-id="20d47-194">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="20d47-194">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="20d47-195">一个或多个多值扩展属性的数组。</span><span class="sxs-lookup"><span data-stu-id="20d47-195">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="20d47-196">id</span><span class="sxs-lookup"><span data-stu-id="20d47-196">id</span></span>|<span data-ttu-id="20d47-197">String</span><span class="sxs-lookup"><span data-stu-id="20d47-197">String</span></span>|<span data-ttu-id="20d47-p105">对于 **multiValueExtendedProperties** 集合中的每个属性，请指定此参数以标识属性。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="20d47-p105">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="20d47-202">值</span><span class="sxs-lookup"><span data-stu-id="20d47-202">value</span></span>|<span data-ttu-id="20d47-203">string</span><span class="sxs-lookup"><span data-stu-id="20d47-203">string</span></span>|<span data-ttu-id="20d47-p106">对于 **multiValueExtendedProperties** 集合中的每个属性，请指定属性值。必需。</span><span class="sxs-lookup"><span data-stu-id="20d47-p106">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="20d47-206">在_新建_资源实例中创建扩展属性时，除了新的 **multiValueExtendedProperties** 集合，请提供资源实例的 JSON 表示形式（即 [邮件](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md) 等）。</span><span class="sxs-lookup"><span data-stu-id="20d47-206">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="20d47-207">响应</span><span class="sxs-lookup"><span data-stu-id="20d47-207">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="20d47-208">响应代码</span><span class="sxs-lookup"><span data-stu-id="20d47-208">Response code</span></span>
<span data-ttu-id="20d47-209">在新建资源实例中成功创建扩展属性的操作返回 `201 Created`（在新的组帖子中除外），根据所用的方法，该操作可以返回 `200 OK` 或 `202 Accepted`。</span><span class="sxs-lookup"><span data-stu-id="20d47-209">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="20d47-210">在现有的资源实例中，成功的创建操作返回 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="20d47-210">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="20d47-211">响应正文</span><span class="sxs-lookup"><span data-stu-id="20d47-211">Response body</span></span>

<span data-ttu-id="20d47-p107">在支持的资源（而不是 [组帖子](../resources/post.md)）中创建扩展属性时，该响应只包括新建或现有的实例，但不包括新的扩展属性。若要查看新创建的扩展属性，请 [获取通过扩展属性展开的实例](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="20d47-p107">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="20d47-p108">在_新建_的组帖子中创建扩展属性时，响应仅包括响应代码，但不包括新帖子或扩展属性。不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="20d47-p108">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="20d47-216">示例</span><span class="sxs-lookup"><span data-stu-id="20d47-216">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="20d47-217">请求 1</span><span class="sxs-lookup"><span data-stu-id="20d47-217">Request 1</span></span>

<span data-ttu-id="20d47-p109">第一个示例在同一个 POST 操作的全新事件中创建一个多值扩展属性。除了通常要包括的新事件的属性，请求正文还包括 **multiValueExtendedProperties** 集合（包含一个扩展属性）。请求正文包括该多值扩展属性的如下参数：</span><span class="sxs-lookup"><span data-stu-id="20d47-p109">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="20d47-221">**id**，将此属性指定为包含指定 GUID 和 `Recreation` 名称的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="20d47-221">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="20d47-222">**value**，将 `Recreation` 指定为包含 3 个字符串值（`["Food", "Hiking", "Swimming"]`）的数组。</span><span class="sxs-lookup"><span data-stu-id="20d47-222">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/events
Content-Type: application/json

{
  "subject": "Family reunion",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together this Thanksgiving!"
  },
  "start": {
      "dateTime": "2015-11-26T09:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-29T21:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "Lauren@contoso.com",
        "name": "Lauren Solis"
      },
      "type": "Required"
    }
  ],
  "multiValueExtendedProperties": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="20d47-223">响应 1</span><span class="sxs-lookup"><span data-stu-id="20d47-223">Response 1</span></span>

<span data-ttu-id="20d47-p110">成功的响应由 `HTTP 201 Created` 响应代码表示，并在响应正文中包括新事件，类似于 [仅创建事件](../api/user-post-events.md) 中的响应。该响应不包括任何新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="20d47-p110">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="20d47-226">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的事件](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="20d47-226">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="20d47-227">请求 2</span><span class="sxs-lookup"><span data-stu-id="20d47-227">Request 2</span></span>

<span data-ttu-id="20d47-p111">第二个示例为指定的邮件创建一个多值扩展属性。扩展属性是 **multiValueExtendedProperties** 集合中的唯一元素。请求正文包括扩展属性的如下参数：</span><span class="sxs-lookup"><span data-stu-id="20d47-p111">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="20d47-231">**id**，将此属性指定为包含指定 GUID 和名称 `Palette` 的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="20d47-231">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="20d47-232">**value**，将 `Palette` 指定为包含 3 个字符串值（`["Green", "Aqua", "Blue"]`）的数组。</span><span class="sxs-lookup"><span data-stu-id="20d47-232">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueExtendedProperties": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="20d47-233">响应 2</span><span class="sxs-lookup"><span data-stu-id="20d47-233">Response 2</span></span>

<span data-ttu-id="20d47-p112">成功的响应由 `HTTP 200 OK` 响应代码表示，并在响应正文中包括指定的邮件，类似于 [更新邮件](../api/message-update.md) 中的响应。该响应不包括新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="20d47-p112">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="20d47-236">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的邮件](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="20d47-236">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


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




