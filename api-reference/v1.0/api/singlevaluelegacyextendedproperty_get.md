# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="62c3d-101">获取 singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="62c3d-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="62c3d-102">可以获取使用特定扩展属性扩展的单个资源实例，或包含与筛选器匹配的扩展属性的资源实例集合。</span><span class="sxs-lookup"><span data-stu-id="62c3d-102">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="62c3d-103">使用查询参数 `$expand`，可以获取使用特定的扩展属性扩展的指定资源实例。</span><span class="sxs-lookup"><span data-stu-id="62c3d-103">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="62c3d-104">在 **id** 属性上使用 `$filter` 和 `eq` 运算符来指定扩展属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-104">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="62c3d-105">这是当前获取 [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="62c3d-105">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="62c3d-106">要获取具有某些扩展属性的资源实例，请使用 `$filter` 查询参数并在 **id** 属性上应用 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="62c3d-106">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="62c3d-107">另外，对于数字扩展属性，请在 **value** 属性上应用以下某个运算符：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="62c3d-107">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="62c3d-108">对于字符串类型的扩展属性，请在 **value** 上应用 `contains`、`startswith`、`eq` 或 `ne` 运算符。</span><span class="sxs-lookup"><span data-stu-id="62c3d-108">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="62c3d-109">该筛选器应用于资源在已登录用户的邮箱中的所有实例。</span><span class="sxs-lookup"><span data-stu-id="62c3d-109">The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span> 

<span data-ttu-id="62c3d-110">在扩展属性的 **id** 中筛选字符串名称 (`Name`) 是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="62c3d-110">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="62c3d-111">筛选扩展属性的 **value** 属性是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="62c3d-111">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="62c3d-112">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="62c3d-112">The following user resources are supported:</span></span>

- [<span data-ttu-id="62c3d-113">邮件</span><span class="sxs-lookup"><span data-stu-id="62c3d-113">message</span></span>](../resources/message.md)
- [<span data-ttu-id="62c3d-114">mailFolder</span><span class="sxs-lookup"><span data-stu-id="62c3d-114">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="62c3d-115">事件</span><span class="sxs-lookup"><span data-stu-id="62c3d-115">event</span></span>](../resources/event.md)
- [<span data-ttu-id="62c3d-116">日历</span><span class="sxs-lookup"><span data-stu-id="62c3d-116">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="62c3d-117">联系人</span><span class="sxs-lookup"><span data-stu-id="62c3d-117">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="62c3d-118">contactFolder</span><span class="sxs-lookup"><span data-stu-id="62c3d-118">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="62c3d-119">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="62c3d-119">As well as the following group resources:</span></span>

- <span data-ttu-id="62c3d-120">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="62c3d-120">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="62c3d-121">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="62c3d-121">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="62c3d-122">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="62c3d-122">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="62c3d-123">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="62c3d-123">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="62c3d-124">权限</span><span class="sxs-lookup"><span data-stu-id="62c3d-124">Permissions</span></span>
<span data-ttu-id="62c3d-p104">若要调用此 API，必须有以下权限之一，具体视要获取的资源而定。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="62c3d-p104">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="62c3d-127">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="62c3d-127">Mail.Read</span></span>
- <span data-ttu-id="62c3d-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="62c3d-128">Calendars.Read</span></span>
- <span data-ttu-id="62c3d-129">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="62c3d-129">Contacts.Read</span></span>
- <span data-ttu-id="62c3d-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="62c3d-130">Group.Read.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="62c3d-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62c3d-131">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="62c3d-132">获取通过与筛选器匹配的扩展属性扩展的资源实例</span><span class="sxs-lookup"><span data-stu-id="62c3d-132">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="62c3d-p105">获取通过与 **id** 属性中的筛选器匹配的扩展属性展开的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](http://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="62c3d-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="62c3d-135">获取**邮件**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-135">Get a **message** instance:</span></span>
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="62c3d-136">获取 **mailFolder** 实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-136">Get a **mailFolder** instance:</span></span>
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="62c3d-137">获取**事件**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-137">Get an **event** instance:</span></span>
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="62c3d-138">获取**日历**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-138">Get a **calendar** instance:</span></span>
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="62c3d-139">获取**联系人**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-139">Get a **contact** instance:</span></span>
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="62c3d-140">获取 **contactFolder** 实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-140">Get a **contactFolder** instance:</span></span>
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="62c3d-141">获取组**事件**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-141">Get a group **event** instance:</span></span>
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="62c3d-142">获取组**帖子**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-142">Get a group **post** instance:</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="62c3d-143">获取包括与筛选器匹配的数值扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="62c3d-143">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="62c3d-144">获取支持的资源实例，其中包含与筛选器匹配的数字扩展属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-144">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="62c3d-145">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`eq`、`ne`、`ge`、`gt`、`le` 或 `lt`。</span><span class="sxs-lookup"><span data-stu-id="62c3d-145">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="62c3d-146">请务必对筛选器字符串中的以下字符应用 [URL 编码](http://www.w3schools.com/tags/ref_urlencode.asp)：冒号、正斜杠和空格。</span><span class="sxs-lookup"><span data-stu-id="62c3d-146">Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="62c3d-147">以下语法行显示对 id 使用 `eq` 运算符的筛选器，对属性值使用另一个 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="62c3d-147">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="62c3d-148">可以使用适用于数值的其他运算符中的任何一个（`ne`、`ge`、`gt`、`le` 或 `lt`）替换 **value** 上的 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="62c3d-148">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="62c3d-149">获取**邮件**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-149">Get **message** instances:</span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="62c3d-150">获取 **mailFolder** 实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-150">Get **mailFolder** instances:</span></span>
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="62c3d-151">获取**事件**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-151">Get **event** instances:</span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="62c3d-152">获取**日历**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-152">Get **calendar** instances:</span></span>
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="62c3d-153">获取**联系人**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-153">Get **contact** instances:</span></span>
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="62c3d-154">获取 **contactFolder** 实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-154">Get **contactFolder** instances:</span></span>
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="62c3d-155">获取组**事件**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-155">Get group **event** instances:</span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="62c3d-156">获取组**贴子**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-156">Get group **post** instances:</span></span>
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="62c3d-157">获取资源实例，其中包括与筛选器匹配的字符串类型的扩展属性</span><span class="sxs-lookup"><span data-stu-id="62c3d-157">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="62c3d-158">获取 **message** 或 **event** 资源的实例，其中包括与筛选器匹配的字符串类型的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-158">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="62c3d-159">筛选器在 **id** 属性上使用 `eq` 运算符，并在 **value** 属性上使用以下运算符之一：`contains`、`startswith`、`eq` 或 `ne`。</span><span class="sxs-lookup"><span data-stu-id="62c3d-159">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="62c3d-160">请务必对筛选器字符串中的以下字符应用 [URL 编码](http://www.w3schools.com/tags/ref_urlencode.asp)：冒号、正斜杠和空格。</span><span class="sxs-lookup"><span data-stu-id="62c3d-160">Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="62c3d-161">获取**邮件**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-161">Get **message** instances:</span></span>
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

<span data-ttu-id="62c3d-162">获取**事件**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-162">Get **event** instances:</span></span>
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

<span data-ttu-id="62c3d-163">获取组**事件**实例： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="62c3d-163">Get group **event** instances:</span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="62c3d-164">Path 参数</span><span class="sxs-lookup"><span data-stu-id="62c3d-164">Path parameters</span></span>
|<span data-ttu-id="62c3d-165">参数</span><span class="sxs-lookup"><span data-stu-id="62c3d-165">Parameter</span></span>|<span data-ttu-id="62c3d-166">类型</span><span class="sxs-lookup"><span data-stu-id="62c3d-166">Type</span></span>|<span data-ttu-id="62c3d-167">说明</span><span class="sxs-lookup"><span data-stu-id="62c3d-167">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="62c3d-168">id_value</span><span class="sxs-lookup"><span data-stu-id="62c3d-168">id_value</span></span>|<span data-ttu-id="62c3d-169">字符串</span><span class="sxs-lookup"><span data-stu-id="62c3d-169">String</span></span>|<span data-ttu-id="62c3d-p109">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="62c3d-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="62c3d-174">property_value</span><span class="sxs-lookup"><span data-stu-id="62c3d-174">property_value</span></span> |<span data-ttu-id="62c3d-175">字符串</span><span class="sxs-lookup"><span data-stu-id="62c3d-175">String</span></span>|<span data-ttu-id="62c3d-176">要匹配的扩展属性的值。</span><span class="sxs-lookup"><span data-stu-id="62c3d-176">The value of the extended property to match.</span></span> <span data-ttu-id="62c3d-177">如果在上面的 **HTTP 请求**部分中列出，则为必需参数。</span><span class="sxs-lookup"><span data-stu-id="62c3d-177">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="62c3d-178">如果 {property_value} 不是字符串，请务必在与 {property_value} 比较时，将 `ep/value` 显式转换为相应的 Edm 数据类型。</span><span class="sxs-lookup"><span data-stu-id="62c3d-178">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="62c3d-179">有关示例，请参阅下面的[请求 4](#request-4)。</span><span class="sxs-lookup"><span data-stu-id="62c3d-179">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="62c3d-180">请求标头</span><span class="sxs-lookup"><span data-stu-id="62c3d-180">Request headers</span></span>
| <span data-ttu-id="62c3d-181">名称</span><span class="sxs-lookup"><span data-stu-id="62c3d-181">Name</span></span>      |<span data-ttu-id="62c3d-182">说明</span><span class="sxs-lookup"><span data-stu-id="62c3d-182">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="62c3d-183">授权</span><span class="sxs-lookup"><span data-stu-id="62c3d-183">Authorization</span></span>  | <span data-ttu-id="62c3d-p111">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62c3d-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62c3d-186">请求正文</span><span class="sxs-lookup"><span data-stu-id="62c3d-186">Request body</span></span>
<span data-ttu-id="62c3d-187">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="62c3d-187">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62c3d-188">响应</span><span class="sxs-lookup"><span data-stu-id="62c3d-188">Response</span></span>

<span data-ttu-id="62c3d-189">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="62c3d-189">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-expanded-with-a-matching-extended-property"></a><span data-ttu-id="62c3d-190">获取通过匹配的扩展属性扩展的资源实例</span><span class="sxs-lookup"><span data-stu-id="62c3d-190">GET resource instance expanded with a matching extended property</span></span>
<span data-ttu-id="62c3d-191">响应正文包括通过匹配的 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="62c3d-191">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="62c3d-192">获取包含与筛选器匹配的扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="62c3d-192">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="62c3d-193">响应主体包含一个或多个对象，它们表示包含匹配的扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="62c3d-193">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="62c3d-194">响应正文不包含扩展属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-194">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="62c3d-195">示例</span><span class="sxs-lookup"><span data-stu-id="62c3d-195">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="62c3d-196">请求 1</span><span class="sxs-lookup"><span data-stu-id="62c3d-196">Request 1</span></span>

<span data-ttu-id="62c3d-p113">第一个示例通过包含一个单值扩展属性获取并展开指定的邮件。此筛选器返回其 **id** 与 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 字符串（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2_bs88AACHsLqWAAA="],
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="62c3d-199">响应 1</span><span class="sxs-lookup"><span data-stu-id="62c3d-199">Response 1</span></span>
<span data-ttu-id="62c3d-200">响应正文包括指定邮件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-200">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="62c3d-p114">注意：为了简单起见，会将此处所示的**邮件**对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="62c3d-203">请求 2</span><span class="sxs-lookup"><span data-stu-id="62c3d-203">Request 2</span></span>

<span data-ttu-id="62c3d-204">第二个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="62c3d-204">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="62c3d-205">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="62c3d-205">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="62c3d-206">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="62c3d-206">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="62c3d-207">它的 **value** 等于字符串 `Green`。</span><span class="sxs-lookup"><span data-stu-id="62c3d-207">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="62c3d-208">响应 2</span><span class="sxs-lookup"><span data-stu-id="62c3d-208">Response 2</span></span>

<span data-ttu-id="62c3d-p116">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。响应正文是类似于[获取邮件集合](../api/user_list_messages.md)中的响应。该响应不包括匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="62c3d-212">请求 3</span><span class="sxs-lookup"><span data-stu-id="62c3d-212">Request 3</span></span>

<span data-ttu-id="62c3d-213">第三个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="62c3d-213">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="62c3d-214">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="62c3d-214">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="62c3d-215">它的 **id** 等同于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）。</span><span class="sxs-lookup"><span data-stu-id="62c3d-215">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="62c3d-216">它的 **value** 包含字符串 `green`。</span><span class="sxs-lookup"><span data-stu-id="62c3d-216">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="62c3d-217">响应 3</span><span class="sxs-lookup"><span data-stu-id="62c3d-217">Response 3</span></span>

<span data-ttu-id="62c3d-218">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-218">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="62c3d-219">例如，如果邮件包含 **id** 等于字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 的单值扩展属性和 **value** `Light green`，则会与筛选器匹配并包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="62c3d-219">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="62c3d-220">响应正文类似于[获取邮件集合](../api/user_list_messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="62c3d-220">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="62c3d-221">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-221">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="62c3d-222">请求 4</span><span class="sxs-lookup"><span data-stu-id="62c3d-222">Request 4</span></span>

<span data-ttu-id="62c3d-223">接下来的两个示例展示了如何获取具有非字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="62c3d-223">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="62c3d-224">为了方便阅读，从中删除了必要的 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="62c3d-224">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="62c3d-225">下面的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="62c3d-225">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="62c3d-226">它的 **id** 与字符串 `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid` 匹配。</span><span class="sxs-lookup"><span data-stu-id="62c3d-226">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="62c3d-227">它的 **value** 是 GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`。</span><span class="sxs-lookup"><span data-stu-id="62c3d-227">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="62c3d-228">若要将属性值与 GUID 比较，请将 `ep/value` 转换为 `Edm.Guid`。</span><span class="sxs-lookup"><span data-stu-id="62c3d-228">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="62c3d-229">接下来的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="62c3d-229">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="62c3d-230">它的 **id** 与字符串 `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete` 匹配。</span><span class="sxs-lookup"><span data-stu-id="62c3d-230">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="62c3d-231">它的 **value** 等于整数 12。</span><span class="sxs-lookup"><span data-stu-id="62c3d-231">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="62c3d-232">若要将属性值与整数比较，请将 `ep/value` 转换为 `Edm.Int32`。</span><span class="sxs-lookup"><span data-stu-id="62c3d-232">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="62c3d-233">响应 4</span><span class="sxs-lookup"><span data-stu-id="62c3d-233">Response 4</span></span>

<span data-ttu-id="62c3d-234">对于前面两个示例中的任意一个，成功响应由 `HTTP 200 OK` 响应代码表示，响应正文包括扩展属性与相应筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-234">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="62c3d-235">响应正文类似于[获取邮件集合](../api/user_list_messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="62c3d-235">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="62c3d-236">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="62c3d-236">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->