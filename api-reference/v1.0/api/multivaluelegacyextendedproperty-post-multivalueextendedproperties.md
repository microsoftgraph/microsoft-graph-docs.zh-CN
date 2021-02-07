---
title: 创建多值扩展属性
description: '在新建或现有的资源实例中创建一个或多个多值扩展属性。 '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d4e0d00fe59f74b0b53d116c5b2a34f73b94edcd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130541"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="127f7-103">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="127f7-103">Create multi-value extended property</span></span>

<span data-ttu-id="127f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="127f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="127f7-105">在新建或现有的资源实例中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="127f7-105">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span>

<span data-ttu-id="127f7-106">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="127f7-106">The following user resources are supported:</span></span>

- [<span data-ttu-id="127f7-107">日历</span><span class="sxs-lookup"><span data-stu-id="127f7-107">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="127f7-108">联系人</span><span class="sxs-lookup"><span data-stu-id="127f7-108">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="127f7-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="127f7-109">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="127f7-110">事件</span><span class="sxs-lookup"><span data-stu-id="127f7-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="127f7-111">mailFolder</span><span class="sxs-lookup"><span data-stu-id="127f7-111">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="127f7-112">邮件</span><span class="sxs-lookup"><span data-stu-id="127f7-112">message</span></span>](../resources/message.md)

<span data-ttu-id="127f7-113">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="127f7-113">As well as the following group resources:</span></span>

- <span data-ttu-id="127f7-114">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="127f7-114">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="127f7-115">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="127f7-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="127f7-116">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="127f7-116">group [post](../resources/post.md)</span></span>

<span data-ttu-id="127f7-117">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="127f7-117">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="127f7-118">权限</span><span class="sxs-lookup"><span data-stu-id="127f7-118">Permissions</span></span>
<span data-ttu-id="127f7-119">根据要创建扩展属性的资源以及请求的权限类型 (委托或应用程序) ，下表中指定的权限是调用此 API 所需的最低权限。</span><span class="sxs-lookup"><span data-stu-id="127f7-119">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="127f7-120">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="127f7-120">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="127f7-121">支持的资源</span><span class="sxs-lookup"><span data-stu-id="127f7-121">Supported resource</span></span> | <span data-ttu-id="127f7-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="127f7-122">Delegated (work or school account)</span></span> | <span data-ttu-id="127f7-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="127f7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="127f7-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="127f7-124">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="127f7-125">日历</span><span class="sxs-lookup"><span data-stu-id="127f7-125">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="127f7-126">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-126">Calendars.ReadWrite</span></span> | <span data-ttu-id="127f7-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="127f7-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-128">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="127f7-129">联系人</span><span class="sxs-lookup"><span data-stu-id="127f7-129">contact</span></span>](../resources/contact.md) | <span data-ttu-id="127f7-130">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-130">Contacts.ReadWrite</span></span> | <span data-ttu-id="127f7-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="127f7-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-132">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="127f7-133">contactFolder</span><span class="sxs-lookup"><span data-stu-id="127f7-133">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="127f7-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="127f7-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="127f7-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-136">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="127f7-137">事件</span><span class="sxs-lookup"><span data-stu-id="127f7-137">event</span></span>](../resources/event.md) | <span data-ttu-id="127f7-138">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-138">Calendars.ReadWrite</span></span> | <span data-ttu-id="127f7-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-139">Calendars.ReadWrite</span></span> |  <span data-ttu-id="127f7-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-140">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="127f7-141">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="127f7-141">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="127f7-142">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="127f7-142">Group.ReadWrite.All</span></span> | <span data-ttu-id="127f7-143">不支持</span><span class="sxs-lookup"><span data-stu-id="127f7-143">Not supported</span></span> | <span data-ttu-id="127f7-144">不支持</span><span class="sxs-lookup"><span data-stu-id="127f7-144">Not supported</span></span> |
| <span data-ttu-id="127f7-145">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="127f7-145">group [event](../resources/event.md)</span></span> | <span data-ttu-id="127f7-146">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="127f7-146">Group.ReadWrite.All</span></span> | <span data-ttu-id="127f7-147">不支持</span><span class="sxs-lookup"><span data-stu-id="127f7-147">Not supported</span></span> | <span data-ttu-id="127f7-148">不支持</span><span class="sxs-lookup"><span data-stu-id="127f7-148">Not supported</span></span> |
| <span data-ttu-id="127f7-149">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="127f7-149">group [post](../resources/post.md)</span></span> | <span data-ttu-id="127f7-150">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="127f7-150">Group.ReadWrite.All</span></span> | <span data-ttu-id="127f7-151">不支持</span><span class="sxs-lookup"><span data-stu-id="127f7-151">Not supported</span></span> | <span data-ttu-id="127f7-152">不支持</span><span class="sxs-lookup"><span data-stu-id="127f7-152">Not supported</span></span> |
| [<span data-ttu-id="127f7-153">mailFolder</span><span class="sxs-lookup"><span data-stu-id="127f7-153">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="127f7-154">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-154">Mail.ReadWrite</span></span> | <span data-ttu-id="127f7-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-155">Mail.ReadWrite</span></span> | <span data-ttu-id="127f7-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-156">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="127f7-157">邮件</span><span class="sxs-lookup"><span data-stu-id="127f7-157">message</span></span>](../resources/message.md) | <span data-ttu-id="127f7-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-158">Mail.ReadWrite</span></span> | <span data-ttu-id="127f7-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-159">Mail.ReadWrite</span></span> | <span data-ttu-id="127f7-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127f7-160">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="127f7-161">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="127f7-161">HTTP request</span></span>
<span data-ttu-id="127f7-162">可以在新建或现有的资源实例中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="127f7-162">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="127f7-p102">若要在 _新的_ 资源实例中创建一个或多个扩展属性，请使用与创建实例相同的 REST 请求，并包括新资源实例的属性和请求正文中的 _扩展属性_。注意，一些资源支持以多种方式创建。有关创建这些资源实例的详细信息，请参阅创建 [邮件](../resources/message.md)、[mailFolder](../api/user-post-mailfolders.md)、[事件](../api/user-post-events.md)、[日历](../api/user-post-calendars.md)、[联系人](../api/user-post-contacts.md)、[contactFolder](../api/user-post-contactfolders.md)、[组事件](../api/group-post-events.md)和 [组帖子](../resources/post.md) 的相应主题。</span><span class="sxs-lookup"><span data-stu-id="127f7-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span>

<span data-ttu-id="127f7-166">以下是请求的语法。</span><span class="sxs-lookup"><span data-stu-id="127f7-166">The following is the syntax of the requests.</span></span>

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

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="127f7-167">若要在现有资源实例中创建一个或多个扩展属性，请在请求中指定实例，并在请求正文中包括扩展属性。</span><span class="sxs-lookup"><span data-stu-id="127f7-167">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="127f7-168">**注意** 不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="127f7-168">**Note** You cannot create an extended property in an existing group post.</span></span>

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

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="127f7-169">请求标头</span><span class="sxs-lookup"><span data-stu-id="127f7-169">Request headers</span></span>
| <span data-ttu-id="127f7-170">名称</span><span class="sxs-lookup"><span data-stu-id="127f7-170">Name</span></span>       | <span data-ttu-id="127f7-171">值</span><span class="sxs-lookup"><span data-stu-id="127f7-171">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="127f7-172">Authorization</span><span class="sxs-lookup"><span data-stu-id="127f7-172">Authorization</span></span> | <span data-ttu-id="127f7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="127f7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="127f7-175">Content-Type</span><span class="sxs-lookup"><span data-stu-id="127f7-175">Content-Type</span></span> | <span data-ttu-id="127f7-176">application/json</span><span class="sxs-lookup"><span data-stu-id="127f7-176">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="127f7-177">请求正文</span><span class="sxs-lookup"><span data-stu-id="127f7-177">Request body</span></span>

<span data-ttu-id="127f7-178">提供每个 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象在资源实例的 **multiValueExtendedProperties** 集合属性中的 JSON 正文。</span><span class="sxs-lookup"><span data-stu-id="127f7-178">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="127f7-179">属性</span><span class="sxs-lookup"><span data-stu-id="127f7-179">Property</span></span>|<span data-ttu-id="127f7-180">类型</span><span class="sxs-lookup"><span data-stu-id="127f7-180">Type</span></span>|<span data-ttu-id="127f7-181">说明</span><span class="sxs-lookup"><span data-stu-id="127f7-181">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="127f7-182">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="127f7-182">multiValueExtendedProperties</span></span>|<span data-ttu-id="127f7-183">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="127f7-183">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="127f7-184">一个或多个多值扩展属性的数组。</span><span class="sxs-lookup"><span data-stu-id="127f7-184">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="127f7-185">id</span><span class="sxs-lookup"><span data-stu-id="127f7-185">id</span></span>|<span data-ttu-id="127f7-186">String</span><span class="sxs-lookup"><span data-stu-id="127f7-186">String</span></span>|<span data-ttu-id="127f7-p104">对于 **multiValueExtendedProperties** 集合中的每个属性，请指定此参数以标识属性。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="127f7-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="127f7-191">值</span><span class="sxs-lookup"><span data-stu-id="127f7-191">value</span></span>|<span data-ttu-id="127f7-192">string</span><span class="sxs-lookup"><span data-stu-id="127f7-192">string</span></span>|<span data-ttu-id="127f7-p105">对于 **multiValueExtendedProperties** 集合中的每个属性，请指定属性值。必需。</span><span class="sxs-lookup"><span data-stu-id="127f7-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="127f7-195">在新建资源实例中创建扩展属性时，除了新的 **multiValueExtendedProperties** 集合外，请提供该资源实例的 JSON 表示形式， (即消息 [、mailFolder](../resources/mailfolder.md) [、event](../resources/event.md)等) 。 [](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="127f7-195">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance as well (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.).</span></span>


## <a name="response"></a><span data-ttu-id="127f7-196">响应</span><span class="sxs-lookup"><span data-stu-id="127f7-196">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="127f7-197">响应代码</span><span class="sxs-lookup"><span data-stu-id="127f7-197">Response code</span></span>
<span data-ttu-id="127f7-198">在新建资源实例中成功创建扩展属性的操作返回 `201 Created`（在新的组帖子中除外），根据所用的方法，该操作可以返回 `200 OK` 或 `202 Accepted`。</span><span class="sxs-lookup"><span data-stu-id="127f7-198">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="127f7-199">在现有的资源实例中，成功的创建操作返回 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="127f7-199">In an existing resource instance, a successful create operation returns `200 OK`.</span></span>


#### <a name="response-body"></a><span data-ttu-id="127f7-200">响应正文</span><span class="sxs-lookup"><span data-stu-id="127f7-200">Response body</span></span>

<span data-ttu-id="127f7-p106">在支持的资源（而不是 [组帖子](../resources/post.md)）中创建扩展属性时，该响应只包括新建或现有的实例，但不包括新的扩展属性。若要查看新创建的扩展属性，请 [获取通过扩展属性展开的实例](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="127f7-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="127f7-p107">在 _新建_ 的组帖子中创建扩展属性时，响应仅包括响应代码，但不包括新帖子或扩展属性。不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="127f7-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="127f7-205">示例</span><span class="sxs-lookup"><span data-stu-id="127f7-205">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="127f7-206">请求 1</span><span class="sxs-lookup"><span data-stu-id="127f7-206">Request 1</span></span>

<span data-ttu-id="127f7-p108">第一个示例在同一个 POST 操作的全新事件中创建一个多值扩展属性。除了通常要包括的新事件的属性，请求正文还包括 **multiValueExtendedProperties** 集合（包含一个扩展属性）。请求正文包括该多值扩展属性的如下参数：</span><span class="sxs-lookup"><span data-stu-id="127f7-p108">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="127f7-210">**id**，将此属性指定为包含指定 GUID 和 `Recreation` 名称的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="127f7-210">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span>
- <span data-ttu-id="127f7-211">**value**，将 `Recreation` 指定为包含 3 个字符串值（`["Food", "Hiking", "Swimming"]`）的数组。</span><span class="sxs-lookup"><span data-stu-id="127f7-211">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
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

##### <a name="response-1"></a><span data-ttu-id="127f7-212">响应 1</span><span class="sxs-lookup"><span data-stu-id="127f7-212">Response 1</span></span>

<span data-ttu-id="127f7-p109">成功的响应由 `HTTP 201 Created` 响应代码表示，并在响应正文中包括新事件，类似于 [仅创建事件](../api/user-post-events.md) 中的响应。该响应不包括任何新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="127f7-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="127f7-215">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的事件](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="127f7-215">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="127f7-216">请求 2</span><span class="sxs-lookup"><span data-stu-id="127f7-216">Request 2</span></span>

<span data-ttu-id="127f7-p110">第二个示例为指定的邮件创建一个多值扩展属性。扩展属性是 **multiValueExtendedProperties** 集合中的唯一元素。请求正文包括扩展属性的如下参数：</span><span class="sxs-lookup"><span data-stu-id="127f7-p110">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="127f7-220">**id**，将此属性指定为包含指定 GUID 和名称 `Palette` 的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="127f7-220">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="127f7-221">**value**，将 `Palette` 指定为包含 3 个字符串值（`["Green", "Aqua", "Blue"]`）的数组。</span><span class="sxs-lookup"><span data-stu-id="127f7-221">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

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

##### <a name="response-2"></a><span data-ttu-id="127f7-222">响应 2</span><span class="sxs-lookup"><span data-stu-id="127f7-222">Response 2</span></span>

<span data-ttu-id="127f7-p111">成功的响应由 `HTTP 200 OK` 响应代码表示，并在响应正文中包括指定的邮件，类似于 [更新邮件](../api/message-update.md) 中的响应。该响应不包括新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="127f7-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="127f7-225">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的邮件](../api/multivaluelegacyextendedproperty-get.md)。</span><span class="sxs-lookup"><span data-stu-id="127f7-225">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


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





