---
title: 发送邮件
description: 使用 JSON 或 MIME 格式发送请求正文中指定的邮件。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5ee3bc0682f6611a06cb5e24e66b2c665a0be123
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645638"
---
# <a name="send-mail"></a><span data-ttu-id="ee884-103">发送邮件</span><span class="sxs-lookup"><span data-stu-id="ee884-103">Send mail</span></span>

<span data-ttu-id="ee884-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee884-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee884-105">使用 JSON 或 MIME 格式发送请求正文中指定的邮件。</span><span class="sxs-lookup"><span data-stu-id="ee884-105">Send the message specified in the request body using either JSON or MIME format.</span></span>

<span data-ttu-id="ee884-106">使用 JSON 格式时，可以[包括附件并使用](../resources/attachment.md)[提及](../resources/mention.md)功能在新邮件中呼叫其他用户。</span><span class="sxs-lookup"><span data-stu-id="ee884-106">When using JSON format you can include an [attachment](../resources/attachment.md) and use a [mention](../resources/mention.md) to call out another user in the new message.</span></span>

<span data-ttu-id="ee884-107">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="ee884-107">When using MIME format:</span></span>
- <span data-ttu-id="ee884-108">在请求正文中提供适用的 [Internet](https://tools.ietf.org/html/rfc2076) 邮件头和 [MIME](https://tools.ietf.org/html/rfc2045)内容，这些内容均以 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="ee884-108">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="ee884-109">将任何附件和 S/MIME 属性添加到 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="ee884-109">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="ee884-110">此方法将邮件保存在"已发送 **的项目"** 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="ee884-110">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="ee884-111">或者， [创建草稿邮件以](../api/user-post-messages.md) 稍后发送。</span><span class="sxs-lookup"><span data-stu-id="ee884-111">Alternatively, [create a draft message](../api/user-post-messages.md) to send later.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee884-112">权限</span><span class="sxs-lookup"><span data-stu-id="ee884-112">Permissions</span></span>
<span data-ttu-id="ee884-113">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="ee884-113">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="ee884-114">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee884-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee884-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee884-115">Permission type</span></span>      | <span data-ttu-id="ee884-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee884-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee884-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee884-117">Delegated (work or school account)</span></span> | <span data-ttu-id="ee884-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ee884-118">Mail.Send</span></span>    |
|<span data-ttu-id="ee884-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee884-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee884-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ee884-120">Mail.Send</span></span>    |
|<span data-ttu-id="ee884-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee884-121">Application</span></span> | <span data-ttu-id="ee884-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ee884-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee884-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee884-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```

## <a name="request-headers"></a><span data-ttu-id="ee884-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee884-124">Request headers</span></span>
| <span data-ttu-id="ee884-125">名称</span><span class="sxs-lookup"><span data-stu-id="ee884-125">Name</span></span>       | <span data-ttu-id="ee884-126">类型</span><span class="sxs-lookup"><span data-stu-id="ee884-126">Type</span></span> | <span data-ttu-id="ee884-127">说明</span><span class="sxs-lookup"><span data-stu-id="ee884-127">Description</span></span>| 
|:---------------|:--------|:----------
| <span data-ttu-id="ee884-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee884-128">Authorization</span></span>  | <span data-ttu-id="ee884-129">string</span><span class="sxs-lookup"><span data-stu-id="ee884-129">string</span></span>  | <span data-ttu-id="ee884-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee884-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ee884-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee884-132">Content-Type</span></span> | <span data-ttu-id="ee884-133">string</span><span class="sxs-lookup"><span data-stu-id="ee884-133">string</span></span>  | <span data-ttu-id="ee884-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="ee884-p103">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="ee884-136">用于 `application/json` JSON 对象和 `text/plain` MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="ee884-136">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee884-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee884-137">Request body</span></span>
<span data-ttu-id="ee884-138">使用 JSON 格式时，请提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ee884-138">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ee884-139">参数</span><span class="sxs-lookup"><span data-stu-id="ee884-139">Parameter</span></span>    | <span data-ttu-id="ee884-140">类型</span><span class="sxs-lookup"><span data-stu-id="ee884-140">Type</span></span>   |<span data-ttu-id="ee884-141">说明</span><span class="sxs-lookup"><span data-stu-id="ee884-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee884-142">邮件</span><span class="sxs-lookup"><span data-stu-id="ee884-142">Message</span></span>|[<span data-ttu-id="ee884-143">Message</span><span class="sxs-lookup"><span data-stu-id="ee884-143">Message</span></span>](../resources/message.md)|<span data-ttu-id="ee884-p104">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="ee884-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="ee884-146">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="ee884-146">SaveToSentItems</span></span>|<span data-ttu-id="ee884-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee884-147">Boolean</span></span>|<span data-ttu-id="ee884-p105">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="ee884-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="ee884-151">若要使用 **提及** 功能在新邮件中呼叫其他用户，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="ee884-151">To use **mention** to call out another user in the new message:</span></span>
- <span data-ttu-id="ee884-152">在请求 **正文中包括必需的 toRecipients** 属性 **、mentions** 属性和任何可写邮件属性。</span><span class="sxs-lookup"><span data-stu-id="ee884-152">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="ee884-153">对于 **mentions** 属性中的每个提及，必须指定 **提及的** 属性。</span><span class="sxs-lookup"><span data-stu-id="ee884-153">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="ee884-154">指定 MIME 格式的正文时，在请求正文中将 MIME 内容作为 **base64** 编码的字符串提供。</span><span class="sxs-lookup"><span data-stu-id="ee884-154">When specifying the body in MIME format, provide the MIME content as **a base64-encoded string** in the request body.</span></span> <span data-ttu-id="ee884-155">不包括参数。</span><span class="sxs-lookup"><span data-stu-id="ee884-155">Do not include parameters.</span></span>

## <a name="response"></a><span data-ttu-id="ee884-156">响应</span><span class="sxs-lookup"><span data-stu-id="ee884-156">Response</span></span>

<span data-ttu-id="ee884-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ee884-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="ee884-159">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息："MIME 内容的 `400 Bad request` base64 字符串无效"。</span><span class="sxs-lookup"><span data-stu-id="ee884-159">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="ee884-160">示例</span><span class="sxs-lookup"><span data-stu-id="ee884-160">Examples</span></span>
### <a name="example-1-send-a-new-email-using-json-format"></a><span data-ttu-id="ee884-161">示例 1：使用 JSON 格式发送新电子邮件</span><span class="sxs-lookup"><span data-stu-id="ee884-161">Example 1: Send a new email using JSON format</span></span>
<span data-ttu-id="ee884-162">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ee884-162">Here is an example of how to call this API.</span></span>
#### <a name="request"></a><span data-ttu-id="ee884-163">请求</span><span class="sxs-lookup"><span data-stu-id="ee884-163">Request</span></span>
<span data-ttu-id="ee884-164">下面是一个请求立即创建和发送邮件的示例。</span><span class="sxs-lookup"><span data-stu-id="ee884-164">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee884-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee884-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 512

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "samanthab@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```
# <a name="c"></a>[<span data-ttu-id="ee884-166">C#</span><span class="sxs-lookup"><span data-stu-id="ee884-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee884-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee884-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee884-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee884-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee884-169">Java</span><span class="sxs-lookup"><span data-stu-id="ee884-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ee884-170">响应</span><span class="sxs-lookup"><span data-stu-id="ee884-170">Response</span></span>
<span data-ttu-id="ee884-171">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ee884-171">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-send-a-message-that-includes-an--mention"></a><span data-ttu-id="ee884-172">示例 2：发送包含 @-mention 的邮件</span><span class="sxs-lookup"><span data-stu-id="ee884-172">Example 2: Send a message that includes an @-mention</span></span>
#### <a name="request"></a><span data-ttu-id="ee884-173">请求</span><span class="sxs-lookup"><span data-stu-id="ee884-173">Request</span></span>
<span data-ttu-id="ee884-174">下一个示例显示已登录用户向 Samantha 的一条消息。</span><span class="sxs-lookup"><span data-stu-id="ee884-174">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="ee884-175">邮件还包括另一个用户 Dana Swope 的提及。</span><span class="sxs-lookup"><span data-stu-id="ee884-175">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee884-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee884-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_mentions"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 344

{
  "Message": {
    "subject": "Project kickoff",
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
}
```

# <a name="c"></a>[<span data-ttu-id="ee884-177">C#</span><span class="sxs-lookup"><span data-stu-id="ee884-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee884-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee884-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee884-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee884-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee884-180">Java</span><span class="sxs-lookup"><span data-stu-id="ee884-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ee884-181">响应</span><span class="sxs-lookup"><span data-stu-id="ee884-181">Response</span></span>
<span data-ttu-id="ee884-182">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ee884-182">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-send-a-message-that-includes-custom-internet-message-headers"></a><span data-ttu-id="ee884-183">示例 3：发送包含自定义 Internet 邮件头的邮件</span><span class="sxs-lookup"><span data-stu-id="ee884-183">Example 3: Send a message that includes custom Internet message headers</span></span> 
#### <a name="request"></a><span data-ttu-id="ee884-184">请求</span><span class="sxs-lookup"><span data-stu-id="ee884-184">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ee884-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee884-185">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->

```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "9/9/2018: concert",
    "body": {
      "contentType": "HTML",
      "content": "The group represents Nevada."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    ],
    "internetMessageHeaders":[
      {
        "name":"x-custom-header-group-name",
        "value":"Nevada"
      },
      {
        "name":"x-custom-header-group-id",
        "value":"NV001"
      }
    ]
  }
}
```

# <a name="c"></a>[<span data-ttu-id="ee884-186">C#</span><span class="sxs-lookup"><span data-stu-id="ee884-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee884-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee884-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee884-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee884-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee884-189">Java</span><span class="sxs-lookup"><span data-stu-id="ee884-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ee884-190">响应</span><span class="sxs-lookup"><span data-stu-id="ee884-190">Response</span></span>
<span data-ttu-id="ee884-191">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ee884-191">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-4-sends-a-message-with-a-file-attachment"></a><span data-ttu-id="ee884-192">示例 4：发送包含文件附件的邮件</span><span class="sxs-lookup"><span data-stu-id="ee884-192">Example 4: Sends a message with a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="ee884-193">请求</span><span class="sxs-lookup"><span data-stu-id="ee884-193">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ee884-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee884-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_attachment"
}-->

```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "meganb@contoso.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "#microsoft.graph.fileAttachment",
        "name": "attachment.txt",
        "contentType": "text/plain",
        "contentBytes": "SGVsbG8gV29ybGQh"
      }
    ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="ee884-195">C#</span><span class="sxs-lookup"><span data-stu-id="ee884-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee884-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee884-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee884-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee884-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee884-198">Java</span><span class="sxs-lookup"><span data-stu-id="ee884-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ee884-199">响应</span><span class="sxs-lookup"><span data-stu-id="ee884-199">Response</span></span>

<span data-ttu-id="ee884-200">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ee884-200">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```
### <a name="example-5-send-a-new-message-using-mime-format"></a><span data-ttu-id="ee884-201">示例 5：使用 MIME 格式发送新邮件</span><span class="sxs-lookup"><span data-stu-id="ee884-201">Example 5: Send a new message using MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="ee884-202">请求</span><span class="sxs-lookup"><span data-stu-id="ee884-202">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "message_send_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCArMDAwMApNZXNzYWdlLUlEOgoJPE1XSFBSMTMw
MU1CMjAwMDAwMDAwRDc2RDlDMjgyMjAwMDA5QUQ5QTlASFdIUFIxMzAxTUIwMDAwLmNvZGVudW0u
cHJvZC5vdXRsb29rLmNvbT4KQ29udGVudC1MYW5ndWFnZTogZW4tVVMKWC1NUy1IYXMtQXR0YWNo
OgpYLU1TLVRORUYtQ29ycmVsYXRvcjoKWC1NUy1Fe
```
#### <a name="response"></a><span data-ttu-id="ee884-203">响应</span><span class="sxs-lookup"><span data-stu-id="ee884-203">Response</span></span>
<span data-ttu-id="ee884-204">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ee884-204">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="ee884-205">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="ee884-205">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
