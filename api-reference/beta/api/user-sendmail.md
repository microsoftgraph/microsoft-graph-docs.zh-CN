---
title: 发送邮件
description: 发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1d3c8592007b98a5f5e225447a7fe163c95275c6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134972"
---
# <a name="send-mail"></a><span data-ttu-id="475f4-104">发送邮件</span><span class="sxs-lookup"><span data-stu-id="475f4-104">Send mail</span></span>

<span data-ttu-id="475f4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="475f4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="475f4-p102">发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="475f4-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="475f4-108">在同一 **个 sendMail** 操作调用中，您可以：</span><span class="sxs-lookup"><span data-stu-id="475f4-108">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="475f4-109">包括 [附件](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="475f4-109">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="475f4-110">使用 [提及](../resources/mention.md) 功能在新邮件中呼叫其他用户</span><span class="sxs-lookup"><span data-stu-id="475f4-110">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="475f4-111">权限</span><span class="sxs-lookup"><span data-stu-id="475f4-111">Permissions</span></span>
<span data-ttu-id="475f4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="475f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="475f4-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="475f4-114">Permission type</span></span>      | <span data-ttu-id="475f4-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="475f4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="475f4-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="475f4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="475f4-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="475f4-117">Mail.Send</span></span>    |
|<span data-ttu-id="475f4-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="475f4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="475f4-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="475f4-119">Mail.Send</span></span>    |
|<span data-ttu-id="475f4-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="475f4-120">Application</span></span> | <span data-ttu-id="475f4-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="475f4-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="475f4-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="475f4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="475f4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="475f4-123">Request headers</span></span>
| <span data-ttu-id="475f4-124">标头</span><span class="sxs-lookup"><span data-stu-id="475f4-124">Header</span></span>       | <span data-ttu-id="475f4-125">值</span><span class="sxs-lookup"><span data-stu-id="475f4-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="475f4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="475f4-126">Authorization</span></span>  | <span data-ttu-id="475f4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="475f4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="475f4-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="475f4-129">Content-Type</span></span>  | <span data-ttu-id="475f4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="475f4-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="475f4-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="475f4-131">Request body</span></span>
<span data-ttu-id="475f4-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="475f4-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="475f4-133">参数</span><span class="sxs-lookup"><span data-stu-id="475f4-133">Parameter</span></span>    | <span data-ttu-id="475f4-134">类型</span><span class="sxs-lookup"><span data-stu-id="475f4-134">Type</span></span>   |<span data-ttu-id="475f4-135">说明</span><span class="sxs-lookup"><span data-stu-id="475f4-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="475f4-136">邮件</span><span class="sxs-lookup"><span data-stu-id="475f4-136">Message</span></span>|[<span data-ttu-id="475f4-137">Message</span><span class="sxs-lookup"><span data-stu-id="475f4-137">Message</span></span>](../resources/message.md)|<span data-ttu-id="475f4-p105">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="475f4-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="475f4-140">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="475f4-140">SaveToSentItems</span></span>|<span data-ttu-id="475f4-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="475f4-141">Boolean</span></span>|<span data-ttu-id="475f4-p106">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="475f4-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="475f4-145">如果要使用 **提及功能** 在新邮件中呼叫其他用户：</span><span class="sxs-lookup"><span data-stu-id="475f4-145">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="475f4-146">在请求正文 **中包括必需的 toRecipients** 属性 **、mentions** 属性和任何可写邮件属性。</span><span class="sxs-lookup"><span data-stu-id="475f4-146">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="475f4-147">对于提及属性中的 **每个** 提及，必须指定 **提及的** 属性。</span><span class="sxs-lookup"><span data-stu-id="475f4-147">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="475f4-148">响应</span><span class="sxs-lookup"><span data-stu-id="475f4-148">Response</span></span>

<span data-ttu-id="475f4-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="475f4-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="475f4-151">示例</span><span class="sxs-lookup"><span data-stu-id="475f4-151">Example</span></span>
<span data-ttu-id="475f4-152">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="475f4-152">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="475f4-153">请求 1</span><span class="sxs-lookup"><span data-stu-id="475f4-153">Request 1</span></span>
<span data-ttu-id="475f4-154">下面是一个立即创建和发送邮件的请求示例。</span><span class="sxs-lookup"><span data-stu-id="475f4-154">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="http"></a>[<span data-ttu-id="475f4-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="475f4-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="475f4-156">C#</span><span class="sxs-lookup"><span data-stu-id="475f4-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="475f4-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="475f4-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="475f4-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="475f4-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="475f4-159">Java</span><span class="sxs-lookup"><span data-stu-id="475f4-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="475f4-160">响应 1</span><span class="sxs-lookup"><span data-stu-id="475f4-160">Response 1</span></span>
<span data-ttu-id="475f4-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="475f4-161">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="475f4-162">请求 2</span><span class="sxs-lookup"><span data-stu-id="475f4-162">Request 2</span></span>
<span data-ttu-id="475f4-163">下一个示例显示登录用户向 Samantha 一封邮件。</span><span class="sxs-lookup"><span data-stu-id="475f4-163">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="475f4-164">邮件还包括另一个用户 Dana Swope 的提及内容。</span><span class="sxs-lookup"><span data-stu-id="475f4-164">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="http"></a>[<span data-ttu-id="475f4-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="475f4-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="475f4-166">C#</span><span class="sxs-lookup"><span data-stu-id="475f4-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="475f4-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="475f4-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="475f4-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="475f4-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="475f4-169">Java</span><span class="sxs-lookup"><span data-stu-id="475f4-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="475f4-170">响应 2</span><span class="sxs-lookup"><span data-stu-id="475f4-170">Response 2</span></span>
<span data-ttu-id="475f4-171">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="475f4-171">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="475f4-172">请求 3</span><span class="sxs-lookup"><span data-stu-id="475f4-172">Request 3</span></span>
<span data-ttu-id="475f4-173">以下示例将创建一个带 Internet 消息标头的消息并进行发送。</span><span class="sxs-lookup"><span data-stu-id="475f4-173">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="http"></a>[<span data-ttu-id="475f4-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="475f4-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="475f4-175">C#</span><span class="sxs-lookup"><span data-stu-id="475f4-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="475f4-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="475f4-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="475f4-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="475f4-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="475f4-178">Java</span><span class="sxs-lookup"><span data-stu-id="475f4-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="475f4-179">响应 3</span><span class="sxs-lookup"><span data-stu-id="475f4-179">Response 3</span></span>
<span data-ttu-id="475f4-180">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="475f4-180">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-4"></a><span data-ttu-id="475f4-181">请求 4</span><span class="sxs-lookup"><span data-stu-id="475f4-181">Request 4</span></span>

<span data-ttu-id="475f4-182">下一个示例将创建包含文件附件的邮件并发送该邮件。</span><span class="sxs-lookup"><span data-stu-id="475f4-182">The next example creates a message with a file attachment and sends the message.</span></span>


# <a name="http"></a>[<span data-ttu-id="475f4-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="475f4-183">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="475f4-184">C#</span><span class="sxs-lookup"><span data-stu-id="475f4-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="475f4-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="475f4-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="475f4-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="475f4-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="475f4-187">Java</span><span class="sxs-lookup"><span data-stu-id="475f4-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-4"></a><span data-ttu-id="475f4-188">响应 4</span><span class="sxs-lookup"><span data-stu-id="475f4-188">Response 4</span></span>

<span data-ttu-id="475f4-189">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="475f4-189">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
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


