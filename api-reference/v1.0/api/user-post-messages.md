---
title: 创建邮件
description: 使用此 API 创建新邮件的草稿。可以在任意文件夹中创建草稿，也可以在发送前更新草稿。若要将邮件保存到“草稿”文件夹，请使用 /messages 快捷方式。
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b2776e4708c6a5a72ee2f9c612f05f5f093b196f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054292"
---
# <a name="create-message"></a><span data-ttu-id="01e0b-105">创建邮件</span><span class="sxs-lookup"><span data-stu-id="01e0b-105">Create Message</span></span>

<span data-ttu-id="01e0b-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01e0b-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="01e0b-p102">使用此 API 创建新邮件的草稿。可以在任意文件夹中创建草稿，也可以在发送前更新草稿。若要将邮件保存到“草稿”文件夹，请使用 /messages 快捷方式。</span><span class="sxs-lookup"><span data-stu-id="01e0b-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="01e0b-110">在同一个 **POST** 调用中创建草稿时，可以添加 [附件](../resources/attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="01e0b-110">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="01e0b-111">权限</span><span class="sxs-lookup"><span data-stu-id="01e0b-111">Permissions</span></span>
<span data-ttu-id="01e0b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01e0b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01e0b-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="01e0b-114">Permission type</span></span>      | <span data-ttu-id="01e0b-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01e0b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01e0b-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01e0b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="01e0b-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01e0b-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="01e0b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01e0b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01e0b-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01e0b-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="01e0b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="01e0b-120">Application</span></span> | <span data-ttu-id="01e0b-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01e0b-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="01e0b-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01e0b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="01e0b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="01e0b-123">Request headers</span></span>
| <span data-ttu-id="01e0b-124">标头</span><span class="sxs-lookup"><span data-stu-id="01e0b-124">Header</span></span>       | <span data-ttu-id="01e0b-125">值</span><span class="sxs-lookup"><span data-stu-id="01e0b-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01e0b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="01e0b-126">Authorization</span></span>  | <span data-ttu-id="01e0b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01e0b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01e0b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01e0b-129">Content-Type</span></span>  | <span data-ttu-id="01e0b-130">application/json</span><span class="sxs-lookup"><span data-stu-id="01e0b-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01e0b-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="01e0b-131">Request body</span></span>
<span data-ttu-id="01e0b-132">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01e0b-132">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="01e0b-133">由于 **邮件** 资源支持 [扩展](/graph/extensibility-overview)因此可以使用 `POST` 操作，并在创建邮件时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="01e0b-133">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="01e0b-134">响应</span><span class="sxs-lookup"><span data-stu-id="01e0b-134">Response</span></span>

<span data-ttu-id="01e0b-135">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01e0b-135">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01e0b-136">示例</span><span class="sxs-lookup"><span data-stu-id="01e0b-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="01e0b-137">请求 1</span><span class="sxs-lookup"><span data-stu-id="01e0b-137">Request 1</span></span>
<span data-ttu-id="01e0b-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01e0b-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01e0b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="01e0b-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="01e0b-140">C#</span><span class="sxs-lookup"><span data-stu-id="01e0b-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01e0b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01e0b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01e0b-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01e0b-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01e0b-143">Java</span><span class="sxs-lookup"><span data-stu-id="01e0b-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="01e0b-144">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01e0b-144">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="01e0b-145">响应 1</span><span class="sxs-lookup"><span data-stu-id="01e0b-145">Response 1</span></span>
<span data-ttu-id="01e0b-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="01e0b-146">Here is an example of the response.</span></span> <span data-ttu-id="01e0b-147">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="01e0b-147">Note: The response object shown here might be shortened for readability.</span></span>
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
    "conversationIndex":"AQHTe7/VAniOJVgCxEmtF1z6ZY1rFQ==",
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

##### <a name="request-2"></a><span data-ttu-id="01e0b-148">请求 2</span><span class="sxs-lookup"><span data-stu-id="01e0b-148">Request 2</span></span>
<span data-ttu-id="01e0b-149">下一个示例在创建邮件草稿时添加了几个客户 Internet 邮件头。</span><span class="sxs-lookup"><span data-stu-id="01e0b-149">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>

# <a name="http"></a>[<span data-ttu-id="01e0b-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="01e0b-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="01e0b-151">C#</span><span class="sxs-lookup"><span data-stu-id="01e0b-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-headers-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01e0b-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01e0b-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-headers-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01e0b-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01e0b-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-headers-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01e0b-154">Java</span><span class="sxs-lookup"><span data-stu-id="01e0b-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-headers-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="01e0b-155">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01e0b-155">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="01e0b-156">响应 2</span><span class="sxs-lookup"><span data-stu-id="01e0b-156">Response 2</span></span>
<span data-ttu-id="01e0b-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="01e0b-157">Here is an example of the response.</span></span> <span data-ttu-id="01e0b-158">注意：默认情况下，POST 响应中不会返回 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="01e0b-158">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="01e0b-159">为简洁起见，也可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="01e0b-159">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="01e0b-160">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="01e0b-160">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="01e0b-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="01e0b-161">See also</span></span>

- [<span data-ttu-id="01e0b-162">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="01e0b-162">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="01e0b-163">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="01e0b-163">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
  ]
}-->

