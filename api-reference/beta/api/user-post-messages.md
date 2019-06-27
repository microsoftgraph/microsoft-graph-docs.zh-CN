---
title: 创建邮件
description: 使用此 API 创建新邮件的草稿。可以在任意文件夹中创建草稿，也可以在发送前更新草稿。若要将邮件保存到“草稿”文件夹，请使用 /messages 快捷方式。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f3157977ee66aab36eef55dec50c7ea387936ce
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269970"
---
# <a name="create-message"></a><span data-ttu-id="7bef0-105">创建邮件</span><span class="sxs-lookup"><span data-stu-id="7bef0-105">Create Message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bef0-p102">使用此 API 创建新邮件的草稿。可以在任意文件夹中创建草稿，也可以在发送前更新草稿。若要将邮件保存到“草稿”文件夹，请使用 /messages 快捷方式。</span><span class="sxs-lookup"><span data-stu-id="7bef0-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="7bef0-109">在同一个**POST**调用中创建草稿时, 可以执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="7bef0-109">While creating the draft in the same **POST** call, you can:</span></span>

- <span data-ttu-id="7bef0-110">包含[附件](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="7bef0-110">Include an [attachment](../resources/attachment.md)</span></span> 
- <span data-ttu-id="7bef0-111">在新邮件中使用[提及](../resources/mention.md)调用其他用户</span><span class="sxs-lookup"><span data-stu-id="7bef0-111">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="7bef0-112">权限</span><span class="sxs-lookup"><span data-stu-id="7bef0-112">Permissions</span></span>
<span data-ttu-id="7bef0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7bef0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bef0-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="7bef0-115">Permission type</span></span>      | <span data-ttu-id="7bef0-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7bef0-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bef0-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7bef0-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7bef0-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bef0-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7bef0-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7bef0-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bef0-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bef0-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7bef0-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="7bef0-121">Application</span></span> | <span data-ttu-id="7bef0-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bef0-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bef0-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bef0-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="7bef0-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bef0-124">Request headers</span></span>
| <span data-ttu-id="7bef0-125">标头</span><span class="sxs-lookup"><span data-stu-id="7bef0-125">Header</span></span>       | <span data-ttu-id="7bef0-126">值</span><span class="sxs-lookup"><span data-stu-id="7bef0-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7bef0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bef0-127">Authorization</span></span>  | <span data-ttu-id="7bef0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7bef0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7bef0-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bef0-130">Content-Type</span></span>  | <span data-ttu-id="7bef0-131">application/json</span><span class="sxs-lookup"><span data-stu-id="7bef0-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7bef0-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bef0-132">Request body</span></span>
<span data-ttu-id="7bef0-133">在请求正文中, 提供[message](../resources/message.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bef0-133">In the request body, supply a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="7bef0-134">如果要使用**提及**在新邮件中呼叫其他用户, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="7bef0-134">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="7bef0-135">在请求正文中包括所需的**toRecipients**属性、**提及**属性和任何可写邮件属性。</span><span class="sxs-lookup"><span data-stu-id="7bef0-135">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="7bef0-136">对于**提及**属性中的每个提及, 您必须指定**提到**的属性。</span><span class="sxs-lookup"><span data-stu-id="7bef0-136">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="7bef0-137">由于**邮件**资源支持[扩展](/graph/extensibility-overview)因此可以使用 `POST` 操作，并在创建邮件时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="7bef0-137">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="7bef0-138">响应</span><span class="sxs-lookup"><span data-stu-id="7bef0-138">Response</span></span>

<span data-ttu-id="7bef0-139">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[message](../resources/message.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7bef0-139">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bef0-140">示例</span><span class="sxs-lookup"><span data-stu-id="7bef0-140">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="7bef0-141">请求 1</span><span class="sxs-lookup"><span data-stu-id="7bef0-141">Request 1</span></span>
<span data-ttu-id="7bef0-142">下面的示例展示了创建新邮件草稿的请求。</span><span class="sxs-lookup"><span data-stu-id="7bef0-142">Here is an example of the request to create a draft of a new message.</span></span>
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
<span data-ttu-id="7bef0-143">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bef0-143">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="7bef0-144">响应 1</span><span class="sxs-lookup"><span data-stu-id="7bef0-144">Response 1</span></span>
<span data-ttu-id="7bef0-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7bef0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7bef0-148">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7bef0-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7bef0-149">C#</span><span class="sxs-lookup"><span data-stu-id="7bef0-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bef0-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bef0-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7bef0-151">目标-C</span><span class="sxs-lookup"><span data-stu-id="7bef0-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_message_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="7bef0-152">请求 2</span><span class="sxs-lookup"><span data-stu-id="7bef0-152">Request 2</span></span>
<span data-ttu-id="7bef0-153">下一个示例显示了通过 Randi Welch 到 Samantha 展台的草稿电子邮件。</span><span class="sxs-lookup"><span data-stu-id="7bef0-153">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="7bef0-154">此外, 该消息还包括其他用户 Dana Swope。</span><span class="sxs-lookup"><span data-stu-id="7bef0-154">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="7bef0-155">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bef0-155">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
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


##### <a name="response-2"></a><span data-ttu-id="7bef0-156">响应 2</span><span class="sxs-lookup"><span data-stu-id="7bef0-156">Response 2</span></span>
<span data-ttu-id="7bef0-p107">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7bef0-p107">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7bef0-160">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7bef0-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7bef0-161">C#</span><span class="sxs-lookup"><span data-stu-id="7bef0-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_with_mentions_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bef0-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bef0-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_with_mentions_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7bef0-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="7bef0-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_message_with_mentions_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-3"></a><span data-ttu-id="7bef0-164">请求 3</span><span class="sxs-lookup"><span data-stu-id="7bef0-164">Request 3</span></span>
<span data-ttu-id="7bef0-165">下一个示例在创建邮件草稿时添加了几个客户 Internet 邮件头。</span><span class="sxs-lookup"><span data-stu-id="7bef0-165">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
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
<span data-ttu-id="7bef0-166">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bef0-166">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="7bef0-167">响应 3</span><span class="sxs-lookup"><span data-stu-id="7bef0-167">Response 3</span></span>
<span data-ttu-id="7bef0-168">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7bef0-168">Here is an example of the response.</span></span> <span data-ttu-id="7bef0-169">注意：默认情况下，POST 响应中不会返回 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="7bef0-169">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="7bef0-170">为简洁起见，也可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7bef0-170">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="7bef0-171">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7bef0-171">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7bef0-172">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7bef0-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7bef0-173">C#</span><span class="sxs-lookup"><span data-stu-id="7bef0-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_with_headers_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bef0-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bef0-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_with_headers_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7bef0-175">目标-C</span><span class="sxs-lookup"><span data-stu-id="7bef0-175">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_message_with_headers_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="7bef0-176">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7bef0-176">See also</span></span>

- [<span data-ttu-id="7bef0-177">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="7bef0-177">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7bef0-178">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="7bef0-178">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7bef0-179">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="7bef0-179">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
