---
title: 'message: createReply'
description: '创建以 JSON 或 MIME 格式答复邮件的草稿。 '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 023b04f37f0320ca3a74801f9d2e92d19553a10c
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645596"
---
# <a name="message-createreply"></a><span data-ttu-id="ab6b2-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="ab6b2-103">message: createReply</span></span>

<span data-ttu-id="ab6b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab6b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab6b2-105">创建以 JSON 或 MIME[](../resources/message.md)格式答复邮件发件人的草稿。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-105">Create a draft to reply to the sender of a [message](../resources/message.md) in either JSON or MIME format.</span></span>

<span data-ttu-id="ab6b2-106">使用 JSON 格式时：</span><span class="sxs-lookup"><span data-stu-id="ab6b2-106">When using JSON format:</span></span>
- <span data-ttu-id="ab6b2-107">指定参数的 comment 或 **body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="ab6b2-108">指定这两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="ab6b2-109">如果在原始邮件中指定了 **replyTo，** 则根据 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ，您应该将答复发送给 **replyTo** 中的收件人，而不是 中的 **收件人**。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-109">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span>
- <span data-ttu-id="ab6b2-110">您可以 [稍后](../api/message-update.md) 更新草稿以将回复内容添加到 **正文或更改** 其他邮件属性。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-110">You can [update](../api/message-update.md) the draft later to add reply content to the **body** or change other message properties.</span></span>

<span data-ttu-id="ab6b2-111">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="ab6b2-111">When using MIME format:</span></span>
- <span data-ttu-id="ab6b2-112">在请求正文中提供适用的 [Internet](https://tools.ietf.org/html/rfc2076) 邮件头和 [MIME](https://tools.ietf.org/html/rfc2045)内容，这些内容均以 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="ab6b2-113">将任何附件和 S/MIME 属性添加到 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="ab6b2-114">[在](../api/message-send.md) 后续操作中发送草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-114">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="ab6b2-115">或者， [在单个操作中](../api/message-reply.md) 回复邮件。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-115">Alternatively, [reply to a message](../api/message-reply.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab6b2-116">权限</span><span class="sxs-lookup"><span data-stu-id="ab6b2-116">Permissions</span></span>
<span data-ttu-id="ab6b2-117">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-117">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="ab6b2-118">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-118">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab6b2-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab6b2-119">Permission type</span></span>      | <span data-ttu-id="ab6b2-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab6b2-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab6b2-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab6b2-121">Delegated (work or school account)</span></span> | <span data-ttu-id="ab6b2-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab6b2-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ab6b2-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab6b2-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab6b2-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab6b2-124">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ab6b2-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab6b2-125">Application</span></span> | <span data-ttu-id="ab6b2-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab6b2-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab6b2-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab6b2-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```

## <a name="request-headers"></a><span data-ttu-id="ab6b2-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab6b2-128">Request headers</span></span>
| <span data-ttu-id="ab6b2-129">名称</span><span class="sxs-lookup"><span data-stu-id="ab6b2-129">Name</span></span>       | <span data-ttu-id="ab6b2-130">类型</span><span class="sxs-lookup"><span data-stu-id="ab6b2-130">Type</span></span> | <span data-ttu-id="ab6b2-131">说明</span><span class="sxs-lookup"><span data-stu-id="ab6b2-131">Description</span></span>| 
|:---------------|:--------|:----------|
| <span data-ttu-id="ab6b2-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab6b2-132">Authorization</span></span>  | <span data-ttu-id="ab6b2-133">string</span><span class="sxs-lookup"><span data-stu-id="ab6b2-133">string</span></span>  | <span data-ttu-id="ab6b2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ab6b2-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab6b2-136">Content-Type</span></span> | <span data-ttu-id="ab6b2-137">string</span><span class="sxs-lookup"><span data-stu-id="ab6b2-137">string</span></span>  | <span data-ttu-id="ab6b2-138">实体正文中的数据性质。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-138">Nature of the data in the body of an entity.</span></span> <br/> <span data-ttu-id="ab6b2-139">用于 `application/json` JSON 对象和 `text/plain` MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-139">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab6b2-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab6b2-140">Request body</span></span>
<span data-ttu-id="ab6b2-141">此方法不需要请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-141">This method does not require a request body.</span></span>

<span data-ttu-id="ab6b2-142">但是，对于使用 MIME 格式创建答复草稿，请为 MIME 内容提供适用的 Internet 邮件头，所有邮件头均在请求正文中以 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-142">However, for creating a reply draft using MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="ab6b2-143">响应</span><span class="sxs-lookup"><span data-stu-id="ab6b2-143">Response</span></span>

<span data-ttu-id="ab6b2-144">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-144">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="ab6b2-145">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息："MIME 内容的 `400 Bad request` base64 字符串无效"。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-145">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="ab6b2-146">示例</span><span class="sxs-lookup"><span data-stu-id="ab6b2-146">Examples</span></span>
### <a name="example-1-create-a-draft-message-in-json-format-to-reply-to-an-existing-message"></a><span data-ttu-id="ab6b2-147">示例 1：创建 JSON 格式的草稿邮件以答复现有邮件。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-147">Example 1: Create a draft message in JSON format to reply to an existing message.</span></span>
<span data-ttu-id="ab6b2-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ab6b2-149">请求</span><span class="sxs-lookup"><span data-stu-id="ab6b2-149">Request</span></span>
<span data-ttu-id="ab6b2-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab6b2-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab6b2-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReply
```
# <a name="c"></a>[<span data-ttu-id="ab6b2-152">C#</span><span class="sxs-lookup"><span data-stu-id="ab6b2-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab6b2-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab6b2-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab6b2-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab6b2-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab6b2-155">Java</span><span class="sxs-lookup"><span data-stu-id="ab6b2-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ab6b2-156">响应</span><span class="sxs-lookup"><span data-stu-id="ab6b2-156">Response</span></span>
<span data-ttu-id="ab6b2-p104">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

### <a name="example-2-create-a-draft-message-in-mime-format-to-reply-to-an-existing-message"></a><span data-ttu-id="ab6b2-159">示例 2：创建 MIME 格式的草稿邮件以答复现有邮件</span><span class="sxs-lookup"><span data-stu-id="ab6b2-159">Example 2: Create a draft message in MIME format to reply to an existing message</span></span>
##### <a name="request"></a><span data-ttu-id="ab6b2-160">请求</span><span class="sxs-lookup"><span data-stu-id="ab6b2-160">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createReply_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply
Content-type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCA
```

##### <a name="response"></a><span data-ttu-id="ab6b2-161">响应</span><span class="sxs-lookup"><span data-stu-id="ab6b2-161">Response</span></span>
<span data-ttu-id="ab6b2-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.message",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

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

<span data-ttu-id="ab6b2-163">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-163">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

