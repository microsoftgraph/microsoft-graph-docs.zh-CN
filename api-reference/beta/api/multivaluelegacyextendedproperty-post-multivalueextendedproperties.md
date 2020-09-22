---
title: 创建多值扩展属性
description: '在新建或现有的资源实例中创建一个或多个多值扩展属性。 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 4e54a58f3d7d2cfd6b7f410ebe4a1ea55f629efe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062401"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="ca8d3-103">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="ca8d3-103">Create multi-value extended property</span></span>

<span data-ttu-id="ca8d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca8d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="ca8d3-105">在新建或现有的资源实例中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-105">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span>

<span data-ttu-id="ca8d3-106">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="ca8d3-106">The following user resources are supported:</span></span>

- [<span data-ttu-id="ca8d3-107">日历</span><span class="sxs-lookup"><span data-stu-id="ca8d3-107">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="ca8d3-108">联系人</span><span class="sxs-lookup"><span data-stu-id="ca8d3-108">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="ca8d3-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ca8d3-109">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="ca8d3-110">event</span><span class="sxs-lookup"><span data-stu-id="ca8d3-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="ca8d3-111">mailFolder</span><span class="sxs-lookup"><span data-stu-id="ca8d3-111">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="ca8d3-112">邮件</span><span class="sxs-lookup"><span data-stu-id="ca8d3-112">message</span></span>](../resources/message.md)
- [<span data-ttu-id="ca8d3-113">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="ca8d3-113">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="ca8d3-114">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="ca8d3-114">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="ca8d3-115">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="ca8d3-115">As well as the following group resources:</span></span>

- <span data-ttu-id="ca8d3-116">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="ca8d3-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="ca8d3-117">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="ca8d3-117">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="ca8d3-118">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="ca8d3-118">group [post](../resources/post.md)</span></span>

<span data-ttu-id="ca8d3-119">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-119">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca8d3-120">权限</span><span class="sxs-lookup"><span data-stu-id="ca8d3-120">Permissions</span></span>
<span data-ttu-id="ca8d3-121">根据您要在其中创建扩展属性的资源以及请求的权限类型 (委派或应用程序) ，在下表中指定的权限是调用此 API 所需的最低权限。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-121">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="ca8d3-122">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-122">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca8d3-123">支持的资源</span><span class="sxs-lookup"><span data-stu-id="ca8d3-123">Supported resource</span></span> | <span data-ttu-id="ca8d3-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca8d3-124">Delegated (work or school account)</span></span> | <span data-ttu-id="ca8d3-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca8d3-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca8d3-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca8d3-126">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="ca8d3-127">calendar</span><span class="sxs-lookup"><span data-stu-id="ca8d3-127">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="ca8d3-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-128">Calendars.ReadWrite</span></span> | <span data-ttu-id="ca8d3-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-129">Calendars.ReadWrite</span></span> | <span data-ttu-id="ca8d3-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-130">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="ca8d3-131">联系人</span><span class="sxs-lookup"><span data-stu-id="ca8d3-131">contact</span></span>](../resources/contact.md) | <span data-ttu-id="ca8d3-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="ca8d3-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="ca8d3-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-134">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="ca8d3-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ca8d3-135">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="ca8d3-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-136">Contacts.ReadWrite</span></span> | <span data-ttu-id="ca8d3-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-137">Contacts.ReadWrite</span></span> | <span data-ttu-id="ca8d3-138">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-138">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="ca8d3-139">事件</span><span class="sxs-lookup"><span data-stu-id="ca8d3-139">event</span></span>](../resources/event.md) | <span data-ttu-id="ca8d3-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-140">Calendars.ReadWrite</span></span> | <span data-ttu-id="ca8d3-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-141">Calendars.ReadWrite</span></span> |  <span data-ttu-id="ca8d3-142">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-142">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="ca8d3-143">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="ca8d3-143">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="ca8d3-144">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8d3-144">Group.ReadWrite.All</span></span> | <span data-ttu-id="ca8d3-145">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8d3-145">Not supported</span></span> | <span data-ttu-id="ca8d3-146">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8d3-146">Not supported</span></span> |
| <span data-ttu-id="ca8d3-147">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="ca8d3-147">group [event](../resources/event.md)</span></span> | <span data-ttu-id="ca8d3-148">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8d3-148">Group.ReadWrite.All</span></span> | <span data-ttu-id="ca8d3-149">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8d3-149">Not supported</span></span> | <span data-ttu-id="ca8d3-150">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8d3-150">Not supported</span></span> |
| <span data-ttu-id="ca8d3-151">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="ca8d3-151">group [post](../resources/post.md)</span></span> | <span data-ttu-id="ca8d3-152">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8d3-152">Group.ReadWrite.All</span></span> | <span data-ttu-id="ca8d3-153">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8d3-153">Not supported</span></span> | <span data-ttu-id="ca8d3-154">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8d3-154">Not supported</span></span> |
| [<span data-ttu-id="ca8d3-155">mailFolder</span><span class="sxs-lookup"><span data-stu-id="ca8d3-155">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="ca8d3-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-156">Mail.ReadWrite</span></span> | <span data-ttu-id="ca8d3-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-157">Mail.ReadWrite</span></span> | <span data-ttu-id="ca8d3-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-158">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="ca8d3-159">邮件</span><span class="sxs-lookup"><span data-stu-id="ca8d3-159">message</span></span>](../resources/message.md) | <span data-ttu-id="ca8d3-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-160">Mail.ReadWrite</span></span> | <span data-ttu-id="ca8d3-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-161">Mail.ReadWrite</span></span> | <span data-ttu-id="ca8d3-162">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-162">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="ca8d3-163">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="ca8d3-163">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="ca8d3-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="ca8d3-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="ca8d3-166">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8d3-166">Not supported</span></span> |
| [<span data-ttu-id="ca8d3-167">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="ca8d3-167">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="ca8d3-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="ca8d3-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8d3-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="ca8d3-170">不支持</span><span class="sxs-lookup"><span data-stu-id="ca8d3-170">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca8d3-171">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca8d3-171">HTTP request</span></span>
<span data-ttu-id="ca8d3-172">可以在新建或现有的资源实例中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-172">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="ca8d3-173">若要在_新的_资源实例中创建一个或多个扩展属性，请使用与创建实例相同的 REST 请求，并包括新资源实例的属性和请求正文中的_扩展属性_。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-173">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="ca8d3-174">注意，一些资源支持以多种方式创建。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-174">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="ca8d3-175">有关创建这些资源实例的详细信息，请参阅创建 [邮件](../resources/message.md)的相应主题： [mailFolder](../api/user-post-mailfolders.md)、 [event](../api/user-post-events.md)、 [calendar](../api/user-post-calendars.md)、 [contact](../api/user-post-contacts.md)、 [contactFolder](../api/user-post-contactfolders.md)、 [outlook task](../resources/outlooktask.md)、 [outlook task folder](../resources/outlooktaskfolder.md)、 [group event](../api/group-post-events.md)和 [group post](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-175">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span>

<span data-ttu-id="ca8d3-176">以下是请求的语法。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-176">The following is the syntax of the requests.</span></span>

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

<span data-ttu-id="ca8d3-177">若要在现有资源实例中创建一个或多个扩展属性，请在请求中指定实例，并在请求正文中包括扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-177">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="ca8d3-178">**注意**不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-178">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="ca8d3-179">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca8d3-179">Request headers</span></span>
| <span data-ttu-id="ca8d3-180">名称</span><span class="sxs-lookup"><span data-stu-id="ca8d3-180">Name</span></span>       | <span data-ttu-id="ca8d3-181">值</span><span class="sxs-lookup"><span data-stu-id="ca8d3-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ca8d3-182">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca8d3-182">Authorization</span></span> | <span data-ttu-id="ca8d3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca8d3-185">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca8d3-185">Content-Type</span></span> | <span data-ttu-id="ca8d3-186">application/json</span><span class="sxs-lookup"><span data-stu-id="ca8d3-186">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca8d3-187">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca8d3-187">Request body</span></span>

<span data-ttu-id="ca8d3-188">提供每个 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象在资源实例的 **multiValueExtendedProperties** 集合属性中的 JSON 正文。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-188">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="ca8d3-189">**属性**</span><span class="sxs-lookup"><span data-stu-id="ca8d3-189">**Property**</span></span>|<span data-ttu-id="ca8d3-190">**类型**</span><span class="sxs-lookup"><span data-stu-id="ca8d3-190">**Type**</span></span>|<span data-ttu-id="ca8d3-191">**说明**</span><span class="sxs-lookup"><span data-stu-id="ca8d3-191">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ca8d3-192">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="ca8d3-192">multiValueExtendedProperties</span></span>|<span data-ttu-id="ca8d3-193">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca8d3-193">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="ca8d3-194">一个或多个多值扩展属性的数组。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-194">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="ca8d3-195">id</span><span class="sxs-lookup"><span data-stu-id="ca8d3-195">id</span></span>|<span data-ttu-id="ca8d3-196">String</span><span class="sxs-lookup"><span data-stu-id="ca8d3-196">String</span></span>|<span data-ttu-id="ca8d3-p104">对于 **multiValueExtendedProperties** 集合中的每个属性，请指定此参数以标识属性。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="ca8d3-201">值</span><span class="sxs-lookup"><span data-stu-id="ca8d3-201">value</span></span>|<span data-ttu-id="ca8d3-202">string</span><span class="sxs-lookup"><span data-stu-id="ca8d3-202">string</span></span>|<span data-ttu-id="ca8d3-p105">对于 **multiValueExtendedProperties** 集合中的每个属性，请指定属性值。必需。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="ca8d3-205">在_新建_资源实例中创建扩展属性时，除了新的 **multiValueExtendedProperties** 集合，请提供资源实例的 JSON 表示形式（即 [邮件](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md) 等）。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-205">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="ca8d3-206">响应</span><span class="sxs-lookup"><span data-stu-id="ca8d3-206">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="ca8d3-207">响应代码</span><span class="sxs-lookup"><span data-stu-id="ca8d3-207">Response code</span></span>
<span data-ttu-id="ca8d3-208">在新建资源实例中成功创建扩展属性的操作返回 `201 Created`（在新的组帖子中除外），根据所用的方法，该操作可以返回 `200 OK` 或 `202 Accepted`。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-208">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="ca8d3-209">在现有的资源实例中，成功的创建操作返回 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-209">In an existing resource instance, a successful create operation returns `200 OK`.</span></span>


#### <a name="response-body"></a><span data-ttu-id="ca8d3-210">响应正文</span><span class="sxs-lookup"><span data-stu-id="ca8d3-210">Response body</span></span>

<span data-ttu-id="ca8d3-p106">在支持的资源（而不是 [组帖子](../resources/post.md)）中创建扩展属性时，该响应只包括新建或现有的实例，但不包括新的扩展属性。若要查看新创建的扩展属性，请 [获取通过扩展属性展开的实例](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="ca8d3-p107">在_新建_的组帖子中创建扩展属性时，响应仅包括响应代码，但不包括新帖子或扩展属性。不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="ca8d3-215">示例</span><span class="sxs-lookup"><span data-stu-id="ca8d3-215">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="ca8d3-216">请求 1</span><span class="sxs-lookup"><span data-stu-id="ca8d3-216">Request 1</span></span>

<span data-ttu-id="ca8d3-p108">第一个示例在同一个 POST 操作的全新事件中创建一个多值扩展属性。除了通常要包括的新事件的属性，请求正文还包括 **multiValueExtendedProperties** 集合（包含一个扩展属性）。请求正文包括该多值扩展属性的如下参数：</span><span class="sxs-lookup"><span data-stu-id="ca8d3-p108">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="ca8d3-220">**id**，将此属性指定为包含指定 GUID 和 `Recreation` 名称的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-220">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span>
- <span data-ttu-id="ca8d3-221">**value**，将 `Recreation` 指定为包含 3 个字符串值（`["Food", "Hiking", "Swimming"]`）的数组。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-221">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>


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

##### <a name="response-1"></a><span data-ttu-id="ca8d3-222">响应 1</span><span class="sxs-lookup"><span data-stu-id="ca8d3-222">Response 1</span></span>

<span data-ttu-id="ca8d3-p109">成功的响应由 `HTTP 201 Created` 响应代码表示，并在响应正文中包括新事件，类似于 [仅创建事件](../api/user-post-events.md) 中的响应。该响应不包括任何新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="ca8d3-225">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的事件](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-225">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="ca8d3-226">请求 2</span><span class="sxs-lookup"><span data-stu-id="ca8d3-226">Request 2</span></span>

<span data-ttu-id="ca8d3-p110">第二个示例为指定的邮件创建一个多值扩展属性。扩展属性是 **multiValueExtendedProperties** 集合中的唯一元素。请求正文包括扩展属性的如下参数：</span><span class="sxs-lookup"><span data-stu-id="ca8d3-p110">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="ca8d3-230">**id**，将此属性指定为包含指定 GUID 和名称 `Palette` 的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-230">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="ca8d3-231">**value**，将 `Palette` 指定为包含 3 个字符串值（`["Green", "Aqua", "Blue"]`）的数组。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-231">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

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

##### <a name="response-2"></a><span data-ttu-id="ca8d3-232">响应 2</span><span class="sxs-lookup"><span data-stu-id="ca8d3-232">Response 2</span></span>

<span data-ttu-id="ca8d3-p111">成功的响应由 `HTTP 200 OK` 响应代码表示，并在响应正文中包括指定的邮件，类似于 [更新邮件](../api/message-update.md) 中的响应。该响应不包括新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="ca8d3-235">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的邮件](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="ca8d3-235">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


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






