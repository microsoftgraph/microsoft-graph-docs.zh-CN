---
title: 发送邮件
description: 发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。
ms.openlocfilehash: 6d8150f7292747e7c1d182395f9a98b1a199389f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008272"
---
# <a name="send-mail"></a><span data-ttu-id="d3b2d-104">发送邮件</span><span class="sxs-lookup"><span data-stu-id="d3b2d-104">Send mail</span></span>

<span data-ttu-id="d3b2d-p102">发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="d3b2d-107">可以在同一 **sendMail** 操作调用中包含[文件附件](../resources/fileattachment.md)。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-107">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3b2d-108">权限</span><span class="sxs-lookup"><span data-stu-id="d3b2d-108">Permissions</span></span>
<span data-ttu-id="d3b2d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d3b2d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3b2d-111">Permission type</span></span>      | <span data-ttu-id="d3b2d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3b2d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3b2d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3b2d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d3b2d-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d3b2d-114">Mail.Send</span></span>    |
|<span data-ttu-id="d3b2d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3b2d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3b2d-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d3b2d-116">Mail.Send</span></span>    |
|<span data-ttu-id="d3b2d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3b2d-117">Application</span></span> | <span data-ttu-id="d3b2d-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d3b2d-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3b2d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3b2d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="d3b2d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3b2d-120">Request headers</span></span>
| <span data-ttu-id="d3b2d-121">标头</span><span class="sxs-lookup"><span data-stu-id="d3b2d-121">Header</span></span>       | <span data-ttu-id="d3b2d-122">值</span><span class="sxs-lookup"><span data-stu-id="d3b2d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d3b2d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3b2d-123">Authorization</span></span>  | <span data-ttu-id="d3b2d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d3b2d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3b2d-126">Content-Type</span></span>  | <span data-ttu-id="d3b2d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d3b2d-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d3b2d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3b2d-128">Request body</span></span>
<span data-ttu-id="d3b2d-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d3b2d-130">参数</span><span class="sxs-lookup"><span data-stu-id="d3b2d-130">Parameter</span></span>    | <span data-ttu-id="d3b2d-131">类型</span><span class="sxs-lookup"><span data-stu-id="d3b2d-131">Type</span></span>   |<span data-ttu-id="d3b2d-132">说明</span><span class="sxs-lookup"><span data-stu-id="d3b2d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3b2d-133">message</span><span class="sxs-lookup"><span data-stu-id="d3b2d-133">message</span></span>|[<span data-ttu-id="d3b2d-134">邮件</span><span class="sxs-lookup"><span data-stu-id="d3b2d-134">Message</span></span>](../resources/message.md)|<span data-ttu-id="d3b2d-p105">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="d3b2d-137">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="d3b2d-137">saveToSentItems</span></span>|<span data-ttu-id="d3b2d-138">布尔</span><span class="sxs-lookup"><span data-stu-id="d3b2d-138">Boolean</span></span>|<span data-ttu-id="d3b2d-p106">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d3b2d-142">响应</span><span class="sxs-lookup"><span data-stu-id="d3b2d-142">Response</span></span>

<span data-ttu-id="d3b2d-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3b2d-145">示例</span><span class="sxs-lookup"><span data-stu-id="d3b2d-145">Example</span></span>
<span data-ttu-id="d3b2d-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-146">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="d3b2d-147">请求 1</span><span class="sxs-lookup"><span data-stu-id="d3b2d-147">Request 1</span></span>
<span data-ttu-id="d3b2d-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-148">Here is an example of the request.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="d3b2d-149">响应 1</span><span class="sxs-lookup"><span data-stu-id="d3b2d-149">Response 1</span></span>
<span data-ttu-id="d3b2d-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="d3b2d-151">请求 2</span><span class="sxs-lookup"><span data-stu-id="d3b2d-151">Request 2</span></span>
<span data-ttu-id="d3b2d-152">下一个示例使用自定义 Internet 邮件头中创建一条消息，并将邮件发送。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-152">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="d3b2d-153">响应 2</span><span class="sxs-lookup"><span data-stu-id="d3b2d-153">Response 2</span></span>
<span data-ttu-id="d3b2d-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d3b2d-154">Here is an example of the response.</span></span>
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
