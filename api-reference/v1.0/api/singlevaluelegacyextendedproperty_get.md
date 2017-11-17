# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="25b25-101">获取 singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="25b25-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="25b25-102">通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="25b25-102">Get resource instances that contain a single-value extended property by using `$expand` or `$filter`.</span></span>

<span data-ttu-id="25b25-p101">使用查询参数 `$expand` 可以获得使用指示扩展属性扩展的指定实例。这是当前获得 [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="25b25-p101">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="25b25-p102">使用查询参数 `$filter`获得指定资源的所有实例，这些实例具有与 **id** 中的筛选器匹配的扩展属性以及 **value** 属性。该筛选器应用于资源在已登录用户的邮箱中的所有实例。</span><span class="sxs-lookup"><span data-stu-id="25b25-p102">Using the query parameter `$filter` allows you to get all the instances of the specified resource that have an extended property matching a filter on the **id** and **value** properties. The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span>

<span data-ttu-id="25b25-107">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="25b25-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="25b25-108">邮件</span><span class="sxs-lookup"><span data-stu-id="25b25-108">message</span></span>](../resources/message.md)
- [<span data-ttu-id="25b25-109">mailFolder</span><span class="sxs-lookup"><span data-stu-id="25b25-109">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="25b25-110">事件</span><span class="sxs-lookup"><span data-stu-id="25b25-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="25b25-111">日历</span><span class="sxs-lookup"><span data-stu-id="25b25-111">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="25b25-112">联系人</span><span class="sxs-lookup"><span data-stu-id="25b25-112">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="25b25-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="25b25-113">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="25b25-114">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="25b25-114">As well as the following group resources:</span></span>

- <span data-ttu-id="25b25-115">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="25b25-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="25b25-116">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="25b25-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="25b25-117">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="25b25-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="25b25-118">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="25b25-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="25b25-119">权限</span><span class="sxs-lookup"><span data-stu-id="25b25-119">Permissions</span></span>
<span data-ttu-id="25b25-p103">若要调用此 API，必须有以下权限之一，具体视要获取的资源而定。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="25b25-p103">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="25b25-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="25b25-122">Mail.Read</span></span>
- <span data-ttu-id="25b25-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="25b25-123">Calendars.Read</span></span>
- <span data-ttu-id="25b25-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="25b25-124">Contacts.Read</span></span>
- <span data-ttu-id="25b25-125">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="25b25-125">Group.Read.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="25b25-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25b25-126">HTTP request</span></span>

#### <a name="get-a-resource-instance-using-expand"></a><span data-ttu-id="25b25-127">使用 `$expand` 获取资源实例</span><span class="sxs-lookup"><span data-stu-id="25b25-127">GET a resource instance using `$expand`</span></span>
<span data-ttu-id="25b25-p104">获取通过与 **id** 属性中的筛选器匹配的扩展属性展开的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](http://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="25b25-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="25b25-130">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-130">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="25b25-131">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-131">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="25b25-132">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-132">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="25b25-133">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-133">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="25b25-134">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-134">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="25b25-135">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-135">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="25b25-136">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-136">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="25b25-137">获取组**帖子**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-137">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="25b25-138">使用 `$filter` 获取资源实例</span><span class="sxs-lookup"><span data-stu-id="25b25-138">GET resource instances using `$filter`</span></span>

<span data-ttu-id="25b25-p105">获取支持的资源实例，这些实例具有与 **id** 中的筛选器匹配的扩展属性以及 **value** 属性。请确保对筛选器字符串中的空格字符应用 [URL 编码](http://www.w3schools.com/tags/ref_urlencode.asp) - 正斜杠和空格。</span><span class="sxs-lookup"><span data-stu-id="25b25-p105">Get instances of a supported resource that have the extended property matching a filter on the **id** and **value** properties. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - forward slash and space.</span></span>


<span data-ttu-id="25b25-141">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-141">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="25b25-142">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-142">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="25b25-143">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-143">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="25b25-144">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-144">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="25b25-145">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-145">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="25b25-146">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-146">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="25b25-147">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-147">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="25b25-148">获取组**帖子**实例：</span><span class="sxs-lookup"><span data-stu-id="25b25-148">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

## <a name="parameters"></a><span data-ttu-id="25b25-149">参数</span><span class="sxs-lookup"><span data-stu-id="25b25-149">Parameters</span></span>
|<span data-ttu-id="25b25-150">**参数**</span><span class="sxs-lookup"><span data-stu-id="25b25-150">**Parameter**</span></span>|<span data-ttu-id="25b25-151">**类型**</span><span class="sxs-lookup"><span data-stu-id="25b25-151">**Type**</span></span>|<span data-ttu-id="25b25-152">**说明**</span><span class="sxs-lookup"><span data-stu-id="25b25-152">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="25b25-153">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="25b25-153">_URL parameters_</span></span>|
|<span data-ttu-id="25b25-154">id_value</span><span class="sxs-lookup"><span data-stu-id="25b25-154">id_value</span></span>|<span data-ttu-id="25b25-155">String</span><span class="sxs-lookup"><span data-stu-id="25b25-155">String</span></span>|<span data-ttu-id="25b25-p106">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="25b25-p106">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="25b25-160">property_value</span><span class="sxs-lookup"><span data-stu-id="25b25-160">property_value</span></span>|<span data-ttu-id="25b25-161">String</span><span class="sxs-lookup"><span data-stu-id="25b25-161">String</span></span>|<span data-ttu-id="25b25-p107">要匹配的扩展属性的值。上面 **HTTP 请求**部分中列出的所必需的参数。</span><span class="sxs-lookup"><span data-stu-id="25b25-p107">The value of the extended property to match. Required where listed in the **HTTP request** section above.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="25b25-164">请求标头</span><span class="sxs-lookup"><span data-stu-id="25b25-164">Request headers</span></span>
| <span data-ttu-id="25b25-165">名称</span><span class="sxs-lookup"><span data-stu-id="25b25-165">Name</span></span>      |<span data-ttu-id="25b25-166">说明</span><span class="sxs-lookup"><span data-stu-id="25b25-166">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="25b25-167">Authorization</span><span class="sxs-lookup"><span data-stu-id="25b25-167">Authorization</span></span>  | <span data-ttu-id="25b25-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25b25-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25b25-170">请求正文</span><span class="sxs-lookup"><span data-stu-id="25b25-170">Request body</span></span>
<span data-ttu-id="25b25-171">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="25b25-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25b25-172">响应</span><span class="sxs-lookup"><span data-stu-id="25b25-172">Response</span></span>

<span data-ttu-id="25b25-173">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="25b25-173">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="25b25-174">使用 `$expand` 获取资源实例</span><span class="sxs-lookup"><span data-stu-id="25b25-174">GET resource instance using `$expand`</span></span>
<span data-ttu-id="25b25-175">响应正文包括通过匹配的 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="25b25-175">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="25b25-176">使用 `$filter` 获取资源实例</span><span class="sxs-lookup"><span data-stu-id="25b25-176">GET resource instances using `$filter`</span></span>
<span data-ttu-id="25b25-p109">响应正文包含一个或多个表示资源实例的对象，这些实例包含匹配的扩展属性。响应正文不包含扩展属性。</span><span class="sxs-lookup"><span data-stu-id="25b25-p109">The response body includes one or more objects representing the resource instances that contain the matching extended property. The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="25b25-179">示例</span><span class="sxs-lookup"><span data-stu-id="25b25-179">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="25b25-180">请求 1</span><span class="sxs-lookup"><span data-stu-id="25b25-180">Request 1</span></span>

<span data-ttu-id="25b25-p110">第一个示例通过包含一个单值扩展属性获取并展开指定的邮件。此筛选器返回其 **id** 与 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 字符串（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="25b25-p110">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
##### <a name="response-1"></a><span data-ttu-id="25b25-183">响应 1</span><span class="sxs-lookup"><span data-stu-id="25b25-183">Response 1</span></span>
<span data-ttu-id="25b25-184">响应正文包括指定邮件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="25b25-184">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="25b25-p111">注意：为了简单起见，会将此处所示的**邮件**对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25b25-p111">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

****

#### <a name="request-2"></a><span data-ttu-id="25b25-187">请求 2</span><span class="sxs-lookup"><span data-stu-id="25b25-187">Request 2</span></span>

<span data-ttu-id="25b25-p112">第二个示例获取具有筛选器中指定的单值扩展属性的邮件。此筛选器将返回如下的扩展属性：</span><span class="sxs-lookup"><span data-stu-id="25b25-p112">The second example gets messages that have the single-value extended property specified in the filter. The filter returns the extended property that has:</span></span>
- <span data-ttu-id="25b25-190">其 **id** 与 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` 字符串（包含 URL 编码，此处为了便于阅读，已将其删除）匹配。</span><span class="sxs-lookup"><span data-stu-id="25b25-190">Its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>
- <span data-ttu-id="25b25-191">其**值**为 `Green`。</span><span class="sxs-lookup"><span data-stu-id="25b25-191">Its **value** being `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/api/v1.0/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

##### <a name="response-2"></a><span data-ttu-id="25b25-192">响应 2</span><span class="sxs-lookup"><span data-stu-id="25b25-192">Response 2</span></span>

<span data-ttu-id="25b25-p113">成功的响应将由 `HTTP 200 OK` 响应代码表示，响应正文包括其扩展属性与筛选器匹配的邮件的所有属性。响应正文是类似于[获取邮件集合](../api/user_list_messages.md)中的响应。该响应不包括匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="25b25-p113">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->