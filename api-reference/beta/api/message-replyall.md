---
title: 消息：replyAll
description: 使用 JSON 或 MIME 格式答复邮件的所有收件人。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 723aa43863e7da80b7be87c92b6f553463f28e86
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645358"
---
# <a name="message-replyall"></a><span data-ttu-id="f7d6d-103">消息：replyAll</span><span class="sxs-lookup"><span data-stu-id="f7d6d-103">message: replyAll</span></span>

<span data-ttu-id="f7d6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7d6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7d6d-105">使用 JSON 或 MIME [格式](../resources/message.md) 答复邮件的所有收件人。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-105">Reply to all recipients of a [message](../resources/message.md) using either JSON or MIME format.</span></span>

<span data-ttu-id="f7d6d-106">使用 JSON 格式时：</span><span class="sxs-lookup"><span data-stu-id="f7d6d-106">When using JSON format:</span></span>
- <span data-ttu-id="f7d6d-107">指定参数的 comment 或 **body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="f7d6d-108">指定这两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="f7d6d-109">如果原始邮件在 **replyTo** 属性中指定收件人，则根据 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ，将答复发送给 **replyTo** 中的收件人，而不是 **from** 属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span>

<span data-ttu-id="f7d6d-110">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="f7d6d-110">When using MIME format:</span></span>
- <span data-ttu-id="f7d6d-111">在请求正文中提供适用的 [Internet](https://tools.ietf.org/html/rfc2076) 邮件头和 [MIME](https://tools.ietf.org/html/rfc2045)内容，这些内容均以 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-111">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="f7d6d-112">将任何附件和 S/MIME 属性添加到 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-112">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="f7d6d-113">此方法将邮件保存在"已发送 **的项目"** 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-113">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="f7d6d-114">或者， [创建一个草稿以全部答复邮件](../api/message-createreplyall.md)， [并稍后](../api/message-send.md) 发送。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-114">Alternatively, [create a draft to reply-all to a message](../api/message-createreplyall.md), and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7d6d-115">权限</span><span class="sxs-lookup"><span data-stu-id="f7d6d-115">Permissions</span></span>
<span data-ttu-id="f7d6d-116">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-116">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="f7d6d-117">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-117">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7d6d-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7d6d-118">Permission type</span></span>      | <span data-ttu-id="f7d6d-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7d6d-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7d6d-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7d6d-120">Delegated (work or school account)</span></span> | <span data-ttu-id="f7d6d-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f7d6d-121">Mail.Send</span></span>    |
|<span data-ttu-id="f7d6d-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7d6d-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7d6d-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f7d6d-123">Mail.Send</span></span>    |
|<span data-ttu-id="f7d6d-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7d6d-124">Application</span></span> | <span data-ttu-id="f7d6d-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f7d6d-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7d6d-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7d6d-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="f7d6d-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7d6d-127">Request headers</span></span>
| <span data-ttu-id="f7d6d-128">名称</span><span class="sxs-lookup"><span data-stu-id="f7d6d-128">Name</span></span>       | <span data-ttu-id="f7d6d-129">类型</span><span class="sxs-lookup"><span data-stu-id="f7d6d-129">Type</span></span> | <span data-ttu-id="f7d6d-130">说明</span><span class="sxs-lookup"><span data-stu-id="f7d6d-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7d6d-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7d6d-131">Authorization</span></span>  | <span data-ttu-id="f7d6d-132">string</span><span class="sxs-lookup"><span data-stu-id="f7d6d-132">string</span></span>  | <span data-ttu-id="f7d6d-133">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-133">Bearer {token}.</span></span> <span data-ttu-id="f7d6d-134">必需</span><span class="sxs-lookup"><span data-stu-id="f7d6d-134">Required</span></span>|
| <span data-ttu-id="f7d6d-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7d6d-135">Content-Type</span></span> | <span data-ttu-id="f7d6d-136">string</span><span class="sxs-lookup"><span data-stu-id="f7d6d-136">string</span></span>  | <span data-ttu-id="f7d6d-137">实体正文中的数据性质。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-137">Nature of the data in the body of an entity.</span></span> <span data-ttu-id="f7d6d-138">必需</span><span class="sxs-lookup"><span data-stu-id="f7d6d-138">Required</span></span> <br/> <span data-ttu-id="f7d6d-139">用于 `application/json` JSON 对象和 `text/plain` MIME 内容</span><span class="sxs-lookup"><span data-stu-id="f7d6d-139">Use `application/json` for a JSON object and `text/plain` for MIME content</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7d6d-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7d6d-140">Request body</span></span>
<span data-ttu-id="f7d6d-141">使用 JSON 格式时，请提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-141">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7d6d-142">参数</span><span class="sxs-lookup"><span data-stu-id="f7d6d-142">Parameter</span></span>    | <span data-ttu-id="f7d6d-143">类型</span><span class="sxs-lookup"><span data-stu-id="f7d6d-143">Type</span></span>   |<span data-ttu-id="f7d6d-144">说明</span><span class="sxs-lookup"><span data-stu-id="f7d6d-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7d6d-145">注释</span><span class="sxs-lookup"><span data-stu-id="f7d6d-145">comment</span></span>|<span data-ttu-id="f7d6d-146">String</span><span class="sxs-lookup"><span data-stu-id="f7d6d-146">String</span></span>|<span data-ttu-id="f7d6d-p105">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="f7d6d-149">message</span><span class="sxs-lookup"><span data-stu-id="f7d6d-149">message</span></span>|[<span data-ttu-id="f7d6d-150">message</span><span class="sxs-lookup"><span data-stu-id="f7d6d-150">message</span></span>](../resources/message.md)|<span data-ttu-id="f7d6d-151">回复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-151">Any writeable properties to update in the reply message.</span></span>|

<span data-ttu-id="f7d6d-152">指定 MIME 格式的正文时，请提供 MIME 内容以及适用的 Internet 邮件头，所有邮件头在请求正文中都以 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-152">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span> <span data-ttu-id="f7d6d-153">此方法将原始邮件的发件人及所有收件人加载为新邮件的收件人。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-153">This method loads the sender and all recipients of the original message as recipients of the new message.</span></span>

## <a name="response"></a><span data-ttu-id="f7d6d-154">响应</span><span class="sxs-lookup"><span data-stu-id="f7d6d-154">Response</span></span>

<span data-ttu-id="f7d6d-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="f7d6d-157">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息："MIME 内容的 `400 Bad request` base64 字符串无效"。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-157">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="f7d6d-158">示例</span><span class="sxs-lookup"><span data-stu-id="f7d6d-158">Examples</span></span>
### <a name="example-1-reply-all-to-a-message-in-json-format"></a><span data-ttu-id="f7d6d-159">示例 1：以 JSON 格式全部答复邮件</span><span class="sxs-lookup"><span data-stu-id="f7d6d-159">Example 1: Reply-all to a message in JSON format</span></span>
<span data-ttu-id="f7d6d-160">以下示例包含注释并将附件添加到全部答复邮件。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-160">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="f7d6d-161">请求</span><span class="sxs-lookup"><span data-stu-id="f7d6d-161">Request</span></span>
<span data-ttu-id="f7d6d-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7d6d-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7d6d-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
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
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```
# <a name="c"></a>[<span data-ttu-id="f7d6d-164">C#</span><span class="sxs-lookup"><span data-stu-id="f7d6d-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7d6d-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7d6d-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7d6d-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7d6d-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7d6d-167">Java</span><span class="sxs-lookup"><span data-stu-id="f7d6d-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f7d6d-168">响应</span><span class="sxs-lookup"><span data-stu-id="f7d6d-168">Response</span></span>
<span data-ttu-id="f7d6d-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-169">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reply-all-to-a-message-in-mime-format"></a><span data-ttu-id="f7d6d-170">示例 2：以 MIME 格式全部答复邮件</span><span class="sxs-lookup"><span data-stu-id="f7d6d-170">Example 2: Reply-all to a message in MIME format</span></span>
##### <a name="request"></a><span data-ttu-id="f7d6d-171">请求</span><span class="sxs-lookup"><span data-stu-id="f7d6d-171">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "message_replyAll_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/replyAll
Content-Type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM...

```

##### <a name="response"></a><span data-ttu-id="f7d6d-172">响应</span><span class="sxs-lookup"><span data-stu-id="f7d6d-172">Response</span></span>
<span data-ttu-id="f7d6d-173">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-173">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="f7d6d-174">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="f7d6d-174">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


