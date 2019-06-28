---
title: 发送邮件
description: 发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 65715f4ffe1df1f11dec93a2d9992b91eb6b29ac
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278664"
---
# <a name="send-mail"></a><span data-ttu-id="f4c36-104">发送邮件</span><span class="sxs-lookup"><span data-stu-id="f4c36-104">Send mail</span></span>

<span data-ttu-id="f4c36-p102">发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="f4c36-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="f4c36-107">可以在同一 **sendMail** 操作调用中包含[文件附件](../resources/fileattachment.md)。</span><span class="sxs-lookup"><span data-stu-id="f4c36-107">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4c36-108">权限</span><span class="sxs-lookup"><span data-stu-id="f4c36-108">Permissions</span></span>
<span data-ttu-id="f4c36-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4c36-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f4c36-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4c36-111">Permission type</span></span>      | <span data-ttu-id="f4c36-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4c36-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4c36-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4c36-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f4c36-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f4c36-114">Mail.Send</span></span>    |
|<span data-ttu-id="f4c36-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4c36-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4c36-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f4c36-116">Mail.Send</span></span>    |
|<span data-ttu-id="f4c36-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4c36-117">Application</span></span> | <span data-ttu-id="f4c36-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f4c36-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4c36-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4c36-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="f4c36-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4c36-120">Request headers</span></span>
| <span data-ttu-id="f4c36-121">标头</span><span class="sxs-lookup"><span data-stu-id="f4c36-121">Header</span></span>       | <span data-ttu-id="f4c36-122">值</span><span class="sxs-lookup"><span data-stu-id="f4c36-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f4c36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4c36-123">Authorization</span></span>  | <span data-ttu-id="f4c36-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4c36-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f4c36-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4c36-126">Content-Type</span></span>  | <span data-ttu-id="f4c36-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f4c36-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f4c36-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4c36-128">Request body</span></span>
<span data-ttu-id="f4c36-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f4c36-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f4c36-130">参数</span><span class="sxs-lookup"><span data-stu-id="f4c36-130">Parameter</span></span>    | <span data-ttu-id="f4c36-131">类型</span><span class="sxs-lookup"><span data-stu-id="f4c36-131">Type</span></span>   |<span data-ttu-id="f4c36-132">描述</span><span class="sxs-lookup"><span data-stu-id="f4c36-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4c36-133">message</span><span class="sxs-lookup"><span data-stu-id="f4c36-133">message</span></span>|[<span data-ttu-id="f4c36-134">Message</span><span class="sxs-lookup"><span data-stu-id="f4c36-134">Message</span></span>](../resources/message.md)|<span data-ttu-id="f4c36-p105">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="f4c36-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="f4c36-137">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="f4c36-137">saveToSentItems</span></span>|<span data-ttu-id="f4c36-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4c36-138">Boolean</span></span>|<span data-ttu-id="f4c36-p106">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="f4c36-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f4c36-142">响应</span><span class="sxs-lookup"><span data-stu-id="f4c36-142">Response</span></span>

<span data-ttu-id="f4c36-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f4c36-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4c36-145">示例</span><span class="sxs-lookup"><span data-stu-id="f4c36-145">Example</span></span>
<span data-ttu-id="f4c36-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f4c36-146">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="f4c36-147">请求 1</span><span class="sxs-lookup"><span data-stu-id="f4c36-147">Request 1</span></span>
<span data-ttu-id="f4c36-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4c36-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
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
          "address": "fannyd@contoso.onmicrosoft.com"
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

##### <a name="response-1"></a><span data-ttu-id="f4c36-149">响应 1</span><span class="sxs-lookup"><span data-stu-id="f4c36-149">Response 1</span></span>
<span data-ttu-id="f4c36-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f4c36-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f4c36-151">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f4c36-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f4c36-152">C#</span><span class="sxs-lookup"><span data-stu-id="f4c36-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4c36-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="f4c36-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f4c36-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4c36-154">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_sendmail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="f4c36-155">请求 2</span><span class="sxs-lookup"><span data-stu-id="f4c36-155">Request 2</span></span>
<span data-ttu-id="f4c36-156">以下示例将创建一个带 Internet 消息标头的消息并进行发送。</span><span class="sxs-lookup"><span data-stu-id="f4c36-156">The next example creates a message with custom Internet message headers and sends the message.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
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

##### <a name="response-2"></a><span data-ttu-id="f4c36-157">响应 2</span><span class="sxs-lookup"><span data-stu-id="f4c36-157">Response 2</span></span>
<span data-ttu-id="f4c36-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f4c36-158">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f4c36-159">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f4c36-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f4c36-160">C#</span><span class="sxs-lookup"><span data-stu-id="f4c36-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4c36-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="f4c36-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f4c36-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4c36-162">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
