---
title: 创建多值扩展属性
description: '在新建或现有的资源实例中创建一个或多个多值扩展属性。 '
localization_priority: Normal
ms.openlocfilehash: 4ed9af6fda2117fee7ef1ac50c69c4f006abd45d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576260"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="bc6ea-103">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="bc6ea-103">Create multi-value extended property</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc6ea-104">在新建或现有的资源实例中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-104">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="bc6ea-105">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="bc6ea-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="bc6ea-106">日历</span><span class="sxs-lookup"><span data-stu-id="bc6ea-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="bc6ea-107">联系人</span><span class="sxs-lookup"><span data-stu-id="bc6ea-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="bc6ea-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="bc6ea-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="bc6ea-109">event</span><span class="sxs-lookup"><span data-stu-id="bc6ea-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="bc6ea-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc6ea-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="bc6ea-111">message</span><span class="sxs-lookup"><span data-stu-id="bc6ea-111">message</span></span>](../resources/message.md)
- [<span data-ttu-id="bc6ea-112">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="bc6ea-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="bc6ea-113">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="bc6ea-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="bc6ea-114">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="bc6ea-114">As well as the following group resources:</span></span>

- <span data-ttu-id="bc6ea-115">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="bc6ea-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="bc6ea-116">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="bc6ea-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="bc6ea-117">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="bc6ea-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="bc6ea-118">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc6ea-119">权限</span><span class="sxs-lookup"><span data-stu-id="bc6ea-119">Permissions</span></span>
<span data-ttu-id="bc6ea-120">正在根据资源创建中的扩展的属性和权限键入 （委派或应用程序） 您请求，至少要调用此 API 是下表中所指定的权限。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-120">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="bc6ea-121">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc6ea-122">支持的资源</span><span class="sxs-lookup"><span data-stu-id="bc6ea-122">Supported resource</span></span> | <span data-ttu-id="bc6ea-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc6ea-123">Delegated (work or school account)</span></span> | <span data-ttu-id="bc6ea-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc6ea-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc6ea-125">Application</span><span class="sxs-lookup"><span data-stu-id="bc6ea-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="bc6ea-126">日历</span><span class="sxs-lookup"><span data-stu-id="bc6ea-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="bc6ea-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="bc6ea-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-128">Calendars.ReadWrite</span></span> | <span data-ttu-id="bc6ea-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-129">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="bc6ea-130">联系人</span><span class="sxs-lookup"><span data-stu-id="bc6ea-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="bc6ea-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="bc6ea-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="bc6ea-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="bc6ea-134">contactFolder</span><span class="sxs-lookup"><span data-stu-id="bc6ea-134">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="bc6ea-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="bc6ea-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-136">Contacts.ReadWrite</span></span> | <span data-ttu-id="bc6ea-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-137">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="bc6ea-138">事件</span><span class="sxs-lookup"><span data-stu-id="bc6ea-138">event</span></span>](../resources/event.md) | <span data-ttu-id="bc6ea-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-139">Calendars.ReadWrite</span></span> | <span data-ttu-id="bc6ea-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-140">Calendars.ReadWrite</span></span> |  <span data-ttu-id="bc6ea-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-141">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="bc6ea-142">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="bc6ea-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="bc6ea-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc6ea-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="bc6ea-144">不支持</span><span class="sxs-lookup"><span data-stu-id="bc6ea-144">Not supported</span></span> | <span data-ttu-id="bc6ea-145">不支持</span><span class="sxs-lookup"><span data-stu-id="bc6ea-145">Not supported</span></span> |
| <span data-ttu-id="bc6ea-146">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="bc6ea-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="bc6ea-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc6ea-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="bc6ea-148">不支持</span><span class="sxs-lookup"><span data-stu-id="bc6ea-148">Not supported</span></span> | <span data-ttu-id="bc6ea-149">不支持</span><span class="sxs-lookup"><span data-stu-id="bc6ea-149">Not supported</span></span> |
| <span data-ttu-id="bc6ea-150">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="bc6ea-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="bc6ea-151">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc6ea-151">Group.ReadWrite.All</span></span> | <span data-ttu-id="bc6ea-152">不支持</span><span class="sxs-lookup"><span data-stu-id="bc6ea-152">Not supported</span></span> | <span data-ttu-id="bc6ea-153">不支持</span><span class="sxs-lookup"><span data-stu-id="bc6ea-153">Not supported</span></span> |
| [<span data-ttu-id="bc6ea-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc6ea-154">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="bc6ea-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-155">Mail.ReadWrite</span></span> | <span data-ttu-id="bc6ea-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-156">Mail.ReadWrite</span></span> | <span data-ttu-id="bc6ea-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-157">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="bc6ea-158">邮件</span><span class="sxs-lookup"><span data-stu-id="bc6ea-158">message</span></span>](../resources/message.md) | <span data-ttu-id="bc6ea-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-159">Mail.ReadWrite</span></span> | <span data-ttu-id="bc6ea-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-160">Mail.ReadWrite</span></span> | <span data-ttu-id="bc6ea-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-161">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="bc6ea-162">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="bc6ea-162">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="bc6ea-163">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-163">Tasks.ReadWrite</span></span> | <span data-ttu-id="bc6ea-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="bc6ea-165">不支持</span><span class="sxs-lookup"><span data-stu-id="bc6ea-165">Not supported</span></span> |
| [<span data-ttu-id="bc6ea-166">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="bc6ea-166">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="bc6ea-167">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-167">Tasks.ReadWrite</span></span> | <span data-ttu-id="bc6ea-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc6ea-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="bc6ea-169">不支持</span><span class="sxs-lookup"><span data-stu-id="bc6ea-169">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc6ea-170">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc6ea-170">HTTP request</span></span>
<span data-ttu-id="bc6ea-171">可以在新建或现有的资源实例中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-171">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="bc6ea-172">若要创建_新_资源实例中的一个或多个扩展的属性，使用相同的 REST 请求作为创建该实例，并在请求正文中包含的新资源实例_和扩展的属性_的属性。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-172">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="bc6ea-173">注意一些资源，以多种方式支持创建。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-173">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="bc6ea-174">有关创建这些资源实例的详细信息，请参阅创建[消息](../resources/message.md)、 [mailFolder](../api/user-post-mailfolders.md)、[事件](../api/user-post-events.md)、[日历](../api/user-post-calendars.md)、[联系人](../api/user-post-contacts.md)、 [contactFolder](../api/user-post-contactfolders.md)，相应主题[Outlook 任务](../resources/outlooktask.md)、 [Outlook 任务文件夹](../resources/outlooktaskfolder.md)，[组事件](../api/group-post-events.md)，并[组文章](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-174">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="bc6ea-175">以下是请求的语法。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-175">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="bc6ea-176">若要在现有资源实例中创建一个或多个扩展属性，请在请求中指定实例，并在请求正文中包括扩展属性。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-176">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="bc6ea-177">**注意**不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-177">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="bc6ea-178">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc6ea-178">Request headers</span></span>
| <span data-ttu-id="bc6ea-179">名称</span><span class="sxs-lookup"><span data-stu-id="bc6ea-179">Name</span></span>       | <span data-ttu-id="bc6ea-180">值</span><span class="sxs-lookup"><span data-stu-id="bc6ea-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bc6ea-181">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc6ea-181">Authorization</span></span> | <span data-ttu-id="bc6ea-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc6ea-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc6ea-184">Content-Type</span></span> | <span data-ttu-id="bc6ea-185">application/json</span><span class="sxs-lookup"><span data-stu-id="bc6ea-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc6ea-186">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc6ea-186">Request body</span></span>

<span data-ttu-id="bc6ea-187">提供资源实例的**multiValueLegacyExtendedProperty**集合属性中的每个[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)对象的 JSON 正文。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-187">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueLegacyExtendedProperty** collection property of the resource instance.</span></span>

|<span data-ttu-id="bc6ea-188">**属性**</span><span class="sxs-lookup"><span data-stu-id="bc6ea-188">**Property**</span></span>|<span data-ttu-id="bc6ea-189">**类型**</span><span class="sxs-lookup"><span data-stu-id="bc6ea-189">**Type**</span></span>|<span data-ttu-id="bc6ea-190">**说明**</span><span class="sxs-lookup"><span data-stu-id="bc6ea-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bc6ea-191">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="bc6ea-191">multiValueLegacyExtendedProperty</span></span>|<span data-ttu-id="bc6ea-192">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="bc6ea-192">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="bc6ea-193">一个或多个多值扩展属性的数组。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-193">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="bc6ea-194">id</span><span class="sxs-lookup"><span data-stu-id="bc6ea-194">id</span></span>|<span data-ttu-id="bc6ea-195">String</span><span class="sxs-lookup"><span data-stu-id="bc6ea-195">String</span></span>|<span data-ttu-id="bc6ea-196">对于**multiValueLegacyExtendedProperty**集合中每个属性，指定此选项可标识该属性。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-196">For each property in the **multiValueLegacyExtendedProperty** collection, specify this to identify the property.</span></span> <span data-ttu-id="bc6ea-197">它必须遵循的受支持的格式之一。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-197">It must follow one of the supported formats.</span></span> <span data-ttu-id="bc6ea-198">有关详细信息，请参阅[Outlook 扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-198">See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information.</span></span> <span data-ttu-id="bc6ea-199">必需。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-199">Required.</span></span>|
|<span data-ttu-id="bc6ea-200">值</span><span class="sxs-lookup"><span data-stu-id="bc6ea-200">value</span></span>|<span data-ttu-id="bc6ea-201">string</span><span class="sxs-lookup"><span data-stu-id="bc6ea-201">string</span></span>|<span data-ttu-id="bc6ea-202">对于**multiValueLegacyExtendedProperty**集合中每个属性，指定该属性值。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-202">For each property in the **multiValueLegacyExtendedProperty** collection, specify the property value.</span></span> <span data-ttu-id="bc6ea-203">必需。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-203">Required.</span></span>|

<span data-ttu-id="bc6ea-204">在_新_的资源实例中，除了新**multiValueLegacyExtendedProperty**集合中，创建的扩展的属性时提供的资源实例 （即，[邮件](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)的 JSON 表示形式[事件](../resources/event.md)等。)</span><span class="sxs-lookup"><span data-stu-id="bc6ea-204">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueLegacyExtendedProperty** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="bc6ea-205">响应</span><span class="sxs-lookup"><span data-stu-id="bc6ea-205">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="bc6ea-206">响应代码</span><span class="sxs-lookup"><span data-stu-id="bc6ea-206">Response code</span></span>
<span data-ttu-id="bc6ea-207">在新建资源实例中成功创建扩展属性的操作返回 `201 Created`（在新的组帖子中除外），根据所用的方法，该操作可以返回 `200 OK` 或 `202 Accepted`。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-207">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="bc6ea-208">在现有的资源实例中，成功的创建操作返回 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-208">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="bc6ea-209">响应正文</span><span class="sxs-lookup"><span data-stu-id="bc6ea-209">Response body</span></span>

<span data-ttu-id="bc6ea-p106">在支持的资源（而不是 [组帖子](../resources/post.md)）中创建扩展属性时，该响应只包括新建或现有的实例，但不包括新的扩展属性。若要查看新创建的扩展属性，请 [获取通过扩展属性展开的实例](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="bc6ea-p107">在_新建_的组帖子中创建扩展属性时，响应仅包括响应代码，但不包括新帖子或扩展属性。不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="bc6ea-214">示例</span><span class="sxs-lookup"><span data-stu-id="bc6ea-214">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="bc6ea-215">请求 1</span><span class="sxs-lookup"><span data-stu-id="bc6ea-215">Request 1</span></span>

<span data-ttu-id="bc6ea-216">此示例创建一个多值扩展属性中所有中相同的 POST 操作的新事件。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-216">The first example creates a multi-value extended property in a new event all in the same POST operation.</span></span> <span data-ttu-id="bc6ea-217">除了您通常要包括的新事件的属性，在请求正文包括**multiValueLegacyExtendedProperty**集合，其中包含一个扩展的属性。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-217">Apart from the properties you'd normally include for a new event, the request body includes the **multiValueLegacyExtendedProperty** collection which contains one extended property.</span></span> <span data-ttu-id="bc6ea-218">在请求正文的多值扩展属性包括：</span><span class="sxs-lookup"><span data-stu-id="bc6ea-218">The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="bc6ea-219">**id**，将此属性指定为包含指定 GUID 和 `Recreation` 名称的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-219">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="bc6ea-220">**value**，将 `Recreation` 指定为包含 3 个字符串值（`["Food", "Hiking", "Swimming"]`）的数组。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-220">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

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
  "multiValueLegacyExtendedProperty": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="bc6ea-221">响应 1</span><span class="sxs-lookup"><span data-stu-id="bc6ea-221">Response 1</span></span>

<span data-ttu-id="bc6ea-p109">成功的响应由 `HTTP 201 Created` 响应代码表示，并在响应正文中包括新事件，类似于 [仅创建事件](../api/user-post-events.md) 中的响应。该响应不包括任何新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="bc6ea-224">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的事件](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-224">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="bc6ea-225">请求 2</span><span class="sxs-lookup"><span data-stu-id="bc6ea-225">Request 2</span></span>

<span data-ttu-id="bc6ea-226">第二个示例创建一个多值扩展属性指定的消息。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-226">The second example creates one multi-value extended property for the specified message.</span></span> <span data-ttu-id="bc6ea-227">**MultiValueLegacyExtendedProperty**集合中的唯一元素的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-227">That extended property is the only element in the **multiValueLegacyExtendedProperty** collection.</span></span> <span data-ttu-id="bc6ea-228">在请求正文的扩展属性包括：</span><span class="sxs-lookup"><span data-stu-id="bc6ea-228">The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="bc6ea-229">**id**，将此属性指定为包含指定 GUID 和名称 `Palette` 的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-229">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="bc6ea-230">**value**，将 `Palette` 指定为包含 3 个字符串值（`["Green", "Aqua", "Blue"]`）的数组。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-230">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueLegacyExtendedProperty": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="bc6ea-231">响应 2</span><span class="sxs-lookup"><span data-stu-id="bc6ea-231">Response 2</span></span>

<span data-ttu-id="bc6ea-p111">成功的响应由 `HTTP 200 OK` 响应代码表示，并在响应正文中包括指定的邮件，类似于 [更新邮件](../api/message-update.md) 中的响应。该响应不包括新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="bc6ea-234">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的邮件](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="bc6ea-234">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


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
  "suppressions": [
    "Error: /api-reference/beta/api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->




