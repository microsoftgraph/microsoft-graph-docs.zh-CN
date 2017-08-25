# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="221f7-101">获取 multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="221f7-101">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="221f7-102">使用 `$expand` 获取包含多值扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="221f7-102">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="221f7-p101">使用查询参数 `$expand`，你可以获得使用指定的扩展属性扩展的指定实例。这是当前获得 [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="221f7-p101">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="221f7-105">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="221f7-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="221f7-106">邮件</span><span class="sxs-lookup"><span data-stu-id="221f7-106">message</span></span>](../resources/message.md)
- [<span data-ttu-id="221f7-107">mailFolder</span><span class="sxs-lookup"><span data-stu-id="221f7-107">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="221f7-108">事件</span><span class="sxs-lookup"><span data-stu-id="221f7-108">event</span></span>](../resources/event.md)
- [<span data-ttu-id="221f7-109">日历</span><span class="sxs-lookup"><span data-stu-id="221f7-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="221f7-110">联系人</span><span class="sxs-lookup"><span data-stu-id="221f7-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="221f7-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="221f7-111">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="221f7-112">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="221f7-112">As well as the following group resources:</span></span>

- <span data-ttu-id="221f7-113">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="221f7-113">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="221f7-114">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="221f7-114">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="221f7-115">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="221f7-115">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="221f7-116">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="221f7-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="221f7-117">权限</span><span class="sxs-lookup"><span data-stu-id="221f7-117">Permissions</span></span>
<span data-ttu-id="221f7-p102">若要调用此 API，必须有以下权限之一，具体视要获取的资源而定。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="221f7-p102">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="221f7-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="221f7-120">Mail.Read</span></span>
- <span data-ttu-id="221f7-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="221f7-121">Calendars.Read</span></span>
- <span data-ttu-id="221f7-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="221f7-122">Contacts.Read</span></span>
- <span data-ttu-id="221f7-123">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="221f7-123">Group.Read.All</span></span> 
 
## <a name="http-request"></a><span data-ttu-id="221f7-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="221f7-124">HTTP request</span></span>

<span data-ttu-id="221f7-p103">获取通过与 **id** 属性中的筛选器匹配的扩展属性扩展的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](http://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="221f7-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="221f7-127">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="221f7-127">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="221f7-128">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="221f7-128">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="221f7-129">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="221f7-129">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="221f7-130">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="221f7-130">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="221f7-131">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="221f7-131">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="221f7-132">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="221f7-132">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="221f7-133">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="221f7-133">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="221f7-134">获取组**帖子**实例：</span><span class="sxs-lookup"><span data-stu-id="221f7-134">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="parameters"></a><span data-ttu-id="221f7-135">参数</span><span class="sxs-lookup"><span data-stu-id="221f7-135">Parameters</span></span>
|<span data-ttu-id="221f7-136">**参数**</span><span class="sxs-lookup"><span data-stu-id="221f7-136">**Parameter**</span></span>|<span data-ttu-id="221f7-137">**类型**</span><span class="sxs-lookup"><span data-stu-id="221f7-137">**Type**</span></span>|<span data-ttu-id="221f7-138">**说明**</span><span class="sxs-lookup"><span data-stu-id="221f7-138">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="221f7-139">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="221f7-139">_URL parameters_</span></span>|
|<span data-ttu-id="221f7-140">id_value</span><span class="sxs-lookup"><span data-stu-id="221f7-140">id_value</span></span>|<span data-ttu-id="221f7-141">String</span><span class="sxs-lookup"><span data-stu-id="221f7-141">String</span></span>|<span data-ttu-id="221f7-p104">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="221f7-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="221f7-146">请求标头</span><span class="sxs-lookup"><span data-stu-id="221f7-146">Request headers</span></span>
| <span data-ttu-id="221f7-147">名称</span><span class="sxs-lookup"><span data-stu-id="221f7-147">Name</span></span>      |<span data-ttu-id="221f7-148">说明</span><span class="sxs-lookup"><span data-stu-id="221f7-148">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="221f7-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="221f7-149">Authorization</span></span>  | <span data-ttu-id="221f7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="221f7-p105">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="221f7-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="221f7-152">Request body</span></span>
<span data-ttu-id="221f7-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="221f7-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="221f7-154">响应</span><span class="sxs-lookup"><span data-stu-id="221f7-154">Response</span></span>

<span data-ttu-id="221f7-155">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="221f7-155">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="221f7-156">响应正文包括通过匹配的 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="221f7-156">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="221f7-157">示例</span><span class="sxs-lookup"><span data-stu-id="221f7-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="221f7-158">请求</span><span class="sxs-lookup"><span data-stu-id="221f7-158">Request</span></span>
<span data-ttu-id="221f7-p106">此示例通过包含一个多值扩展属性获取并扩展指定的事件。此筛选器返回其 **id** 与字符串 `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation`（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221f7-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="221f7-161">响应</span><span class="sxs-lookup"><span data-stu-id="221f7-161">Response</span></span>

<span data-ttu-id="221f7-162">响应正文包括指定事件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221f7-162">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="221f7-p107">注意：为了简单起见，会将此处所示的 **event** 对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="221f7-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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