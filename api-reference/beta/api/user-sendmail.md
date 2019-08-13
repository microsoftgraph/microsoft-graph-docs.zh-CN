---
title: 发送邮件
description: 发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 806dbeff7540be3d31d63e9f685d797feb266650
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325909"
---
# <a name="send-mail"></a><span data-ttu-id="29832-104">发送邮件</span><span class="sxs-lookup"><span data-stu-id="29832-104">Send mail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29832-p102">发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="29832-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="29832-107">在同一**sendMail**操作调用中, 可以执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="29832-107">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="29832-108">包含[附件](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="29832-108">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="29832-109">在新邮件中使用[提及](../resources/mention.md)调用其他用户</span><span class="sxs-lookup"><span data-stu-id="29832-109">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="29832-110">权限</span><span class="sxs-lookup"><span data-stu-id="29832-110">Permissions</span></span>
<span data-ttu-id="29832-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29832-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="29832-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="29832-113">Permission type</span></span>      | <span data-ttu-id="29832-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29832-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29832-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29832-115">Delegated (work or school account)</span></span> | <span data-ttu-id="29832-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="29832-116">Mail.Send</span></span>    |
|<span data-ttu-id="29832-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29832-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29832-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="29832-118">Mail.Send</span></span>    |
|<span data-ttu-id="29832-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="29832-119">Application</span></span> | <span data-ttu-id="29832-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="29832-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="29832-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29832-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="29832-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="29832-122">Request headers</span></span>
| <span data-ttu-id="29832-123">标头</span><span class="sxs-lookup"><span data-stu-id="29832-123">Header</span></span>       | <span data-ttu-id="29832-124">值</span><span class="sxs-lookup"><span data-stu-id="29832-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29832-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="29832-125">Authorization</span></span>  | <span data-ttu-id="29832-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29832-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="29832-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29832-128">Content-Type</span></span>  | <span data-ttu-id="29832-129">application/json</span><span class="sxs-lookup"><span data-stu-id="29832-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29832-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="29832-130">Request body</span></span>
<span data-ttu-id="29832-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="29832-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="29832-132">参数</span><span class="sxs-lookup"><span data-stu-id="29832-132">Parameter</span></span>    | <span data-ttu-id="29832-133">类型</span><span class="sxs-lookup"><span data-stu-id="29832-133">Type</span></span>   |<span data-ttu-id="29832-134">说明</span><span class="sxs-lookup"><span data-stu-id="29832-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29832-135">邮件</span><span class="sxs-lookup"><span data-stu-id="29832-135">Message</span></span>|[<span data-ttu-id="29832-136">Message</span><span class="sxs-lookup"><span data-stu-id="29832-136">Message</span></span>](../resources/message.md)|<span data-ttu-id="29832-p105">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="29832-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="29832-139">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="29832-139">SaveToSentItems</span></span>|<span data-ttu-id="29832-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="29832-140">Boolean</span></span>|<span data-ttu-id="29832-p106">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="29832-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="29832-144">如果要使用**提及**在新邮件中呼叫其他用户, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="29832-144">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="29832-145">在请求正文中包括所需的**toRecipients**属性、**提及**属性和任何可写邮件属性。</span><span class="sxs-lookup"><span data-stu-id="29832-145">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="29832-146">对于**提及**属性中的每个提及, 您必须指定**提到**的属性。</span><span class="sxs-lookup"><span data-stu-id="29832-146">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="29832-147">响应</span><span class="sxs-lookup"><span data-stu-id="29832-147">Response</span></span>

<span data-ttu-id="29832-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="29832-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29832-150">示例</span><span class="sxs-lookup"><span data-stu-id="29832-150">Example</span></span>
<span data-ttu-id="29832-151">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="29832-151">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="29832-152">请求 1</span><span class="sxs-lookup"><span data-stu-id="29832-152">Request 1</span></span>
<span data-ttu-id="29832-153">下面的示例展示了在即时创建和发送邮件的请求。</span><span class="sxs-lookup"><span data-stu-id="29832-153">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="29832-154">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="29832-154">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="29832-155">C#</span><span class="sxs-lookup"><span data-stu-id="29832-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29832-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29832-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29832-157">目标-C</span><span class="sxs-lookup"><span data-stu-id="29832-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="29832-158">Java</span><span class="sxs-lookup"><span data-stu-id="29832-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="29832-159">响应 1</span><span class="sxs-lookup"><span data-stu-id="29832-159">Response 1</span></span>
<span data-ttu-id="29832-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="29832-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="29832-161">请求 2</span><span class="sxs-lookup"><span data-stu-id="29832-161">Request 2</span></span>
<span data-ttu-id="29832-162">下一个示例显示了登录用户 Samantha 展台的邮件。</span><span class="sxs-lookup"><span data-stu-id="29832-162">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="29832-163">此外, 该消息还包括其他用户 Dana Swope。</span><span class="sxs-lookup"><span data-stu-id="29832-163">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="29832-164">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="29832-164">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="29832-165">C#</span><span class="sxs-lookup"><span data-stu-id="29832-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29832-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29832-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29832-167">目标-C</span><span class="sxs-lookup"><span data-stu-id="29832-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="29832-168">Java</span><span class="sxs-lookup"><span data-stu-id="29832-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="29832-169">响应 2</span><span class="sxs-lookup"><span data-stu-id="29832-169">Response 2</span></span>
<span data-ttu-id="29832-170">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="29832-170">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="29832-171">请求 3</span><span class="sxs-lookup"><span data-stu-id="29832-171">Request 3</span></span>
<span data-ttu-id="29832-172">以下示例将创建一个带 Internet 消息标头的消息并进行发送。</span><span class="sxs-lookup"><span data-stu-id="29832-172">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="29832-173">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="29832-173">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="29832-174">C#</span><span class="sxs-lookup"><span data-stu-id="29832-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29832-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29832-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29832-176">目标-C</span><span class="sxs-lookup"><span data-stu-id="29832-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="29832-177">Java</span><span class="sxs-lookup"><span data-stu-id="29832-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="29832-178">响应 3</span><span class="sxs-lookup"><span data-stu-id="29832-178">Response 3</span></span>
<span data-ttu-id="29832-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="29832-179">Here is an example of the response.</span></span>
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
