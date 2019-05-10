---
title: 创建邮件
description: 使用此 API 创建新邮件的草稿。可以在任意文件夹中创建草稿，也可以在发送前更新草稿。若要将邮件保存到“草稿”文件夹，请使用 /messages 快捷方式。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1662617500133e3aca52f990f37f4d3fe72bbd86
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33600956"
---
# <a name="create-message"></a><span data-ttu-id="c06a8-105">创建邮件</span><span class="sxs-lookup"><span data-stu-id="c06a8-105">Create Message</span></span>

<span data-ttu-id="c06a8-p102">使用此 API 创建新邮件的草稿。可以在任意文件夹中创建草稿，也可以在发送前更新草稿。若要将邮件保存到“草稿”文件夹，请使用 /messages 快捷方式。</span><span class="sxs-lookup"><span data-stu-id="c06a8-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="c06a8-109">在同一个 **POST** 调用中创建草稿时，可以添加[附件](../resources/attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="c06a8-109">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c06a8-110">权限</span><span class="sxs-lookup"><span data-stu-id="c06a8-110">Permissions</span></span>
<span data-ttu-id="c06a8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c06a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c06a8-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c06a8-113">Permission type</span></span>      | <span data-ttu-id="c06a8-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c06a8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c06a8-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c06a8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c06a8-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c06a8-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c06a8-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c06a8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c06a8-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c06a8-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c06a8-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c06a8-119">Application</span></span> | <span data-ttu-id="c06a8-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c06a8-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c06a8-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c06a8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="c06a8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c06a8-122">Request headers</span></span>
| <span data-ttu-id="c06a8-123">标头</span><span class="sxs-lookup"><span data-stu-id="c06a8-123">Header</span></span>       | <span data-ttu-id="c06a8-124">值</span><span class="sxs-lookup"><span data-stu-id="c06a8-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c06a8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c06a8-125">Authorization</span></span>  | <span data-ttu-id="c06a8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c06a8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c06a8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c06a8-128">Content-Type</span></span>  | <span data-ttu-id="c06a8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c06a8-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c06a8-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c06a8-130">Request body</span></span>
<span data-ttu-id="c06a8-131">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c06a8-131">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="c06a8-132">由于**邮件**资源支持[扩展](/graph/extensibility-overview)因此可以使用 `POST` 操作，并在创建邮件时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="c06a8-132">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="c06a8-133">响应</span><span class="sxs-lookup"><span data-stu-id="c06a8-133">Response</span></span>

<span data-ttu-id="c06a8-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c06a8-134">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c06a8-135">示例</span><span class="sxs-lookup"><span data-stu-id="c06a8-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c06a8-136">请求 1</span><span class="sxs-lookup"><span data-stu-id="c06a8-136">Request 1</span></span>
<span data-ttu-id="c06a8-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c06a8-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
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
<span data-ttu-id="c06a8-138">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c06a8-138">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="c06a8-139">响应 1</span><span class="sxs-lookup"><span data-stu-id="c06a8-139">Response 1</span></span>
<span data-ttu-id="c06a8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c06a8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti\"",
    "id":"AAMkADNlNYjSAAA=",
    "createdDateTime":"2017-07-22T01:53:56Z",
    "lastModifiedDateTime":"2017-07-22T01:53:57Z",
    "changeKey":"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti",
    "categories":[

    ],
    "receivedDateTime":"2017-07-22T01:53:57Z",
    "sentDateTime":"2017-07-22T01:53:57Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB@MWHPR1301MB.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkADNlNWAAAAAAEPAAA=",
    "conversationId":"AAQkADNlNFdXGBnqtY=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADNlNYjSAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c06a8-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c06a8-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c06a8-144">C#</span><span class="sxs-lookup"><span data-stu-id="c06a8-144">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c06a8-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="c06a8-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_from_user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="c06a8-146">请求 2</span><span class="sxs-lookup"><span data-stu-id="c06a8-146">Request 2</span></span>
<span data-ttu-id="c06a8-147">下一个示例在创建邮件草稿时添加了几个客户 Internet 邮件头。</span><span class="sxs-lookup"><span data-stu-id="c06a8-147">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
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
<span data-ttu-id="c06a8-148">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c06a8-148">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="c06a8-149">响应 2</span><span class="sxs-lookup"><span data-stu-id="c06a8-149">Response 2</span></span>
<span data-ttu-id="c06a8-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c06a8-150">Here is an example of the response.</span></span> <span data-ttu-id="c06a8-151">注意：默认情况下，POST 响应中不会返回 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="c06a8-151">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="c06a8-152">为简洁起见，也可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c06a8-152">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="c06a8-153">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c06a8-153">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c06a8-154">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c06a8-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c06a8-155">C#</span><span class="sxs-lookup"><span data-stu-id="c06a8-155">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_with_headers_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c06a8-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="c06a8-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_with_headers_from_user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="c06a8-157">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c06a8-157">See also</span></span>

- [<span data-ttu-id="c06a8-158">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c06a8-158">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c06a8-159">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="c06a8-159">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
