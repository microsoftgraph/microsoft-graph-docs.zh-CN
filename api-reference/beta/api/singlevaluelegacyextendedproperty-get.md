---
title: 获取 singleValueLegacyExtendedProperty
description: 您可以获取单个资源实例展开为一个特定的扩展的属性或资源实例的集合
localization_priority: Normal
ms.openlocfilehash: ee9d51f945650c8051badd27f1b934d03f47cc7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873183"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="dbf53-103">获取 singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="dbf53-103">Get singleValueLegacyExtendedProperty</span></span>

> <span data-ttu-id="dbf53-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dbf53-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbf53-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dbf53-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbf53-106">可以获取使用特定扩展属性扩展的单个资源实例，或包含与筛选器匹配的扩展属性的资源实例集合。</span><span class="sxs-lookup"><span data-stu-id="dbf53-106">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="dbf53-107">使用查询参数 `$expand`，可以获取使用特定的扩展属性扩展的指定资源实例。</span><span class="sxs-lookup"><span data-stu-id="dbf53-107">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="dbf53-108">在 **id** 属性上使用 `$filter` 和 `eq` 运算符来指定扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-108">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="dbf53-109">这是当前获取 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="dbf53-109">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="dbf53-110">要获取具有某些扩展属性的资源实例，请使用 `$filter` 查询参数并在 **id** 属性上应用 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="dbf53-110">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="dbf53-111">另外，对于数字扩展属性，请在 **value** 属性上应用以下某个运算符：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="dbf53-111">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="dbf53-112">对于字符串类型的扩展属性，请在 **value** 上应用 `contains`、`startswith`、`eq` 或 `ne` 运算符。</span><span class="sxs-lookup"><span data-stu-id="dbf53-112">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span> 

<span data-ttu-id="dbf53-113">在扩展属性的 **id** 中筛选字符串名称 (`Name`) 是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="dbf53-113">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="dbf53-114">筛选扩展属性的 **value** 属性是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="dbf53-114">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="dbf53-115">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="dbf53-115">The following user resources are supported:</span></span>

- [<span data-ttu-id="dbf53-116">日历</span><span class="sxs-lookup"><span data-stu-id="dbf53-116">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="dbf53-117">联系人</span><span class="sxs-lookup"><span data-stu-id="dbf53-117">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="dbf53-118">contactFolder</span><span class="sxs-lookup"><span data-stu-id="dbf53-118">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="dbf53-119">事件</span><span class="sxs-lookup"><span data-stu-id="dbf53-119">event</span></span>](../resources/event.md)
- [<span data-ttu-id="dbf53-120">mailFolder</span><span class="sxs-lookup"><span data-stu-id="dbf53-120">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="dbf53-121">message</span><span class="sxs-lookup"><span data-stu-id="dbf53-121">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="dbf53-122">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="dbf53-122">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="dbf53-123">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="dbf53-123">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="dbf53-124">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="dbf53-124">As well as the following group resources:</span></span>

- <span data-ttu-id="dbf53-125">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="dbf53-125">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="dbf53-126">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="dbf53-126">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="dbf53-127">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="dbf53-127">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="dbf53-128">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="dbf53-128">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbf53-129">权限</span><span class="sxs-lookup"><span data-stu-id="dbf53-129">Permissions</span></span>
<span data-ttu-id="dbf53-130">根据资源获得的扩展的属性和权限键入 （委派或应用程序） 您请求，若要调用此 API 至少是下表中所指定的权限。</span><span class="sxs-lookup"><span data-stu-id="dbf53-130">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="dbf53-131">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbf53-131">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dbf53-132">支持的资源</span><span class="sxs-lookup"><span data-stu-id="dbf53-132">Supported resource</span></span> | <span data-ttu-id="dbf53-133">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbf53-133">Delegated (work or school account)</span></span> | <span data-ttu-id="dbf53-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbf53-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbf53-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbf53-135">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="dbf53-136">日历</span><span class="sxs-lookup"><span data-stu-id="dbf53-136">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="dbf53-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-137">Calendars.Read</span></span> | <span data-ttu-id="dbf53-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-138">Calendars.Read</span></span> | <span data-ttu-id="dbf53-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-139">Calendars.Read</span></span> |
| [<span data-ttu-id="dbf53-140">联系人</span><span class="sxs-lookup"><span data-stu-id="dbf53-140">contact</span></span>](../resources/contact.md) | <span data-ttu-id="dbf53-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-141">Contacts.Read</span></span> | <span data-ttu-id="dbf53-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-142">Contacts.Read</span></span> | <span data-ttu-id="dbf53-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-143">Contacts.Read</span></span> |
| [<span data-ttu-id="dbf53-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="dbf53-144">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="dbf53-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-145">Contacts.Read</span></span> | <span data-ttu-id="dbf53-146">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-146">Contacts.Read</span></span> | <span data-ttu-id="dbf53-147">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-147">Contacts.Read</span></span> |
| [<span data-ttu-id="dbf53-148">事件</span><span class="sxs-lookup"><span data-stu-id="dbf53-148">event</span></span>](../resources/event.md) | <span data-ttu-id="dbf53-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-149">Calendars.Read</span></span> | <span data-ttu-id="dbf53-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-150">Calendars.Read</span></span> |  <span data-ttu-id="dbf53-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-151">Calendars.Read</span></span>|
| <span data-ttu-id="dbf53-152">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="dbf53-152">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="dbf53-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbf53-153">Group.Read.All</span></span> | <span data-ttu-id="dbf53-154">不支持</span><span class="sxs-lookup"><span data-stu-id="dbf53-154">Not supported</span></span> | <span data-ttu-id="dbf53-155">不支持</span><span class="sxs-lookup"><span data-stu-id="dbf53-155">Not supported</span></span> |
| <span data-ttu-id="dbf53-156">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="dbf53-156">group [event](../resources/event.md)</span></span> | <span data-ttu-id="dbf53-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbf53-157">Group.Read.All</span></span> | <span data-ttu-id="dbf53-158">不支持</span><span class="sxs-lookup"><span data-stu-id="dbf53-158">Not supported</span></span> | <span data-ttu-id="dbf53-159">不支持</span><span class="sxs-lookup"><span data-stu-id="dbf53-159">Not supported</span></span> |
| <span data-ttu-id="dbf53-160">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="dbf53-160">group [post](../resources/post.md)</span></span> | <span data-ttu-id="dbf53-161">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbf53-161">Group.Read.All</span></span> | <span data-ttu-id="dbf53-162">不支持</span><span class="sxs-lookup"><span data-stu-id="dbf53-162">Not supported</span></span> | <span data-ttu-id="dbf53-163">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbf53-163">Group.Read.All</span></span> |
| [<span data-ttu-id="dbf53-164">mailFolder</span><span class="sxs-lookup"><span data-stu-id="dbf53-164">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="dbf53-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-165">Mail.Read</span></span> | <span data-ttu-id="dbf53-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-166">Mail.Read</span></span> | <span data-ttu-id="dbf53-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-167">Mail.Read</span></span> |
| [<span data-ttu-id="dbf53-168">message</span><span class="sxs-lookup"><span data-stu-id="dbf53-168">message</span></span>](../resources/message.md) | <span data-ttu-id="dbf53-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-169">Mail.Read</span></span> | <span data-ttu-id="dbf53-170">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-170">Mail.Read</span></span> | <span data-ttu-id="dbf53-171">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-171">Mail.Read</span></span> |
| [<span data-ttu-id="dbf53-172">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="dbf53-172">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="dbf53-173">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-173">Tasks.Read</span></span> | <span data-ttu-id="dbf53-174">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-174">Tasks.Read</span></span> | <span data-ttu-id="dbf53-175">不支持</span><span class="sxs-lookup"><span data-stu-id="dbf53-175">Not supported</span></span> |
| [<span data-ttu-id="dbf53-176">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="dbf53-176">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="dbf53-177">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-177">Tasks.Read</span></span> | <span data-ttu-id="dbf53-178">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="dbf53-178">Tasks.Read</span></span> | <span data-ttu-id="dbf53-179">不支持</span><span class="sxs-lookup"><span data-stu-id="dbf53-179">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="dbf53-180">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbf53-180">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="dbf53-181">获取通过与筛选器匹配的扩展属性扩展的资源实例</span><span class="sxs-lookup"><span data-stu-id="dbf53-181">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="dbf53-p106">获取通过与 **id** 属性中的筛选器匹配的扩展属性展开的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="dbf53-p106">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="dbf53-184">获取**邮件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-184">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="dbf53-185">获取一个**mailFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-185">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="dbf53-186">获取**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-186">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="dbf53-187">获取**日历**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-187">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="dbf53-188">获取**联系人**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-188">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="dbf53-189">获取一个**contactFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-189">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="dbf53-190">获取**outlookTask**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-190">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="dbf53-191">获取**outlookTaskFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-191">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="dbf53-192">获取组**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-192">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="dbf53-193">获取一个组**发布**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-193">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="dbf53-194">获取包括与筛选器匹配的数值扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="dbf53-194">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="dbf53-195">获取支持的资源实例，其中包含与筛选器匹配的数字扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-195">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="dbf53-196">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="dbf53-196">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="dbf53-197">请确保您应用使确保您应用于[URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)冒号、 正斜杠和空间下列中的筛选器字符串的字符。</span><span class="sxs-lookup"><span data-stu-id="dbf53-197">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="dbf53-198">以下语法行显示对 id 使用 `eq` 运算符的筛选器，对属性值使用另一个 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="dbf53-198">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="dbf53-199">可以使用适用于数值的其他运算符中的任何一个（`ne`、`ge`、`gt`、`le` 或 `lt`）替换 **value** 上的 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="dbf53-199">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="dbf53-200">获取**消息**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-200">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="dbf53-201">获取**mailFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-201">Get **mailFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="dbf53-202">获取**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-202">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="dbf53-203">获取**日历**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-203">Get **calendar** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="dbf53-204">获取**联系人**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-204">Get **contact** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="dbf53-205">获取**contactFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-205">Get **contactFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="dbf53-206">获取**outlookTask**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-206">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="dbf53-207">获取**outlookTaskFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-207">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="dbf53-208">获取组**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-208">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="dbf53-209">获取组**发布**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-209">Get group **post** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="dbf53-210">获取资源实例，其中包括与筛选器匹配的字符串类型的扩展属性</span><span class="sxs-lookup"><span data-stu-id="dbf53-210">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="dbf53-211">获取 **message** 或 **event** 资源的实例，其中包括与筛选器匹配的字符串类型的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-211">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="dbf53-212">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`contains`、`startswith`、`eq` 或 `ne`。</span><span class="sxs-lookup"><span data-stu-id="dbf53-212">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="dbf53-213">请务必对筛选器字符串中的以下字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)：冒号、正斜杠和空格。</span><span class="sxs-lookup"><span data-stu-id="dbf53-213">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="dbf53-214">获取**消息**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-214">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="dbf53-215">获取**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-215">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="dbf53-216">获取组**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="dbf53-216">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="dbf53-217">路径参数</span><span class="sxs-lookup"><span data-stu-id="dbf53-217">Path parameters</span></span>
|<span data-ttu-id="dbf53-218">**参数**</span><span class="sxs-lookup"><span data-stu-id="dbf53-218">**Parameter**</span></span>|<span data-ttu-id="dbf53-219">**类型**</span><span class="sxs-lookup"><span data-stu-id="dbf53-219">**Type**</span></span>|<span data-ttu-id="dbf53-220">**说明**</span><span class="sxs-lookup"><span data-stu-id="dbf53-220">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dbf53-221">id_value</span><span class="sxs-lookup"><span data-stu-id="dbf53-221">id_value</span></span>|<span data-ttu-id="dbf53-222">String</span><span class="sxs-lookup"><span data-stu-id="dbf53-222">String</span></span>|<span data-ttu-id="dbf53-p110">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="dbf53-p110">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="dbf53-227">property_value</span><span class="sxs-lookup"><span data-stu-id="dbf53-227">property_value</span></span> |<span data-ttu-id="dbf53-228">String</span><span class="sxs-lookup"><span data-stu-id="dbf53-228">String</span></span>|<span data-ttu-id="dbf53-229">要匹配的扩展属性的值。</span><span class="sxs-lookup"><span data-stu-id="dbf53-229">The value of the extended property to match.</span></span> <span data-ttu-id="dbf53-230">如果在上面的 **HTTP 请求**部分中列出，则为必需参数。</span><span class="sxs-lookup"><span data-stu-id="dbf53-230">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="dbf53-231">如果 {property_value} 不是字符串，请务必在与 {property_value} 比较时，将 `ep/value` 显式转换为相应的 Edm 数据类型。</span><span class="sxs-lookup"><span data-stu-id="dbf53-231">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="dbf53-232">有关示例，请参阅下面的[请求 4](#request-4)。</span><span class="sxs-lookup"><span data-stu-id="dbf53-232">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="dbf53-233">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbf53-233">Request headers</span></span>
| <span data-ttu-id="dbf53-234">名称</span><span class="sxs-lookup"><span data-stu-id="dbf53-234">Name</span></span>      |<span data-ttu-id="dbf53-235">说明</span><span class="sxs-lookup"><span data-stu-id="dbf53-235">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dbf53-236">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbf53-236">Authorization</span></span>  | <span data-ttu-id="dbf53-p112">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dbf53-p112">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbf53-239">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbf53-239">Request body</span></span>
<span data-ttu-id="dbf53-240">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dbf53-240">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbf53-241">响应</span><span class="sxs-lookup"><span data-stu-id="dbf53-241">Response</span></span>

<span data-ttu-id="dbf53-242">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="dbf53-242">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="dbf53-243">使用 `$expand` 获取资源实例</span><span class="sxs-lookup"><span data-stu-id="dbf53-243">GET resource instance using `$expand`</span></span>
<span data-ttu-id="dbf53-244">响应正文包括通过匹配的 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="dbf53-244">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="dbf53-245">获取包含与筛选器匹配的扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="dbf53-245">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="dbf53-246">响应主体包含一个或多个对象，它们表示包含匹配的扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="dbf53-246">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="dbf53-247">响应正文不包含扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-247">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="dbf53-248">示例</span><span class="sxs-lookup"><span data-stu-id="dbf53-248">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="dbf53-249">请求 1</span><span class="sxs-lookup"><span data-stu-id="dbf53-249">Request 1</span></span>

<span data-ttu-id="dbf53-p114">第一个示例通过包含一个单值扩展属性获取并展开指定的邮件。此筛选器返回其 **id** 与 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 字符串（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-p114">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="dbf53-252">响应 1</span><span class="sxs-lookup"><span data-stu-id="dbf53-252">Response 1</span></span>
<span data-ttu-id="dbf53-253">响应正文包括指定邮件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-253">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="dbf53-p115">注意：为了简单起见，会将此处所示的**邮件**对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-p115">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

#### <a name="request-2"></a><span data-ttu-id="dbf53-256">请求 2</span><span class="sxs-lookup"><span data-stu-id="dbf53-256">Request 2</span></span>

<span data-ttu-id="dbf53-257">第二个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="dbf53-257">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="dbf53-258">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="dbf53-258">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="dbf53-259">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="dbf53-259">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="dbf53-260">它的 **value** 等于字符串 `Green`。</span><span class="sxs-lookup"><span data-stu-id="dbf53-260">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="dbf53-261">响应 2</span><span class="sxs-lookup"><span data-stu-id="dbf53-261">Response 2</span></span>

<span data-ttu-id="dbf53-p117">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。响应正文是类似于[获取邮件集合](../api/user-list-messages.md)中的响应。该响应不包括匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-p117">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="dbf53-265">请求 3</span><span class="sxs-lookup"><span data-stu-id="dbf53-265">Request 3</span></span>

<span data-ttu-id="dbf53-266">第三个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="dbf53-266">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="dbf53-267">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="dbf53-267">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="dbf53-268">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="dbf53-268">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="dbf53-269">它的 **value** 包含字符串 `green`。</span><span class="sxs-lookup"><span data-stu-id="dbf53-269">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="dbf53-270">响应 3</span><span class="sxs-lookup"><span data-stu-id="dbf53-270">Response 3</span></span>

<span data-ttu-id="dbf53-271">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-271">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="dbf53-272">例如，如果邮件包含 **id** 等于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 的单值扩展属性和 **value** `Light green`，则会与筛选器匹配并包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="dbf53-272">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="dbf53-273">响应正文类似于[获取邮件集合](../api/user-list-messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="dbf53-273">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="dbf53-274">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-274">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="dbf53-275">请求 4</span><span class="sxs-lookup"><span data-stu-id="dbf53-275">Request 4</span></span>

<span data-ttu-id="dbf53-276">接下来的两个示例展示了如何获取具有非字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="dbf53-276">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="dbf53-277">为了方便阅读，从中删除了必要的 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="dbf53-277">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="dbf53-278">下面的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="dbf53-278">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="dbf53-279">它的 **id** 与字符串 `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid` 匹配。</span><span class="sxs-lookup"><span data-stu-id="dbf53-279">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="dbf53-280">它的 **value** 是 GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`。</span><span class="sxs-lookup"><span data-stu-id="dbf53-280">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="dbf53-281">若要将属性值与 GUID 比较，请将 `ep/value` 转换为 `Edm.Guid`。</span><span class="sxs-lookup"><span data-stu-id="dbf53-281">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="dbf53-282">接下来的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="dbf53-282">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="dbf53-283">它的 **id** 与字符串 `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete` 匹配。</span><span class="sxs-lookup"><span data-stu-id="dbf53-283">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="dbf53-284">它的 **value** 等于整数 12。</span><span class="sxs-lookup"><span data-stu-id="dbf53-284">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="dbf53-285">若要将属性值与整数比较，请将 `ep/value` 转换为 `Edm.Int32`。</span><span class="sxs-lookup"><span data-stu-id="dbf53-285">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="dbf53-286">响应 4</span><span class="sxs-lookup"><span data-stu-id="dbf53-286">Response 4</span></span>

<span data-ttu-id="dbf53-287">对于前面两个示例中的任意一个，成功响应由 `HTTP 200 OK` 响应代码表示，响应正文包括扩展属性与相应筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-287">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="dbf53-288">响应正文类似于[获取邮件集合](../api/user-list-messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="dbf53-288">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="dbf53-289">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dbf53-289">The response does not include the matching extended property.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
