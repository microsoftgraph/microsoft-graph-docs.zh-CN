---
title: 获取 singleValueLegacyExtendedProperty
description: 您可以获取单个资源实例展开为一个特定的扩展的属性或资源实例的集合
localization_priority: Normal
ms.openlocfilehash: ead4881737f4431138d444ffe8df131c22c131fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525092"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="66067-103">获取 singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="66067-103">Get singleValueLegacyExtendedProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66067-104">可以获取使用特定扩展属性扩展的单个资源实例，或包含与筛选器匹配的扩展属性的资源实例集合。</span><span class="sxs-lookup"><span data-stu-id="66067-104">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="66067-105">使用查询参数 `$expand`，可以获取使用特定的扩展属性扩展的指定资源实例。</span><span class="sxs-lookup"><span data-stu-id="66067-105">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="66067-106">在 **id** 属性上使用 `$filter` 和 `eq` 运算符来指定扩展属性。</span><span class="sxs-lookup"><span data-stu-id="66067-106">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="66067-107">这是当前获取 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="66067-107">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="66067-108">要获取具有某些扩展属性的资源实例，请使用 `$filter` 查询参数并在 **id** 属性上应用 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="66067-108">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="66067-109">另外，对于数字扩展属性，请在 **value** 属性上应用以下某个运算符：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="66067-109">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="66067-110">对于字符串类型的扩展属性，请在 **value** 上应用 `contains`、`startswith`、`eq` 或 `ne` 运算符。</span><span class="sxs-lookup"><span data-stu-id="66067-110">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span> 

<span data-ttu-id="66067-111">在扩展属性的 **id** 中筛选字符串名称 (`Name`) 是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="66067-111">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="66067-112">筛选扩展属性的 **value** 属性是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="66067-112">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="66067-113">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="66067-113">The following user resources are supported:</span></span>

- [<span data-ttu-id="66067-114">日历</span><span class="sxs-lookup"><span data-stu-id="66067-114">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="66067-115">联系人</span><span class="sxs-lookup"><span data-stu-id="66067-115">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="66067-116">contactFolder</span><span class="sxs-lookup"><span data-stu-id="66067-116">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="66067-117">event</span><span class="sxs-lookup"><span data-stu-id="66067-117">event</span></span>](../resources/event.md)
- [<span data-ttu-id="66067-118">mailFolder</span><span class="sxs-lookup"><span data-stu-id="66067-118">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="66067-119">message</span><span class="sxs-lookup"><span data-stu-id="66067-119">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="66067-120">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="66067-120">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="66067-121">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="66067-121">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="66067-122">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="66067-122">As well as the following group resources:</span></span>

- <span data-ttu-id="66067-123">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="66067-123">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="66067-124">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="66067-124">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="66067-125">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="66067-125">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="66067-126">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="66067-126">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="66067-127">权限</span><span class="sxs-lookup"><span data-stu-id="66067-127">Permissions</span></span>
<span data-ttu-id="66067-128">根据资源获得的扩展的属性和权限键入 （委派或应用程序） 您请求，若要调用此 API 至少是下表中所指定的权限。</span><span class="sxs-lookup"><span data-stu-id="66067-128">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="66067-129">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66067-129">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66067-130">支持的资源</span><span class="sxs-lookup"><span data-stu-id="66067-130">Supported resource</span></span> | <span data-ttu-id="66067-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66067-131">Delegated (work or school account)</span></span> | <span data-ttu-id="66067-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66067-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66067-133">应用程序</span><span class="sxs-lookup"><span data-stu-id="66067-133">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="66067-134">日历</span><span class="sxs-lookup"><span data-stu-id="66067-134">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="66067-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66067-135">Calendars.Read</span></span> | <span data-ttu-id="66067-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66067-136">Calendars.Read</span></span> | <span data-ttu-id="66067-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66067-137">Calendars.Read</span></span> |
| [<span data-ttu-id="66067-138">联系人</span><span class="sxs-lookup"><span data-stu-id="66067-138">contact</span></span>](../resources/contact.md) | <span data-ttu-id="66067-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66067-139">Contacts.Read</span></span> | <span data-ttu-id="66067-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66067-140">Contacts.Read</span></span> | <span data-ttu-id="66067-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66067-141">Contacts.Read</span></span> |
| [<span data-ttu-id="66067-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="66067-142">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="66067-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66067-143">Contacts.Read</span></span> | <span data-ttu-id="66067-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66067-144">Contacts.Read</span></span> | <span data-ttu-id="66067-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66067-145">Contacts.Read</span></span> |
| [<span data-ttu-id="66067-146">event</span><span class="sxs-lookup"><span data-stu-id="66067-146">event</span></span>](../resources/event.md) | <span data-ttu-id="66067-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66067-147">Calendars.Read</span></span> | <span data-ttu-id="66067-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66067-148">Calendars.Read</span></span> |  <span data-ttu-id="66067-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66067-149">Calendars.Read</span></span>|
| <span data-ttu-id="66067-150">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="66067-150">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="66067-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="66067-151">Group.Read.All</span></span> | <span data-ttu-id="66067-152">不支持</span><span class="sxs-lookup"><span data-stu-id="66067-152">Not supported</span></span> | <span data-ttu-id="66067-153">不支持</span><span class="sxs-lookup"><span data-stu-id="66067-153">Not supported</span></span> |
| <span data-ttu-id="66067-154">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="66067-154">group [event](../resources/event.md)</span></span> | <span data-ttu-id="66067-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="66067-155">Group.Read.All</span></span> | <span data-ttu-id="66067-156">不支持</span><span class="sxs-lookup"><span data-stu-id="66067-156">Not supported</span></span> | <span data-ttu-id="66067-157">不支持</span><span class="sxs-lookup"><span data-stu-id="66067-157">Not supported</span></span> |
| <span data-ttu-id="66067-158">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="66067-158">group [post](../resources/post.md)</span></span> | <span data-ttu-id="66067-159">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="66067-159">Group.Read.All</span></span> | <span data-ttu-id="66067-160">不支持</span><span class="sxs-lookup"><span data-stu-id="66067-160">Not supported</span></span> | <span data-ttu-id="66067-161">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="66067-161">Group.Read.All</span></span> |
| [<span data-ttu-id="66067-162">mailFolder</span><span class="sxs-lookup"><span data-stu-id="66067-162">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="66067-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66067-163">Mail.Read</span></span> | <span data-ttu-id="66067-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66067-164">Mail.Read</span></span> | <span data-ttu-id="66067-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66067-165">Mail.Read</span></span> |
| [<span data-ttu-id="66067-166">message</span><span class="sxs-lookup"><span data-stu-id="66067-166">message</span></span>](../resources/message.md) | <span data-ttu-id="66067-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66067-167">Mail.Read</span></span> | <span data-ttu-id="66067-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66067-168">Mail.Read</span></span> | <span data-ttu-id="66067-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66067-169">Mail.Read</span></span> |
| [<span data-ttu-id="66067-170">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="66067-170">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="66067-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="66067-171">Tasks.Read</span></span> | <span data-ttu-id="66067-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="66067-172">Tasks.Read</span></span> | <span data-ttu-id="66067-173">不支持</span><span class="sxs-lookup"><span data-stu-id="66067-173">Not supported</span></span> |
| [<span data-ttu-id="66067-174">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="66067-174">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="66067-175">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="66067-175">Tasks.Read</span></span> | <span data-ttu-id="66067-176">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="66067-176">Tasks.Read</span></span> | <span data-ttu-id="66067-177">不支持</span><span class="sxs-lookup"><span data-stu-id="66067-177">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="66067-178">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66067-178">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="66067-179">获取通过与筛选器匹配的扩展属性扩展的资源实例</span><span class="sxs-lookup"><span data-stu-id="66067-179">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="66067-p105">获取通过与 **id** 属性中的筛选器匹配的扩展属性展开的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="66067-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="66067-182">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="66067-182">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="66067-183">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-183">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="66067-184">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="66067-184">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="66067-185">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="66067-185">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="66067-186">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="66067-186">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="66067-187">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-187">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="66067-188">获取**outlookTask**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="66067-188">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="66067-189">获取**outlookTaskFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="66067-189">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="66067-190">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="66067-190">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="66067-191">获取组 **post** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-191">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="66067-192">获取包括与筛选器匹配的数值扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="66067-192">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="66067-193">获取支持的资源实例，其中包含与筛选器匹配的数字扩展属性。</span><span class="sxs-lookup"><span data-stu-id="66067-193">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="66067-194">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="66067-194">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="66067-195">请确保您应用使确保您应用于[URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)冒号、 正斜杠和空间下列中的筛选器字符串的字符。</span><span class="sxs-lookup"><span data-stu-id="66067-195">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="66067-196">以下语法行显示对 id 使用 `eq` 运算符的筛选器，对属性值使用另一个 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="66067-196">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="66067-197">可以使用适用于数值的其他运算符中的任何一个（`ne`、`ge`、`gt`、`le` 或 `lt`）替换 **value** 上的 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="66067-197">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="66067-198">获取 **message** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-198">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="66067-199">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-199">Get **mailFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="66067-200">获取 **event** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-200">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="66067-201">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="66067-201">Get **calendar** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="66067-202">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="66067-202">Get **contact** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="66067-203">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-203">Get **contactFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="66067-204">获取**outlookTask**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="66067-204">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="66067-205">获取**outlookTaskFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="66067-205">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="66067-206">获取组 **event** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-206">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="66067-207">获取组 **post** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-207">Get group **post** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="66067-208">获取资源实例，其中包括与筛选器匹配的字符串类型的扩展属性</span><span class="sxs-lookup"><span data-stu-id="66067-208">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="66067-209">获取 **message** 或 **event** 资源的实例，其中包括与筛选器匹配的字符串类型的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="66067-209">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="66067-210">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`contains`、`startswith`、`eq` 或 `ne`。</span><span class="sxs-lookup"><span data-stu-id="66067-210">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="66067-211">请务必对筛选器字符串中的以下字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)：冒号、正斜杠和空格。</span><span class="sxs-lookup"><span data-stu-id="66067-211">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="66067-212">获取 **message** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-212">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="66067-213">获取 **event** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-213">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="66067-214">获取组 **event** 实例：</span><span class="sxs-lookup"><span data-stu-id="66067-214">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="66067-215">路径参数</span><span class="sxs-lookup"><span data-stu-id="66067-215">Path parameters</span></span>
|<span data-ttu-id="66067-216">**参数**</span><span class="sxs-lookup"><span data-stu-id="66067-216">**Parameter**</span></span>|<span data-ttu-id="66067-217">**类型**</span><span class="sxs-lookup"><span data-stu-id="66067-217">**Type**</span></span>|<span data-ttu-id="66067-218">**说明**</span><span class="sxs-lookup"><span data-stu-id="66067-218">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="66067-219">id_value</span><span class="sxs-lookup"><span data-stu-id="66067-219">id_value</span></span>|<span data-ttu-id="66067-220">String</span><span class="sxs-lookup"><span data-stu-id="66067-220">String</span></span>|<span data-ttu-id="66067-p109">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="66067-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="66067-225">property_value</span><span class="sxs-lookup"><span data-stu-id="66067-225">property_value</span></span> |<span data-ttu-id="66067-226">String</span><span class="sxs-lookup"><span data-stu-id="66067-226">String</span></span>|<span data-ttu-id="66067-227">要匹配的扩展属性的值。</span><span class="sxs-lookup"><span data-stu-id="66067-227">The value of the extended property to match.</span></span> <span data-ttu-id="66067-228">如果在上面的 **HTTP 请求**部分中列出，则为必需参数。</span><span class="sxs-lookup"><span data-stu-id="66067-228">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="66067-229">如果 {property_value} 不是字符串，请务必在与 {property_value} 比较时，将 `ep/value` 显式转换为相应的 Edm 数据类型。</span><span class="sxs-lookup"><span data-stu-id="66067-229">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="66067-230">有关示例，请参阅下面的[请求 4](#request-4)。</span><span class="sxs-lookup"><span data-stu-id="66067-230">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="66067-231">请求标头</span><span class="sxs-lookup"><span data-stu-id="66067-231">Request headers</span></span>
| <span data-ttu-id="66067-232">名称</span><span class="sxs-lookup"><span data-stu-id="66067-232">Name</span></span>      |<span data-ttu-id="66067-233">说明</span><span class="sxs-lookup"><span data-stu-id="66067-233">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66067-234">Authorization</span><span class="sxs-lookup"><span data-stu-id="66067-234">Authorization</span></span>  | <span data-ttu-id="66067-p111">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66067-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66067-237">请求正文</span><span class="sxs-lookup"><span data-stu-id="66067-237">Request body</span></span>
<span data-ttu-id="66067-238">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66067-238">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66067-239">响应</span><span class="sxs-lookup"><span data-stu-id="66067-239">Response</span></span>

<span data-ttu-id="66067-240">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="66067-240">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="66067-241">使用 `$expand` 获取资源实例</span><span class="sxs-lookup"><span data-stu-id="66067-241">GET resource instance using `$expand`</span></span>
<span data-ttu-id="66067-242">响应正文包括通过匹配的 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="66067-242">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="66067-243">获取包含与筛选器匹配的扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="66067-243">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="66067-244">响应主体包含一个或多个对象，它们表示包含匹配的扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="66067-244">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="66067-245">响应正文不包含扩展属性。</span><span class="sxs-lookup"><span data-stu-id="66067-245">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="66067-246">示例</span><span class="sxs-lookup"><span data-stu-id="66067-246">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="66067-247">请求 1</span><span class="sxs-lookup"><span data-stu-id="66067-247">Request 1</span></span>

<span data-ttu-id="66067-p113">第一个示例通过包含一个单值扩展属性获取并展开指定的邮件。此筛选器返回其 **id** 与 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 字符串（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="66067-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="66067-250">响应 1</span><span class="sxs-lookup"><span data-stu-id="66067-250">Response 1</span></span>
<span data-ttu-id="66067-251">响应正文包括指定邮件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="66067-251">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="66067-p114">注意：为了简单起见，会将此处所示的**邮件**对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66067-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="66067-254">请求 2</span><span class="sxs-lookup"><span data-stu-id="66067-254">Request 2</span></span>

<span data-ttu-id="66067-255">第二个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="66067-255">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="66067-256">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="66067-256">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="66067-257">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="66067-257">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="66067-258">它的 **value** 等于字符串 `Green`。</span><span class="sxs-lookup"><span data-stu-id="66067-258">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="66067-259">响应 2</span><span class="sxs-lookup"><span data-stu-id="66067-259">Response 2</span></span>

<span data-ttu-id="66067-p116">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。响应正文是类似于[获取邮件集合](../api/user-list-messages.md)中的响应。该响应不包括匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="66067-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="66067-263">请求 3</span><span class="sxs-lookup"><span data-stu-id="66067-263">Request 3</span></span>

<span data-ttu-id="66067-264">第三个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="66067-264">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="66067-265">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="66067-265">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="66067-266">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="66067-266">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="66067-267">它的 **value** 包含字符串 `green`。</span><span class="sxs-lookup"><span data-stu-id="66067-267">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="66067-268">响应 3</span><span class="sxs-lookup"><span data-stu-id="66067-268">Response 3</span></span>

<span data-ttu-id="66067-269">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="66067-269">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="66067-270">例如，如果邮件包含 **id** 等于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 的单值扩展属性和 **value** `Light green`，则会与筛选器匹配并包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="66067-270">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="66067-271">响应正文类似于[获取邮件集合](../api/user-list-messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="66067-271">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="66067-272">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="66067-272">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="66067-273">请求 4</span><span class="sxs-lookup"><span data-stu-id="66067-273">Request 4</span></span>

<span data-ttu-id="66067-274">接下来的两个示例展示了如何获取具有非字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="66067-274">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="66067-275">为了方便阅读，从中删除了必要的 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="66067-275">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="66067-276">下面的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="66067-276">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="66067-277">它的 **id** 与字符串 `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid` 匹配。</span><span class="sxs-lookup"><span data-stu-id="66067-277">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="66067-278">它的 **value** 是 GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`。</span><span class="sxs-lookup"><span data-stu-id="66067-278">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="66067-279">若要将属性值与 GUID 比较，请将 `ep/value` 转换为 `Edm.Guid`。</span><span class="sxs-lookup"><span data-stu-id="66067-279">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="66067-280">接下来的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="66067-280">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="66067-281">它的 **id** 与字符串 `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete` 匹配。</span><span class="sxs-lookup"><span data-stu-id="66067-281">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="66067-282">它的 **value** 等于整数 12。</span><span class="sxs-lookup"><span data-stu-id="66067-282">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="66067-283">若要将属性值与整数比较，请将 `ep/value` 转换为 `Edm.Int32`。</span><span class="sxs-lookup"><span data-stu-id="66067-283">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="66067-284">响应 4</span><span class="sxs-lookup"><span data-stu-id="66067-284">Response 4</span></span>

<span data-ttu-id="66067-285">对于前面两个示例中的任意一个，成功响应由 `HTTP 200 OK` 响应代码表示，响应正文包括扩展属性与相应筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="66067-285">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="66067-286">响应正文类似于[获取邮件集合](../api/user-list-messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="66067-286">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="66067-287">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="66067-287">The response does not include the matching extended property.</span></span>


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
    "Error: /api-reference/beta/api/singlevaluelegacyextendedproperty-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
