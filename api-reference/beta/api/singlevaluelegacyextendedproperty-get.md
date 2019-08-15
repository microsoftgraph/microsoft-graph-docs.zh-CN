---
title: 获取 singleValueLegacyExtendedProperty
description: 可以使用特定的扩展属性或资源实例集合来获取扩展的单个资源实例
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d931f3050c0ff6a8f6507feb91cda371aa4b2e0d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410029"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="0853a-103">获取 singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="0853a-103">Get singleValueLegacyExtendedProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0853a-104">可以获取使用特定扩展属性扩展的单个资源实例，或包含与筛选器匹配的扩展属性的资源实例集合。</span><span class="sxs-lookup"><span data-stu-id="0853a-104">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="0853a-105">使用查询参数 `$expand`，可以获取使用特定的扩展属性扩展的指定资源实例。</span><span class="sxs-lookup"><span data-stu-id="0853a-105">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="0853a-106">在 **id** 属性上使用 `$filter` 和 `eq` 运算符来指定扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-106">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="0853a-107">这是当前获取 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="0853a-107">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="0853a-108">要获取具有某些扩展属性的资源实例，请使用 `$filter` 查询参数并在 **id** 属性上应用 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="0853a-108">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="0853a-109">另外，对于数字扩展属性，请在 **value** 属性上应用以下某个运算符：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="0853a-109">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="0853a-110">对于字符串类型的扩展属性，请在 **value** 上应用 `contains`、`startswith`、`eq` 或 `ne` 运算符。</span><span class="sxs-lookup"><span data-stu-id="0853a-110">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span> 

<span data-ttu-id="0853a-111">在扩展属性的 **id** 中筛选字符串名称 (`Name`) 是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="0853a-111">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="0853a-112">筛选扩展属性的 **value** 属性是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="0853a-112">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="0853a-113">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="0853a-113">The following user resources are supported:</span></span>

- [<span data-ttu-id="0853a-114">日历</span><span class="sxs-lookup"><span data-stu-id="0853a-114">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="0853a-115">联系人</span><span class="sxs-lookup"><span data-stu-id="0853a-115">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="0853a-116">contactFolder</span><span class="sxs-lookup"><span data-stu-id="0853a-116">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="0853a-117">事件</span><span class="sxs-lookup"><span data-stu-id="0853a-117">event</span></span>](../resources/event.md)
- [<span data-ttu-id="0853a-118">mailFolder</span><span class="sxs-lookup"><span data-stu-id="0853a-118">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="0853a-119">邮件</span><span class="sxs-lookup"><span data-stu-id="0853a-119">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="0853a-120">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="0853a-120">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="0853a-121">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="0853a-121">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="0853a-122">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="0853a-122">As well as the following group resources:</span></span>

- <span data-ttu-id="0853a-123">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="0853a-123">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="0853a-124">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="0853a-124">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="0853a-125">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="0853a-125">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="0853a-126">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="0853a-126">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0853a-127">权限</span><span class="sxs-lookup"><span data-stu-id="0853a-127">Permissions</span></span>
<span data-ttu-id="0853a-128">根据您要获取的扩展属性的资源以及所请求的权限类型 (委派或应用程序), 必须至少调用下表中指定的权限, 才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0853a-128">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="0853a-129">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0853a-129">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0853a-130">支持的资源</span><span class="sxs-lookup"><span data-stu-id="0853a-130">Supported resource</span></span> | <span data-ttu-id="0853a-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0853a-131">Delegated (work or school account)</span></span> | <span data-ttu-id="0853a-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0853a-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0853a-133">应用程序</span><span class="sxs-lookup"><span data-stu-id="0853a-133">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="0853a-134">calendar</span><span class="sxs-lookup"><span data-stu-id="0853a-134">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="0853a-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-135">Calendars.Read</span></span> | <span data-ttu-id="0853a-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-136">Calendars.Read</span></span> | <span data-ttu-id="0853a-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-137">Calendars.Read</span></span> |
| [<span data-ttu-id="0853a-138">联系人</span><span class="sxs-lookup"><span data-stu-id="0853a-138">contact</span></span>](../resources/contact.md) | <span data-ttu-id="0853a-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-139">Contacts.Read</span></span> | <span data-ttu-id="0853a-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-140">Contacts.Read</span></span> | <span data-ttu-id="0853a-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-141">Contacts.Read</span></span> |
| [<span data-ttu-id="0853a-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="0853a-142">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="0853a-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-143">Contacts.Read</span></span> | <span data-ttu-id="0853a-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-144">Contacts.Read</span></span> | <span data-ttu-id="0853a-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-145">Contacts.Read</span></span> |
| [<span data-ttu-id="0853a-146">事件</span><span class="sxs-lookup"><span data-stu-id="0853a-146">event</span></span>](../resources/event.md) | <span data-ttu-id="0853a-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-147">Calendars.Read</span></span> | <span data-ttu-id="0853a-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-148">Calendars.Read</span></span> |  <span data-ttu-id="0853a-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-149">Calendars.Read</span></span>|
| <span data-ttu-id="0853a-150">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="0853a-150">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="0853a-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0853a-151">Group.Read.All</span></span> | <span data-ttu-id="0853a-152">不支持</span><span class="sxs-lookup"><span data-stu-id="0853a-152">Not supported</span></span> | <span data-ttu-id="0853a-153">不支持</span><span class="sxs-lookup"><span data-stu-id="0853a-153">Not supported</span></span> |
| <span data-ttu-id="0853a-154">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="0853a-154">group [event](../resources/event.md)</span></span> | <span data-ttu-id="0853a-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0853a-155">Group.Read.All</span></span> | <span data-ttu-id="0853a-156">不支持</span><span class="sxs-lookup"><span data-stu-id="0853a-156">Not supported</span></span> | <span data-ttu-id="0853a-157">不支持</span><span class="sxs-lookup"><span data-stu-id="0853a-157">Not supported</span></span> |
| <span data-ttu-id="0853a-158">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="0853a-158">group [post](../resources/post.md)</span></span> | <span data-ttu-id="0853a-159">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0853a-159">Group.Read.All</span></span> | <span data-ttu-id="0853a-160">不支持</span><span class="sxs-lookup"><span data-stu-id="0853a-160">Not supported</span></span> | <span data-ttu-id="0853a-161">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0853a-161">Group.Read.All</span></span> |
| [<span data-ttu-id="0853a-162">mailFolder</span><span class="sxs-lookup"><span data-stu-id="0853a-162">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="0853a-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-163">Mail.Read</span></span> | <span data-ttu-id="0853a-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-164">Mail.Read</span></span> | <span data-ttu-id="0853a-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-165">Mail.Read</span></span> |
| [<span data-ttu-id="0853a-166">邮件</span><span class="sxs-lookup"><span data-stu-id="0853a-166">message</span></span>](../resources/message.md) | <span data-ttu-id="0853a-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-167">Mail.Read</span></span> | <span data-ttu-id="0853a-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-168">Mail.Read</span></span> | <span data-ttu-id="0853a-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-169">Mail.Read</span></span> |
| [<span data-ttu-id="0853a-170">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="0853a-170">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="0853a-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-171">Tasks.Read</span></span> | <span data-ttu-id="0853a-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-172">Tasks.Read</span></span> | <span data-ttu-id="0853a-173">不支持</span><span class="sxs-lookup"><span data-stu-id="0853a-173">Not supported</span></span> |
| [<span data-ttu-id="0853a-174">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="0853a-174">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="0853a-175">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-175">Tasks.Read</span></span> | <span data-ttu-id="0853a-176">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0853a-176">Tasks.Read</span></span> | <span data-ttu-id="0853a-177">不支持</span><span class="sxs-lookup"><span data-stu-id="0853a-177">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="0853a-178">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0853a-178">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="0853a-179">获取通过与筛选器匹配的扩展属性扩展的资源实例</span><span class="sxs-lookup"><span data-stu-id="0853a-179">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="0853a-p105">获取通过与 **id** 属性中的筛选器匹配的扩展属性展开的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="0853a-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="0853a-182">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-182">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="0853a-183">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-183">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="0853a-184">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-184">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="0853a-185">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-185">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="0853a-186">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-186">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="0853a-187">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-187">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="0853a-188">获取**outlookTask**实例:</span><span class="sxs-lookup"><span data-stu-id="0853a-188">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="0853a-189">获取**outlookTaskFolder**实例:</span><span class="sxs-lookup"><span data-stu-id="0853a-189">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="0853a-190">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-190">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="0853a-191">获取组 **post** 实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-191">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="0853a-192">获取包括与筛选器匹配的数值扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="0853a-192">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="0853a-193">获取支持的资源实例，其中包含与筛选器匹配的数字扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-193">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="0853a-194">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="0853a-194">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="0853a-195">确保应用将[URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)应用于筛选器字符串-冒号、正斜杠和空格中的以下字符。</span><span class="sxs-lookup"><span data-stu-id="0853a-195">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="0853a-196">以下语法行显示对 id 使用 `eq` 运算符的筛选器，对属性值使用另一个 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="0853a-196">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="0853a-197">可以使用适用于数值的其他运算符中的任何一个（`ne`、`ge`、`gt`、`le` 或 `lt`）替换 **value** 上的 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="0853a-197">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="0853a-198">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-198">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="0853a-199">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-199">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="0853a-200">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-200">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="0853a-201">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-201">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="0853a-202">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-202">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="0853a-203">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-203">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="0853a-204">获取**outlookTask**实例:</span><span class="sxs-lookup"><span data-stu-id="0853a-204">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="0853a-205">获取**outlookTaskFolder**实例:</span><span class="sxs-lookup"><span data-stu-id="0853a-205">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="0853a-206">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-206">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="0853a-207">获取组 **post** 实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-207">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="0853a-208">获取资源实例，其中包括与筛选器匹配的字符串类型的扩展属性</span><span class="sxs-lookup"><span data-stu-id="0853a-208">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="0853a-209">获取 **message** 或 **event** 资源的实例，其中包括与筛选器匹配的字符串类型的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-209">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="0853a-210">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`contains`、`startswith`、`eq` 或 `ne`。</span><span class="sxs-lookup"><span data-stu-id="0853a-210">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="0853a-211">请务必对筛选器字符串中的以下字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)：冒号、正斜杠和空格。</span><span class="sxs-lookup"><span data-stu-id="0853a-211">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="0853a-212">获取 **message** 实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-212">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
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

<span data-ttu-id="0853a-213">获取 **event** 实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-213">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
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

<span data-ttu-id="0853a-214">获取组 **event** 实例：</span><span class="sxs-lookup"><span data-stu-id="0853a-214">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="0853a-215">路径参数</span><span class="sxs-lookup"><span data-stu-id="0853a-215">Path parameters</span></span>
|<span data-ttu-id="0853a-216">**参数**</span><span class="sxs-lookup"><span data-stu-id="0853a-216">**Parameter**</span></span>|<span data-ttu-id="0853a-217">**类型**</span><span class="sxs-lookup"><span data-stu-id="0853a-217">**Type**</span></span>|<span data-ttu-id="0853a-218">**说明**</span><span class="sxs-lookup"><span data-stu-id="0853a-218">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0853a-219">id_value</span><span class="sxs-lookup"><span data-stu-id="0853a-219">id_value</span></span>|<span data-ttu-id="0853a-220">String</span><span class="sxs-lookup"><span data-stu-id="0853a-220">String</span></span>|<span data-ttu-id="0853a-p109">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="0853a-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="0853a-225">property_value</span><span class="sxs-lookup"><span data-stu-id="0853a-225">property_value</span></span> |<span data-ttu-id="0853a-226">String</span><span class="sxs-lookup"><span data-stu-id="0853a-226">String</span></span>|<span data-ttu-id="0853a-227">要匹配的扩展属性的值。</span><span class="sxs-lookup"><span data-stu-id="0853a-227">The value of the extended property to match.</span></span> <span data-ttu-id="0853a-228">如果在上面的 **HTTP 请求**部分中列出，则为必需参数。</span><span class="sxs-lookup"><span data-stu-id="0853a-228">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="0853a-229">如果 {property_value} 不是字符串，请务必在与 {property_value} 比较时，将 `ep/value` 显式转换为相应的 Edm 数据类型。</span><span class="sxs-lookup"><span data-stu-id="0853a-229">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="0853a-230">有关示例，请参阅下面的[请求 4](#request-4)。</span><span class="sxs-lookup"><span data-stu-id="0853a-230">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0853a-231">请求标头</span><span class="sxs-lookup"><span data-stu-id="0853a-231">Request headers</span></span>
| <span data-ttu-id="0853a-232">名称</span><span class="sxs-lookup"><span data-stu-id="0853a-232">Name</span></span>      |<span data-ttu-id="0853a-233">说明</span><span class="sxs-lookup"><span data-stu-id="0853a-233">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0853a-234">Authorization</span><span class="sxs-lookup"><span data-stu-id="0853a-234">Authorization</span></span>  | <span data-ttu-id="0853a-p111">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0853a-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0853a-237">请求正文</span><span class="sxs-lookup"><span data-stu-id="0853a-237">Request body</span></span>
<span data-ttu-id="0853a-238">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0853a-238">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0853a-239">响应</span><span class="sxs-lookup"><span data-stu-id="0853a-239">Response</span></span>

<span data-ttu-id="0853a-240">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0853a-240">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="0853a-241">使用 `$expand` 获取资源实例</span><span class="sxs-lookup"><span data-stu-id="0853a-241">GET resource instance using `$expand`</span></span>
<span data-ttu-id="0853a-242">响应正文包括通过匹配的 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="0853a-242">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="0853a-243">获取包含与筛选器匹配的扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="0853a-243">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="0853a-244">响应主体包含一个或多个对象，它们表示包含匹配的扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="0853a-244">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="0853a-245">响应正文不包含扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-245">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="0853a-246">示例</span><span class="sxs-lookup"><span data-stu-id="0853a-246">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="0853a-247">请求 1</span><span class="sxs-lookup"><span data-stu-id="0853a-247">Request 1</span></span>

<span data-ttu-id="0853a-p113">第一个示例通过包含一个单值扩展属性获取并展开指定的邮件。此筛选器返回其 **id** 与 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 字符串（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0853a-250">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0853a-250">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=/?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0853a-251">C#</span><span class="sxs-lookup"><span data-stu-id="0853a-251">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-singlevaluelegacyextendedproperty-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0853a-252">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0853a-252">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-singlevaluelegacyextendedproperty-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0853a-253">目标-C</span><span class="sxs-lookup"><span data-stu-id="0853a-253">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-singlevaluelegacyextendedproperty-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response-1"></a><span data-ttu-id="0853a-254">响应 1</span><span class="sxs-lookup"><span data-stu-id="0853a-254">Response 1</span></span>
<span data-ttu-id="0853a-255">响应正文包括指定邮件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-255">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="0853a-p114">注意：为了简单起见，会将此处所示的**邮件**对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="0853a-258">请求 2</span><span class="sxs-lookup"><span data-stu-id="0853a-258">Request 2</span></span>

<span data-ttu-id="0853a-259">第二个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="0853a-259">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="0853a-260">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="0853a-260">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="0853a-261">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="0853a-261">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="0853a-262">它的 **value** 等于字符串 `Green`。</span><span class="sxs-lookup"><span data-stu-id="0853a-262">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="0853a-263">响应 2</span><span class="sxs-lookup"><span data-stu-id="0853a-263">Response 2</span></span>

<span data-ttu-id="0853a-p116">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。响应正文是类似于[获取邮件集合](../api/user-list-messages.md)中的响应。该响应不包括匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="0853a-267">请求 3</span><span class="sxs-lookup"><span data-stu-id="0853a-267">Request 3</span></span>

<span data-ttu-id="0853a-268">第三个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="0853a-268">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="0853a-269">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="0853a-269">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="0853a-270">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="0853a-270">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="0853a-271">它的 **value** 包含字符串 `green`。</span><span class="sxs-lookup"><span data-stu-id="0853a-271">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="0853a-272">响应 3</span><span class="sxs-lookup"><span data-stu-id="0853a-272">Response 3</span></span>

<span data-ttu-id="0853a-273">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-273">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="0853a-274">例如，如果邮件包含 **id** 等于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 的单值扩展属性和 **value** `Light green`，则会与筛选器匹配并包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="0853a-274">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="0853a-275">响应正文类似于[获取邮件集合](../api/user-list-messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="0853a-275">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="0853a-276">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-276">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="0853a-277">请求 4</span><span class="sxs-lookup"><span data-stu-id="0853a-277">Request 4</span></span>

<span data-ttu-id="0853a-278">接下来的两个示例展示了如何获取具有非字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="0853a-278">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="0853a-279">为了方便阅读，从中删除了必要的 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="0853a-279">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="0853a-280">下面的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="0853a-280">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="0853a-281">它的 **id** 与字符串 `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid` 匹配。</span><span class="sxs-lookup"><span data-stu-id="0853a-281">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="0853a-282">它的 **value** 是 GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`。</span><span class="sxs-lookup"><span data-stu-id="0853a-282">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="0853a-283">若要将属性值与 GUID 比较，请将 `ep/value` 转换为 `Edm.Guid`。</span><span class="sxs-lookup"><span data-stu-id="0853a-283">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="0853a-284">接下来的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="0853a-284">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="0853a-285">它的 **id** 与字符串 `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete` 匹配。</span><span class="sxs-lookup"><span data-stu-id="0853a-285">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="0853a-286">它的 **value** 等于整数 12。</span><span class="sxs-lookup"><span data-stu-id="0853a-286">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="0853a-287">若要将属性值与整数比较，请将 `ep/value` 转换为 `Edm.Int32`。</span><span class="sxs-lookup"><span data-stu-id="0853a-287">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="0853a-288">响应 4</span><span class="sxs-lookup"><span data-stu-id="0853a-288">Response 4</span></span>

<span data-ttu-id="0853a-289">对于前面两个示例中的任意一个，成功响应由 `HTTP 200 OK` 响应代码表示，响应正文包括扩展属性与相应筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-289">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="0853a-290">响应正文类似于[获取邮件集合](../api/user-list-messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="0853a-290">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="0853a-291">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0853a-291">The response does not include the matching extended property.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
