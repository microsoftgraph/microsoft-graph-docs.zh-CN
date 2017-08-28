# <a name="create-open-extension"></a><span data-ttu-id="83bec-101">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="83bec-101">Create open extension</span></span>

<span data-ttu-id="83bec-102">创建开放扩展（[openTypeExtension](../resources/openTypeExtension.md) 对象），并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="83bec-102">Create an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) and add custom properties in a new or existing instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="83bec-103">权限</span><span class="sxs-lookup"><span data-stu-id="83bec-103">Permissions</span></span>

<span data-ttu-id="83bec-p101">若要调用此 API，必须有以下权限之一，具体视要在其中创建扩展的资源而定。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="83bec-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extension in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="83bec-106">**支持的资源**</span><span class="sxs-lookup"><span data-stu-id="83bec-106">**Supported resource**</span></span>|<span data-ttu-id="83bec-107">**权限**</span><span class="sxs-lookup"><span data-stu-id="83bec-107">**Permission**</span></span>|<span data-ttu-id="83bec-108">**支持的资源**</span><span class="sxs-lookup"><span data-stu-id="83bec-108">**Supported resource**</span></span>|<span data-ttu-id="83bec-109">**权限**</span><span class="sxs-lookup"><span data-stu-id="83bec-109">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="83bec-110">设备</span><span class="sxs-lookup"><span data-stu-id="83bec-110">device</span></span>](../resources/device.md) | <span data-ttu-id="83bec-111">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83bec-111">Device.ReadWrite.All</span></span> | [<span data-ttu-id="83bec-112">事件</span><span class="sxs-lookup"><span data-stu-id="83bec-112">event</span></span>](../resources/event.md) | <span data-ttu-id="83bec-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83bec-113">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="83bec-114">组</span><span class="sxs-lookup"><span data-stu-id="83bec-114">group</span></span>](../resources/group.md) | <span data-ttu-id="83bec-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83bec-115">Group.ReadWrite.All</span></span> | [<span data-ttu-id="83bec-116">组事件</span><span class="sxs-lookup"><span data-stu-id="83bec-116">group event</span></span>](../resources/event.md) | <span data-ttu-id="83bec-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83bec-117">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="83bec-118">组帖子</span><span class="sxs-lookup"><span data-stu-id="83bec-118">group post</span></span>](../resources/post.md) | <span data-ttu-id="83bec-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83bec-119">Group.ReadWrite.All</span></span> | [<span data-ttu-id="83bec-120">邮件</span><span class="sxs-lookup"><span data-stu-id="83bec-120">message</span></span>](../resources/message.md) | <span data-ttu-id="83bec-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83bec-121">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="83bec-122">组织</span><span class="sxs-lookup"><span data-stu-id="83bec-122">organization</span></span>](../resources/organization.md) | <span data-ttu-id="83bec-123">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83bec-123">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="83bec-124">个人联系人</span><span class="sxs-lookup"><span data-stu-id="83bec-124">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="83bec-125">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83bec-125">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="83bec-126">用户</span><span class="sxs-lookup"><span data-stu-id="83bec-126">user</span></span>](../resources/user.md) | <span data-ttu-id="83bec-127">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83bec-127">Directory.AccessAsUser.All</span></span> | | |

## <a name="http-request"></a><span data-ttu-id="83bec-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83bec-128">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="83bec-129">在新资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="83bec-129">Create an extension in a new resource instance</span></span>

<span data-ttu-id="83bec-130">使用与创建实例相同的 REST 请求。</span><span class="sxs-lookup"><span data-stu-id="83bec-130">Use the same REST request as creating the instance.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="83bec-p102">**注意：**以上语法显示了一些创建支持的资源实例的常见方法。可以用来创建这些资源实例的所有其他 POST 语法均支持以类似的方式从中创建开放扩展。</span><span class="sxs-lookup"><span data-stu-id="83bec-p102">**Note:** The above syntax shows some common ways to create the supported resource instances. All other POST syntax that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="83bec-133">若要了解如何在请求正文中添加新资源实例和扩展的属性，请参阅[请求正文](#request-body)部分。</span><span class="sxs-lookup"><span data-stu-id="83bec-133">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="83bec-134">在现有资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="83bec-134">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="83bec-135">在请求中标识资源实例，然后对 **extensions** 导航属性执行 `POST`。</span><span class="sxs-lookup"><span data-stu-id="83bec-135">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

><span data-ttu-id="83bec-p103">**注意：**以上语法显示一些标识资源实例的常见方法，以便在其中创建一个扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式在其中创建开放扩展。</span><span class="sxs-lookup"><span data-stu-id="83bec-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to create an extension in it. All other syntax that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="83bec-138">若要了解如何在请求正文中添加扩展，请参阅[请求正文](#request-body)部分。</span><span class="sxs-lookup"><span data-stu-id="83bec-138">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="parameters"></a><span data-ttu-id="83bec-139">参数</span><span class="sxs-lookup"><span data-stu-id="83bec-139">Parameters</span></span>
|<span data-ttu-id="83bec-140">**参数**</span><span class="sxs-lookup"><span data-stu-id="83bec-140">**Parameter**</span></span>|<span data-ttu-id="83bec-141">**类型**</span><span class="sxs-lookup"><span data-stu-id="83bec-141">**Type**</span></span>|<span data-ttu-id="83bec-142">**说明**</span><span class="sxs-lookup"><span data-stu-id="83bec-142">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="83bec-143">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="83bec-143">_URL parameters_</span></span>|
|<span data-ttu-id="83bec-144">id</span><span class="sxs-lookup"><span data-stu-id="83bec-144">id</span></span>|<span data-ttu-id="83bec-145">string</span><span class="sxs-lookup"><span data-stu-id="83bec-145">string</span></span>|<span data-ttu-id="83bec-p104">对象在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="83bec-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="83bec-148">请求标头</span><span class="sxs-lookup"><span data-stu-id="83bec-148">Request headers</span></span>
| <span data-ttu-id="83bec-149">名称</span><span class="sxs-lookup"><span data-stu-id="83bec-149">Name</span></span>       | <span data-ttu-id="83bec-150">值</span><span class="sxs-lookup"><span data-stu-id="83bec-150">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="83bec-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="83bec-151">Authorization</span></span> | <span data-ttu-id="83bec-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83bec-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83bec-154">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83bec-154">Content-Type</span></span> | <span data-ttu-id="83bec-155">application/json</span><span class="sxs-lookup"><span data-stu-id="83bec-155">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="83bec-156">请求正文</span><span class="sxs-lookup"><span data-stu-id="83bec-156">Request body</span></span>

<span data-ttu-id="83bec-p106">提供 [openTypeExtension](../resources/openTypeExtension.md) 的 JSON 正文（具有以下所需的名称-值对）以及其他任意自定义数据。JSON 负载中的数据可以是基元类型或基元类型数组。</span><span class="sxs-lookup"><span data-stu-id="83bec-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="83bec-159">名称</span><span class="sxs-lookup"><span data-stu-id="83bec-159">Name</span></span>       | <span data-ttu-id="83bec-160">值</span><span class="sxs-lookup"><span data-stu-id="83bec-160">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="83bec-161">@odata.type</span><span class="sxs-lookup"><span data-stu-id="83bec-161">@odata.type</span></span> | <span data-ttu-id="83bec-162">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="83bec-162">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="83bec-163">extensionName</span><span class="sxs-lookup"><span data-stu-id="83bec-163">extensionName</span></span> | <span data-ttu-id="83bec-164">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="83bec-164">%unique_string%</span></span> |

<span data-ttu-id="83bec-165">在_新_资源实例中创建扩展插件时，除了新的 **openTypeExtension** 对象之外，还要提供 JSON 表示形式的相关属性才能创建此类资源实例。</span><span class="sxs-lookup"><span data-stu-id="83bec-165">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="83bec-166">响应</span><span class="sxs-lookup"><span data-stu-id="83bec-166">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="83bec-167">响应代码</span><span class="sxs-lookup"><span data-stu-id="83bec-167">Response code</span></span>
<span data-ttu-id="83bec-168">响应代码可以是 `201 Created`，也可以是 `202 Accepted`，具体视操作而定。</span><span class="sxs-lookup"><span data-stu-id="83bec-168">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="83bec-p107">采用与创建资源实例相同的操作创建扩展插件时，操作成功后返回的响应代码与仅通过此操作来创建资源实例（而不创建扩展插件）时返回的一样。请参阅有关创建实例的相应主题，如[上 ](#create-an-extension-in-a-new-resource-instance)所列。</span><span class="sxs-lookup"><span data-stu-id="83bec-p107">When creating an extension in the same operation as creating a resource instance, a successful operation returns the same response code as when the operation is used to create only the resource instance without the extension. Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

#### <a name="response-body"></a><span data-ttu-id="83bec-171">响应正文</span><span class="sxs-lookup"><span data-stu-id="83bec-171">Response body</span></span>
| <span data-ttu-id="83bec-172">应用场景</span><span class="sxs-lookup"><span data-stu-id="83bec-172">Scenario</span></span>       | <span data-ttu-id="83bec-173">资源</span><span class="sxs-lookup"><span data-stu-id="83bec-173">Resource</span></span>  | <span data-ttu-id="83bec-174">响应正文</span><span class="sxs-lookup"><span data-stu-id="83bec-174">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="83bec-175">在显式创建_新_资源实例的同时创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="83bec-175">Creating an extension while explicitly creating a _new_ resource instance</span></span> | [<span data-ttu-id="83bec-176">联系人](../resources/contact.md)、[事件](../resources/event.md)、[邮件</span><span class="sxs-lookup"><span data-stu-id="83bec-176">contact](../resources/contact.md), [event](../resources/event.md), [message</span></span>](../resources/message.md) | <span data-ttu-id="83bec-177">包括使用 [openTypeExtension](../resources/openTypeExtension.md) 对象扩展的新实例。</span><span class="sxs-lookup"><span data-stu-id="83bec-177">Includes the new instance expanded with the [openTypeExtension](../resources/openTypeExtension.md) object.</span></span> |
| <span data-ttu-id="83bec-178">在隐式创建资源实例的同时创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="83bec-178">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="83bec-179">帖子</span><span class="sxs-lookup"><span data-stu-id="83bec-179">post</span></span>](../resources/post.md) | <span data-ttu-id="83bec-180">响应只包括响应代码，不包括响应正文。</span><span class="sxs-lookup"><span data-stu-id="83bec-180">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="83bec-181">在_现有_资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="83bec-181">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="83bec-182">所有支持的资源</span><span class="sxs-lookup"><span data-stu-id="83bec-182">All supported resources</span></span> | <span data-ttu-id="83bec-183">包括 **openTypeExtension** 对象。</span><span class="sxs-lookup"><span data-stu-id="83bec-183">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="83bec-184">示例</span><span class="sxs-lookup"><span data-stu-id="83bec-184">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="83bec-185">请求 1</span><span class="sxs-lookup"><span data-stu-id="83bec-185">Request 1</span></span>

<span data-ttu-id="83bec-p108">第一个示例在同一个调用中创建一个邮件和一个扩展。请求正文包含以下内容：</span><span class="sxs-lookup"><span data-stu-id="83bec-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="83bec-188">新邮件的典型 **subject**、**body** 和 **toRecipients** 属性。</span><span class="sxs-lookup"><span data-stu-id="83bec-188">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span> 
- <span data-ttu-id="83bec-189">对于扩展：</span><span class="sxs-lookup"><span data-stu-id="83bec-189">And for the extension:</span></span>

  - <span data-ttu-id="83bec-190">`Microsoft.Graph.OpenTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="83bec-190">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
  - <span data-ttu-id="83bec-191">扩展名“Com.Contoso.Referral”。</span><span class="sxs-lookup"><span data-stu-id="83bec-191">The extension name "Com.Contoso.Referral".</span></span> 
  - <span data-ttu-id="83bec-192">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `dealValue`。</span><span class="sxs-lookup"><span data-stu-id="83bec-192">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="83bec-193">响应 1</span><span class="sxs-lookup"><span data-stu-id="83bec-193">Response 1</span></span>

<span data-ttu-id="83bec-p109">下面是第一个示例的响应。响应正文包括新邮件的属性以及新扩展的以下属性：</span><span class="sxs-lookup"><span data-stu-id="83bec-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="83bec-196">具有完全限定的名称 `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral` 的 **Id** 属性。</span><span class="sxs-lookup"><span data-stu-id="83bec-196">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span> 
- <span data-ttu-id="83bec-197">请求中指定的默认属性 **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="83bec-197">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="83bec-198">请求中指定的作为 3 个自定义属性存储的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="83bec-198">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="83bec-p110">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83bec-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
      "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```


****

##### <a name="request-2"></a><span data-ttu-id="83bec-201">请求 2</span><span class="sxs-lookup"><span data-stu-id="83bec-201">Request 2</span></span>

<span data-ttu-id="83bec-p111">第二个示例在指定邮件中创建扩展。请求正文包括扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="83bec-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="83bec-204">`Microsoft.Graph.OpenTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="83bec-204">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="83bec-205">扩展名“Com.Contoso.Referral”。</span><span class="sxs-lookup"><span data-stu-id="83bec-205">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="83bec-206">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`dealValue` 和 `expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="83bec-206">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{ 
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension", 
  "extensionName" : "Com.Contoso.Referral", 
  "companyName" : "Wingtip Toys", 
  "dealValue" : 500050, 
  "expirationDate" : "2015-12-03T10:00:00.000Z" 
} 
```

##### <a name="response-2"></a><span data-ttu-id="83bec-207">响应 2</span><span class="sxs-lookup"><span data-stu-id="83bec-207">Response 2</span></span>

<span data-ttu-id="83bec-p112">下面是第二个示例的响应。请求正文包括新扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="83bec-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="83bec-210">默认属性 **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="83bec-210">The default property **extensionName**.</span></span>
- <span data-ttu-id="83bec-211">具有完全限定的名称 `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral` 的 **Id** 属性。</span><span class="sxs-lookup"><span data-stu-id="83bec-211">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span> 
- <span data-ttu-id="83bec-212">要存储的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="83bec-212">The custom data to be stored.</span></span>  

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

##### <a name="request-3"></a><span data-ttu-id="83bec-213">请求 3</span><span class="sxs-lookup"><span data-stu-id="83bec-213">Request 3</span></span>

<span data-ttu-id="83bec-p113">第三个示例在指定组事件中创建扩展。请求正文包括扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="83bec-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="83bec-216">`Microsoft.Graph.OpenTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="83bec-216">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="83bec-217">扩展名“Com.Contoso.Deal”。</span><span class="sxs-lookup"><span data-stu-id="83bec-217">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="83bec-218">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`dealValue` 和 `expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="83bec-218">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions 

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

##### <a name="response-3"></a><span data-ttu-id="83bec-219">响应 3</span><span class="sxs-lookup"><span data-stu-id="83bec-219">Response 3</span></span>

<span data-ttu-id="83bec-220">下面是第三个示例请求的响应。</span><span class="sxs-lookup"><span data-stu-id="83bec-220">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

##### <a name="request-4"></a><span data-ttu-id="83bec-221">请求 4</span><span class="sxs-lookup"><span data-stu-id="83bec-221">Request 4</span></span>

<span data-ttu-id="83bec-p114">第四个示例对现有的组帖子使用相同的 **reply** 操作调用，在新的组帖子中创建扩展。**reply** 操作创建新帖子和嵌入帖子中的新扩展。请求正文包括 **post** 属性，此属性又包含新帖子的 **body** 以及新扩展的以下数据：</span><span class="sxs-lookup"><span data-stu-id="83bec-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="83bec-225">`Microsoft.Graph.OpenTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="83bec-225">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="83bec-226">扩展名“Com.Contoso.HR”。</span><span class="sxs-lookup"><span data-stu-id="83bec-226">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="83bec-227">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `topPicks` 字符串数组。</span><span class="sxs-lookup"><span data-stu-id="83bec-227">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/microsoft.graph.reply 

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]        
  }
}
```

##### <a name="response-4"></a><span data-ttu-id="83bec-228">响应 4</span><span class="sxs-lookup"><span data-stu-id="83bec-228">Response 4</span></span>

<span data-ttu-id="83bec-p115">下面是第四个示例的响应。新的组帖子中成功创建扩展仅会产生 HTTP 202 响应代码。</span><span class="sxs-lookup"><span data-stu-id="83bec-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```


****

##### <a name="request-5"></a><span data-ttu-id="83bec-231">响应 5</span><span class="sxs-lookup"><span data-stu-id="83bec-231">Request 5</span></span>

<span data-ttu-id="83bec-p116">第五个示例使用 POST 操作创建对话，在新的组帖子中创建扩展。POST 操作创建新对话、线程和帖子以及嵌入帖子中的新扩展。请求正文包括 **Topic** 和 **Threads** 属性以及新对话的子 **post** 对象。**post** 对象又包含新帖子的 **body** 和以下扩展数据：</span><span class="sxs-lookup"><span data-stu-id="83bec-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="83bec-236">`Microsoft.Graph.OpenTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="83bec-236">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="83bec-237">扩展名“Com.Contoso.HR”。</span><span class="sxs-lookup"><span data-stu-id="83bec-237">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="83bec-238">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `topPicks` 字符串数组。</span><span class="sxs-lookup"><span data-stu-id="83bec-238">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]  
            }  
          ] 
        } 
      ]  
    } 
  ]
}
```

##### <a name="response-5"></a><span data-ttu-id="83bec-239">响应 5</span><span class="sxs-lookup"><span data-stu-id="83bec-239">Response 5</span></span>

<span data-ttu-id="83bec-p117">下面是第五个示例的响应，其中包含新对话和线程 ID。这个新线程包含自动创建的帖子，帖子又包含新扩展。</span><span class="sxs-lookup"><span data-stu-id="83bec-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span> 

<span data-ttu-id="83bec-p118">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83bec-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="83bec-p119">若要获取新扩展，首先 [获取此线程中的所有帖子](../api/conversationthread_list_posts.md)，线程中最初应该只有一个帖子。然后应用帖子 ID 和扩展名 `Com.Contoso.Benefits` 以[获取扩展](../api/opentypeextension_get.md)。</span><span class="sxs-lookup"><span data-stu-id="83bec-p119">To get the new extension, first [get all the posts](../api/conversationthread_list_posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension_get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
