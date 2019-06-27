---
title: 获取 singleValueLegacyExtendedProperty
description: 可以使用特定的扩展属性或资源实例集合来获取扩展的单个资源实例
localization_priority: Normal
ms.openlocfilehash: c4e028ecd7e881d42ee165560beced4dd097c553
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279252"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="fdefa-103">获取 singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="fdefa-103">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="fdefa-104">可以获取使用特定扩展属性扩展的单个资源实例，或包含与筛选器匹配的扩展属性的资源实例集合。</span><span class="sxs-lookup"><span data-stu-id="fdefa-104">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="fdefa-105">使用查询参数 `$expand`，可以获取使用特定的扩展属性扩展的指定资源实例。</span><span class="sxs-lookup"><span data-stu-id="fdefa-105">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="fdefa-106">在 **id** 属性上使用 `$filter` 和 `eq` 运算符来指定扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-106">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="fdefa-107">这是当前获取 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="fdefa-107">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="fdefa-108">要获取具有某些扩展属性的资源实例，请使用 `$filter` 查询参数并在 **id** 属性上应用 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="fdefa-108">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="fdefa-109">另外，对于数字扩展属性，请在 **value** 属性上应用以下某个运算符：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="fdefa-109">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="fdefa-110">对于字符串类型的扩展属性，请在 **value** 上应用 `contains`、`startswith`、`eq` 或 `ne` 运算符。</span><span class="sxs-lookup"><span data-stu-id="fdefa-110">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="fdefa-111">该筛选器应用于资源在已登录用户的邮箱中的所有实例。</span><span class="sxs-lookup"><span data-stu-id="fdefa-111">The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span> 

<span data-ttu-id="fdefa-112">在扩展属性的 **id** 中筛选字符串名称 (`Name`) 是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="fdefa-112">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="fdefa-113">筛选扩展属性的 **value** 属性是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="fdefa-113">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="fdefa-114">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="fdefa-114">The following user resources are supported:</span></span>

- [<span data-ttu-id="fdefa-115">日历</span><span class="sxs-lookup"><span data-stu-id="fdefa-115">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="fdefa-116">联系人</span><span class="sxs-lookup"><span data-stu-id="fdefa-116">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="fdefa-117">contactFolder</span><span class="sxs-lookup"><span data-stu-id="fdefa-117">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="fdefa-118">事件</span><span class="sxs-lookup"><span data-stu-id="fdefa-118">event</span></span>](../resources/event.md)
- [<span data-ttu-id="fdefa-119">mailFolder</span><span class="sxs-lookup"><span data-stu-id="fdefa-119">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="fdefa-120">邮件</span><span class="sxs-lookup"><span data-stu-id="fdefa-120">message</span></span>](../resources/message.md) 

<span data-ttu-id="fdefa-121">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="fdefa-121">As well as the following group resources:</span></span>

- <span data-ttu-id="fdefa-122">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="fdefa-122">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="fdefa-123">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="fdefa-123">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="fdefa-124">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="fdefa-124">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="fdefa-125">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="fdefa-125">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdefa-126">权限</span><span class="sxs-lookup"><span data-stu-id="fdefa-126">Permissions</span></span>
<span data-ttu-id="fdefa-127">根据您要获取的扩展属性的资源以及所请求的权限类型 (委派或应用程序), 必须至少调用下表中指定的权限, 才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="fdefa-127">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="fdefa-128">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fdefa-128">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fdefa-129">支持的资源</span><span class="sxs-lookup"><span data-stu-id="fdefa-129">Supported resource</span></span> | <span data-ttu-id="fdefa-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fdefa-130">Delegated (work or school account)</span></span> | <span data-ttu-id="fdefa-131">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fdefa-131">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdefa-132">应用程序</span><span class="sxs-lookup"><span data-stu-id="fdefa-132">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="fdefa-133">calendar</span><span class="sxs-lookup"><span data-stu-id="fdefa-133">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="fdefa-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-134">Calendars.Read</span></span> | <span data-ttu-id="fdefa-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-135">Calendars.Read</span></span> | <span data-ttu-id="fdefa-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-136">Calendars.Read</span></span> |
| [<span data-ttu-id="fdefa-137">联系人</span><span class="sxs-lookup"><span data-stu-id="fdefa-137">contact</span></span>](../resources/contact.md) | <span data-ttu-id="fdefa-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-138">Contacts.Read</span></span> | <span data-ttu-id="fdefa-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-139">Contacts.Read</span></span> | <span data-ttu-id="fdefa-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-140">Contacts.Read</span></span> |
| [<span data-ttu-id="fdefa-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="fdefa-141">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="fdefa-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-142">Contacts.Read</span></span> | <span data-ttu-id="fdefa-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-143">Contacts.Read</span></span> | <span data-ttu-id="fdefa-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-144">Contacts.Read</span></span> |
| [<span data-ttu-id="fdefa-145">事件</span><span class="sxs-lookup"><span data-stu-id="fdefa-145">event</span></span>](../resources/event.md) | <span data-ttu-id="fdefa-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-146">Calendars.Read</span></span> | <span data-ttu-id="fdefa-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-147">Calendars.Read</span></span> |  <span data-ttu-id="fdefa-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-148">Calendars.Read</span></span>|
| <span data-ttu-id="fdefa-149">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="fdefa-149">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="fdefa-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdefa-150">Group.Read.All</span></span> | <span data-ttu-id="fdefa-151">不支持</span><span class="sxs-lookup"><span data-stu-id="fdefa-151">Not supported</span></span> | <span data-ttu-id="fdefa-152">不支持</span><span class="sxs-lookup"><span data-stu-id="fdefa-152">Not supported</span></span> |
| <span data-ttu-id="fdefa-153">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="fdefa-153">group [event](../resources/event.md)</span></span> | <span data-ttu-id="fdefa-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdefa-154">Group.Read.All</span></span> | <span data-ttu-id="fdefa-155">不支持</span><span class="sxs-lookup"><span data-stu-id="fdefa-155">Not supported</span></span> | <span data-ttu-id="fdefa-156">不支持</span><span class="sxs-lookup"><span data-stu-id="fdefa-156">Not supported</span></span> |
| <span data-ttu-id="fdefa-157">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="fdefa-157">group [post](../resources/post.md)</span></span> | <span data-ttu-id="fdefa-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdefa-158">Group.Read.All</span></span> | <span data-ttu-id="fdefa-159">不支持</span><span class="sxs-lookup"><span data-stu-id="fdefa-159">Not supported</span></span> | <span data-ttu-id="fdefa-160">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdefa-160">Group.Read.All</span></span> |
| [<span data-ttu-id="fdefa-161">mailFolder</span><span class="sxs-lookup"><span data-stu-id="fdefa-161">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="fdefa-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-162">Mail.Read</span></span> | <span data-ttu-id="fdefa-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-163">Mail.Read</span></span> | <span data-ttu-id="fdefa-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-164">Mail.Read</span></span> |
| [<span data-ttu-id="fdefa-165">邮件</span><span class="sxs-lookup"><span data-stu-id="fdefa-165">message</span></span>](../resources/message.md) | <span data-ttu-id="fdefa-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-166">Mail.Read</span></span> | <span data-ttu-id="fdefa-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-167">Mail.Read</span></span> | <span data-ttu-id="fdefa-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fdefa-168">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdefa-169">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fdefa-169">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="fdefa-170">获取通过与筛选器匹配的扩展属性扩展的资源实例</span><span class="sxs-lookup"><span data-stu-id="fdefa-170">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="fdefa-p105">获取通过与 **id** 属性中的筛选器匹配的扩展属性展开的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="fdefa-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="fdefa-173">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-173">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="fdefa-174">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-174">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="fdefa-175">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-175">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="fdefa-176">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-176">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="fdefa-177">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-177">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="fdefa-178">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-178">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="fdefa-179">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-179">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="fdefa-180">获取组 **post** 实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-180">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="fdefa-181">获取包括与筛选器匹配的数值扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="fdefa-181">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="fdefa-182">获取支持的资源实例，其中包含与筛选器匹配的数字扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-182">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="fdefa-183">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="fdefa-183">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="fdefa-184">请务必对筛选器字符串中的以下字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)：冒号、正斜杠和空格。</span><span class="sxs-lookup"><span data-stu-id="fdefa-184">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="fdefa-185">以下语法行显示对 id 使用 `eq` 运算符的筛选器，对属性值使用另一个 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="fdefa-185">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="fdefa-186">可以使用适用于数值的其他运算符中的任何一个（`ne`、`ge`、`gt`、`le` 或 `lt`）替换 **value** 上的 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="fdefa-186">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="fdefa-187">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-187">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="fdefa-188">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-188">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="fdefa-189">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-189">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="fdefa-190">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-190">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="fdefa-191">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-191">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="fdefa-192">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-192">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="fdefa-193">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-193">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="fdefa-194">获取组 **post** 实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-194">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="fdefa-195">获取资源实例，其中包括与筛选器匹配的字符串类型的扩展属性</span><span class="sxs-lookup"><span data-stu-id="fdefa-195">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="fdefa-196">获取 **message** 或 **event** 资源的实例，其中包括与筛选器匹配的字符串类型的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-196">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="fdefa-197">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`contains`、`startswith`、`eq` 或 `ne`。</span><span class="sxs-lookup"><span data-stu-id="fdefa-197">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="fdefa-198">请务必对筛选器字符串中的以下字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)：冒号、正斜杠和空格。</span><span class="sxs-lookup"><span data-stu-id="fdefa-198">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="fdefa-199">获取 **message** 实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-199">Get **message** instances:</span></span>
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

<span data-ttu-id="fdefa-200">获取 **event** 实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-200">Get **event** instances:</span></span>
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

<span data-ttu-id="fdefa-201">获取组 **event** 实例：</span><span class="sxs-lookup"><span data-stu-id="fdefa-201">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="fdefa-202">路径参数</span><span class="sxs-lookup"><span data-stu-id="fdefa-202">Path parameters</span></span>
|<span data-ttu-id="fdefa-203">参数</span><span class="sxs-lookup"><span data-stu-id="fdefa-203">Parameter</span></span>|<span data-ttu-id="fdefa-204">类型</span><span class="sxs-lookup"><span data-stu-id="fdefa-204">Type</span></span>|<span data-ttu-id="fdefa-205">说明</span><span class="sxs-lookup"><span data-stu-id="fdefa-205">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fdefa-206">id_value</span><span class="sxs-lookup"><span data-stu-id="fdefa-206">id_value</span></span>|<span data-ttu-id="fdefa-207">String</span><span class="sxs-lookup"><span data-stu-id="fdefa-207">String</span></span>|<span data-ttu-id="fdefa-p109">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="fdefa-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="fdefa-212">property_value</span><span class="sxs-lookup"><span data-stu-id="fdefa-212">property_value</span></span> |<span data-ttu-id="fdefa-213">String</span><span class="sxs-lookup"><span data-stu-id="fdefa-213">String</span></span>|<span data-ttu-id="fdefa-214">要匹配的扩展属性的值。</span><span class="sxs-lookup"><span data-stu-id="fdefa-214">The value of the extended property to match.</span></span> <span data-ttu-id="fdefa-215">如果在上面的 **HTTP 请求**部分中列出，则为必需参数。</span><span class="sxs-lookup"><span data-stu-id="fdefa-215">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="fdefa-216">如果 {property_value} 不是字符串，请务必在与 {property_value} 比较时，将 `ep/value` 显式转换为相应的 Edm 数据类型。</span><span class="sxs-lookup"><span data-stu-id="fdefa-216">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="fdefa-217">有关示例，请参阅下面的[请求 4](#request-4)。</span><span class="sxs-lookup"><span data-stu-id="fdefa-217">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fdefa-218">请求标头</span><span class="sxs-lookup"><span data-stu-id="fdefa-218">Request headers</span></span>
| <span data-ttu-id="fdefa-219">名称</span><span class="sxs-lookup"><span data-stu-id="fdefa-219">Name</span></span>      |<span data-ttu-id="fdefa-220">说明</span><span class="sxs-lookup"><span data-stu-id="fdefa-220">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fdefa-221">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdefa-221">Authorization</span></span>  | <span data-ttu-id="fdefa-p111">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fdefa-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdefa-224">请求正文</span><span class="sxs-lookup"><span data-stu-id="fdefa-224">Request body</span></span>
<span data-ttu-id="fdefa-225">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fdefa-225">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdefa-226">响应</span><span class="sxs-lookup"><span data-stu-id="fdefa-226">Response</span></span>

<span data-ttu-id="fdefa-227">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fdefa-227">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-expanded-with-a-matching-extended-property"></a><span data-ttu-id="fdefa-228">获取通过匹配的扩展属性扩展的资源实例</span><span class="sxs-lookup"><span data-stu-id="fdefa-228">GET resource instance expanded with a matching extended property</span></span>
<span data-ttu-id="fdefa-229">响应正文包括通过匹配的 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="fdefa-229">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="fdefa-230">获取包含与筛选器匹配的扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="fdefa-230">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="fdefa-231">响应主体包含一个或多个对象，它们表示包含匹配的扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="fdefa-231">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="fdefa-232">响应正文不包含扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-232">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="fdefa-233">示例</span><span class="sxs-lookup"><span data-stu-id="fdefa-233">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="fdefa-234">请求 1</span><span class="sxs-lookup"><span data-stu-id="fdefa-234">Request 1</span></span>

<span data-ttu-id="fdefa-p113">第一个示例通过包含一个单值扩展属性获取并展开指定的邮件。此筛选器返回其 **id** 与 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 字符串（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2_bs88AACHsLqWAAA="],
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="fdefa-237">响应 1</span><span class="sxs-lookup"><span data-stu-id="fdefa-237">Response 1</span></span>
<span data-ttu-id="fdefa-238">响应正文包括指定邮件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-238">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="fdefa-p114">注意：为了简单起见，会将此处所示的**邮件**对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fdefa-241">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="fdefa-241">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fdefa-242">C#</span><span class="sxs-lookup"><span data-stu-id="fdefa-242">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_singlevaluelegacyextendedproperty_1-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fdefa-243">Javascript</span><span class="sxs-lookup"><span data-stu-id="fdefa-243">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_singlevaluelegacyextendedproperty_1-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fdefa-244">目标-C</span><span class="sxs-lookup"><span data-stu-id="fdefa-244">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_singlevaluelegacyextendedproperty_1-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request-2"></a><span data-ttu-id="fdefa-245">请求 2</span><span class="sxs-lookup"><span data-stu-id="fdefa-245">Request 2</span></span>

<span data-ttu-id="fdefa-246">第二个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="fdefa-246">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="fdefa-247">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="fdefa-247">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="fdefa-248">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="fdefa-248">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="fdefa-249">它的 **value** 等于字符串 `Green`。</span><span class="sxs-lookup"><span data-stu-id="fdefa-249">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="fdefa-250">响应 2</span><span class="sxs-lookup"><span data-stu-id="fdefa-250">Response 2</span></span>

<span data-ttu-id="fdefa-p116">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。响应正文是类似于[获取邮件集合](../api/user-list-messages.md)中的响应。该响应不包括匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="fdefa-254">请求 3</span><span class="sxs-lookup"><span data-stu-id="fdefa-254">Request 3</span></span>

<span data-ttu-id="fdefa-255">第三个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="fdefa-255">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="fdefa-256">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="fdefa-256">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="fdefa-257">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="fdefa-257">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="fdefa-258">它的 **value** 包含字符串 `green`。</span><span class="sxs-lookup"><span data-stu-id="fdefa-258">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="fdefa-259">响应 3</span><span class="sxs-lookup"><span data-stu-id="fdefa-259">Response 3</span></span>

<span data-ttu-id="fdefa-260">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-260">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="fdefa-261">例如，如果邮件包含 **id** 等于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 的单值扩展属性和 **value** `Light green`，则会与筛选器匹配并包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="fdefa-261">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="fdefa-262">响应正文类似于[获取邮件集合](../api/user-list-messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="fdefa-262">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="fdefa-263">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-263">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="fdefa-264">请求 4</span><span class="sxs-lookup"><span data-stu-id="fdefa-264">Request 4</span></span>

<span data-ttu-id="fdefa-265">接下来的两个示例展示了如何获取具有非字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="fdefa-265">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="fdefa-266">为了方便阅读，从中删除了必要的 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="fdefa-266">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="fdefa-267">下面的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="fdefa-267">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="fdefa-268">它的 **id** 与字符串 `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid` 匹配。</span><span class="sxs-lookup"><span data-stu-id="fdefa-268">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="fdefa-269">它的 **value** 是 GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`。</span><span class="sxs-lookup"><span data-stu-id="fdefa-269">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="fdefa-270">若要将属性值与 GUID 比较，请将 `ep/value` 转换为 `Edm.Guid`。</span><span class="sxs-lookup"><span data-stu-id="fdefa-270">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="fdefa-271">接下来的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="fdefa-271">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="fdefa-272">它的 **id** 与字符串 `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete` 匹配。</span><span class="sxs-lookup"><span data-stu-id="fdefa-272">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="fdefa-273">它的 **value** 等于整数 12。</span><span class="sxs-lookup"><span data-stu-id="fdefa-273">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="fdefa-274">若要将属性值与整数比较，请将 `ep/value` 转换为 `Edm.Int32`。</span><span class="sxs-lookup"><span data-stu-id="fdefa-274">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="fdefa-275">响应 4</span><span class="sxs-lookup"><span data-stu-id="fdefa-275">Response 4</span></span>

<span data-ttu-id="fdefa-276">对于前面两个示例中的任意一个，成功响应由 `HTTP 200 OK` 响应代码表示，响应正文包括扩展属性与相应筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-276">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="fdefa-277">响应正文类似于[获取邮件集合](../api/user-list-messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="fdefa-277">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="fdefa-278">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fdefa-278">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/singlevaluelegacyextendedproperty-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/singlevaluelegacyextendedproperty-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/singlevaluelegacyextendedproperty-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
