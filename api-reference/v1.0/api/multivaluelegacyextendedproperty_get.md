# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="234d6-101">获取 multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="234d6-101">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="234d6-102">使用 `$expand` 获取包含多值扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="234d6-102">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="234d6-103">使用查询参数 `$expand`，可以获取使用指明的扩展属性扩展的指定实例。</span><span class="sxs-lookup"><span data-stu-id="234d6-103">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="234d6-104">这是当前获取 [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="234d6-104">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="234d6-105">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="234d6-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="234d6-106">日历</span><span class="sxs-lookup"><span data-stu-id="234d6-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="234d6-107">联系人</span><span class="sxs-lookup"><span data-stu-id="234d6-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="234d6-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="234d6-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="234d6-109">事件</span><span class="sxs-lookup"><span data-stu-id="234d6-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="234d6-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="234d6-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="234d6-111">message</span><span class="sxs-lookup"><span data-stu-id="234d6-111">message</span></span>](../resources/message.md) 

<span data-ttu-id="234d6-112">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="234d6-112">As well as the following group resources:</span></span>

- <span data-ttu-id="234d6-113">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="234d6-113">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="234d6-114">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="234d6-114">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="234d6-115">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="234d6-115">group [post](../resources/post.md)</span></span>

<span data-ttu-id="234d6-116">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="234d6-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="234d6-117">权限</span><span class="sxs-lookup"><span data-stu-id="234d6-117">Permissions</span></span>
<span data-ttu-id="234d6-118">根据资源获得的扩展的属性和权限键入 （委派或应用程序） 您请求，若要调用此 API 至少是下表中所指定的权限。</span><span class="sxs-lookup"><span data-stu-id="234d6-118">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="234d6-119">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="234d6-119">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="234d6-120">支持的资源</span><span class="sxs-lookup"><span data-stu-id="234d6-120">Supported resource</span></span> | <span data-ttu-id="234d6-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="234d6-121">Delegated (work or school account)</span></span> | <span data-ttu-id="234d6-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="234d6-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="234d6-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="234d6-123">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="234d6-124">日历</span><span class="sxs-lookup"><span data-stu-id="234d6-124">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="234d6-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-125">Calendars.Read</span></span> | <span data-ttu-id="234d6-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-126">Calendars.Read</span></span> | <span data-ttu-id="234d6-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-127">Calendars.Read</span></span> |
| [<span data-ttu-id="234d6-128">联系人</span><span class="sxs-lookup"><span data-stu-id="234d6-128">contact</span></span>](../resources/contact.md) | <span data-ttu-id="234d6-129">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-129">Contacts.Read</span></span> | <span data-ttu-id="234d6-130">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-130">Contacts.Read</span></span> | <span data-ttu-id="234d6-131">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-131">Contacts.Read</span></span> |
| [<span data-ttu-id="234d6-132">contactFolder</span><span class="sxs-lookup"><span data-stu-id="234d6-132">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="234d6-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-133">Contacts.Read</span></span> | <span data-ttu-id="234d6-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-134">Contacts.Read</span></span> | <span data-ttu-id="234d6-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-135">Contacts.Read</span></span> |
| [<span data-ttu-id="234d6-136">事件</span><span class="sxs-lookup"><span data-stu-id="234d6-136">event</span></span>](../resources/event.md) | <span data-ttu-id="234d6-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-137">Calendars.Read</span></span> | <span data-ttu-id="234d6-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-138">Calendars.Read</span></span> |  <span data-ttu-id="234d6-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-139">Calendars.Read</span></span>|
| <span data-ttu-id="234d6-140">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="234d6-140">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="234d6-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="234d6-141">Group.Read.All</span></span> | <span data-ttu-id="234d6-142">不支持</span><span class="sxs-lookup"><span data-stu-id="234d6-142">Not supported</span></span> | <span data-ttu-id="234d6-143">不支持</span><span class="sxs-lookup"><span data-stu-id="234d6-143">Not supported</span></span> |
| <span data-ttu-id="234d6-144">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="234d6-144">group [event](../resources/event.md)</span></span> | <span data-ttu-id="234d6-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="234d6-145">Group.Read.All</span></span> | <span data-ttu-id="234d6-146">不支持</span><span class="sxs-lookup"><span data-stu-id="234d6-146">Not supported</span></span> | <span data-ttu-id="234d6-147">不支持</span><span class="sxs-lookup"><span data-stu-id="234d6-147">Not supported</span></span> |
| <span data-ttu-id="234d6-148">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="234d6-148">group [post](../resources/post.md)</span></span> | <span data-ttu-id="234d6-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="234d6-149">Group.Read.All</span></span> | <span data-ttu-id="234d6-150">不支持</span><span class="sxs-lookup"><span data-stu-id="234d6-150">Not supported</span></span> | <span data-ttu-id="234d6-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="234d6-151">Group.Read.All</span></span> |
| [<span data-ttu-id="234d6-152">mailFolder</span><span class="sxs-lookup"><span data-stu-id="234d6-152">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="234d6-153">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-153">Mail.Read</span></span> | <span data-ttu-id="234d6-154">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-154">Mail.Read</span></span> | <span data-ttu-id="234d6-155">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-155">Mail.Read</span></span> |
| [<span data-ttu-id="234d6-156">message</span><span class="sxs-lookup"><span data-stu-id="234d6-156">message</span></span>](../resources/message.md) | <span data-ttu-id="234d6-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-157">Mail.Read</span></span> | <span data-ttu-id="234d6-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-158">Mail.Read</span></span> | <span data-ttu-id="234d6-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="234d6-159">Mail.Read</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="234d6-160">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="234d6-160">HTTP request</span></span>

<span data-ttu-id="234d6-p103">获取通过与 **id** 属性中的筛选器匹配的扩展属性扩展的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="234d6-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="234d6-163">获取**邮件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="234d6-163">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="234d6-164">获取一个**mailFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="234d6-164">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="234d6-165">获取**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="234d6-165">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="234d6-166">获取**日历**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="234d6-166">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="234d6-167">获取**联系人**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="234d6-167">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="234d6-168">获取一个**contactFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="234d6-168">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="234d6-169">获取组**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="234d6-169">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="234d6-170">获取一个组**发布**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="234d6-170">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="234d6-171">路径参数</span><span class="sxs-lookup"><span data-stu-id="234d6-171">Path parameters</span></span>
|<span data-ttu-id="234d6-172">参数</span><span class="sxs-lookup"><span data-stu-id="234d6-172">Parameter</span></span>|<span data-ttu-id="234d6-173">类型</span><span class="sxs-lookup"><span data-stu-id="234d6-173">Type</span></span>|<span data-ttu-id="234d6-174">说明</span><span class="sxs-lookup"><span data-stu-id="234d6-174">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="234d6-175">id_value</span><span class="sxs-lookup"><span data-stu-id="234d6-175">id_value</span></span>|<span data-ttu-id="234d6-176">String</span><span class="sxs-lookup"><span data-stu-id="234d6-176">String</span></span>|<span data-ttu-id="234d6-p104">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="234d6-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="234d6-181">请求标头</span><span class="sxs-lookup"><span data-stu-id="234d6-181">Request headers</span></span>
| <span data-ttu-id="234d6-182">名称</span><span class="sxs-lookup"><span data-stu-id="234d6-182">Name</span></span>      |<span data-ttu-id="234d6-183">说明</span><span class="sxs-lookup"><span data-stu-id="234d6-183">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="234d6-184">Authorization</span><span class="sxs-lookup"><span data-stu-id="234d6-184">Authorization</span></span>  | <span data-ttu-id="234d6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="234d6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="234d6-187">请求正文</span><span class="sxs-lookup"><span data-stu-id="234d6-187">Request body</span></span>
<span data-ttu-id="234d6-188">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="234d6-188">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="234d6-189">响应</span><span class="sxs-lookup"><span data-stu-id="234d6-189">Response</span></span>

<span data-ttu-id="234d6-190">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="234d6-190">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="234d6-191">响应正文包括通过匹配的 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="234d6-191">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="234d6-192">示例</span><span class="sxs-lookup"><span data-stu-id="234d6-192">Example</span></span>
##### <a name="request"></a><span data-ttu-id="234d6-193">请求</span><span class="sxs-lookup"><span data-stu-id="234d6-193">Request</span></span>
<span data-ttu-id="234d6-p106">此示例通过包含一个多值扩展属性获取并扩展指定的事件。此筛选器返回其 **id** 与字符串 `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation`（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="234d6-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="234d6-196">响应</span><span class="sxs-lookup"><span data-stu-id="234d6-196">Response</span></span>

<span data-ttu-id="234d6-197">响应正文包括指定事件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="234d6-197">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="234d6-p107">注意：为了简单起见，会将此处所示的 **event** 对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="234d6-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
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
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
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