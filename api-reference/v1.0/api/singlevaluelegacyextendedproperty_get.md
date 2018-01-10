# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="55a21-101">获取 singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="55a21-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="55a21-102">通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="55a21-102">Get resource instances that contain a single-value extended property by using `$expand` or `$filter`.</span></span>

<span data-ttu-id="55a21-p101">使用查询参数 `$expand` 可以获得使用指示扩展属性扩展的指定实例。这是当前获得 [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="55a21-p101">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="55a21-p102">使用查询参数 `$filter`获得指定资源的所有实例，这些实例具有与 **id** 中的筛选器匹配的扩展属性以及 **value** 属性。该筛选器应用于资源在已登录用户的邮箱中的所有实例。</span><span class="sxs-lookup"><span data-stu-id="55a21-p102">Using the query parameter `$filter` allows you to get all the instances of the specified resource that have an extended property matching a filter on the **id** and **value** properties. The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span>

<span data-ttu-id="55a21-107">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="55a21-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="55a21-108">邮件</span><span class="sxs-lookup"><span data-stu-id="55a21-108">message</span></span>](../resources/message.md)
- [<span data-ttu-id="55a21-109">mailFolder</span><span class="sxs-lookup"><span data-stu-id="55a21-109">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="55a21-110">事件</span><span class="sxs-lookup"><span data-stu-id="55a21-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="55a21-111">日历</span><span class="sxs-lookup"><span data-stu-id="55a21-111">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="55a21-112">联系人</span><span class="sxs-lookup"><span data-stu-id="55a21-112">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="55a21-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="55a21-113">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="55a21-114">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="55a21-114">As well as the following group resources:</span></span>

- <span data-ttu-id="55a21-115">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="55a21-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="55a21-116">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="55a21-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="55a21-117">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="55a21-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="55a21-118">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="55a21-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="55a21-119">权限</span><span class="sxs-lookup"><span data-stu-id="55a21-119">Permissions</span></span>
<span data-ttu-id="55a21-p103">若要调用此 API，必须有以下权限之一，具体视要获取的资源而定。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="55a21-p103">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="55a21-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="55a21-122">Mail.Read</span></span>
- <span data-ttu-id="55a21-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="55a21-123">Calendars.Read</span></span>
- <span data-ttu-id="55a21-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="55a21-124">Contacts.Read</span></span>
- <span data-ttu-id="55a21-125">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="55a21-125">Group.Read.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="55a21-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55a21-126">HTTP request</span></span>

#### <a name="get-a-resource-instance-using-expand"></a><span data-ttu-id="55a21-127">使用 `$expand` 获取资源实例</span><span class="sxs-lookup"><span data-stu-id="55a21-127">GET a resource instance using `$expand`</span></span>
<span data-ttu-id="55a21-p104">获取通过与 **id** 属性中的筛选器匹配的扩展属性展开的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码]((http://www.w3schools.com/tags/ref_urlencode.asp))。</span><span class="sxs-lookup"><span data-stu-id="55a21-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding]((http://www.w3schools.com/tags/ref_urlencode.asp)) to the space characters in the filter string.</span></span>

<span data-ttu-id="55a21-130">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-130">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="55a21-131">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-131">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="55a21-132">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-132">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="55a21-133">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-133">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="55a21-134">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-134">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="55a21-135">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-135">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="55a21-136">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-136">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="55a21-137">获取组**帖子**实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-137">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="55a21-138">使用 `$filter` 获取资源实例</span><span class="sxs-lookup"><span data-stu-id="55a21-138">GET resource instances using `$filter`</span></span>

<span data-ttu-id="55a21-139">获取支持的资源实例，其中包含与 **id** 和 **value** 属性筛选器匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="55a21-139">Get instances of a supported resource that have the extended property matching a filter on the **id** and **value** properties. Make sure you apply URL encoding to the following characters in the filter string - forward slash and space.</span></span> <span data-ttu-id="55a21-140">请务必对筛选器字符串中的以下字符应用 [URL 编码]((http://www.w3schools.com/tags/ref_urlencode.asp))：冒号、正斜杠和空格。</span><span class="sxs-lookup"><span data-stu-id="55a21-140">Get instances of a supported resource that have the extended property matching a filter on the id and value properties. Make sure you apply [URL encoding]((http://www.w3schools.com/tags/ref_urlencode.asp)) to the following characters in the filter string - forward slash and space.</span></span>


<span data-ttu-id="55a21-141">获取 **message** 实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-141">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="55a21-142">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-142">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="55a21-143">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-143">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="55a21-144">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-144">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="55a21-145">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-145">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="55a21-146">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-146">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="55a21-147">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-147">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="55a21-148">获取组**帖子**实例：</span><span class="sxs-lookup"><span data-stu-id="55a21-148">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

## <a name="parameters"></a><span data-ttu-id="55a21-149">参数</span><span class="sxs-lookup"><span data-stu-id="55a21-149">Parameters</span></span>
|<span data-ttu-id="55a21-150">**参数**</span><span class="sxs-lookup"><span data-stu-id="55a21-150">**Parameter**</span></span>|<span data-ttu-id="55a21-151">**类型**</span><span class="sxs-lookup"><span data-stu-id="55a21-151">**Type**</span></span>|<span data-ttu-id="55a21-152">**说明**</span><span class="sxs-lookup"><span data-stu-id="55a21-152">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="55a21-153">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="55a21-153">_URL parameters_</span></span>|
|<span data-ttu-id="55a21-154">id_value</span><span class="sxs-lookup"><span data-stu-id="55a21-154">id_value</span></span>|<span data-ttu-id="55a21-155">String</span><span class="sxs-lookup"><span data-stu-id="55a21-155">String</span></span>|<span data-ttu-id="55a21-p106">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="55a21-p106">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="55a21-160">property_value</span><span class="sxs-lookup"><span data-stu-id="55a21-160">property_value</span></span> |<span data-ttu-id="55a21-161">String</span><span class="sxs-lookup"><span data-stu-id="55a21-161">String</span></span>|<span data-ttu-id="55a21-162">要匹配的扩展属性的值。</span><span class="sxs-lookup"><span data-stu-id="55a21-162">The value of the extended property to match. Required where listed in the HTTP request section.</span></span> <span data-ttu-id="55a21-163">如果在上面的 **HTTP 请求**部分中列出，则为必需参数。</span><span class="sxs-lookup"><span data-stu-id="55a21-163">The value of the extended property to match. Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="55a21-164">如果 {property_value} 不是字符串，请务必在与 {property_value} 比较时，将 `ep/value` 显式转换为相应的 Edm 数据类型。</span><span class="sxs-lookup"><span data-stu-id="55a21-164">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="55a21-165">有关示例，请参阅下面的[请求 3](#request-3)。</span><span class="sxs-lookup"><span data-stu-id="55a21-165">See [request 3](#request-3) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="55a21-166">请求头</span><span class="sxs-lookup"><span data-stu-id="55a21-166">Request headers</span></span>
| <span data-ttu-id="55a21-167">名称</span><span class="sxs-lookup"><span data-stu-id="55a21-167">Name</span></span>      |<span data-ttu-id="55a21-168">说明</span><span class="sxs-lookup"><span data-stu-id="55a21-168">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="55a21-169">Authorization</span><span class="sxs-lookup"><span data-stu-id="55a21-169">Authorization</span></span>  | <span data-ttu-id="55a21-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="55a21-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55a21-172">请求正文</span><span class="sxs-lookup"><span data-stu-id="55a21-172">Request body</span></span>
<span data-ttu-id="55a21-173">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="55a21-173">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55a21-174">响应</span><span class="sxs-lookup"><span data-stu-id="55a21-174">Response</span></span>

<span data-ttu-id="55a21-175">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="55a21-175">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="55a21-176">使用 `$expand` 获取资源实例</span><span class="sxs-lookup"><span data-stu-id="55a21-176">GET resource instance using `$expand`</span></span>
<span data-ttu-id="55a21-177">响应正文包括通过匹配的 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="55a21-177">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="55a21-178">使用 `$filter` 获取资源实例</span><span class="sxs-lookup"><span data-stu-id="55a21-178">GET resource instances using `$filter`</span></span>
<span data-ttu-id="55a21-p109">响应正文包含一个或多个表示资源实例的对象，这些实例包含匹配的扩展属性。响应正文不包含扩展属性。</span><span class="sxs-lookup"><span data-stu-id="55a21-p109">The response body includes one or more objects representing the resource instances that contain the matching extended property. The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="55a21-181">示例</span><span class="sxs-lookup"><span data-stu-id="55a21-181">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="55a21-182">请求 1</span><span class="sxs-lookup"><span data-stu-id="55a21-182">Request 1</span></span>

<span data-ttu-id="55a21-p110">第一个示例通过包含一个单值扩展属性获取并展开指定的邮件。此筛选器返回其 **id** 与 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 字符串（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="55a21-p110">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="55a21-185">响应 1</span><span class="sxs-lookup"><span data-stu-id="55a21-185">Response 1</span></span>
<span data-ttu-id="55a21-186">响应正文包括指定邮件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="55a21-186">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="55a21-p111">注意：为了简单起见，会将此处所示的**邮件**对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="55a21-p111">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="55a21-189">请求 2</span><span class="sxs-lookup"><span data-stu-id="55a21-189">Request 2</span></span>

<span data-ttu-id="55a21-190">第二个示例展示了如何获取具有筛选器中指定的字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="55a21-190">The second example gets messages that have the single-value extended property specified in the filter. The filter returns the extended property that has:</span></span> <span data-ttu-id="55a21-191">此筛选器查找如下扩展属性：</span><span class="sxs-lookup"><span data-stu-id="55a21-191">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="55a21-192">它的 **id** 与字符串 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`（包含 URL 编码，但此处为了方便阅读，已将其删除）匹配。</span><span class="sxs-lookup"><span data-stu-id="55a21-192">Its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="55a21-193">它的 **value** 是字符串 `Green`。</span><span class="sxs-lookup"><span data-stu-id="55a21-193">Its **value** being the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="55a21-194">响应 2</span><span class="sxs-lookup"><span data-stu-id="55a21-194">Response 2</span></span>

<span data-ttu-id="55a21-p113">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。响应正文是类似于[获取邮件集合](../api/user_list_messages.md)中的响应。该响应不包括匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="55a21-p113">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="55a21-198">请求 3</span><span class="sxs-lookup"><span data-stu-id="55a21-198">Request 3</span></span>

<span data-ttu-id="55a21-199">接下来的两个示例展示了如何获取具有非字符串类型单值扩展属性的邮件。</span><span class="sxs-lookup"><span data-stu-id="55a21-199">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="55a21-200">为了方便阅读，从中删除了必要的 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="55a21-200">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="55a21-201">下面的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="55a21-201">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="55a21-202">它的 **id** 与字符串 `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid` 匹配。</span><span class="sxs-lookup"><span data-stu-id="55a21-202">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="55a21-203">它的 **value** 是 GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`。</span><span class="sxs-lookup"><span data-stu-id="55a21-203">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="55a21-204">若要将属性值与 GUID 比较，请将 `ep/value` 转换为 `Edm.Guid`。</span><span class="sxs-lookup"><span data-stu-id="55a21-204">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="55a21-205">接下来的示例展示了查找以下扩展属性的筛选器：</span><span class="sxs-lookup"><span data-stu-id="55a21-205">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="55a21-206">它的 **id** 与字符串 `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete` 匹配。</span><span class="sxs-lookup"><span data-stu-id="55a21-206">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="55a21-207">它的 **value** 等于整数 12。</span><span class="sxs-lookup"><span data-stu-id="55a21-207">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="55a21-208">若要将属性值与整数比较，请将 `ep/value` 转换为 `Edm.Int32`。</span><span class="sxs-lookup"><span data-stu-id="55a21-208">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-3"></a><span data-ttu-id="55a21-209">响应 3</span><span class="sxs-lookup"><span data-stu-id="55a21-209">Response 3</span></span>

<span data-ttu-id="55a21-210">对于前面两个示例中的任意一个，成功响应由 `HTTP 200 OK` 响应代码表示，响应正文包括扩展属性与相应筛选器匹配的邮件的所有属性。</span><span class="sxs-lookup"><span data-stu-id="55a21-210">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="55a21-211">响应正文类似于[获取邮件集合](../api/user_list_messages.md)中的响应。</span><span class="sxs-lookup"><span data-stu-id="55a21-211">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="55a21-212">响应中不包含匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="55a21-212">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->