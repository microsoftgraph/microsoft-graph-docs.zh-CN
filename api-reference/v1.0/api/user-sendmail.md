---
title: 发送邮件
description: 发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cfb9fcd33a87b2112616241757a44f515f968df6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137212"
---
# <a name="send-mail"></a><span data-ttu-id="effa6-104">发送邮件</span><span class="sxs-lookup"><span data-stu-id="effa6-104">Send mail</span></span>

<span data-ttu-id="effa6-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="effa6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="effa6-p102">发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="effa6-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="effa6-108">可以在同一 **sendMail** 操作调用中包含 [文件附件](../resources/fileattachment.md)。</span><span class="sxs-lookup"><span data-stu-id="effa6-108">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="effa6-109">权限</span><span class="sxs-lookup"><span data-stu-id="effa6-109">Permissions</span></span>
<span data-ttu-id="effa6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="effa6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="effa6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="effa6-112">Permission type</span></span>      | <span data-ttu-id="effa6-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="effa6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="effa6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="effa6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="effa6-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="effa6-115">Mail.Send</span></span>    |
|<span data-ttu-id="effa6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="effa6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="effa6-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="effa6-117">Mail.Send</span></span>    |
|<span data-ttu-id="effa6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="effa6-118">Application</span></span> | <span data-ttu-id="effa6-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="effa6-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="effa6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="effa6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="effa6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="effa6-121">Request headers</span></span>
| <span data-ttu-id="effa6-122">标头</span><span class="sxs-lookup"><span data-stu-id="effa6-122">Header</span></span>       | <span data-ttu-id="effa6-123">值</span><span class="sxs-lookup"><span data-stu-id="effa6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="effa6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="effa6-124">Authorization</span></span>  | <span data-ttu-id="effa6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="effa6-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="effa6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="effa6-127">Content-Type</span></span>  | <span data-ttu-id="effa6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="effa6-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="effa6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="effa6-129">Request body</span></span>
<span data-ttu-id="effa6-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="effa6-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="effa6-131">参数</span><span class="sxs-lookup"><span data-stu-id="effa6-131">Parameter</span></span>    | <span data-ttu-id="effa6-132">类型</span><span class="sxs-lookup"><span data-stu-id="effa6-132">Type</span></span>   |<span data-ttu-id="effa6-133">描述</span><span class="sxs-lookup"><span data-stu-id="effa6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="effa6-134">message</span><span class="sxs-lookup"><span data-stu-id="effa6-134">message</span></span>|[<span data-ttu-id="effa6-135">Message</span><span class="sxs-lookup"><span data-stu-id="effa6-135">Message</span></span>](../resources/message.md)|<span data-ttu-id="effa6-p105">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="effa6-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="effa6-138">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="effa6-138">saveToSentItems</span></span>|<span data-ttu-id="effa6-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="effa6-139">Boolean</span></span>|<span data-ttu-id="effa6-p106">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="effa6-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="effa6-143">响应</span><span class="sxs-lookup"><span data-stu-id="effa6-143">Response</span></span>

<span data-ttu-id="effa6-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="effa6-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="effa6-146">示例</span><span class="sxs-lookup"><span data-stu-id="effa6-146">Example</span></span>
<span data-ttu-id="effa6-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="effa6-147">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="effa6-148">请求 1</span><span class="sxs-lookup"><span data-stu-id="effa6-148">Request 1</span></span>
<span data-ttu-id="effa6-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="effa6-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="effa6-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="effa6-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="effa6-151">C#</span><span class="sxs-lookup"><span data-stu-id="effa6-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="effa6-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="effa6-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="effa6-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="effa6-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="effa6-154">Java</span><span class="sxs-lookup"><span data-stu-id="effa6-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="effa6-155">响应 1</span><span class="sxs-lookup"><span data-stu-id="effa6-155">Response 1</span></span>
<span data-ttu-id="effa6-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="effa6-156">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="effa6-157">请求 2</span><span class="sxs-lookup"><span data-stu-id="effa6-157">Request 2</span></span>
<span data-ttu-id="effa6-158">以下示例将创建一个带 Internet 消息标头的消息并进行发送。</span><span class="sxs-lookup"><span data-stu-id="effa6-158">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="http"></a>[<span data-ttu-id="effa6-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="effa6-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="effa6-160">C#</span><span class="sxs-lookup"><span data-stu-id="effa6-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="effa6-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="effa6-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="effa6-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="effa6-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="effa6-163">Java</span><span class="sxs-lookup"><span data-stu-id="effa6-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="effa6-164">响应 2</span><span class="sxs-lookup"><span data-stu-id="effa6-164">Response 2</span></span>
<span data-ttu-id="effa6-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="effa6-165">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="effa6-166">请求 3</span><span class="sxs-lookup"><span data-stu-id="effa6-166">Request 3</span></span>

<span data-ttu-id="effa6-167">下一个示例将创建包含文件附件的邮件并发送该邮件。</span><span class="sxs-lookup"><span data-stu-id="effa6-167">The next example creates a message with a file attachment and sends the message.</span></span>


# <a name="http"></a>[<span data-ttu-id="effa6-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="effa6-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_attachment"
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
# <a name="c"></a>[<span data-ttu-id="effa6-169">C#</span><span class="sxs-lookup"><span data-stu-id="effa6-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="effa6-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="effa6-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="effa6-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="effa6-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="effa6-172">Java</span><span class="sxs-lookup"><span data-stu-id="effa6-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="effa6-173">响应 3</span><span class="sxs-lookup"><span data-stu-id="effa6-173">Response 3</span></span>

<span data-ttu-id="effa6-174">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="effa6-174">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

