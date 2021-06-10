---
title: 创建邮件
description: 采用 JSON 或 MIME 格式创建新邮件的草稿。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4305a14ba2726102427c4f0b4c733656be2fd03b
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868908"
---
# <a name="create-message"></a><span data-ttu-id="a2a89-103">创建邮件</span><span class="sxs-lookup"><span data-stu-id="a2a89-103">Create Message</span></span>

<span data-ttu-id="a2a89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2a89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2a89-105">采用 JSON 或 MIME 格式创建新邮件的草稿。</span><span class="sxs-lookup"><span data-stu-id="a2a89-105">Create a draft of a new message in either JSON or MIME format.</span></span>

<span data-ttu-id="a2a89-106">使用 JSON 格式时，可以：</span><span class="sxs-lookup"><span data-stu-id="a2a89-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="a2a89-107">包括附件[](../resources/attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="a2a89-107">Include an [attachment](../resources/attachment.md).</span></span>
- <span data-ttu-id="a2a89-108">使用 [提及](../resources/mention.md) 功能在新邮件中呼叫其他用户。</span><span class="sxs-lookup"><span data-stu-id="a2a89-108">Use a [mention](../resources/mention.md) to call out another user in the new message.</span></span>
- <span data-ttu-id="a2a89-109">随后 [更新](../api/message-update.md)草稿以将内容添加到 **正文**，或更改其他邮件属性。</span><span class="sxs-lookup"><span data-stu-id="a2a89-109">[Update](../api/message-update.md) the draft later to add content to the **body** or change other message properties.</span></span>

<span data-ttu-id="a2a89-110">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="a2a89-110">When using MIME format:</span></span>
- <span data-ttu-id="a2a89-111">提供适用的 [Internet 邮件头](https://tools.ietf.org/html/rfc2076) 和 [MIME 内容](https://tools.ietf.org/html/rfc2045)，所有内容在请求正文中都通过 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="a2a89-111">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="a2a89-112">向 MIME 内容添加任何附件和 S/MIME 属性。</span><span class="sxs-lookup"><span data-stu-id="a2a89-112">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="a2a89-113">默认情况下，此操作将草稿保存在“草稿”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="a2a89-113">By default, this operation saves the draft in the Drafts folder.</span></span>

<span data-ttu-id="a2a89-114">在后续操作中[发送](/graph/api-reference/beta/api/message-send.md)草稿消息。</span><span class="sxs-lookup"><span data-stu-id="a2a89-114">[Send](/graph/api-reference/beta/api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="a2a89-115">或者，[在单个操作中](../api/user-sendmail.md)发送新邮件，或创建转发草稿，以[](../api/message-createforward.md)[答复](../api/message-createreply.md)或[全部](../api/message-createreplyall.md)答复现有邮件。</span><span class="sxs-lookup"><span data-stu-id="a2a89-115">Alternatively, [send a new message](../api/user-sendmail.md) in a single action, or create a draft [to forward](../api/message-createforward.md), [to reply](../api/message-createreply.md) or [to reply-all](../api/message-createreplyall.md) to an existing message.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2a89-116">权限</span><span class="sxs-lookup"><span data-stu-id="a2a89-116">Permissions</span></span>
<span data-ttu-id="a2a89-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2a89-p101">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2a89-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2a89-119">Permission type</span></span>      | <span data-ttu-id="a2a89-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2a89-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2a89-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2a89-121">Delegated (work or school account)</span></span> | <span data-ttu-id="a2a89-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2a89-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a2a89-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2a89-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2a89-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2a89-124">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a2a89-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2a89-125">Application</span></span> | <span data-ttu-id="a2a89-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2a89-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2a89-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2a89-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="a2a89-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2a89-128">Request headers</span></span>
| <span data-ttu-id="a2a89-129">名称</span><span class="sxs-lookup"><span data-stu-id="a2a89-129">Name</span></span>       | <span data-ttu-id="a2a89-130">类型</span><span class="sxs-lookup"><span data-stu-id="a2a89-130">Type</span></span> | <span data-ttu-id="a2a89-131">说明</span><span class="sxs-lookup"><span data-stu-id="a2a89-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2a89-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2a89-132">Authorization</span></span>  | <span data-ttu-id="a2a89-133">string</span><span class="sxs-lookup"><span data-stu-id="a2a89-133">string</span></span>  | <span data-ttu-id="a2a89-134">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="a2a89-134">Bearer {token}.</span></span>|
| <span data-ttu-id="a2a89-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2a89-135">Content-Type</span></span> | <span data-ttu-id="a2a89-136">string</span><span class="sxs-lookup"><span data-stu-id="a2a89-136">string</span></span>  | <span data-ttu-id="a2a89-p102">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="a2a89-p102">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="a2a89-139">用于 `application/json` JSON 对象和 `text/plain` MIME 内容</span><span class="sxs-lookup"><span data-stu-id="a2a89-139">Use `application/json` for a JSON object and `text/plain` for MIME content</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2a89-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2a89-140">Request body</span></span>
<span data-ttu-id="a2a89-141">使用 JSON 格式时，提供 message 对象的 JSON [表示](../resources/message.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="a2a89-141">When using JSON format, provide a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="a2a89-142">当指定 MIME 格式的正文时，请提供 MIME 内容与适用的 Internet 邮件头（“收件人”、“抄送”、“密件抄送”、“主题”）所有内容在请求正文中编码为 **base64** 格式。</span><span class="sxs-lookup"><span data-stu-id="a2a89-142">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

<span data-ttu-id="a2a89-143">若要使用 **提及** 功能在新邮件中呼叫其他用户，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a2a89-143">To use **mention** to call out another user in the new message:</span></span>
- <span data-ttu-id="a2a89-144">在请求 **正文中包括必需的 toRecipients** 属性 **、mentions** 属性和任何可写邮件属性。</span><span class="sxs-lookup"><span data-stu-id="a2a89-144">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="a2a89-145">对于 **mentions** 属性中的每个提及，必须指定 **提及的** 属性。</span><span class="sxs-lookup"><span data-stu-id="a2a89-145">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="a2a89-146">由于 **邮件** 资源支持 [扩展](/graph/extensibility-overview)因此可以使用 `POST` 操作，并在创建邮件时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="a2a89-146">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>


## <a name="response"></a><span data-ttu-id="a2a89-147">响应</span><span class="sxs-lookup"><span data-stu-id="a2a89-147">Response</span></span>

<span data-ttu-id="a2a89-148">如果成功，此方法在响应 `201 Created` 正文中返回 [响应](../resources/message.md) 代码和 message 对象。</span><span class="sxs-lookup"><span data-stu-id="a2a89-148">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="a2a89-149">如果请求正文包含错误的 MIME 内容，此方法将返回 `400 Bad request` 和以下错误消息：“无效的 base64 字符串 MIME 内容”。</span><span class="sxs-lookup"><span data-stu-id="a2a89-149">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="a2a89-150">示例</span><span class="sxs-lookup"><span data-stu-id="a2a89-150">Examples</span></span>
### <a name="example-1-create-a-message-draft-in-json-format"></a><span data-ttu-id="a2a89-151">示例 1：创建 JSON 格式的邮件草稿</span><span class="sxs-lookup"><span data-stu-id="a2a89-151">Example 1: Create a message draft in JSON format</span></span>
#### <a name="request"></a><span data-ttu-id="a2a89-152">请求</span><span class="sxs-lookup"><span data-stu-id="a2a89-152">Request</span></span>
<span data-ttu-id="a2a89-153">下面是一个请求创建新邮件草稿的示例。</span><span class="sxs-lookup"><span data-stu-id="a2a89-153">Here is an example of the request to create a draft of a new message.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2a89-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2a89-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a2a89-155">C#</span><span class="sxs-lookup"><span data-stu-id="a2a89-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2a89-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2a89-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2a89-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2a89-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2a89-158">Java</span><span class="sxs-lookup"><span data-stu-id="a2a89-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a2a89-159">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2a89-159">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="a2a89-160">响应</span><span class="sxs-lookup"><span data-stu-id="a2a89-160">Response</span></span>
<span data-ttu-id="a2a89-p103">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a2a89-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-create-a-draft-message-that-includes-an--mention"></a><span data-ttu-id="a2a89-163">示例 2：创建包含 @-mention 的草稿邮件</span><span class="sxs-lookup"><span data-stu-id="a2a89-163">Example 2: Create a draft message that includes an @-mention</span></span>
#### <a name="request"></a><span data-ttu-id="a2a89-164">请求</span><span class="sxs-lookup"><span data-stu-id="a2a89-164">Request</span></span>
<span data-ttu-id="a2a89-165">下一个示例显示 Randi Welch 发往 Samantha 一份草稿电子邮件。</span><span class="sxs-lookup"><span data-stu-id="a2a89-165">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="a2a89-166">邮件还包括另一个用户 Dana Swope 的提及。</span><span class="sxs-lookup"><span data-stu-id="a2a89-166">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="a2a89-167">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2a89-167">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2a89-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2a89-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a2a89-169">C#</span><span class="sxs-lookup"><span data-stu-id="a2a89-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-mentions-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2a89-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2a89-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-mentions-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2a89-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2a89-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-mentions-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2a89-172">Java</span><span class="sxs-lookup"><span data-stu-id="a2a89-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-mentions-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="a2a89-173">响应</span><span class="sxs-lookup"><span data-stu-id="a2a89-173">Response</span></span>
<span data-ttu-id="a2a89-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2a89-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3-create-a-draft-message-that-includes-custom-internet-message-headers"></a><span data-ttu-id="a2a89-177">示例 3：创建包含自定义 Internet 邮件头的草稿邮件</span><span class="sxs-lookup"><span data-stu-id="a2a89-177">Example 3: Create a draft message that includes custom Internet message headers</span></span>
#### <a name="request"></a><span data-ttu-id="a2a89-178">请求</span><span class="sxs-lookup"><span data-stu-id="a2a89-178">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a2a89-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2a89-179">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a2a89-180">C#</span><span class="sxs-lookup"><span data-stu-id="a2a89-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-headers-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2a89-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2a89-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-headers-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2a89-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2a89-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-headers-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2a89-183">Java</span><span class="sxs-lookup"><span data-stu-id="a2a89-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-headers-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a2a89-184">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2a89-184">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="a2a89-185">响应</span><span class="sxs-lookup"><span data-stu-id="a2a89-185">Response</span></span>
<span data-ttu-id="a2a89-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a2a89-186">Here is an example of the response.</span></span> <span data-ttu-id="a2a89-187">注意：默认情况下，POST 响应中不会返回 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="a2a89-187">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="a2a89-188">为简洁起见，也可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a2a89-188">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="a2a89-189">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a2a89-189">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-4-create-a-message-draft-in-mime-format"></a><span data-ttu-id="a2a89-190">示例 4：创建 MIME 格式的邮件草稿</span><span class="sxs-lookup"><span data-stu-id="a2a89-190">Example 4: Create a message draft in MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="a2a89-191">请求</span><span class="sxs-lookup"><span data-stu-id="a2a89-191">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_create_draft_mime_beta"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCArMDAwMApNZXNzYWdlLUlEOgoJPE1XSFBSMTMw
MU1CMjAwMDAwMDAwRDc2RDlDMjgyMjAwMDA5QUQ5QTlASFdIUFIxMzAxTUIwMDAwLmNvZGVudW0u
cHJvZC5vdXRsb29rLmNvbT4KQ29udGVudC1MYW5ndWFnZTogZW4tVVMKWC1NUy1IYXMtQXR0YWNo
OgpYLU1TLVRORUYtQ29ycmVsYXRv
```


#### <a name="response"></a><span data-ttu-id="a2a89-192">响应</span><span class="sxs-lookup"><span data-stu-id="a2a89-192">Response</span></span>
<span data-ttu-id="a2a89-193">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a2a89-193">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.message",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('0aaa0aa0-0000-0a00-a00a-0000009000a0')/messages/$entity",
    "@odata.etag": "W/\"AAAAAAAAAAAa00AAAa0aAaAa0a0AAAaAAAAaAa0a\"",
    "id": "AAMkADA1MTAAAAqldOAAA=",
    "createdDateTime": "2021-04-23T18:13:44Z",
    "lastModifiedDateTime": "2021-04-23T18:13:44Z",
    "changeKey": "AAAAAAAAAAAA00aaaa000aaA",
    "categories": [],
    "receivedDateTime": "2021-04-23T18:13:44Z",
    "sentDateTime": "2021-02-28T07:15:00Z",
    "hasAttachments": false,
    "internetMessageId": "<AAAAAAAAAA@AAAAAAA0001AA0000.codcod00.prod.outlook.com>",
    "subject": "Internal Resume Submission: Sales Associate",
    "bodyPreview": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here...",
    "importance": "normal",
    "parentFolderId": "LKJDSKJHkjhfakKJHFKWKKJHKJdhkjHDK==",
    "conversationId": "SDSFSmFSDGI5LWZhYjc4fsdfsd=",
    "conversationIndex": "Adfsdfsdfsdfw==",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": true,
    "isDraft": true,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkAGNhOWAvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "body": {
        "contentType": "text",
        "content": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here... Regards,Alex"
    },
    "sender": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    }
}
```

<span data-ttu-id="a2a89-194">如果请求正文包含错误的 MIME 内容，此方法返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="a2a89-194">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 400 Bad Request
Content-type: application/json

{
    "error": {
        "code": "ErrorMimeContentInvalidBase64String",
        "message": "Invalid base64 string for MIME content."
    }
}
```

## <a name="see-also"></a><span data-ttu-id="a2a89-195">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a2a89-195">See also</span></span>

- [<span data-ttu-id="a2a89-196">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a2a89-196">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a2a89-197">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="a2a89-197">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a2a89-198">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="a2a89-198">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
