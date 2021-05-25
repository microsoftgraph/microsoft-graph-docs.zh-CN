---
title: 'message: createReplyAll'
description: 创建草稿以 JSON 或 MIME 格式答复邮件的所有收件人
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9eac6d007e77d6e4e840299d8ac50530dd3172b3
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645575"
---
# <a name="message-createreplyall"></a><span data-ttu-id="61e43-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="61e43-103">message: createReplyAll</span></span>

<span data-ttu-id="61e43-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61e43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61e43-105">创建一个草稿以 JSON 或 MIME[](../resources/message.md)格式答复邮件的发件人和所有收件人。</span><span class="sxs-lookup"><span data-stu-id="61e43-105">Create a draft to reply to the sender and all recipients of a [message](../resources/message.md) in either JSON or MIME format.</span></span>

<span data-ttu-id="61e43-106">使用 JSON 格式时：</span><span class="sxs-lookup"><span data-stu-id="61e43-106">When using JSON format:</span></span>
- <span data-ttu-id="61e43-107">指定参数的 comment 或 **body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="61e43-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="61e43-108">指定这两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="61e43-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="61e43-109">如果原始邮件在 **replyTo** 属性中指定收件人，则根据 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ，您应将答复发送给 **replyTo** 和 **toRecipients** 属性中的收件人，而不是 **from** 和 **toRecipients** 属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="61e43-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the **replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 
- <span data-ttu-id="61e43-110">您可以 [稍后](../api/message-update.md) 更新草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="61e43-110">You can [update](../api/message-update.md) the draft message later.</span></span>

<span data-ttu-id="61e43-111">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="61e43-111">When using MIME format:</span></span>
- <span data-ttu-id="61e43-112">在请求正文中提供适用的 [Internet](https://tools.ietf.org/html/rfc2076) 邮件头和 [MIME](https://tools.ietf.org/html/rfc2045)内容，这些内容均以 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="61e43-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="61e43-113">将任何附件和 S/MIME 属性添加到 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="61e43-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="61e43-114">[在](../api/message-send.md) 后续操作中发送草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="61e43-114">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="61e43-115">或者， [在单个操作中全部](../api/message-replyall.md) 答复邮件。</span><span class="sxs-lookup"><span data-stu-id="61e43-115">Alternatively, [reply-all to a message](../api/message-replyall.md) in a single action.</span></span>

## <a name="permissions"></a><span data-ttu-id="61e43-116">权限</span><span class="sxs-lookup"><span data-stu-id="61e43-116">Permissions</span></span>
<span data-ttu-id="61e43-117">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="61e43-117">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="61e43-118">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61e43-118">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61e43-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="61e43-119">Permission type</span></span>      | <span data-ttu-id="61e43-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61e43-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61e43-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61e43-121">Delegated (work or school account)</span></span> | <span data-ttu-id="61e43-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61e43-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="61e43-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61e43-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61e43-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61e43-124">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="61e43-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="61e43-125">Application</span></span> | <span data-ttu-id="61e43-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61e43-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="61e43-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61e43-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="61e43-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="61e43-128">Request headers</span></span>
| <span data-ttu-id="61e43-129">名称</span><span class="sxs-lookup"><span data-stu-id="61e43-129">Name</span></span>       | <span data-ttu-id="61e43-130">类型</span><span class="sxs-lookup"><span data-stu-id="61e43-130">Type</span></span> | <span data-ttu-id="61e43-131">说明</span><span class="sxs-lookup"><span data-stu-id="61e43-131">Description</span></span>| 
|:---------------|:--------|:----------|
| <span data-ttu-id="61e43-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="61e43-132">Authorization</span></span>  | <span data-ttu-id="61e43-133">string</span><span class="sxs-lookup"><span data-stu-id="61e43-133">string</span></span>  | <span data-ttu-id="61e43-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="61e43-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="61e43-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61e43-136">Content-Type</span></span> | <span data-ttu-id="61e43-137">string</span><span class="sxs-lookup"><span data-stu-id="61e43-137">string</span></span>  | <span data-ttu-id="61e43-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="61e43-p104">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="61e43-140">用于 `application/json` JSON 对象和 `text/plain` MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="61e43-140">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61e43-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="61e43-141">Request body</span></span>
<span data-ttu-id="61e43-142">使用 JSON 格式时，请提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="61e43-142">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="61e43-143">参数</span><span class="sxs-lookup"><span data-stu-id="61e43-143">Parameter</span></span>    | <span data-ttu-id="61e43-144">类型</span><span class="sxs-lookup"><span data-stu-id="61e43-144">Type</span></span>   |<span data-ttu-id="61e43-145">说明</span><span class="sxs-lookup"><span data-stu-id="61e43-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61e43-146">注释</span><span class="sxs-lookup"><span data-stu-id="61e43-146">comment</span></span>|<span data-ttu-id="61e43-147">String</span><span class="sxs-lookup"><span data-stu-id="61e43-147">String</span></span>|<span data-ttu-id="61e43-p105">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="61e43-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="61e43-150">message</span><span class="sxs-lookup"><span data-stu-id="61e43-150">message</span></span>|[<span data-ttu-id="61e43-151">message</span><span class="sxs-lookup"><span data-stu-id="61e43-151">message</span></span>](../resources/message.md)|<span data-ttu-id="61e43-152">在全部答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="61e43-152">Any writeable properties to update in the reply-all message.</span></span>|

<span data-ttu-id="61e43-153">指定 MIME 格式的正文时，请提供 MIME 内容以及适用的 Internet 邮件头，所有邮件头在请求正文中都以 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="61e43-153">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="61e43-154">响应</span><span class="sxs-lookup"><span data-stu-id="61e43-154">Response</span></span>

<span data-ttu-id="61e43-155">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="61e43-155">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="61e43-156">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息："MIME 内容的 `400 Bad request` base64 字符串无效"。</span><span class="sxs-lookup"><span data-stu-id="61e43-156">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="61e43-157">示例</span><span class="sxs-lookup"><span data-stu-id="61e43-157">Examples</span></span>
### <a name="example-1-create-a-draft-in-json-format-to-reply-all-to-an-existing-message"></a><span data-ttu-id="61e43-158">示例 1：创建 JSON 格式的草稿以全部答复现有邮件</span><span class="sxs-lookup"><span data-stu-id="61e43-158">Example 1: Create a draft in JSON format to reply-all to an existing message</span></span>
<span data-ttu-id="61e43-159">以下示例创建一个草稿以全部答复，并将附件和注释全部添加到一个 **createReplyAll** 调用中。</span><span class="sxs-lookup"><span data-stu-id="61e43-159">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="61e43-160">请求</span><span class="sxs-lookup"><span data-stu-id="61e43-160">Request</span></span>
<span data-ttu-id="61e43-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="61e43-161">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="61e43-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="61e43-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/createReplyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "if the project gets approved, please take a look at the attached guidelines before you decide on the name." 
}
```
# <a name="c"></a>[<span data-ttu-id="61e43-163">C#</span><span class="sxs-lookup"><span data-stu-id="61e43-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61e43-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61e43-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61e43-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61e43-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61e43-166">Java</span><span class="sxs-lookup"><span data-stu-id="61e43-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="61e43-167">响应</span><span class="sxs-lookup"><span data-stu-id="61e43-167">Response</span></span>
<span data-ttu-id="61e43-p106">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="61e43-p106">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKpAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DP\"",
  "id": "AAMkADA1MTAAAH5JKpAAA=",
  "subject": "RE: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body dir=\"ltr\">\r\nif the project gets approved, please take a look at the attached guidelines before you decide on the name.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:36:32 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group\r\n<div>Samantha, Randi, would you name the group please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n</body>\r\n</html>"
  },
  "sender": {
    "emailAddress": {
      "name": "Admin",
      "address": "admin@contoso.onmicrosoft.com"
    }
  },
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress": {
        "name": "Randi Welch",
        "address": "randiw@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

### <a name="example-2-create-a-draft-using-mime-format-to-reply-all-to-an-existing-message"></a><span data-ttu-id="61e43-170">示例 2：使用 MIME 格式创建草稿以全部答复现有邮件</span><span class="sxs-lookup"><span data-stu-id="61e43-170">Example 2: Create a draft using MIME format to reply-all to an existing message</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createReplyAll
Content-Type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np...
```
##### <a name="response"></a><span data-ttu-id="61e43-171">响应</span><span class="sxs-lookup"><span data-stu-id="61e43-171">Response</span></span>
<span data-ttu-id="61e43-172">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="61e43-172">Here is an example of the response.</span></span>

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

<span data-ttu-id="61e43-173">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="61e43-173">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


