---
title: 获取 singleValueLegacyExtendedProperty
description: 可以使用特定的扩展属性或资源实例集合来获取扩展的单个资源实例
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d83bb1a072d2f42e0769495793acda1d124a1a19
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038219"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="366ee-103">获取 singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="366ee-103">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="366ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="366ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="366ee-105">可以获取使用特定扩展属性扩展的单个资源实例，或包含与筛选器匹配的扩展属性的资源实例集合。</span><span class="sxs-lookup"><span data-stu-id="366ee-105">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="366ee-106">使用查询参数 `$expand`，可以获取使用特定的扩展属性扩展的指定资源实例。</span><span class="sxs-lookup"><span data-stu-id="366ee-106">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="366ee-107">在 **id** 属性上使用 `$filter` 和 `eq` 运算符来指定扩展属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-107">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="366ee-108">这是当前获取 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="366ee-108">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="366ee-109">要获取具有某些扩展属性的资源实例，请使用 `$filter` 查询参数并在 **id** 属性上应用 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="366ee-109">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="366ee-110">另外，对于数字扩展属性，请在 **value** 属性上应用以下某个运算符：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="366ee-110">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="366ee-111">对于字符串类型的扩展属性，请在 **value** 上应用 `contains`、`startswith`、`eq` 或 `ne` 运算符。</span><span class="sxs-lookup"><span data-stu-id="366ee-111">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="366ee-112">该筛选器应用于资源在已登录用户的邮箱中的所有实例。</span><span class="sxs-lookup"><span data-stu-id="366ee-112">The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span>

<span data-ttu-id="366ee-113">在扩展属性的 **id** 中筛选字符串名称 (`Name`) 是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="366ee-113">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="366ee-114">筛选扩展属性的 **value** 属性是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="366ee-114">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="366ee-115">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="366ee-115">The following user resources are supported:</span></span>

- [<span data-ttu-id="366ee-116">日历</span><span class="sxs-lookup"><span data-stu-id="366ee-116">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="366ee-117">联系人</span><span class="sxs-lookup"><span data-stu-id="366ee-117">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="366ee-118">contactFolder</span><span class="sxs-lookup"><span data-stu-id="366ee-118">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="366ee-119">事件</span><span class="sxs-lookup"><span data-stu-id="366ee-119">event</span></span>](../resources/event.md)
- [<span data-ttu-id="366ee-120">mailFolder</span><span class="sxs-lookup"><span data-stu-id="366ee-120">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="366ee-121">邮件</span><span class="sxs-lookup"><span data-stu-id="366ee-121">message</span></span>](../resources/message.md)

<span data-ttu-id="366ee-122">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="366ee-122">As well as the following group resources:</span></span>

- <span data-ttu-id="366ee-123">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="366ee-123">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="366ee-124">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="366ee-124">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="366ee-125">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="366ee-125">group [post](../resources/post.md)</span></span>

<span data-ttu-id="366ee-126">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="366ee-126">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="366ee-127">权限</span><span class="sxs-lookup"><span data-stu-id="366ee-127">Permissions</span></span>
<span data-ttu-id="366ee-128">根据要获取扩展属性的资源以及您请求的权限类型 (委派或应用程序) ，在下表中指定的权限是调用此 API 所需的最低权限。</span><span class="sxs-lookup"><span data-stu-id="366ee-128">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="366ee-129">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="366ee-129">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="366ee-130">支持的资源</span><span class="sxs-lookup"><span data-stu-id="366ee-130">Supported resource</span></span> | <span data-ttu-id="366ee-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="366ee-131">Delegated (work or school account)</span></span> | <span data-ttu-id="366ee-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="366ee-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="366ee-133">应用程序</span><span class="sxs-lookup"><span data-stu-id="366ee-133">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="366ee-134">calendar</span><span class="sxs-lookup"><span data-stu-id="366ee-134">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="366ee-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-135">Calendars.Read</span></span> | <span data-ttu-id="366ee-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-136">Calendars.Read</span></span> | <span data-ttu-id="366ee-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-137">Calendars.Read</span></span> |
| [<span data-ttu-id="366ee-138">联系人</span><span class="sxs-lookup"><span data-stu-id="366ee-138">contact</span></span>](../resources/contact.md) | <span data-ttu-id="366ee-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-139">Contacts.Read</span></span> | <span data-ttu-id="366ee-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-140">Contacts.Read</span></span> | <span data-ttu-id="366ee-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-141">Contacts.Read</span></span> |
| [<span data-ttu-id="366ee-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="366ee-142">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="366ee-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-143">Contacts.Read</span></span> | <span data-ttu-id="366ee-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-144">Contacts.Read</span></span> | <span data-ttu-id="366ee-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-145">Contacts.Read</span></span> |
| [<span data-ttu-id="366ee-146">事件</span><span class="sxs-lookup"><span data-stu-id="366ee-146">event</span></span>](../resources/event.md) | <span data-ttu-id="366ee-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-147">Calendars.Read</span></span> | <span data-ttu-id="366ee-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-148">Calendars.Read</span></span> |  <span data-ttu-id="366ee-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-149">Calendars.Read</span></span>|
| <span data-ttu-id="366ee-150">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="366ee-150">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="366ee-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="366ee-151">Group.Read.All</span></span> | <span data-ttu-id="366ee-152">不支持</span><span class="sxs-lookup"><span data-stu-id="366ee-152">Not supported</span></span> | <span data-ttu-id="366ee-153">不支持</span><span class="sxs-lookup"><span data-stu-id="366ee-153">Not supported</span></span> |
| <span data-ttu-id="366ee-154">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="366ee-154">group [event](../resources/event.md)</span></span> | <span data-ttu-id="366ee-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="366ee-155">Group.Read.All</span></span> | <span data-ttu-id="366ee-156">不支持</span><span class="sxs-lookup"><span data-stu-id="366ee-156">Not supported</span></span> | <span data-ttu-id="366ee-157">不支持</span><span class="sxs-lookup"><span data-stu-id="366ee-157">Not supported</span></span> |
| <span data-ttu-id="366ee-158">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="366ee-158">group [post](../resources/post.md)</span></span> | <span data-ttu-id="366ee-159">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="366ee-159">Group.Read.All</span></span> | <span data-ttu-id="366ee-160">不支持</span><span class="sxs-lookup"><span data-stu-id="366ee-160">Not supported</span></span> | <span data-ttu-id="366ee-161">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="366ee-161">Group.Read.All</span></span> |
| [<span data-ttu-id="366ee-162">mailFolder</span><span class="sxs-lookup"><span data-stu-id="366ee-162">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="366ee-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-163">Mail.Read</span></span> | <span data-ttu-id="366ee-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-164">Mail.Read</span></span> | <span data-ttu-id="366ee-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-165">Mail.Read</span></span> |
| [<span data-ttu-id="366ee-166">邮件</span><span class="sxs-lookup"><span data-stu-id="366ee-166">message</span></span>](../resources/message.md) | <span data-ttu-id="366ee-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-167">Mail.Read</span></span> | <span data-ttu-id="366ee-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-168">Mail.Read</span></span> | <span data-ttu-id="366ee-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="366ee-169">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="366ee-170">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="366ee-170">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="366ee-171">获取通过与筛选器匹配的扩展属性扩展的资源实例</span><span class="sxs-lookup"><span data-stu-id="366ee-171">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="366ee-p105">获取通过与 **id** 属性中的筛选器匹配的扩展属性展开的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="366ee-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="366ee-174">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-174">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="366ee-175">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-175">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="366ee-176">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-176">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="366ee-177">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-177">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="366ee-178">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-178">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="366ee-179">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-179">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="366ee-180">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-180">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="366ee-181">获取组 **post** 实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-181">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="366ee-182">获取包括与筛选器匹配的数值扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="366ee-182">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="366ee-183">获取支持的资源实例，其中包含与筛选器匹配的数字扩展属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-183">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="366ee-184">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="366ee-184">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span>
<span data-ttu-id="366ee-185">请务必对筛选器字符串中的以下字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)：冒号、正斜杠和空格。</span><span class="sxs-lookup"><span data-stu-id="366ee-185">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="366ee-186">以下语法行显示对 id 使用 `eq` 运算符的筛选器，对属性值使用另一个 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="366ee-186">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="366ee-187">可以使用适用于数值的其他运算符中的任何一个（`ne`、`ge`、`gt`、`le` 或 `lt`）替换 **value** 上的 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="366ee-187">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="366ee-188">获取 **message** 实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-188">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="366ee-189">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-189">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="366ee-190">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-190">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="366ee-191">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-191">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="366ee-192">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-192">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="366ee-193">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-193">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="366ee-194">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-194">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="366ee-195">获取组 **post** 实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-195">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="366ee-196">获取资源实例，其中包括与筛选器匹配的字符串类型的扩展属性</span><span class="sxs-lookup"><span data-stu-id="366ee-196">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="366ee-197">获取 **message** 或 **event** 资源的实例，其中包括与筛选器匹配的字符串类型的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-197">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="366ee-198">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`contains`、`startswith`、`eq` 或 `ne`。</span><span class="sxs-lookup"><span data-stu-id="366ee-198">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="366ee-199">请务必对筛选器字符串中的以下字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)：冒号、正斜杠和空格。</span><span class="sxs-lookup"><span data-stu-id="366ee-199">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="366ee-200">获取 **message** 实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-200">Get **message** instances:</span></span>
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

<span data-ttu-id="366ee-201">获取 **event** 实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-201">Get **event** instances:</span></span>
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

<span data-ttu-id="366ee-202">获取组 **event** 实例：</span><span class="sxs-lookup"><span data-stu-id="366ee-202">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="366ee-203">路径参数</span><span class="sxs-lookup"><span data-stu-id="366ee-203">Path parameters</span></span>
|<span data-ttu-id="366ee-204">参数</span><span class="sxs-lookup"><span data-stu-id="366ee-204">Parameter</span></span>|<span data-ttu-id="366ee-205">类型</span><span class="sxs-lookup"><span data-stu-id="366ee-205">Type</span></span>|<span data-ttu-id="366ee-206">说明</span><span class="sxs-lookup"><span data-stu-id="366ee-206">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="366ee-207">id_value</span><span class="sxs-lookup"><span data-stu-id="366ee-207">id_value</span></span>|<span data-ttu-id="366ee-208">String</span><span class="sxs-lookup"><span data-stu-id="366ee-208">String</span></span>|<span data-ttu-id="366ee-p109">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="366ee-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="366ee-213">property_value</span><span class="sxs-lookup"><span data-stu-id="366ee-213">property_value</span></span> |<span data-ttu-id="366ee-214">String</span><span class="sxs-lookup"><span data-stu-id="366ee-214">String</span></span>|<span data-ttu-id="366ee-215">要匹配的扩展属性的值。</span><span class="sxs-lookup"><span data-stu-id="366ee-215">The value of the extended property to match.</span></span> <span data-ttu-id="366ee-216">如果在上面的 **HTTP 请求**部分中列出，则为必需参数。</span><span class="sxs-lookup"><span data-stu-id="366ee-216">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="366ee-217">如果 {property_value} 不是字符串，请务必在与 {property_value} 比较时，将 `ep/value` 显式转换为相应的 Edm 数据类型。</span><span class="sxs-lookup"><span data-stu-id="366ee-217">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="366ee-218">有关示例，请参阅下面的[请求 4](#request-4)。</span><span class="sxs-lookup"><span data-stu-id="366ee-218">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="366ee-219">请求标头</span><span class="sxs-lookup"><span data-stu-id="366ee-219">Request headers</span></span>
| <span data-ttu-id="366ee-220">名称</span><span class="sxs-lookup"><span data-stu-id="366ee-220">Name</span></span>      |<span data-ttu-id="366ee-221">说明</span><span class="sxs-lookup"><span data-stu-id="366ee-221">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="366ee-222">Authorization</span><span class="sxs-lookup"><span data-stu-id="366ee-222">Authorization</span></span>  | <span data-ttu-id="366ee-p111">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="366ee-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="366ee-225">请求正文</span><span class="sxs-lookup"><span data-stu-id="366ee-225">Request body</span></span>
<span data-ttu-id="366ee-226">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="366ee-226">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="366ee-227">响应</span><span class="sxs-lookup"><span data-stu-id="366ee-227">Response</span></span>

<span data-ttu-id="366ee-228">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="366ee-228">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-expanded-with-a-matching-extended-property"></a><span data-ttu-id="366ee-229">获取通过匹配的扩展属性扩展的资源实例</span><span class="sxs-lookup"><span data-stu-id="366ee-229">GET resource instance expanded with a matching extended property</span></span>
<span data-ttu-id="366ee-230">响应正文包括通过匹配的 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="366ee-230">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>

#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="366ee-231">获取包含与筛选器匹配的扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="366ee-231">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="366ee-232">响应主体包含一个或多个对象，它们表示包含匹配的扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="366ee-232">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="366ee-233">响应正文不包含扩展属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-233">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="366ee-234">示例</span><span class="sxs-lookup"><span data-stu-id="366ee-234">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="366ee-235">请求 1</span><span class="sxs-lookup"><span data-stu-id="366ee-235">Request 1</span></span>

<span data-ttu-id="366ee-p113">第一个示例通过包含一个单值扩展属性获取并展开指定的邮件。此筛选器返回其 **id** 与 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 字符串（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>


# <a name="http"></a>[<span data-ttu-id="366ee-238">HTTP</span><span class="sxs-lookup"><span data-stu-id="366ee-238">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2_bs88AACHsLqWAAA="],
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
# <a name="c"></a>[<span data-ttu-id="366ee-239">C#</span><span class="sxs-lookup"><span data-stu-id="366ee-239">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-singlevaluelegacyextendedproperty-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="366ee-240">JavaScript</span><span class="sxs-lookup"><span data-stu-id="366ee-240">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-singlevaluelegacyextendedproperty-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="366ee-241">Objective-C</span><span class="sxs-lookup"><span data-stu-id="366ee-241">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-singlevaluelegacyextendedproperty-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="366ee-242">Java</span><span class="sxs-lookup"><span data-stu-id="366ee-242">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-singlevaluelegacyextendedproperty-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response-1"></a><span data-ttu-id="366ee-243">响应 1</span><span class="sxs-lookup"><span data-stu-id="366ee-243">Response 1</span></span>
<span data-ttu-id="366ee-244">响应正文包括指定邮件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-244">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="366ee-p114">注意：为了简单起见，会将此处所示的**邮件**对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
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
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

#### <a name="request-2"></a><span data-ttu-id="366ee-247">请求 2</span><span class="sxs-lookup"><span data-stu-id="366ee-247">Request 2</span></span>

<span data-ttu-id="366ee-248">第二个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="366ee-248">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="366ee-249">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="366ee-249">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="366ee-250">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="366ee-250">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="366ee-251">它的 **value** 等于字符串 `Green`。</span><span class="sxs-lookup"><span data-stu-id="366ee-251">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="366ee-252">响应 2</span><span class="sxs-lookup"><span data-stu-id="366ee-252">Response 2</span></span>

<span data-ttu-id="366ee-p116">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。响应正文是类似于[获取邮件集合](../api/user-list-messages.md)中的响应。该响应不包括匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="366ee-256">请求 3</span><span class="sxs-lookup"><span data-stu-id="366ee-256">Request 3</span></span>

<span data-ttu-id="366ee-257">第三个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="366ee-257">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="366ee-258">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="366ee-258">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="366ee-259">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="366ee-259">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="366ee-260">它的 **value** 包含字符串 `green`。</span><span class="sxs-lookup"><span data-stu-id="366ee-260">Its **value** containing the string `green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="366ee-261">响应 3</span><span class="sxs-lookup"><span data-stu-id="366ee-261">Response 3</span></span>

<span data-ttu-id="366ee-262">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-262">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="366ee-263">例如，如果邮件包含 **id** 等于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 的单值扩展属性和 **value** `Light green`，则会与筛选器匹配并包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="366ee-263">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="366ee-264">响应正文类似于[获取邮件集合](../api/user-list-messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="366ee-264">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="366ee-265">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-265">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="366ee-266">请求 4</span><span class="sxs-lookup"><span data-stu-id="366ee-266">Request 4</span></span>

<span data-ttu-id="366ee-267">接下来的两个示例展示了如何获取具有非字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="366ee-267">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="366ee-268">为了方便阅读，从中删除了必要的 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="366ee-268">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="366ee-269">下面的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="366ee-269">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="366ee-270">它的 **id** 与字符串 `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid` 匹配。</span><span class="sxs-lookup"><span data-stu-id="366ee-270">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="366ee-271">它的 **value** 是 GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`。</span><span class="sxs-lookup"><span data-stu-id="366ee-271">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="366ee-272">若要将属性值与 GUID 比较，请将 `ep/value` 转换为 `Edm.Guid`。</span><span class="sxs-lookup"><span data-stu-id="366ee-272">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="366ee-273">接下来的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="366ee-273">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="366ee-274">它的 **id** 与字符串 `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete` 匹配。</span><span class="sxs-lookup"><span data-stu-id="366ee-274">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="366ee-275">它的 **value** 等于整数 12。</span><span class="sxs-lookup"><span data-stu-id="366ee-275">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="366ee-276">若要将属性值与整数比较，请将 `ep/value` 转换为 `Edm.Int32`。</span><span class="sxs-lookup"><span data-stu-id="366ee-276">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="366ee-277">响应 4</span><span class="sxs-lookup"><span data-stu-id="366ee-277">Response 4</span></span>

<span data-ttu-id="366ee-278">对于前面两个示例中的任意一个，成功响应由 `HTTP 200 OK` 响应代码表示，响应正文包括扩展属性与相应筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-278">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="366ee-279">响应正文类似于[获取邮件集合](../api/user-list-messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="366ee-279">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="366ee-280">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-280">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

