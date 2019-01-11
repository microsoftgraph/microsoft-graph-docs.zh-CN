---
title: 获取 multiValueLegacyExtendedProperty
description: 展开。
localization_priority: Normal
ms.openlocfilehash: 2dd97797fb15641e772d27d6ffb9652fabe3c04b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837742"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="12bf0-103">获取 multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="12bf0-103">Get multiValueLegacyExtendedProperty</span></span>

> <span data-ttu-id="12bf0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12bf0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12bf0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12bf0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12bf0-106">使用 `$expand` 获取包含多值扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="12bf0-106">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="12bf0-107">使用查询参数 `$expand`，可以获取使用指明的扩展属性扩展的指定实例。</span><span class="sxs-lookup"><span data-stu-id="12bf0-107">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="12bf0-108">这是当前获取 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="12bf0-108">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="12bf0-109">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="12bf0-109">The following user resources are supported:</span></span>

- [<span data-ttu-id="12bf0-110">日历</span><span class="sxs-lookup"><span data-stu-id="12bf0-110">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="12bf0-111">联系人</span><span class="sxs-lookup"><span data-stu-id="12bf0-111">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="12bf0-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="12bf0-112">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="12bf0-113">事件</span><span class="sxs-lookup"><span data-stu-id="12bf0-113">event</span></span>](../resources/event.md)
- [<span data-ttu-id="12bf0-114">mailFolder</span><span class="sxs-lookup"><span data-stu-id="12bf0-114">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="12bf0-115">message</span><span class="sxs-lookup"><span data-stu-id="12bf0-115">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="12bf0-116">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="12bf0-116">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="12bf0-117">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="12bf0-117">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="12bf0-118">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="12bf0-118">As well as the following group resources:</span></span>

- <span data-ttu-id="12bf0-119">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="12bf0-119">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="12bf0-120">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="12bf0-120">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="12bf0-121">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="12bf0-121">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="12bf0-122">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="12bf0-122">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="12bf0-123">权限</span><span class="sxs-lookup"><span data-stu-id="12bf0-123">Permissions</span></span>
<span data-ttu-id="12bf0-124">根据资源获得的扩展的属性和权限键入 （委派或应用程序） 您请求，若要调用此 API 至少是下表中所指定的权限。</span><span class="sxs-lookup"><span data-stu-id="12bf0-124">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="12bf0-125">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12bf0-125">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12bf0-126">支持的资源</span><span class="sxs-lookup"><span data-stu-id="12bf0-126">Supported resource</span></span> | <span data-ttu-id="12bf0-127">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12bf0-127">Delegated (work or school account)</span></span> | <span data-ttu-id="12bf0-128">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12bf0-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12bf0-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="12bf0-129">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="12bf0-130">日历</span><span class="sxs-lookup"><span data-stu-id="12bf0-130">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="12bf0-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-131">Calendars.Read</span></span> | <span data-ttu-id="12bf0-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-132">Calendars.Read</span></span> | <span data-ttu-id="12bf0-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-133">Calendars.Read</span></span> |
| [<span data-ttu-id="12bf0-134">联系人</span><span class="sxs-lookup"><span data-stu-id="12bf0-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="12bf0-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-135">Contacts.Read</span></span> | <span data-ttu-id="12bf0-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-136">Contacts.Read</span></span> | <span data-ttu-id="12bf0-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-137">Contacts.Read</span></span> |
| [<span data-ttu-id="12bf0-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="12bf0-138">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="12bf0-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-139">Contacts.Read</span></span> | <span data-ttu-id="12bf0-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-140">Contacts.Read</span></span> | <span data-ttu-id="12bf0-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-141">Contacts.Read</span></span> |
| [<span data-ttu-id="12bf0-142">事件</span><span class="sxs-lookup"><span data-stu-id="12bf0-142">event</span></span>](../resources/event.md) | <span data-ttu-id="12bf0-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-143">Calendars.Read</span></span> | <span data-ttu-id="12bf0-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-144">Calendars.Read</span></span> |  <span data-ttu-id="12bf0-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-145">Calendars.Read</span></span>|
| <span data-ttu-id="12bf0-146">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="12bf0-146">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="12bf0-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="12bf0-147">Group.Read.All</span></span> | <span data-ttu-id="12bf0-148">不支持</span><span class="sxs-lookup"><span data-stu-id="12bf0-148">Not supported</span></span> | <span data-ttu-id="12bf0-149">不支持</span><span class="sxs-lookup"><span data-stu-id="12bf0-149">Not supported</span></span> |
| <span data-ttu-id="12bf0-150">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="12bf0-150">group [event](../resources/event.md)</span></span> | <span data-ttu-id="12bf0-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="12bf0-151">Group.Read.All</span></span> | <span data-ttu-id="12bf0-152">不支持</span><span class="sxs-lookup"><span data-stu-id="12bf0-152">Not supported</span></span> | <span data-ttu-id="12bf0-153">不支持</span><span class="sxs-lookup"><span data-stu-id="12bf0-153">Not supported</span></span> |
| <span data-ttu-id="12bf0-154">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="12bf0-154">group [post](../resources/post.md)</span></span> | <span data-ttu-id="12bf0-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="12bf0-155">Group.Read.All</span></span> | <span data-ttu-id="12bf0-156">不支持</span><span class="sxs-lookup"><span data-stu-id="12bf0-156">Not supported</span></span> | <span data-ttu-id="12bf0-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="12bf0-157">Group.Read.All</span></span> |
| [<span data-ttu-id="12bf0-158">mailFolder</span><span class="sxs-lookup"><span data-stu-id="12bf0-158">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="12bf0-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-159">Mail.Read</span></span> | <span data-ttu-id="12bf0-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-160">Mail.Read</span></span> | <span data-ttu-id="12bf0-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-161">Mail.Read</span></span> |
| [<span data-ttu-id="12bf0-162">message</span><span class="sxs-lookup"><span data-stu-id="12bf0-162">message</span></span>](../resources/message.md) | <span data-ttu-id="12bf0-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-163">Mail.Read</span></span> | <span data-ttu-id="12bf0-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-164">Mail.Read</span></span> | <span data-ttu-id="12bf0-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-165">Mail.Read</span></span> |
| [<span data-ttu-id="12bf0-166">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="12bf0-166">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="12bf0-167">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-167">Tasks.Read</span></span> | <span data-ttu-id="12bf0-168">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-168">Tasks.Read</span></span> | <span data-ttu-id="12bf0-169">不支持</span><span class="sxs-lookup"><span data-stu-id="12bf0-169">Not supported</span></span> |
| [<span data-ttu-id="12bf0-170">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="12bf0-170">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="12bf0-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-171">Tasks.Read</span></span> | <span data-ttu-id="12bf0-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="12bf0-172">Tasks.Read</span></span> | <span data-ttu-id="12bf0-173">不支持</span><span class="sxs-lookup"><span data-stu-id="12bf0-173">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="12bf0-174">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12bf0-174">HTTP request</span></span>

<span data-ttu-id="12bf0-p104">获取通过与 **id** 属性中的筛选器匹配的扩展属性扩展的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="12bf0-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="12bf0-177">获取**邮件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="12bf0-177">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="12bf0-178">获取一个**mailFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="12bf0-178">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="12bf0-179">获取**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="12bf0-179">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="12bf0-180">获取**日历**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="12bf0-180">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="12bf0-181">获取**联系人**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="12bf0-181">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="12bf0-182">获取一个**contactFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="12bf0-182">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="12bf0-183">获取**outlookTask**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="12bf0-183">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="12bf0-184">获取**outlookTaskFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="12bf0-184">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="12bf0-185">获取组**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="12bf0-185">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="12bf0-186">获取一个组**发布**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="12bf0-186">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="12bf0-187">路径参数</span><span class="sxs-lookup"><span data-stu-id="12bf0-187">Path parameters</span></span>
|<span data-ttu-id="12bf0-188">**参数**</span><span class="sxs-lookup"><span data-stu-id="12bf0-188">**Parameter**</span></span>|<span data-ttu-id="12bf0-189">**类型**</span><span class="sxs-lookup"><span data-stu-id="12bf0-189">**Type**</span></span>|<span data-ttu-id="12bf0-190">**说明**</span><span class="sxs-lookup"><span data-stu-id="12bf0-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="12bf0-191">id_value</span><span class="sxs-lookup"><span data-stu-id="12bf0-191">id_value</span></span>|<span data-ttu-id="12bf0-192">String</span><span class="sxs-lookup"><span data-stu-id="12bf0-192">String</span></span>|<span data-ttu-id="12bf0-p105">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="12bf0-p105">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="12bf0-197">请求标头</span><span class="sxs-lookup"><span data-stu-id="12bf0-197">Request headers</span></span>
| <span data-ttu-id="12bf0-198">名称</span><span class="sxs-lookup"><span data-stu-id="12bf0-198">Name</span></span>      |<span data-ttu-id="12bf0-199">说明</span><span class="sxs-lookup"><span data-stu-id="12bf0-199">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="12bf0-200">Authorization</span><span class="sxs-lookup"><span data-stu-id="12bf0-200">Authorization</span></span>  | <span data-ttu-id="12bf0-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="12bf0-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12bf0-203">请求正文</span><span class="sxs-lookup"><span data-stu-id="12bf0-203">Request body</span></span>
<span data-ttu-id="12bf0-204">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="12bf0-204">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12bf0-205">响应</span><span class="sxs-lookup"><span data-stu-id="12bf0-205">Response</span></span>

<span data-ttu-id="12bf0-206">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="12bf0-206">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="12bf0-207">响应正文包括通过匹配的 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="12bf0-207">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="12bf0-208">示例</span><span class="sxs-lookup"><span data-stu-id="12bf0-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12bf0-209">请求</span><span class="sxs-lookup"><span data-stu-id="12bf0-209">Request</span></span>
<span data-ttu-id="12bf0-p107">此示例通过包含一个多值扩展属性获取并扩展指定的事件。此筛选器返回其 **id** 与字符串 `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation`（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="12bf0-p107">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="12bf0-212">响应</span><span class="sxs-lookup"><span data-stu-id="12bf0-212">Response</span></span>

<span data-ttu-id="12bf0-213">响应正文包括指定事件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="12bf0-213">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="12bf0-p108">注意：为了简单起见，会将此处所示的 **event** 对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12bf0-p108">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
