# <a name="create-single-value-extended-property"></a><span data-ttu-id="ed687-101">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="ed687-101">Create single-value extended property</span></span>

<span data-ttu-id="ed687-102">在新建或现有的资源实例中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ed687-102">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="ed687-103">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="ed687-103">The following user resources are supported:</span></span>

- [<span data-ttu-id="ed687-104">邮件</span><span class="sxs-lookup"><span data-stu-id="ed687-104">message</span></span>](../resources/message.md)
- [<span data-ttu-id="ed687-105">mailFolder</span><span class="sxs-lookup"><span data-stu-id="ed687-105">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="ed687-106">事件</span><span class="sxs-lookup"><span data-stu-id="ed687-106">event</span></span>](../resources/event.md)
- [<span data-ttu-id="ed687-107">日历</span><span class="sxs-lookup"><span data-stu-id="ed687-107">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="ed687-108">联系人</span><span class="sxs-lookup"><span data-stu-id="ed687-108">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="ed687-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ed687-109">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="ed687-110">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="ed687-110">As well as the following group resources:</span></span>

- <span data-ttu-id="ed687-111">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="ed687-111">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="ed687-112">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="ed687-112">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="ed687-113">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="ed687-113">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="ed687-114">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="ed687-114">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed687-115">权限</span><span class="sxs-lookup"><span data-stu-id="ed687-115">Permissions</span></span>
<span data-ttu-id="ed687-p101">要调用此 API，需要以下范围之一，具体视将在其中创建扩展查件的资源而定。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ed687-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extended property in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="ed687-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed687-118">Mail.ReadWrite</span></span>
- <span data-ttu-id="ed687-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed687-119">Calendars.ReadWrite</span></span>
- <span data-ttu-id="ed687-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed687-120">Contacts.ReadWrite</span></span>
- <span data-ttu-id="ed687-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed687-121">Group.ReadWrite.All</span></span>
 
## <a name="http-request"></a><span data-ttu-id="ed687-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed687-122">HTTP request</span></span>
<span data-ttu-id="ed687-123">可以在新建或现有的资源实例中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ed687-123">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="ed687-p102">若要在_新的_资源实例中创建一个或多个扩展属性，请使用与创建实例相同的 REST 请求，并包括新资源实例的属性和请求正文中的_扩展属性_。注意，一些资源支持以多种方式创建。有关创建这些资源实例的详细信息，请参阅创建 [邮件](../resources/message.md)、[mailFolder](../api/user_post_mailfolders.md)、[事件](../api/user_post_events.md)、[日历](../api/user_post_calendars.md)、[联系人](../api/user_post_contacts.md)、[contactFolder](../api/user_post_contactfolders.md)、[组事件](../api/group_post_events.md)和[组帖子](../resources/post.md) 的相应主题。</span><span class="sxs-lookup"><span data-stu-id="ed687-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="ed687-127">以下是请求的语法。</span><span class="sxs-lookup"><span data-stu-id="ed687-127">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="ed687-128">若要在现有资源实例中创建一个或多个扩展属性，请在请求中指定实例，并在请求正文中包括扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ed687-128">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="ed687-129">**注意**不能在现有的组帖子中创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ed687-129">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="ed687-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed687-130">Request headers</span></span>
| <span data-ttu-id="ed687-131">名称</span><span class="sxs-lookup"><span data-stu-id="ed687-131">Name</span></span>       | <span data-ttu-id="ed687-132">值</span><span class="sxs-lookup"><span data-stu-id="ed687-132">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ed687-133">授权</span><span class="sxs-lookup"><span data-stu-id="ed687-133">Authorization</span></span> | <span data-ttu-id="ed687-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed687-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed687-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed687-136">Content-Type</span></span> | <span data-ttu-id="ed687-137">application/json</span><span class="sxs-lookup"><span data-stu-id="ed687-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed687-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed687-138">Request body</span></span>

<span data-ttu-id="ed687-139">提供每个 [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) 对象在资源实例的 **singleValueExtendedProperties** 集合属性中的 JSON 正文。</span><span class="sxs-lookup"><span data-stu-id="ed687-139">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="ed687-140">属性</span><span class="sxs-lookup"><span data-stu-id="ed687-140">Property</span></span>|<span data-ttu-id="ed687-141">类型</span><span class="sxs-lookup"><span data-stu-id="ed687-141">Type</span></span>|<span data-ttu-id="ed687-142">说明</span><span class="sxs-lookup"><span data-stu-id="ed687-142">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ed687-143">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="ed687-143">singleValueExtendedProperties</span></span>|<span data-ttu-id="ed687-144">[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed687-144">[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection</span></span>| <span data-ttu-id="ed687-145">一个或多个单值扩展属性的数组。</span><span class="sxs-lookup"><span data-stu-id="ed687-145">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="ed687-146">id</span><span class="sxs-lookup"><span data-stu-id="ed687-146">id</span></span>|<span data-ttu-id="ed687-147">String</span><span class="sxs-lookup"><span data-stu-id="ed687-147">String</span></span>|<span data-ttu-id="ed687-p104">对于 **singleValueExtendedProperties** 集合中的每个属性，请指定此参数以标识属性。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="ed687-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="ed687-152">值</span><span class="sxs-lookup"><span data-stu-id="ed687-152">value</span></span>|<span data-ttu-id="ed687-153">string</span><span class="sxs-lookup"><span data-stu-id="ed687-153">string</span></span>|<span data-ttu-id="ed687-p105">对于 **singleValueExtendedProperties** 集合中的每个属性，请指定属性值。必需。</span><span class="sxs-lookup"><span data-stu-id="ed687-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="ed687-156">在_新的_资源实例中创建扩展属性时，除了新的 **singleValueExtendedProperties** 集合，请提供资源实例的 JSON 表示形式（即 [邮件](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md) 等）。</span><span class="sxs-lookup"><span data-stu-id="ed687-156">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="ed687-157">响应</span><span class="sxs-lookup"><span data-stu-id="ed687-157">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="ed687-158">响应代码</span><span class="sxs-lookup"><span data-stu-id="ed687-158">Response code</span></span>
<span data-ttu-id="ed687-159">在新建资源实例中成功创建扩展属性的操作返回 `201 Created`（在新的组帖子中除外），根据所用的方法，该操作可以返回 `200 OK` 或 `202 Accepted`。</span><span class="sxs-lookup"><span data-stu-id="ed687-159">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="ed687-160">在现有的资源实例中，成功的创建操作返回 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="ed687-160">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="ed687-161">响应正文</span><span class="sxs-lookup"><span data-stu-id="ed687-161">Response body</span></span>

<span data-ttu-id="ed687-p106">创建扩展属性时，该响应只包括新建或现有的实例，但不包括新的扩展属性。若要查看新创建的扩展属性，请 [获取通过扩展属性扩展的实例](../api/singlevaluelegacyextendedproperty_get.md)。</span><span class="sxs-lookup"><span data-stu-id="ed687-p106">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

<span data-ttu-id="ed687-164">通过回复线程或帖子在_新建_[组帖子](../resources/post.md)中创建扩展属性时，响应仅包括响应代码，但不包括新帖子或扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ed687-164">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="ed687-165">示例</span><span class="sxs-lookup"><span data-stu-id="ed687-165">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="ed687-166">请求 1</span><span class="sxs-lookup"><span data-stu-id="ed687-166">Request 1</span></span>

<span data-ttu-id="ed687-p107">第一个示例在相同的 POST 操作中创建一个新事件和一个单值扩展属性。除了通常要包括的新事件的属性，请求正文还包括 **singleValueExtendedProperties** 集合，该集合包含一个单值扩展属性和以下属性：</span><span class="sxs-lookup"><span data-stu-id="ed687-p107">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>
- <span data-ttu-id="ed687-169">**id** 将属性类型指定为 `String`、GUID 和名为 `Fun` 的属性。</span><span class="sxs-lookup"><span data-stu-id="ed687-169">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="ed687-170">**value** 将 `Food` 指定为 `Fun` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="ed687-170">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Celebrate Thanksgiving",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together!"
  },
  "start": {
      "dateTime": "2015-11-26T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-26T23:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    }
  ],
  "singleValueExtendedProperties": [
     {
           "id":"String {66f5a359-4659-4830-9070-00040ec6ac6e} Name Fun",
           "value":"Food"
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="ed687-171">响应 1</span><span class="sxs-lookup"><span data-stu-id="ed687-171">Response 1</span></span>

<span data-ttu-id="ed687-p108">成功的响应由 `HTTP 201 Created` 响应代码表示，并在响应正文中包括新事件，类似于 [仅创建事件](../api/user_post_events.md) 中的响应。该响应不包括任何新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ed687-p108">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user_post_events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="ed687-174">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的事件](../api/singlevaluelegacyextendedproperty_get.md)。</span><span class="sxs-lookup"><span data-stu-id="ed687-174">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="ed687-175">请求 2</span><span class="sxs-lookup"><span data-stu-id="ed687-175">Request 2</span></span>

<span data-ttu-id="ed687-p109">第二个示例为指定的现有邮件创建一个单值扩展属性。扩展属性是 **singleValueExtendedProperties** 数组中的唯一元素。请求正文包括扩展属性的以下参数：</span><span class="sxs-lookup"><span data-stu-id="ed687-p109">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="ed687-179">**id** 将属性类型指定为 `String`、GUID 和名为 `Color` 的属性。</span><span class="sxs-lookup"><span data-stu-id="ed687-179">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="ed687-180">**value** 将 `Green` 指定为 `Color` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="ed687-180">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=

Content-Type: application/json

{
  "singleValueExtendedProperties": [
      {
         "id":"String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
         "value":"Green"
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="ed687-181">响应 2</span><span class="sxs-lookup"><span data-stu-id="ed687-181">Response 2</span></span>

<span data-ttu-id="ed687-p110">成功的响应由 `HTTP 200 OK` 响应代码表示，并在响应正文中包括指定的邮件，类似于 [更新邮件](../api/message_update.md) 中的响应。该响应不包括新建的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ed687-p110">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message_update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="ed687-184">若要查看新建的扩展属性，请 [获取通过扩展属性扩展的邮件](../api/singlevaluelegacyextendedproperty_get.md)。</span><span class="sxs-lookup"><span data-stu-id="ed687-184">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

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

