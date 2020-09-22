---
title: 发送邮件
description: 发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5ecfb05e3808c18a7dad79cb8a1512598927857f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064442"
---
# <a name="send-mail"></a><span data-ttu-id="4a599-104">发送邮件</span><span class="sxs-lookup"><span data-stu-id="4a599-104">Send mail</span></span>

<span data-ttu-id="4a599-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a599-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a599-p102">发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="4a599-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="4a599-108">在同一 **sendMail** 操作调用中，可以执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="4a599-108">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="4a599-109">包含 [附件](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="4a599-109">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="4a599-110">在新邮件中使用 [提及](../resources/mention.md) 调用其他用户</span><span class="sxs-lookup"><span data-stu-id="4a599-110">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="4a599-111">权限</span><span class="sxs-lookup"><span data-stu-id="4a599-111">Permissions</span></span>
<span data-ttu-id="4a599-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a599-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4a599-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a599-114">Permission type</span></span>      | <span data-ttu-id="4a599-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a599-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a599-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a599-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4a599-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4a599-117">Mail.Send</span></span>    |
|<span data-ttu-id="4a599-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a599-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a599-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4a599-119">Mail.Send</span></span>    |
|<span data-ttu-id="4a599-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a599-120">Application</span></span> | <span data-ttu-id="4a599-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4a599-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a599-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a599-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="4a599-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a599-123">Request headers</span></span>
| <span data-ttu-id="4a599-124">标头</span><span class="sxs-lookup"><span data-stu-id="4a599-124">Header</span></span>       | <span data-ttu-id="4a599-125">值</span><span class="sxs-lookup"><span data-stu-id="4a599-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a599-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a599-126">Authorization</span></span>  | <span data-ttu-id="4a599-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4a599-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4a599-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a599-129">Content-Type</span></span>  | <span data-ttu-id="4a599-130">application/json</span><span class="sxs-lookup"><span data-stu-id="4a599-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a599-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a599-131">Request body</span></span>
<span data-ttu-id="4a599-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4a599-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4a599-133">参数</span><span class="sxs-lookup"><span data-stu-id="4a599-133">Parameter</span></span>    | <span data-ttu-id="4a599-134">类型</span><span class="sxs-lookup"><span data-stu-id="4a599-134">Type</span></span>   |<span data-ttu-id="4a599-135">说明</span><span class="sxs-lookup"><span data-stu-id="4a599-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a599-136">邮件</span><span class="sxs-lookup"><span data-stu-id="4a599-136">Message</span></span>|[<span data-ttu-id="4a599-137">Message</span><span class="sxs-lookup"><span data-stu-id="4a599-137">Message</span></span>](../resources/message.md)|<span data-ttu-id="4a599-p105">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="4a599-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="4a599-140">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="4a599-140">SaveToSentItems</span></span>|<span data-ttu-id="4a599-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a599-141">Boolean</span></span>|<span data-ttu-id="4a599-p106">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="4a599-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="4a599-145">如果要使用 **提及** 在新邮件中呼叫其他用户，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="4a599-145">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="4a599-146">在请求正文中包括所需的 **toRecipients** 属性、 **提及** 属性和任何可写邮件属性。</span><span class="sxs-lookup"><span data-stu-id="4a599-146">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="4a599-147">对于 **提及** 属性中的每个提及，您必须指定 **提到** 的属性。</span><span class="sxs-lookup"><span data-stu-id="4a599-147">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="4a599-148">响应</span><span class="sxs-lookup"><span data-stu-id="4a599-148">Response</span></span>

<span data-ttu-id="4a599-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4a599-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a599-151">示例</span><span class="sxs-lookup"><span data-stu-id="4a599-151">Example</span></span>
<span data-ttu-id="4a599-152">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4a599-152">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="4a599-153">请求 1</span><span class="sxs-lookup"><span data-stu-id="4a599-153">Request 1</span></span>
<span data-ttu-id="4a599-154">下面的示例展示了在即时创建和发送邮件的请求。</span><span class="sxs-lookup"><span data-stu-id="4a599-154">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a599-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a599-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4a599-156">C#</span><span class="sxs-lookup"><span data-stu-id="4a599-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a599-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a599-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a599-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a599-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="4a599-159">响应 1</span><span class="sxs-lookup"><span data-stu-id="4a599-159">Response 1</span></span>
<span data-ttu-id="4a599-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4a599-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="4a599-161">请求 2</span><span class="sxs-lookup"><span data-stu-id="4a599-161">Request 2</span></span>
<span data-ttu-id="4a599-162">下一个示例显示了登录用户 Samantha 展台的邮件。</span><span class="sxs-lookup"><span data-stu-id="4a599-162">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="4a599-163">此外，该消息还包括其他用户 Dana Swope。</span><span class="sxs-lookup"><span data-stu-id="4a599-163">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a599-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a599-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4a599-165">C#</span><span class="sxs-lookup"><span data-stu-id="4a599-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a599-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a599-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a599-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a599-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="4a599-168">响应 2</span><span class="sxs-lookup"><span data-stu-id="4a599-168">Response 2</span></span>
<span data-ttu-id="4a599-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4a599-169">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="4a599-170">请求 3</span><span class="sxs-lookup"><span data-stu-id="4a599-170">Request 3</span></span>
<span data-ttu-id="4a599-171">以下示例将创建一个带 Internet 消息标头的消息并进行发送。</span><span class="sxs-lookup"><span data-stu-id="4a599-171">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a599-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a599-172">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4a599-173">C#</span><span class="sxs-lookup"><span data-stu-id="4a599-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a599-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a599-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a599-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a599-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="4a599-176">响应 3</span><span class="sxs-lookup"><span data-stu-id="4a599-176">Response 3</span></span>
<span data-ttu-id="4a599-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4a599-177">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-4"></a><span data-ttu-id="4a599-178">请求 4</span><span class="sxs-lookup"><span data-stu-id="4a599-178">Request 4</span></span>

<span data-ttu-id="4a599-179">下一个示例将创建包含文件附件的邮件并发送该邮件。</span><span class="sxs-lookup"><span data-stu-id="4a599-179">The next example creates a message with a file attachment and sends the message.</span></span>


# <a name="http"></a>[<span data-ttu-id="4a599-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a599-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4a599-181">C#</span><span class="sxs-lookup"><span data-stu-id="4a599-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a599-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a599-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a599-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a599-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-4"></a><span data-ttu-id="4a599-184">响应 4</span><span class="sxs-lookup"><span data-stu-id="4a599-184">Response 4</span></span>

<span data-ttu-id="4a599-185">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4a599-185">Here is an example of the response.</span></span>
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


