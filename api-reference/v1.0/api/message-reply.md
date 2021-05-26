---
title: 消息：答复
description: '使用 JSON 或 MIME 格式答复邮件的发件人。 '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b5b288f91a4f8657a17be1c26ed3d8407446c23f
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645272"
---
# <a name="message-reply"></a><span data-ttu-id="c0000-103">消息：答复</span><span class="sxs-lookup"><span data-stu-id="c0000-103">message: reply</span></span>

<span data-ttu-id="c0000-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0000-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0000-105">使用 JSON 或 MIME [格式](../resources/message.md) 答复邮件的发件人。</span><span class="sxs-lookup"><span data-stu-id="c0000-105">Reply to the sender of a [message](../resources/message.md) using either JSON or MIME format.</span></span>

<span data-ttu-id="c0000-106">使用 JSON 格式时：</span><span class="sxs-lookup"><span data-stu-id="c0000-106">When using JSON format:</span></span>
- <span data-ttu-id="c0000-107">指定参数的 comment 或 **body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="c0000-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="c0000-108">指定这两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="c0000-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="c0000-109">如果原始邮件在 **replyTo** 属性中指定收件人，则根据 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ，将答复发送给 **replyTo** 中的收件人，而不是 **from** 属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="c0000-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span>

<span data-ttu-id="c0000-110">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="c0000-110">When using MIME format:</span></span>
- <span data-ttu-id="c0000-111">在请求正文中提供适用的 [Internet](https://tools.ietf.org/html/rfc2076) 邮件头和 [MIME](https://tools.ietf.org/html/rfc2045)内容，这些内容均以 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="c0000-111">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="c0000-112">将任何附件和 S/MIME 属性添加到 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="c0000-112">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="c0000-113">此方法将邮件保存在"已发送 **的项目"** 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="c0000-113">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="c0000-114">或者，[创建一个草稿以答复现有邮件](../api/message-createreply.md)[，并稍后](../api/message-send.md)发送。</span><span class="sxs-lookup"><span data-stu-id="c0000-114">Alternatively, [create a draft to reply to an existing message](../api/message-createreply.md) and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0000-115">权限</span><span class="sxs-lookup"><span data-stu-id="c0000-115">Permissions</span></span>
<span data-ttu-id="c0000-116">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="c0000-116">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="c0000-117">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0000-117">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0000-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0000-118">Permission type</span></span>      | <span data-ttu-id="c0000-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0000-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0000-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0000-120">Delegated (work or school account)</span></span> | <span data-ttu-id="c0000-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c0000-121">Mail.Send</span></span>    |
|<span data-ttu-id="c0000-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0000-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0000-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c0000-123">Mail.Send</span></span>    |
|<span data-ttu-id="c0000-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0000-124">Application</span></span> | <span data-ttu-id="c0000-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c0000-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0000-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0000-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="c0000-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0000-127">Request headers</span></span>
| <span data-ttu-id="c0000-128">名称</span><span class="sxs-lookup"><span data-stu-id="c0000-128">Name</span></span>       | <span data-ttu-id="c0000-129">类型</span><span class="sxs-lookup"><span data-stu-id="c0000-129">Type</span></span> | <span data-ttu-id="c0000-130">说明</span><span class="sxs-lookup"><span data-stu-id="c0000-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c0000-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0000-131">Authorization</span></span>  | <span data-ttu-id="c0000-132">string</span><span class="sxs-lookup"><span data-stu-id="c0000-132">string</span></span>  | <span data-ttu-id="c0000-133">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="c0000-133">Bearer {token}.</span></span> <span data-ttu-id="c0000-134">必需</span><span class="sxs-lookup"><span data-stu-id="c0000-134">Required</span></span> |
| <span data-ttu-id="c0000-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0000-135">Content-Type</span></span> | <span data-ttu-id="c0000-136">string</span><span class="sxs-lookup"><span data-stu-id="c0000-136">string</span></span>  | <span data-ttu-id="c0000-137">实体正文中的数据性质。</span><span class="sxs-lookup"><span data-stu-id="c0000-137">Nature of the data in the body of an entity.</span></span> <span data-ttu-id="c0000-138">必需</span><span class="sxs-lookup"><span data-stu-id="c0000-138">Required</span></span> <br/> <span data-ttu-id="c0000-139">用于 `application/json` JSON 对象和 `text/plain` MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="c0000-139">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0000-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0000-140">Request body</span></span>
<span data-ttu-id="c0000-141">使用 JSON 格式时，在请求正文中提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c0000-141">When using JSON format, provide a JSON object in the request body with the following parameters.</span></span>

| <span data-ttu-id="c0000-142">参数</span><span class="sxs-lookup"><span data-stu-id="c0000-142">Parameter</span></span>    | <span data-ttu-id="c0000-143">类型</span><span class="sxs-lookup"><span data-stu-id="c0000-143">Type</span></span>   | <span data-ttu-id="c0000-144">说明</span><span class="sxs-lookup"><span data-stu-id="c0000-144">Description</span></span> |
|---------------|-------|---------|
| <span data-ttu-id="c0000-145">注释</span><span class="sxs-lookup"><span data-stu-id="c0000-145">comment</span></span> | <span data-ttu-id="c0000-146">String</span><span class="sxs-lookup"><span data-stu-id="c0000-146">String</span></span> | <span data-ttu-id="c0000-p105">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="c0000-p105">A comment to include. Can be an empty string.</span></span> |
| <span data-ttu-id="c0000-149">message</span><span class="sxs-lookup"><span data-stu-id="c0000-149">message</span></span> | [<span data-ttu-id="c0000-150">message</span><span class="sxs-lookup"><span data-stu-id="c0000-150">message</span></span>](../resources/message.md) | <span data-ttu-id="c0000-151">回复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="c0000-151">Any writeable properties to update in the reply message.</span></span> |

<span data-ttu-id="c0000-152">指定 MIME 格式的正文时，请提供 MIME 内容以及适用的 Internet 邮件头，所有邮件头在请求正文中都以 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="c0000-152">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span> <span data-ttu-id="c0000-153">此方法使用原始邮件的发件人作为收件人。</span><span class="sxs-lookup"><span data-stu-id="c0000-153">This method uses the sender of the original message as recipient.</span></span>

## <a name="response"></a><span data-ttu-id="c0000-154">响应</span><span class="sxs-lookup"><span data-stu-id="c0000-154">Response</span></span>

<span data-ttu-id="c0000-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c0000-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="c0000-157">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息："MIME 内容的 `400 Bad request` base64 字符串无效"。</span><span class="sxs-lookup"><span data-stu-id="c0000-157">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="c0000-158">示例</span><span class="sxs-lookup"><span data-stu-id="c0000-158">Examples</span></span>
### <a name="example-1-reply-in-json-format-to-an-existing-message"></a><span data-ttu-id="c0000-159">示例 1：以 JSON 格式答复现有邮件</span><span class="sxs-lookup"><span data-stu-id="c0000-159">Example 1: Reply in JSON format to an existing message</span></span>
<span data-ttu-id="c0000-160">以下示例包含注释，并将收件人添加到回复邮件中。</span><span class="sxs-lookup"><span data-stu-id="c0000-160">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="c0000-161">请求</span><span class="sxs-lookup"><span data-stu-id="c0000-161">Request</span></span>
<span data-ttu-id="c0000-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0000-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0000-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0000-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_reply_v1",
  "sampleKeys": ["AAMkADA1MTAAAAqldOAAA="]
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group please?" 
}
```
# <a name="c"></a>[<span data-ttu-id="c0000-164">C#</span><span class="sxs-lookup"><span data-stu-id="c0000-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0000-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0000-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0000-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0000-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0000-167">Java</span><span class="sxs-lookup"><span data-stu-id="c0000-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c0000-168">响应</span><span class="sxs-lookup"><span data-stu-id="c0000-168">Response</span></span>
<span data-ttu-id="c0000-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c0000-169">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="exaxmple-2-reply-in-mime-format-to-an-existing-message"></a><span data-ttu-id="c0000-170">Exaxmple 2：以 MIME 格式答复现有邮件</span><span class="sxs-lookup"><span data-stu-id="c0000-170">Exaxmple 2: Reply in MIME format to an existing message</span></span>
##### <a name="request"></a><span data-ttu-id="c0000-171">请求</span><span class="sxs-lookup"><span data-stu-id="c0000-171">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np
```
##### <a name="response"></a><span data-ttu-id="c0000-172">响应</span><span class="sxs-lookup"><span data-stu-id="c0000-172">Response</span></span>
<span data-ttu-id="c0000-173">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c0000-173">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="c0000-174">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="c0000-174">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

