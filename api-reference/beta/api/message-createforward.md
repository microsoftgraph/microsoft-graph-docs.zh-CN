---
title: 'message: createForward'
description: 创建草稿以转发 JSON 或 MIME 格式的现有邮件。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 758ca460786eb7e59c41762f8dfa4209b20a62b9
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870421"
---
# <a name="message-createforward"></a><span data-ttu-id="204d6-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="204d6-103">message: createForward</span></span>

<span data-ttu-id="204d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="204d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="204d6-105">创建以 JSON 或[](../resources/message.md)MIME 格式转发现有邮件的草稿。</span><span class="sxs-lookup"><span data-stu-id="204d6-105">Create a draft to forward an existing [message](../resources/message.md), in either JSON or MIME format.</span></span>

<span data-ttu-id="204d6-106">使用 JSON 格式时，可以：</span><span class="sxs-lookup"><span data-stu-id="204d6-106">When using JSON format, you can:</span></span> 
- <span data-ttu-id="204d6-107">指定参数的 comment 或 **body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="204d6-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="204d6-108">指定这两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="204d6-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="204d6-109">指定参数 `toRecipients` 的参数或 **toRecipients** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="204d6-109">Specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="204d6-110">指定两者或同时指定两者都将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="204d6-110">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="204d6-111">随后 [更新](../api/message-update.md)草稿以将内容添加到 **正文**，或更改其他邮件属性。</span><span class="sxs-lookup"><span data-stu-id="204d6-111">[Update](../api/message-update.md) the draft later to add content to the **body** or change other message properties.</span></span>

<span data-ttu-id="204d6-112">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="204d6-112">When using MIME format:</span></span>
- <span data-ttu-id="204d6-113">提供适用的 [Internet 邮件头](https://tools.ietf.org/html/rfc2076) 和 [MIME 内容](https://tools.ietf.org/html/rfc2045)，所有内容在请求正文中都通过 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="204d6-113">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="204d6-114">向 MIME 内容添加任何附件和 S/MIME 属性。</span><span class="sxs-lookup"><span data-stu-id="204d6-114">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="204d6-115">在后续操作中[发送](../api/message-send.md)草稿消息。</span><span class="sxs-lookup"><span data-stu-id="204d6-115">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="204d6-116">或者， [在单个操作](../api/message-forward.md) 中转发邮件。</span><span class="sxs-lookup"><span data-stu-id="204d6-116">Alternatively, [forward a message](../api/message-forward.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="204d6-117">权限</span><span class="sxs-lookup"><span data-stu-id="204d6-117">Permissions</span></span>
<span data-ttu-id="204d6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="204d6-p103">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="204d6-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="204d6-120">Permission type</span></span>      | <span data-ttu-id="204d6-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="204d6-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="204d6-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="204d6-122">Delegated (work or school account)</span></span> | <span data-ttu-id="204d6-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="204d6-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="204d6-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="204d6-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="204d6-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="204d6-125">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="204d6-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="204d6-126">Application</span></span> | <span data-ttu-id="204d6-127">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="204d6-127">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="204d6-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="204d6-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="204d6-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="204d6-129">Request headers</span></span>
| <span data-ttu-id="204d6-130">名称</span><span class="sxs-lookup"><span data-stu-id="204d6-130">Name</span></span>       | <span data-ttu-id="204d6-131">类型</span><span class="sxs-lookup"><span data-stu-id="204d6-131">Type</span></span> | <span data-ttu-id="204d6-132">说明</span><span class="sxs-lookup"><span data-stu-id="204d6-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="204d6-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="204d6-133">Authorization</span></span>  | <span data-ttu-id="204d6-134">string</span><span class="sxs-lookup"><span data-stu-id="204d6-134">string</span></span>  | <span data-ttu-id="204d6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="204d6-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="204d6-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="204d6-137">Content-Type</span></span> | <span data-ttu-id="204d6-138">string</span><span class="sxs-lookup"><span data-stu-id="204d6-138">string</span></span>  | <span data-ttu-id="204d6-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="204d6-p105">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="204d6-141">对 JSON 对象使用 `application/json`，对 MIME 内容使用 `text/plain`。</span><span class="sxs-lookup"><span data-stu-id="204d6-141">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span>|

## <a name="request-body"></a><span data-ttu-id="204d6-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="204d6-142">Request body</span></span>
<span data-ttu-id="204d6-143">若要发送 JSON 对象，请提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="204d6-143">To send a JSON object provide the following parameters.</span></span>

| <span data-ttu-id="204d6-144">参数</span><span class="sxs-lookup"><span data-stu-id="204d6-144">Parameter</span></span>    | <span data-ttu-id="204d6-145">类型</span><span class="sxs-lookup"><span data-stu-id="204d6-145">Type</span></span>   |<span data-ttu-id="204d6-146">说明</span><span class="sxs-lookup"><span data-stu-id="204d6-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="204d6-147">注释</span><span class="sxs-lookup"><span data-stu-id="204d6-147">comment</span></span>|<span data-ttu-id="204d6-148">String</span><span class="sxs-lookup"><span data-stu-id="204d6-148">String</span></span>|<span data-ttu-id="204d6-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="204d6-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="204d6-151">toRecipients</span><span class="sxs-lookup"><span data-stu-id="204d6-151">toRecipients</span></span>|<span data-ttu-id="204d6-152">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="204d6-152">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="204d6-153">收件人列表</span><span class="sxs-lookup"><span data-stu-id="204d6-153">The list of recipients.</span></span>|
|<span data-ttu-id="204d6-154">message</span><span class="sxs-lookup"><span data-stu-id="204d6-154">message</span></span>|[<span data-ttu-id="204d6-155">message</span><span class="sxs-lookup"><span data-stu-id="204d6-155">message</span></span>](../resources/message.md)|<span data-ttu-id="204d6-156">回复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="204d6-156">Any writeable properties to update in the reply message.</span></span>|

<span data-ttu-id="204d6-157">当指定 MIME 格式的正文时，请提供 MIME 内容与适用的 Internet 邮件头（“收件人”、“抄送”、“密件抄送”、“主题”）所有内容在请求正文中编码为 **base64** 格式。</span><span class="sxs-lookup"><span data-stu-id="204d6-157">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="204d6-158">响应</span><span class="sxs-lookup"><span data-stu-id="204d6-158">Response</span></span>

<span data-ttu-id="204d6-159">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="204d6-159">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="204d6-160">如果请求正文包含错误的 MIME 内容，此方法将返回 `400 Bad request` 和以下错误消息：“无效的 base64 字符串 MIME 内容”。</span><span class="sxs-lookup"><span data-stu-id="204d6-160">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="204d6-161">示例</span><span class="sxs-lookup"><span data-stu-id="204d6-161">Examples</span></span>

### <a name="example-1-create-a-draft-message-in-json-format-to-forward-an-existing-message"></a><span data-ttu-id="204d6-162">示例 1：创建 JSON 格式的草稿邮件以转发现有邮件</span><span class="sxs-lookup"><span data-stu-id="204d6-162">Example 1: Create a draft message in JSON format to forward an existing message</span></span>
<span data-ttu-id="204d6-163">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="204d6-163">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="204d6-164">请求</span><span class="sxs-lookup"><span data-stu-id="204d6-164">Request</span></span>
<span data-ttu-id="204d6-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="204d6-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="204d6-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="204d6-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this; you'll need this if the project gets approved." 
}
```
# <a name="c"></a>[<span data-ttu-id="204d6-167">C#</span><span class="sxs-lookup"><span data-stu-id="204d6-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="204d6-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="204d6-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="204d6-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="204d6-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="204d6-170">Java</span><span class="sxs-lookup"><span data-stu-id="204d6-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createforward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="204d6-171">响应</span><span class="sxs-lookup"><span data-stu-id="204d6-171">Response</span></span>
<span data-ttu-id="204d6-p107">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="204d6-p107">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKqAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DQ\"",
  "id": "AAMkADA1MTAAAH5JKqAAA=",
  "subject": "FW: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>\r\nDana, just want to make sure you get this; you'll need this if the project gets approved.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:47:54 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group</body>\r\n</html>\r\n"
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
        "name": "Dana Swope",
        "address": "danas@contoso.onmicrosoft.com"
      }
    }
  ]
}
```


### <a name="example-2-create-a-draft-message-in-mime-format-to-forward-an-existing-message"></a><span data-ttu-id="204d6-174">示例 2：创建 MIME 格式的草稿邮件以转发现有邮件</span><span class="sxs-lookup"><span data-stu-id="204d6-174">Example 2: Create a draft message in MIME format to forward an existing message</span></span>

##### <a name="request"></a><span data-ttu-id="204d6-175">请求</span><span class="sxs-lookup"><span data-stu-id="204d6-175">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_createForward_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
Content-Type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCArMDAwMApNZXNzYWdlLUlEOgoJPE1XSFBSMTMw
MU1CMjAwMDAwMDAwRDc2RDlDMjgyMjAwMDA5QUQ5QTlASFdIUFIxMzAxTUIwMDAwLmNvZGVudW0u
cHJvZC5vdXRsb29rLmNvbT4KQ29udGVudC1MYW5ndWFnZTogZW4tVVMKWC1NUy1IYXMtQXR0YWNo
OgpYLU1TLVRORUYtQ29ycmVsYXRvcjoKWC1NUy1FeGNoYW5n
```

##### <a name="response"></a><span data-ttu-id="204d6-176">响应</span><span class="sxs-lookup"><span data-stu-id="204d6-176">Response</span></span>
<span data-ttu-id="204d6-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="204d6-177">Here is an example of the response.</span></span>

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

<span data-ttu-id="204d6-178">如果请求正文包含错误的 MIME 内容，此方法返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="204d6-178">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
