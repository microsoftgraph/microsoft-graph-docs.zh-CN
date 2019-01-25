---
title: 发送邮件
description: 发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: afa50b466bd7a90af4fedbdad4c5f7c5b4627b8c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517209"
---
# <a name="send-mail"></a><span data-ttu-id="a10a0-104">发送邮件</span><span class="sxs-lookup"><span data-stu-id="a10a0-104">Send mail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a10a0-p102">发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="a10a0-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="a10a0-107">在同一**sendMail**操作呼叫，您可以：</span><span class="sxs-lookup"><span data-stu-id="a10a0-107">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="a10a0-108">包含[附件](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="a10a0-108">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="a10a0-109">使用[提及](../resources/mention.md)指出在新邮件中的另一个用户</span><span class="sxs-lookup"><span data-stu-id="a10a0-109">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="a10a0-110">权限</span><span class="sxs-lookup"><span data-stu-id="a10a0-110">Permissions</span></span>
<span data-ttu-id="a10a0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a10a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a10a0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a10a0-113">Permission type</span></span>      | <span data-ttu-id="a10a0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a10a0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a10a0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a10a0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a10a0-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a10a0-116">Mail.Send</span></span>    |
|<span data-ttu-id="a10a0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a10a0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a10a0-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a10a0-118">Mail.Send</span></span>    |
|<span data-ttu-id="a10a0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a10a0-119">Application</span></span> | <span data-ttu-id="a10a0-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a10a0-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="a10a0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a10a0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="a10a0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a10a0-122">Request headers</span></span>
| <span data-ttu-id="a10a0-123">标头</span><span class="sxs-lookup"><span data-stu-id="a10a0-123">Header</span></span>       | <span data-ttu-id="a10a0-124">值</span><span class="sxs-lookup"><span data-stu-id="a10a0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a10a0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a10a0-125">Authorization</span></span>  | <span data-ttu-id="a10a0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a10a0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a10a0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a10a0-128">Content-Type</span></span>  | <span data-ttu-id="a10a0-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a10a0-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a10a0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a10a0-130">Request body</span></span>
<span data-ttu-id="a10a0-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a10a0-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a10a0-132">参数</span><span class="sxs-lookup"><span data-stu-id="a10a0-132">Parameter</span></span>    | <span data-ttu-id="a10a0-133">类型</span><span class="sxs-lookup"><span data-stu-id="a10a0-133">Type</span></span>   |<span data-ttu-id="a10a0-134">说明</span><span class="sxs-lookup"><span data-stu-id="a10a0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a10a0-135">Message</span><span class="sxs-lookup"><span data-stu-id="a10a0-135">Message</span></span>|[<span data-ttu-id="a10a0-136">邮件</span><span class="sxs-lookup"><span data-stu-id="a10a0-136">Message</span></span>](../resources/message.md)|<span data-ttu-id="a10a0-p105">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="a10a0-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="a10a0-139">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="a10a0-139">SaveToSentItems</span></span>|<span data-ttu-id="a10a0-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="a10a0-140">Boolean</span></span>|<span data-ttu-id="a10a0-p106">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="a10a0-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="a10a0-144">如果您想要使用**提及**指出在新邮件中的另一个用户：</span><span class="sxs-lookup"><span data-stu-id="a10a0-144">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="a10a0-145">在请求正文中包含所需的**toRecipients**属性、**提到**属性和任何可写的邮件属性。</span><span class="sxs-lookup"><span data-stu-id="a10a0-145">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="a10a0-146">对于每个提及的**提到**属性中，您必须指定**提到**属性。</span><span class="sxs-lookup"><span data-stu-id="a10a0-146">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="a10a0-147">响应</span><span class="sxs-lookup"><span data-stu-id="a10a0-147">Response</span></span>

<span data-ttu-id="a10a0-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a10a0-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a10a0-150">示例</span><span class="sxs-lookup"><span data-stu-id="a10a0-150">Example</span></span>
<span data-ttu-id="a10a0-151">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a10a0-151">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="a10a0-152">请求 1</span><span class="sxs-lookup"><span data-stu-id="a10a0-152">Request 1</span></span>
<span data-ttu-id="a10a0-153">下面是请求的创建和发送即时消息示例。</span><span class="sxs-lookup"><span data-stu-id="a10a0-153">Here is an example of the request to create and send a message on the fly.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="a10a0-154">响应 1</span><span class="sxs-lookup"><span data-stu-id="a10a0-154">Response 1</span></span>
<span data-ttu-id="a10a0-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a10a0-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="a10a0-156">请求 2</span><span class="sxs-lookup"><span data-stu-id="a10a0-156">Request 2</span></span>
<span data-ttu-id="a10a0-157">下面的示例演示孙亭到登录用户通过一条消息。</span><span class="sxs-lookup"><span data-stu-id="a10a0-157">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="a10a0-158">此消息还包括其他用户，Dana Swope 某个提及。</span><span class="sxs-lookup"><span data-stu-id="a10a0-158">The message also includes a mention of another user, Dana Swope.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="a10a0-159">响应 2</span><span class="sxs-lookup"><span data-stu-id="a10a0-159">Response 2</span></span>
<span data-ttu-id="a10a0-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a10a0-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="a10a0-161">请求 3</span><span class="sxs-lookup"><span data-stu-id="a10a0-161">Request 3</span></span>
<span data-ttu-id="a10a0-162">下一个示例使用自定义 Internet 邮件头中创建一条消息，并将邮件发送。</span><span class="sxs-lookup"><span data-stu-id="a10a0-162">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-3"></a><span data-ttu-id="a10a0-163">响应 3</span><span class="sxs-lookup"><span data-stu-id="a10a0-163">Response 3</span></span>
<span data-ttu-id="a10a0-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a10a0-164">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
