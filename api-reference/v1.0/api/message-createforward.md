---
title: 'message: createForward'
description: 创建草稿以转发 JSON 或 MIME 格式的现有邮件。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9892fb41a6115abfad0e7c19167911db533ad213
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645603"
---
# <a name="message-createforward"></a><span data-ttu-id="5d76f-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="5d76f-103">message: createForward</span></span>

<span data-ttu-id="5d76f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d76f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d76f-105">创建以 JSON 或[](../resources/message.md)MIME 格式转发现有邮件的草稿。</span><span class="sxs-lookup"><span data-stu-id="5d76f-105">Create a draft to forward an existing [message](../resources/message.md), in either JSON or MIME format.</span></span>

<span data-ttu-id="5d76f-106">使用 JSON 格式时，可以：</span><span class="sxs-lookup"><span data-stu-id="5d76f-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="5d76f-107">指定参数的 comment 或 **body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="5d76f-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="5d76f-108">指定这两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="5d76f-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="5d76f-109">指定参数 `toRecipients` 的参数或 **toRecipients** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="5d76f-109">Specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="5d76f-110">指定两者或同时指定两者都将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="5d76f-110">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="5d76f-111">[稍后](../api/message-update.md) 更新草稿以将内容添加到 **正文或更改** 其他邮件属性。</span><span class="sxs-lookup"><span data-stu-id="5d76f-111">[Update](../api/message-update.md) the draft later to add content to the **body** or change other message properties.</span></span>

<span data-ttu-id="5d76f-112">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="5d76f-112">When using MIME format:</span></span>
- <span data-ttu-id="5d76f-113">在请求正文中提供适用的 [Internet](https://tools.ietf.org/html/rfc2076) 邮件头和 [MIME](https://tools.ietf.org/html/rfc2045)内容，这些内容均以 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="5d76f-113">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="5d76f-114">将任何附件和 S/MIME 属性添加到 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="5d76f-114">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="5d76f-115">[在](../api/message-send.md) 后续操作中发送草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="5d76f-115">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="5d76f-116">或者， [在单个操作](../api/message-forward.md) 中转发邮件。</span><span class="sxs-lookup"><span data-stu-id="5d76f-116">Alternatively, [forward a message](../api/message-forward.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d76f-117">权限</span><span class="sxs-lookup"><span data-stu-id="5d76f-117">Permissions</span></span>
<span data-ttu-id="5d76f-118">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="5d76f-118">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="5d76f-119">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d76f-119">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d76f-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d76f-120">Permission type</span></span>      | <span data-ttu-id="5d76f-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d76f-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d76f-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d76f-122">Delegated (work or school account)</span></span> | <span data-ttu-id="5d76f-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d76f-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5d76f-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d76f-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d76f-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d76f-125">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5d76f-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d76f-126">Application</span></span> | <span data-ttu-id="5d76f-127">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d76f-127">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d76f-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d76f-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```

## <a name="request-headers"></a><span data-ttu-id="5d76f-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d76f-129">Request headers</span></span>

| <span data-ttu-id="5d76f-130">名称</span><span class="sxs-lookup"><span data-stu-id="5d76f-130">Name</span></span>       | <span data-ttu-id="5d76f-131">类型</span><span class="sxs-lookup"><span data-stu-id="5d76f-131">Type</span></span> | <span data-ttu-id="5d76f-132">说明</span><span class="sxs-lookup"><span data-stu-id="5d76f-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d76f-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d76f-133">Authorization</span></span>  | <span data-ttu-id="5d76f-134">string</span><span class="sxs-lookup"><span data-stu-id="5d76f-134">string</span></span>  | <span data-ttu-id="5d76f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d76f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d76f-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d76f-137">Content-Type</span></span> | <span data-ttu-id="5d76f-138">string</span><span class="sxs-lookup"><span data-stu-id="5d76f-138">string</span></span>  | <span data-ttu-id="5d76f-139">实体正文中的数据性质。</span><span class="sxs-lookup"><span data-stu-id="5d76f-139">Nature of the data in the body of an entity.</span></span> <br/> <span data-ttu-id="5d76f-140">用于 `application/json` JSON 对象和 `text/plain` MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="5d76f-140">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d76f-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d76f-141">Request body</span></span>
<span data-ttu-id="5d76f-142">此方法不需要请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d76f-142">This method does not require a request body.</span></span>

<span data-ttu-id="5d76f-143">但是，若要使用 MIME 格式创建转发草稿，请为 MIME 内容提供适用的 Internet 邮件头 ("收件人"、"抄送"、"密件抄送"、"主题") ，请求正文中均以 **base64** 格式编码。</span><span class="sxs-lookup"><span data-stu-id="5d76f-143">However, for creating a forward draft using MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span> 

## <a name="response"></a><span data-ttu-id="5d76f-144">响应</span><span class="sxs-lookup"><span data-stu-id="5d76f-144">Response</span></span>

<span data-ttu-id="5d76f-145">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d76f-145">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="5d76f-146">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息："MIME 内容的 `400 Bad request` base64 字符串无效"。</span><span class="sxs-lookup"><span data-stu-id="5d76f-146">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="5d76f-147">示例</span><span class="sxs-lookup"><span data-stu-id="5d76f-147">Examples</span></span>

### <a name="example-1-create-a-draft-message-in-json-format-to-forward-an-existing-message"></a><span data-ttu-id="5d76f-148">示例 1：创建 JSON 格式的草稿邮件以转发现有邮件</span><span class="sxs-lookup"><span data-stu-id="5d76f-148">Example 1: Create a draft message in JSON format to forward an existing message</span></span>
<span data-ttu-id="5d76f-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5d76f-149">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5d76f-150">请求</span><span class="sxs-lookup"><span data-stu-id="5d76f-150">Request</span></span>

<span data-ttu-id="5d76f-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5d76f-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d76f-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d76f-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
```
# <a name="c"></a>[<span data-ttu-id="5d76f-153">C#</span><span class="sxs-lookup"><span data-stu-id="5d76f-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d76f-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d76f-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d76f-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d76f-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d76f-156">Java</span><span class="sxs-lookup"><span data-stu-id="5d76f-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createforward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5d76f-157">响应</span><span class="sxs-lookup"><span data-stu-id="5d76f-157">Response</span></span>

<span data-ttu-id="5d76f-p105">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5d76f-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-2-create-a-draft-message-in-mime-format-to-forward-an-existing-message"></a><span data-ttu-id="5d76f-160">示例 2 创建 MIME 格式的草稿邮件以转发现有邮件</span><span class="sxs-lookup"><span data-stu-id="5d76f-160">Example 2 Create a draft message in MIME format to forward an existing message</span></span>
##### <a name="request"></a><span data-ttu-id="5d76f-161">请求</span><span class="sxs-lookup"><span data-stu-id="5d76f-161">Request</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.message",
  "truncated": true
} -->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/createForward
Content-type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCArMDAwMApNZXNzYWdlLUlEOgoJPE1XSFBSMTMw
MU1CMjAwMDAwMDAwRDc2RDlDMjgyMjAwMDA5QUQ5QTlASF
```

##### <a name="response"></a><span data-ttu-id="5d76f-162">响应</span><span class="sxs-lookup"><span data-stu-id="5d76f-162">Response</span></span>
<span data-ttu-id="5d76f-163">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5d76f-163">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
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

<span data-ttu-id="5d76f-164">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="5d76f-164">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

