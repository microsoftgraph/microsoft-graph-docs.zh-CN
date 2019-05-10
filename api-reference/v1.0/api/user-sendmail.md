---
title: 发送邮件
description: 发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6f50ff6b9dbc2e83a611f0cc34d163b95aa48ee2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33600784"
---
# <a name="send-mail"></a><span data-ttu-id="d6304-104">发送邮件</span><span class="sxs-lookup"><span data-stu-id="d6304-104">Send mail</span></span>

<span data-ttu-id="d6304-p102">发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="d6304-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="d6304-107">可以在同一 **sendMail** 操作调用中包含[文件附件](../resources/fileattachment.md)。</span><span class="sxs-lookup"><span data-stu-id="d6304-107">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6304-108">权限</span><span class="sxs-lookup"><span data-stu-id="d6304-108">Permissions</span></span>
<span data-ttu-id="d6304-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6304-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d6304-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6304-111">Permission type</span></span>      | <span data-ttu-id="d6304-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6304-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6304-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6304-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d6304-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d6304-114">Mail.Send</span></span>    |
|<span data-ttu-id="d6304-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6304-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6304-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d6304-116">Mail.Send</span></span>    |
|<span data-ttu-id="d6304-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6304-117">Application</span></span> | <span data-ttu-id="d6304-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d6304-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6304-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6304-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="d6304-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6304-120">Request headers</span></span>
| <span data-ttu-id="d6304-121">标头</span><span class="sxs-lookup"><span data-stu-id="d6304-121">Header</span></span>       | <span data-ttu-id="d6304-122">值</span><span class="sxs-lookup"><span data-stu-id="d6304-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d6304-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6304-123">Authorization</span></span>  | <span data-ttu-id="d6304-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6304-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d6304-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6304-126">Content-Type</span></span>  | <span data-ttu-id="d6304-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d6304-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d6304-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6304-128">Request body</span></span>
<span data-ttu-id="d6304-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d6304-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d6304-130">参数</span><span class="sxs-lookup"><span data-stu-id="d6304-130">Parameter</span></span>    | <span data-ttu-id="d6304-131">类型</span><span class="sxs-lookup"><span data-stu-id="d6304-131">Type</span></span>   |<span data-ttu-id="d6304-132">描述</span><span class="sxs-lookup"><span data-stu-id="d6304-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6304-133">message</span><span class="sxs-lookup"><span data-stu-id="d6304-133">message</span></span>|[<span data-ttu-id="d6304-134">Message</span><span class="sxs-lookup"><span data-stu-id="d6304-134">Message</span></span>](../resources/message.md)|<span data-ttu-id="d6304-p105">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="d6304-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="d6304-137">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="d6304-137">saveToSentItems</span></span>|<span data-ttu-id="d6304-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6304-138">Boolean</span></span>|<span data-ttu-id="d6304-p106">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="d6304-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d6304-142">响应</span><span class="sxs-lookup"><span data-stu-id="d6304-142">Response</span></span>

<span data-ttu-id="d6304-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d6304-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6304-145">示例</span><span class="sxs-lookup"><span data-stu-id="d6304-145">Example</span></span>
<span data-ttu-id="d6304-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d6304-146">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="d6304-147">请求 1</span><span class="sxs-lookup"><span data-stu-id="d6304-147">Request 1</span></span>
<span data-ttu-id="d6304-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6304-148">Here is an example of the request.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="d6304-149">响应 1</span><span class="sxs-lookup"><span data-stu-id="d6304-149">Response 1</span></span>
<span data-ttu-id="d6304-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d6304-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d6304-151">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d6304-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d6304-152">C#</span><span class="sxs-lookup"><span data-stu-id="d6304-152">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6304-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6304-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="d6304-154">请求 2</span><span class="sxs-lookup"><span data-stu-id="d6304-154">Request 2</span></span>
<span data-ttu-id="d6304-155">以下示例将创建一个带 Internet 消息标头的消息并进行发送。</span><span class="sxs-lookup"><span data-stu-id="d6304-155">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="d6304-156">响应 2</span><span class="sxs-lookup"><span data-stu-id="d6304-156">Response 2</span></span>
<span data-ttu-id="d6304-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d6304-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d6304-158">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d6304-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d6304-159">C#</span><span class="sxs-lookup"><span data-stu-id="d6304-159">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6304-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6304-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
