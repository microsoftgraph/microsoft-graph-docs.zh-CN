# <a name="get-message"></a><span data-ttu-id="9481f-101">获取邮件</span><span class="sxs-lookup"><span data-stu-id="9481f-101">Get message</span></span>

<span data-ttu-id="9481f-102">检索[邮件](../resources/message.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9481f-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="9481f-103">目前，此操作返回纯 HTML 格式的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="9481f-103">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="9481f-104">有两种应用可以在另一个用户的邮件文件夹中获取邮件的情景：</span><span class="sxs-lookup"><span data-stu-id="9481f-104">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="9481f-105">如果应用拥有应用程序权限，或者，</span><span class="sxs-lookup"><span data-stu-id="9481f-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="9481f-106">如果应用拥有来自一个用户的适当的委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已授予该用户委派访问权限。</span><span class="sxs-lookup"><span data-stu-id="9481f-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="9481f-107">请参阅[详细信息和示例](../../../concepts/outlook-share-messages-folders.md)。</span><span class="sxs-lookup"><span data-stu-id="9481f-107">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>

<span data-ttu-id="9481f-108">由于**邮件**资源支持[扩展](../../../concepts/extensibility_overview.md)，因此也可使用 `GET` 操作获取**邮件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="9481f-108">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="9481f-109">权限</span><span class="sxs-lookup"><span data-stu-id="9481f-109">Permissions</span></span>
<span data-ttu-id="9481f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9481f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9481f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="9481f-112">Permission type</span></span>      | <span data-ttu-id="9481f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9481f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9481f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9481f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9481f-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9481f-115">Mail.Read</span></span>    |
|<span data-ttu-id="9481f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9481f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9481f-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9481f-117">Mail.Read</span></span>    |
|<span data-ttu-id="9481f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="9481f-118">Application</span></span> | <span data-ttu-id="9481f-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9481f-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="9481f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9481f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9481f-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9481f-121">Optional query parameters</span></span>
<span data-ttu-id="9481f-122">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9481f-122">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9481f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="9481f-123">Request headers</span></span>
| <span data-ttu-id="9481f-124">名称</span><span class="sxs-lookup"><span data-stu-id="9481f-124">Name</span></span>       | <span data-ttu-id="9481f-125">类型</span><span class="sxs-lookup"><span data-stu-id="9481f-125">Type</span></span> | <span data-ttu-id="9481f-126">说明</span><span class="sxs-lookup"><span data-stu-id="9481f-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9481f-127">授权</span><span class="sxs-lookup"><span data-stu-id="9481f-127">Authorization</span></span>  | <span data-ttu-id="9481f-128">字符串</span><span class="sxs-lookup"><span data-stu-id="9481f-128">string</span></span>  | <span data-ttu-id="9481f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9481f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9481f-131">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="9481f-131">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="9481f-132">字符串</span><span class="sxs-lookup"><span data-stu-id="9481f-132">string</span></span> | <span data-ttu-id="9481f-133">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="9481f-133">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="9481f-134">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="9481f-134">Values can be "text" or "html".</span></span> <span data-ttu-id="9481f-135">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="9481f-135">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="9481f-136">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="9481f-136">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="9481f-137">可选。</span><span class="sxs-lookup"><span data-stu-id="9481f-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9481f-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="9481f-138">Request body</span></span>
<span data-ttu-id="9481f-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9481f-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9481f-140">响应</span><span class="sxs-lookup"><span data-stu-id="9481f-140">Response</span></span>

<span data-ttu-id="9481f-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9481f-141">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9481f-142">示例</span><span class="sxs-lookup"><span data-stu-id="9481f-142">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="9481f-143">请求 1</span><span class="sxs-lookup"><span data-stu-id="9481f-143">Request 1</span></span>
<span data-ttu-id="9481f-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9481f-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="9481f-145">响应 1</span><span class="sxs-lookup"><span data-stu-id="9481f-145">Response 1</span></span>
<span data-ttu-id="9481f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9481f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ\"",
    "id":"AAMkADhMGAAA=",
    "createdDateTime":"2018-09-09T03:15:05Z",
    "lastModifiedDateTime":"2018-09-09T03:15:08Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T03:15:08Z",
    "sentDateTime":"2018-09-09T03:15:06Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR6E1BE060@MWHPR1120.namprd22.prod.outlook.com>",
    "subject":"9/9/2018: concert",
    "bodyPreview":"The group represents Nevada.",
    "importance":"normal",
    "parentFolderId":"AAMkADcbAAAAAAEJAAA=",
    "conversationId":"AAQkADOUpag6yWs=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADMGAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Nevada.\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="9481f-149">请求 2</span><span class="sxs-lookup"><span data-stu-id="9481f-149">Request 2</span></span>
<span data-ttu-id="9481f-150">下面的示例使用 `$select` 查询参数来获取邮件的的 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="9481f-150">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="9481f-151">响应 2</span><span class="sxs-lookup"><span data-stu-id="9481f-151">Response 2</span></span>
<span data-ttu-id="9481f-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9481f-152">Here is an example of the response.</span></span> <span data-ttu-id="9481f-153">注意：为简便起见，响应对象中的邮件标头集有所删减。</span><span class="sxs-lookup"><span data-stu-id="9481f-153">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="9481f-154">实际调用将返回所有标头。</span><span class="sxs-lookup"><span data-stu-id="9481f-154">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages(internetMessageHeaders)/$entity",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "internetMessageHeaders":[
        {
            "name":"MIME-Version",
            "value":"1.0"
        },
        {
            "name":"Content-Type",
            "value":"multipart/report"
        },
        {
            "name":"x-custom-header-group-name",
            "value":"Washington"
        },
        {
            "name":"x-custom-header-group-id",
            "value":"WA001"
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="9481f-155">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9481f-155">See also</span></span>

- [<span data-ttu-id="9481f-156">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="9481f-156">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="9481f-157">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="9481f-157">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
