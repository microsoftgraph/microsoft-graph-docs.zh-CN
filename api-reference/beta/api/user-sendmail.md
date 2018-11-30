---
title: 发送邮件
description: 发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。
ms.openlocfilehash: 8103a1f0b4004e602c23d114e199b60fa96c15e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048634"
---
# <a name="send-mail"></a><span data-ttu-id="cd26f-104">发送邮件</span><span class="sxs-lookup"><span data-stu-id="cd26f-104">Send mail</span></span>

> <span data-ttu-id="cd26f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cd26f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd26f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cd26f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd26f-p103">发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="cd26f-p103">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="cd26f-109">在同一**sendMail**操作呼叫，您可以：</span><span class="sxs-lookup"><span data-stu-id="cd26f-109">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="cd26f-110">包含[附件](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="cd26f-110">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="cd26f-111">使用[提及](../resources/mention.md)指出在新邮件中的另一个用户</span><span class="sxs-lookup"><span data-stu-id="cd26f-111">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="cd26f-112">权限</span><span class="sxs-lookup"><span data-stu-id="cd26f-112">Permissions</span></span>
<span data-ttu-id="cd26f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd26f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cd26f-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd26f-115">Permission type</span></span>      | <span data-ttu-id="cd26f-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd26f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd26f-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd26f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="cd26f-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cd26f-118">Mail.Send</span></span>    |
|<span data-ttu-id="cd26f-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd26f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd26f-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cd26f-120">Mail.Send</span></span>    |
|<span data-ttu-id="cd26f-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd26f-121">Application</span></span> | <span data-ttu-id="cd26f-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cd26f-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd26f-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd26f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="cd26f-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd26f-124">Request headers</span></span>
| <span data-ttu-id="cd26f-125">标头</span><span class="sxs-lookup"><span data-stu-id="cd26f-125">Header</span></span>       | <span data-ttu-id="cd26f-126">值</span><span class="sxs-lookup"><span data-stu-id="cd26f-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cd26f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd26f-127">Authorization</span></span>  | <span data-ttu-id="cd26f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd26f-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd26f-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd26f-130">Content-Type</span></span>  | <span data-ttu-id="cd26f-131">application/json</span><span class="sxs-lookup"><span data-stu-id="cd26f-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd26f-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd26f-132">Request body</span></span>
<span data-ttu-id="cd26f-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cd26f-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cd26f-134">参数</span><span class="sxs-lookup"><span data-stu-id="cd26f-134">Parameter</span></span>    | <span data-ttu-id="cd26f-135">类型</span><span class="sxs-lookup"><span data-stu-id="cd26f-135">Type</span></span>   |<span data-ttu-id="cd26f-136">说明</span><span class="sxs-lookup"><span data-stu-id="cd26f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd26f-137">Message</span><span class="sxs-lookup"><span data-stu-id="cd26f-137">Message</span></span>|[<span data-ttu-id="cd26f-138">邮件</span><span class="sxs-lookup"><span data-stu-id="cd26f-138">Message</span></span>](../resources/message.md)|<span data-ttu-id="cd26f-p106">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="cd26f-p106">The message to send. Required.</span></span>|
|<span data-ttu-id="cd26f-141">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="cd26f-141">SaveToSentItems</span></span>|<span data-ttu-id="cd26f-142">布尔</span><span class="sxs-lookup"><span data-stu-id="cd26f-142">Boolean</span></span>|<span data-ttu-id="cd26f-p107">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="cd26f-p107">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="cd26f-146">如果您想要使用**提及**指出在新邮件中的另一个用户：</span><span class="sxs-lookup"><span data-stu-id="cd26f-146">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="cd26f-147">在请求正文中包含所需的**toRecipients**属性、**提到**属性和任何可写的邮件属性。</span><span class="sxs-lookup"><span data-stu-id="cd26f-147">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="cd26f-148">对于每个提及的**提到**属性中，您必须指定**提到**属性。</span><span class="sxs-lookup"><span data-stu-id="cd26f-148">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="cd26f-149">响应</span><span class="sxs-lookup"><span data-stu-id="cd26f-149">Response</span></span>

<span data-ttu-id="cd26f-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cd26f-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd26f-152">示例</span><span class="sxs-lookup"><span data-stu-id="cd26f-152">Example</span></span>
<span data-ttu-id="cd26f-153">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="cd26f-153">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="cd26f-154">请求 1</span><span class="sxs-lookup"><span data-stu-id="cd26f-154">Request 1</span></span>
<span data-ttu-id="cd26f-155">下面是请求的创建和发送即时消息示例。</span><span class="sxs-lookup"><span data-stu-id="cd26f-155">Here is an example of the request to create and send a message on the fly.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="cd26f-156">响应 1</span><span class="sxs-lookup"><span data-stu-id="cd26f-156">Response 1</span></span>
<span data-ttu-id="cd26f-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cd26f-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="cd26f-158">请求 2</span><span class="sxs-lookup"><span data-stu-id="cd26f-158">Request 2</span></span>
<span data-ttu-id="cd26f-159">下面的示例演示孙亭到登录用户通过一条消息。</span><span class="sxs-lookup"><span data-stu-id="cd26f-159">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="cd26f-160">此消息还包括其他用户，Dana Swope 某个提及。</span><span class="sxs-lookup"><span data-stu-id="cd26f-160">The message also includes a mention of another user, Dana Swope.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="cd26f-161">响应 2</span><span class="sxs-lookup"><span data-stu-id="cd26f-161">Response 2</span></span>
<span data-ttu-id="cd26f-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cd26f-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="cd26f-163">请求 3</span><span class="sxs-lookup"><span data-stu-id="cd26f-163">Request 3</span></span>
<span data-ttu-id="cd26f-164">下一个示例使用自定义 Internet 邮件头中创建一条消息，并将邮件发送。</span><span class="sxs-lookup"><span data-stu-id="cd26f-164">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-3"></a><span data-ttu-id="cd26f-165">响应 3</span><span class="sxs-lookup"><span data-stu-id="cd26f-165">Response 3</span></span>
<span data-ttu-id="cd26f-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cd26f-166">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
