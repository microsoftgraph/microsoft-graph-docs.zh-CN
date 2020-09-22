---
title: 创建邮件
description: 使用此 API 创建新邮件的草稿。可以在任意文件夹中创建草稿，也可以在发送前更新草稿。若要将邮件保存到“草稿”文件夹，请使用 /messages 快捷方式。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0ee34bf4cf4a7f3f654dd86ce618fc4945a5b9c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087738"
---
# <a name="create-message"></a><span data-ttu-id="95332-105">创建邮件</span><span class="sxs-lookup"><span data-stu-id="95332-105">Create Message</span></span>

<span data-ttu-id="95332-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95332-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95332-p102">使用此 API 创建新邮件的草稿。可以在任意文件夹中创建草稿，也可以在发送前更新草稿。若要将邮件保存到“草稿”文件夹，请使用 /messages 快捷方式。</span><span class="sxs-lookup"><span data-stu-id="95332-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="95332-110">在同一个 **POST** 调用中创建草稿时，可以执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="95332-110">While creating the draft in the same **POST** call, you can:</span></span>

- <span data-ttu-id="95332-111">包含 [附件](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="95332-111">Include an [attachment](../resources/attachment.md)</span></span> 
- <span data-ttu-id="95332-112">在新邮件中使用 [提及](../resources/mention.md) 调用其他用户</span><span class="sxs-lookup"><span data-stu-id="95332-112">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="95332-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="95332-113">Permissions</span></span>
<span data-ttu-id="95332-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95332-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95332-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="95332-116">Permission type</span></span>      | <span data-ttu-id="95332-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="95332-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95332-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95332-118">Delegated (work or school account)</span></span> | <span data-ttu-id="95332-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95332-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="95332-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95332-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95332-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95332-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="95332-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="95332-122">Application</span></span> | <span data-ttu-id="95332-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95332-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="95332-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95332-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="95332-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="95332-125">Request headers</span></span>
| <span data-ttu-id="95332-126">标头</span><span class="sxs-lookup"><span data-stu-id="95332-126">Header</span></span>       | <span data-ttu-id="95332-127">值</span><span class="sxs-lookup"><span data-stu-id="95332-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95332-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="95332-128">Authorization</span></span>  | <span data-ttu-id="95332-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="95332-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="95332-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95332-131">Content-Type</span></span>  | <span data-ttu-id="95332-132">application/json</span><span class="sxs-lookup"><span data-stu-id="95332-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95332-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="95332-133">Request body</span></span>
<span data-ttu-id="95332-134">在请求正文中，提供 [message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95332-134">In the request body, supply a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="95332-135">如果要使用 **提及** 在新邮件中呼叫其他用户，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="95332-135">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="95332-136">在请求正文中包括所需的 **toRecipients** 属性、 **提及** 属性和任何可写邮件属性。</span><span class="sxs-lookup"><span data-stu-id="95332-136">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="95332-137">对于 **提及** 属性中的每个提及，您必须指定 **提到** 的属性。</span><span class="sxs-lookup"><span data-stu-id="95332-137">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="95332-138">由于**邮件**资源支持[扩展](/graph/extensibility-overview)因此可以使用 `POST` 操作，并在创建邮件时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="95332-138">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="95332-139">响应</span><span class="sxs-lookup"><span data-stu-id="95332-139">Response</span></span>

<span data-ttu-id="95332-140">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95332-140">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95332-141">示例</span><span class="sxs-lookup"><span data-stu-id="95332-141">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="95332-142">请求 1</span><span class="sxs-lookup"><span data-stu-id="95332-142">Request 1</span></span>
<span data-ttu-id="95332-143">下面的示例展示了创建新邮件草稿的请求。</span><span class="sxs-lookup"><span data-stu-id="95332-143">Here is an example of the request to create a draft of a new message.</span></span>

# <a name="http"></a>[<span data-ttu-id="95332-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="95332-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject":"Did you see last night's game?",
    "importance":"Low",
    "body":{
        "contentType":"HTML",
        "content":"They were <b>awesome</b>!"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="95332-145">C#</span><span class="sxs-lookup"><span data-stu-id="95332-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95332-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95332-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95332-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95332-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="95332-148">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95332-148">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="95332-149">响应 1</span><span class="sxs-lookup"><span data-stu-id="95332-149">Response 1</span></span>
<span data-ttu-id="95332-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95332-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('ad787b4f-1fda-4523-8e48-ffedb7f4635f')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t\"",
    "id":"AAMkAGRWAAAFSmKXAAA=",
    "createdDateTime":"2017-12-23T07:29:57Z",
    "lastModifiedDateTime":"2017-12-23T07:29:58Z",
    "changeKey":"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t",
    "categories":[

    ],
    "receivedDateTime":"2017-12-23T07:29:58Z",
    "sentDateTime":"2017-12-23T07:29:58Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR130@MWHPR130.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkAGRWAAAAAAEPAAA=",
    "conversationId":"AAQkAGRVYAsRJrRdc_mWNaxU=",
    "conversationIndex":"AQHTe7/VAniOJVgCxEmtF1z6ZY1rFQ==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkAGRWAAAFSmKXAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"AdeleV@contoso.onmicrosoft.com",
                "address":"AdeleV@contoso.onmicrosoft.com"
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

##### <a name="request-2"></a><span data-ttu-id="95332-153">请求 2</span><span class="sxs-lookup"><span data-stu-id="95332-153">Request 2</span></span>
<span data-ttu-id="95332-154">下一个示例显示了通过 Randi Welch 到 Samantha 展台的草稿电子邮件。</span><span class="sxs-lookup"><span data-stu-id="95332-154">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="95332-155">此外，该消息还包括其他用户 Dana Swope。</span><span class="sxs-lookup"><span data-stu-id="95332-155">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="95332-156">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95332-156">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="95332-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="95332-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_with_mentions_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject": "Party planning",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {    
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="95332-158">C#</span><span class="sxs-lookup"><span data-stu-id="95332-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-mentions-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95332-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95332-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-mentions-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95332-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95332-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-mentions-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response-2"></a><span data-ttu-id="95332-161">响应 2</span><span class="sxs-lookup"><span data-stu-id="95332-161">Response 2</span></span>
<span data-ttu-id="95332-p107">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95332-p107">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/Messages/$entity",
  "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')",
  "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAbYj7\"",
  "id":"AQMkADJmMTUAAAW1fsAAAAA==",
  "body":{
    "contentType":"Text",
    "content":""
  },
  "bodyPreview":"",
  "sender":null,
  "from":null,
  "subject": "Party planning",
  "toRecipients":[
    {
      "emailAddress":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      }
    }
  ],
  "mentionsPreview":{
    "isMentioned":false
  },
  "mentions@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages('AQMkADJmMTUAAAW1fsAAAAA%3D%3D')/mentions",
  "mentions":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')/mentions('4577bba4-b063-4cea-9073-6f7ca815fcec')",
      "id":"4577bba4-b063-4cea-9073-6f7ca815fcec",
      "mentioned":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-22T02:22:44Z",
      "serverCreatedDateTime":"2016-07-22T02:22:44.201Z",
      "deepLink":null,
      "application":null
    }
  ]
}

```

##### <a name="request-3"></a><span data-ttu-id="95332-165">请求 3</span><span class="sxs-lookup"><span data-stu-id="95332-165">Request 3</span></span>
<span data-ttu-id="95332-166">下一个示例在创建邮件草稿时添加了几个客户 Internet 邮件头。</span><span class="sxs-lookup"><span data-stu-id="95332-166">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>

# <a name="http"></a>[<span data-ttu-id="95332-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="95332-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject":"9/8/2018: concert",
    "body":{
        "contentType":"HTML",
        "content":"The group represents Washington."
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "internetMessageHeaders":[
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
# <a name="c"></a>[<span data-ttu-id="95332-168">C#</span><span class="sxs-lookup"><span data-stu-id="95332-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-headers-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95332-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95332-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-headers-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95332-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95332-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-headers-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="95332-171">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95332-171">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="95332-172">响应 3</span><span class="sxs-lookup"><span data-stu-id="95332-172">Response 3</span></span>
<span data-ttu-id="95332-173">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="95332-173">Here is an example of the response.</span></span> <span data-ttu-id="95332-174">注意：默认情况下，POST 响应中不会返回 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="95332-174">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="95332-175">为简洁起见，也可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="95332-175">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="95332-176">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="95332-176">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_with_headers_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE\"",
    "id":"AAMkADhNmAAA=",
    "createdDateTime":"2018-09-09T02:54:56Z",
    "lastModifiedDateTime":"2018-09-09T02:54:56Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T02:54:56Z",
    "sentDateTime":"2018-09-09T02:54:56Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR220MB1120.namprd22.prod.outlook.com>",
    "subject":"9/8/2018: concert",
    "bodyPreview":"The group represents Washington.",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEPAAA=",
    "conversationId":"AAQkADhNCuP8OKSm-0NE=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhNmAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Washington.\r\n</body>\r\n</html>\r\n"
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

## <a name="see-also"></a><span data-ttu-id="95332-177">另请参阅</span><span class="sxs-lookup"><span data-stu-id="95332-177">See also</span></span>

- [<span data-ttu-id="95332-178">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="95332-178">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="95332-179">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="95332-179">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="95332-180">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="95332-180">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


