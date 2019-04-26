---
title: 创建单值扩展属性
description: '在新建或现有的资源实例中创建一个或多个单值扩展属性。 '
localization_priority: Normal
ms.openlocfilehash: 193cf8608829e2f4c06f49fa9675b7384941e7e7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330985"
---
# <a name="create-single-value-extended-property"></a><span data-ttu-id="84a8b-103">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="84a8b-103">Create single-value extended property</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84a8b-104">在新建或现有的资源实例中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="84a8b-104">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="84a8b-105">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="84a8b-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="84a8b-106">日历</span><span class="sxs-lookup"><span data-stu-id="84a8b-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="84a8b-107">联系人</span><span class="sxs-lookup"><span data-stu-id="84a8b-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="84a8b-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="84a8b-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="84a8b-109">event</span><span class="sxs-lookup"><span data-stu-id="84a8b-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="84a8b-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="84a8b-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="84a8b-111">邮件</span><span class="sxs-lookup"><span data-stu-id="84a8b-111">message</span></span>](../resources/message.md)
- [<span data-ttu-id="84a8b-112">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="84a8b-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="84a8b-113">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="84a8b-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="84a8b-114">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="84a8b-114">As well as the following group resources:</span></span>

- <span data-ttu-id="84a8b-115">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="84a8b-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="84a8b-116">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="84a8b-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="84a8b-117">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="84a8b-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="84a8b-118">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="84a8b-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="84a8b-119">权限</span><span class="sxs-lookup"><span data-stu-id="84a8b-119">Permissions</span></span>
<span data-ttu-id="84a8b-120">根据您要在其中创建扩展属性的资源以及所请求的权限类型 (委派或应用程序), 在下表中指定的权限是调用此 API 所需的最低权限。</span><span class="sxs-lookup"><span data-stu-id="84a8b-120">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="84a8b-121">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84a8b-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84a8b-122">支持的资源</span><span class="sxs-lookup"><span data-stu-id="84a8b-122">Supported resource</span></span> | <span data-ttu-id="84a8b-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84a8b-123">Delegated (work or school account)</span></span> | <span data-ttu-id="84a8b-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84a8b-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84a8b-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="84a8b-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="84a8b-126">日历</span><span class="sxs-lookup"><span data-stu-id="84a8b-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="84a8b-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="84a8b-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-128">Calendars.ReadWrite</span></span> | <span data-ttu-id="84a8b-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-129">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="84a8b-130">联系人</span><span class="sxs-lookup"><span data-stu-id="84a8b-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="84a8b-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="84a8b-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="84a8b-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="84a8b-134">contactFolder</span><span class="sxs-lookup"><span data-stu-id="84a8b-134">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="84a8b-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="84a8b-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-136">Contacts.ReadWrite</span></span> | <span data-ttu-id="84a8b-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-137">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="84a8b-138">事件</span><span class="sxs-lookup"><span data-stu-id="84a8b-138">event</span></span>](../resources/event.md) | <span data-ttu-id="84a8b-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-139">Calendars.ReadWrite</span></span> | <span data-ttu-id="84a8b-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-140">Calendars.ReadWrite</span></span> |  <span data-ttu-id="84a8b-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-141">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="84a8b-142">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="84a8b-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="84a8b-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a8b-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="84a8b-144">不支持</span><span class="sxs-lookup"><span data-stu-id="84a8b-144">Not supported</span></span> | <span data-ttu-id="84a8b-145">不支持</span><span class="sxs-lookup"><span data-stu-id="84a8b-145">Not supported</span></span> |
| <span data-ttu-id="84a8b-146">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="84a8b-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="84a8b-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a8b-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="84a8b-148">不支持</span><span class="sxs-lookup"><span data-stu-id="84a8b-148">Not supported</span></span> | <span data-ttu-id="84a8b-149">不支持</span><span class="sxs-lookup"><span data-stu-id="84a8b-149">Not supported</span></span> |
| <span data-ttu-id="84a8b-150">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="84a8b-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="84a8b-151">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a8b-151">Group.ReadWrite.All</span></span> | <span data-ttu-id="84a8b-152">不支持</span><span class="sxs-lookup"><span data-stu-id="84a8b-152">Not supported</span></span> | <span data-ttu-id="84a8b-153">不支持</span><span class="sxs-lookup"><span data-stu-id="84a8b-153">Not supported</span></span> |
| [<span data-ttu-id="84a8b-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="84a8b-154">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="84a8b-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-155">Mail.ReadWrite</span></span> | <span data-ttu-id="84a8b-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-156">Mail.ReadWrite</span></span> | <span data-ttu-id="84a8b-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-157">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="84a8b-158">邮件</span><span class="sxs-lookup"><span data-stu-id="84a8b-158">message</span></span>](../resources/message.md) | <span data-ttu-id="84a8b-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-159">Mail.ReadWrite</span></span> | <span data-ttu-id="84a8b-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-160">Mail.ReadWrite</span></span> | <span data-ttu-id="84a8b-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-161">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="84a8b-162">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="84a8b-162">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="84a8b-163">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-163">Tasks.ReadWrite</span></span> | <span data-ttu-id="84a8b-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="84a8b-165">不支持</span><span class="sxs-lookup"><span data-stu-id="84a8b-165">Not supported</span></span> |
| [<span data-ttu-id="84a8b-166">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="84a8b-166">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="84a8b-167">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-167">Tasks.ReadWrite</span></span> | <span data-ttu-id="84a8b-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a8b-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="84a8b-169">不支持</span><span class="sxs-lookup"><span data-stu-id="84a8b-169">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="84a8b-170">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84a8b-170">HTTP request</span></span>
<span data-ttu-id="84a8b-171">可以在新建或现有的资源实例中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="84a8b-171">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="84a8b-172">若要在_新的_资源实例中创建一个或多个扩展属性，请使用与创建实例相同的 REST 请求，并包括新资源实例的属性和请求正文中的_扩展属性_。</span><span class="sxs-lookup"><span data-stu-id="84a8b-172">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="84a8b-173">注意，一些资源支持以多种方式创建。</span><span class="sxs-lookup"><span data-stu-id="84a8b-173">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="84a8b-174">有关创建这些资源实例的详细信息, 请参阅创建[邮件](../resources/message.md)的相应主题[mailFolder](../api/user-post-mailfolders.md)、[事件](../api/user-post-events.md)、[日历](../api/user-post-calendars.md)、[联系人](../api/user-post-contacts.md)、 [contactFolder](../api/user-post-contactfolders.md)、 [Outlook 任务](../resources/outlooktask.md)、 [Outlook 任务文件夹](../resources/outlooktaskfolder.md)、[组事件](../api/group-post-events.md)和[组帖子](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="84a8b-174">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="84a8b-175">以下是请求的语法。</span><span class="sxs-lookup"><span data-stu-id="84a8b-175">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="84a8b-176">若要在现有资源实例中创建一个或多个扩展属性，请在请求中指定实例，并在请求正文中包括扩展属性。</span><span class="sxs-lookup"><span data-stu-id="84a8b-176">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="84a8b-177">**注意**不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="84a8b-177">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="84a8b-178">请求标头</span><span class="sxs-lookup"><span data-stu-id="84a8b-178">Request headers</span></span>
| <span data-ttu-id="84a8b-179">名称</span><span class="sxs-lookup"><span data-stu-id="84a8b-179">Name</span></span>       | <span data-ttu-id="84a8b-180">值</span><span class="sxs-lookup"><span data-stu-id="84a8b-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="84a8b-181">Authorization</span><span class="sxs-lookup"><span data-stu-id="84a8b-181">Authorization</span></span> | <span data-ttu-id="84a8b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84a8b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84a8b-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84a8b-184">Content-Type</span></span> | <span data-ttu-id="84a8b-185">application/json</span><span class="sxs-lookup"><span data-stu-id="84a8b-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="84a8b-186">请求正文</span><span class="sxs-lookup"><span data-stu-id="84a8b-186">Request body</span></span>

<span data-ttu-id="84a8b-187">提供每个 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象在资源实例的 **singleValueExtendedProperties** 集合属性中的 JSON 正文。</span><span class="sxs-lookup"><span data-stu-id="84a8b-187">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="84a8b-188">**属性**</span><span class="sxs-lookup"><span data-stu-id="84a8b-188">**Property**</span></span>|<span data-ttu-id="84a8b-189">**类型**</span><span class="sxs-lookup"><span data-stu-id="84a8b-189">**Type**</span></span>|<span data-ttu-id="84a8b-190">**说明**</span><span class="sxs-lookup"><span data-stu-id="84a8b-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="84a8b-191">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="84a8b-191">singleValueExtendedProperties</span></span>|<span data-ttu-id="84a8b-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="84a8b-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="84a8b-193">一个或多个单值扩展属性的数组。</span><span class="sxs-lookup"><span data-stu-id="84a8b-193">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="84a8b-194">id</span><span class="sxs-lookup"><span data-stu-id="84a8b-194">id</span></span>|<span data-ttu-id="84a8b-195">String</span><span class="sxs-lookup"><span data-stu-id="84a8b-195">String</span></span>|<span data-ttu-id="84a8b-p104">对于 **singleValueExtendedProperties** 集合中的每个属性，请指定此参数以标识属性。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="84a8b-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="84a8b-200">值</span><span class="sxs-lookup"><span data-stu-id="84a8b-200">value</span></span>|<span data-ttu-id="84a8b-201">string</span><span class="sxs-lookup"><span data-stu-id="84a8b-201">string</span></span>|<span data-ttu-id="84a8b-p105">对于 **singleValueExtendedProperties** 集合中的每个属性，请指定属性值。必需。</span><span class="sxs-lookup"><span data-stu-id="84a8b-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="84a8b-204">在_新的_资源实例中创建扩展属性时，除了新的 **singleValueExtendedProperties** 集合，请提供资源实例的 JSON 表示形式（即 [邮件](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md) 等）。</span><span class="sxs-lookup"><span data-stu-id="84a8b-204">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="84a8b-205">响应</span><span class="sxs-lookup"><span data-stu-id="84a8b-205">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="84a8b-206">响应代码</span><span class="sxs-lookup"><span data-stu-id="84a8b-206">Response code</span></span>
<span data-ttu-id="84a8b-207">在新建资源实例中成功创建扩展属性的操作返回 `201 Created`（在新的组帖子中除外），根据所用的方法，该操作可以返回 `200 OK` 或 `202 Accepted`。</span><span class="sxs-lookup"><span data-stu-id="84a8b-207">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="84a8b-208">在现有的资源实例中，成功的创建操作返回 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="84a8b-208">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="84a8b-209">响应正文</span><span class="sxs-lookup"><span data-stu-id="84a8b-209">Response body</span></span>

<span data-ttu-id="84a8b-p106">创建扩展属性时，该响应只包括新建或现有的实例，但不包括新的扩展属性。若要查看新创建的扩展属性，请 [获取通过扩展属性扩展的实例](../api/singlevaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="84a8b-p106">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="84a8b-212">通过回复线程或帖子在_新建_[组帖子](../resources/post.md)中创建扩展属性时，响应仅包括响应代码，但不包括新帖子或扩展属性。</span><span class="sxs-lookup"><span data-stu-id="84a8b-212">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="84a8b-213">示例</span><span class="sxs-lookup"><span data-stu-id="84a8b-213">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="84a8b-214">请求 1</span><span class="sxs-lookup"><span data-stu-id="84a8b-214">Request 1</span></span>

<span data-ttu-id="84a8b-p107">第一个示例在相同的 POST 操作中创建一个新事件和一个单值扩展属性。除了通常要包括的新事件的属性，请求正文还包括 **singleValueExtendedProperties** 集合，该集合包含一个单值扩展属性和以下属性：</span><span class="sxs-lookup"><span data-stu-id="84a8b-p107">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>

- <span data-ttu-id="84a8b-217">**id** 将属性类型指定为 `String`、GUID 和名为 `Fun` 的属性。</span><span class="sxs-lookup"><span data-stu-id="84a8b-217">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="84a8b-218">**value** 将 `Food` 指定为 `Fun` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="84a8b-218">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

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

##### <a name="response-1"></a><span data-ttu-id="84a8b-219">响应 1</span><span class="sxs-lookup"><span data-stu-id="84a8b-219">Response 1</span></span>

<span data-ttu-id="84a8b-p108">成功的响应由 `HTTP 201 Created` 响应代码表示，并在响应正文中包括新事件，类似于 [仅创建事件](../api/user-post-events.md) 中的响应。该响应不包括任何新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="84a8b-p108">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="84a8b-222">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的事件](../api/singlevaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="84a8b-222">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="84a8b-223">请求 2</span><span class="sxs-lookup"><span data-stu-id="84a8b-223">Request 2</span></span>

<span data-ttu-id="84a8b-p109">第二个示例为指定的现有邮件创建一个单值扩展属性。扩展属性是 **singleValueExtendedProperties** 数组中的唯一元素。请求正文包括扩展属性的以下参数：</span><span class="sxs-lookup"><span data-stu-id="84a8b-p109">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="84a8b-227">**id** 将属性类型指定为 `String`、GUID 和名为 `Color` 的属性。</span><span class="sxs-lookup"><span data-stu-id="84a8b-227">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="84a8b-228">**value** 将 `Green` 指定为 `Color` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="84a8b-228">**value** specifies `Green` as the value of the `Color` property.</span></span>

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

##### <a name="response-2"></a><span data-ttu-id="84a8b-229">响应 2</span><span class="sxs-lookup"><span data-stu-id="84a8b-229">Response 2</span></span>

<span data-ttu-id="84a8b-p110">成功的响应由 `HTTP 200 OK` 响应代码表示，并在响应正文中包括指定的邮件，类似于 [更新邮件](../api/message-update.md) 中的响应。该响应不包括新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="84a8b-p110">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="84a8b-232">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的邮件](../api/singlevaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="84a8b-232">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

