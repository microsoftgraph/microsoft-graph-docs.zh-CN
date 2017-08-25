# <a name="create-multi-value-extended-property"></a><span data-ttu-id="8314a-101">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="8314a-101">Create multi-value extended property</span></span>

<span data-ttu-id="8314a-102">在新建或现有的资源实例中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8314a-102">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="8314a-103">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="8314a-103">The following user resources are supported:</span></span>

- [<span data-ttu-id="8314a-104">邮件</span><span class="sxs-lookup"><span data-stu-id="8314a-104">message</span></span>](../resources/message.md)
- [<span data-ttu-id="8314a-105">mailFolder</span><span class="sxs-lookup"><span data-stu-id="8314a-105">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="8314a-106">事件</span><span class="sxs-lookup"><span data-stu-id="8314a-106">event</span></span>](../resources/event.md)
- [<span data-ttu-id="8314a-107">日历</span><span class="sxs-lookup"><span data-stu-id="8314a-107">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="8314a-108">联系人</span><span class="sxs-lookup"><span data-stu-id="8314a-108">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="8314a-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="8314a-109">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="8314a-110">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="8314a-110">As well as the following group resources:</span></span>

- <span data-ttu-id="8314a-111">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="8314a-111">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="8314a-112">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="8314a-112">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="8314a-113">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="8314a-113">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="8314a-114">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="8314a-114">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="8314a-115">权限</span><span class="sxs-lookup"><span data-stu-id="8314a-115">Permissions</span></span>
<span data-ttu-id="8314a-p101">要调用此 API，需要以下范围之一，具体视将在其中创建扩展查件的资源而定。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8314a-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extended property in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="8314a-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8314a-118">Mail.ReadWrite</span></span>
- <span data-ttu-id="8314a-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8314a-119">Calendars.ReadWrite</span></span>
- <span data-ttu-id="8314a-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8314a-120">Contacts.ReadWrite</span></span>
- <span data-ttu-id="8314a-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8314a-121">Group.ReadWrite.All</span></span>
 
## <a name="http-request"></a><span data-ttu-id="8314a-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8314a-122">HTTP request</span></span>
<span data-ttu-id="8314a-123">可以在新建或现有的资源实例中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8314a-123">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="8314a-p102">若要在_新的_资源实例中创建一个或多个扩展属性，请使用与创建实例相同的 REST 请求，并包括新资源实例的属性和请求正文中的_扩展属性_。注意，一些资源支持以多种方式创建。有关创建这些资源实例的详细信息，请参阅创建 [邮件](../resources/message.md)、[mailFolder](../api/user_post_mailfolders.md)、[事件](../api/user_post_events.md)、[日历](../api/user_post_calendars.md)、[联系人](../api/user_post_contacts.md)、[contactFolder](../api/user_post_contactfolders.md)、[组事件](../api/group_post_events.md)和[组帖子](../resources/post.md) 的相应主题。</span><span class="sxs-lookup"><span data-stu-id="8314a-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="8314a-127">以下是请求的语法。</span><span class="sxs-lookup"><span data-stu-id="8314a-127">The following is the syntax of the requests.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="8314a-128">若要在现有资源实例中创建一个或多个扩展属性，请在请求中指定实例，并在请求正文中包括扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8314a-128">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="8314a-129">**注意**不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8314a-129">**Note** You cannot create an extended property in an existing group post.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /groups/{id}/events/{id}
```


## <a name="parameters"></a><span data-ttu-id="8314a-130">参数</span><span class="sxs-lookup"><span data-stu-id="8314a-130">Parameters</span></span>
|<span data-ttu-id="8314a-131">**参数**</span><span class="sxs-lookup"><span data-stu-id="8314a-131">**Parameter**</span></span>|<span data-ttu-id="8314a-132">**类型**</span><span class="sxs-lookup"><span data-stu-id="8314a-132">**Type**</span></span>|<span data-ttu-id="8314a-133">**说明**</span><span class="sxs-lookup"><span data-stu-id="8314a-133">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8314a-134">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="8314a-134">_URL parameters_</span></span>|
|<span data-ttu-id="8314a-135">id</span><span class="sxs-lookup"><span data-stu-id="8314a-135">id</span></span>|<span data-ttu-id="8314a-136">string</span><span class="sxs-lookup"><span data-stu-id="8314a-136">string</span></span>|<span data-ttu-id="8314a-p103">对象在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="8314a-p103">A unique identifier for an object in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="8314a-139">_Body 参数_</span><span class="sxs-lookup"><span data-stu-id="8314a-139">_Body parameters_</span></span>|
|<span data-ttu-id="8314a-140">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="8314a-140">multiValueExtendedProperties</span></span>|<span data-ttu-id="8314a-141">[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="8314a-141">[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection</span></span>| <span data-ttu-id="8314a-142">一个或多个多值扩展属性的数组。</span><span class="sxs-lookup"><span data-stu-id="8314a-142">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="8314a-143">id</span><span class="sxs-lookup"><span data-stu-id="8314a-143">id</span></span>|<span data-ttu-id="8314a-144">String</span><span class="sxs-lookup"><span data-stu-id="8314a-144">String</span></span>|<span data-ttu-id="8314a-p104">对于 **multiValueExtendedProperties** 集合中的每个属性，请指定此参数以标识属性。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="8314a-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="8314a-149">值</span><span class="sxs-lookup"><span data-stu-id="8314a-149">value</span></span>|<span data-ttu-id="8314a-150">string</span><span class="sxs-lookup"><span data-stu-id="8314a-150">string</span></span>|<span data-ttu-id="8314a-p105">对于 **multiValueExtendedProperties** 集合中的每个属性，请指定属性值。必需。</span><span class="sxs-lookup"><span data-stu-id="8314a-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="8314a-153">请求标头</span><span class="sxs-lookup"><span data-stu-id="8314a-153">Request headers</span></span>
| <span data-ttu-id="8314a-154">名称</span><span class="sxs-lookup"><span data-stu-id="8314a-154">Name</span></span>       | <span data-ttu-id="8314a-155">值</span><span class="sxs-lookup"><span data-stu-id="8314a-155">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="8314a-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="8314a-156">Authorization</span></span> | <span data-ttu-id="8314a-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8314a-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8314a-159">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8314a-159">Content-Type</span></span> | <span data-ttu-id="8314a-160">application/json</span><span class="sxs-lookup"><span data-stu-id="8314a-160">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8314a-161">请求正文</span><span class="sxs-lookup"><span data-stu-id="8314a-161">Request body</span></span>

<span data-ttu-id="8314a-162">提供每个 [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) 对象在资源实例的 **multiValueExtendedProperties** 集合属性中的 JSON 正文。</span><span class="sxs-lookup"><span data-stu-id="8314a-162">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

<span data-ttu-id="8314a-163">在_新建_资源实例中创建扩展属性时，除了新的 **multiValueExtendedProperties** 集合，请提供资源实例的 JSON 表示形式（即 [邮件](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md) 等）。</span><span class="sxs-lookup"><span data-stu-id="8314a-163">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="8314a-164">响应</span><span class="sxs-lookup"><span data-stu-id="8314a-164">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="8314a-165">响应代码</span><span class="sxs-lookup"><span data-stu-id="8314a-165">Response code</span></span>
<span data-ttu-id="8314a-166">在新建资源实例中成功创建扩展属性的操作返回 `201 Created`（在新的组帖子中除外），根据所用的方法，该操作可以返回 `200 OK` 或 `202 Accepted`。</span><span class="sxs-lookup"><span data-stu-id="8314a-166">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="8314a-167">在现有的资源实例中，成功的创建操作返回 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="8314a-167">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="8314a-168">响应正文</span><span class="sxs-lookup"><span data-stu-id="8314a-168">Response body</span></span>

<span data-ttu-id="8314a-p107">在支持的资源（而不是 [组帖子](../resources/post.md)）中创建扩展属性时，该响应只包括新建或现有的实例，但不包括新的扩展属性。若要查看新创建的扩展属性，请 [获取通过扩展属性展开的实例](../api/multivaluelegacyextendedproperty_get.md)。</span><span class="sxs-lookup"><span data-stu-id="8314a-p107">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>

<span data-ttu-id="8314a-p108">在_新建_的组帖子中创建扩展属性时，响应仅包括响应代码，但不包括新帖子或扩展属性。不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8314a-p108">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="8314a-173">示例</span><span class="sxs-lookup"><span data-stu-id="8314a-173">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="8314a-174">请求 1</span><span class="sxs-lookup"><span data-stu-id="8314a-174">Request 1</span></span>

<span data-ttu-id="8314a-p109">第一个示例在同一个 POST 操作的全新事件中创建一个多值扩展属性。除了通常要包括的新事件的属性，请求正文还包括 **multiValueExtendedProperties** 集合（包含一个扩展属性）。请求正文包括该多值扩展属性的如下参数：</span><span class="sxs-lookup"><span data-stu-id="8314a-p109">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="8314a-178">**id**，将此属性指定为包含指定 GUID 和 `Recreation` 名称的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="8314a-178">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="8314a-179">**value**，将 `Recreation` 指定为包含 3 个字符串值（`["Food", "Hiking", "Swimming"]`）的数组。</span><span class="sxs-lookup"><span data-stu-id="8314a-179">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Family reunion",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together this Thanksgiving!"
  },
  "start": {
      "dateTime": "2015-11-26T09:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-29T21:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "Lauren@contoso.com",
        "name": "Lauren Solis"
      },
      "type": "Required"
    }
  ],
  "multiValueExtendedProperties": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="8314a-180">响应 1</span><span class="sxs-lookup"><span data-stu-id="8314a-180">Response 1</span></span>

<span data-ttu-id="8314a-p110">成功的响应由 `HTTP 201 Created` 响应代码表示，并在响应正文中包括新事件，类似于 [仅创建事件](../api/user_post_events.md) 中的响应。该响应不包括任何新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8314a-p110">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user_post_events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="8314a-183">若要查看新建的扩展属性，请 [获取通过扩展属性展开的事件](../api/multivaluelegacyextendedproperty_get.md)。</span><span class="sxs-lookup"><span data-stu-id="8314a-183">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="8314a-184">请求 2</span><span class="sxs-lookup"><span data-stu-id="8314a-184">Request 2</span></span>

<span data-ttu-id="8314a-p111">第二个示例为指定的邮件创建一个多值扩展属性。扩展属性是 **multiValueExtendedProperties** 集合中的唯一元素。请求正文包括扩展属性的如下参数：</span><span class="sxs-lookup"><span data-stu-id="8314a-p111">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="8314a-188">**id**，将此属性指定为包含指定 GUID 和名称 `Palette` 的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="8314a-188">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="8314a-189">**value**，将 `Palette` 指定为包含 3 个字符串值（`["Green", "Aqua", "Blue"]`）的数组。</span><span class="sxs-lookup"><span data-stu-id="8314a-189">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueExtendedProperties": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="8314a-190">响应 2</span><span class="sxs-lookup"><span data-stu-id="8314a-190">Response 2</span></span>

<span data-ttu-id="8314a-p112">成功的响应由 `HTTP 200 OK` 响应代码表示，并在响应正文中包括指定的邮件，类似于 [更新邮件](../api/message_update.md) 中的响应。该响应不包括新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8314a-p112">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message_update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="8314a-193">若要查看新建的扩展属性，请 [获取通过扩展属性展开的邮件](../api/multivaluelegacyextendedproperty_get.md)。</span><span class="sxs-lookup"><span data-stu-id="8314a-193">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->




