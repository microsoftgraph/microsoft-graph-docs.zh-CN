---
title: 发送邮件
description: 使用 JSON 或 MIME 格式发送请求正文中指定的邮件。
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 460e09371869fec98b24bd81dc5ab44cc8b199b8
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870386"
---
# <a name="send-mail"></a><span data-ttu-id="f888c-103">发送邮件</span><span class="sxs-lookup"><span data-stu-id="f888c-103">Send mail</span></span>

<span data-ttu-id="f888c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f888c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f888c-105">使用 JSON 或 MIME 格式发送请求正文中指定的邮件。</span><span class="sxs-lookup"><span data-stu-id="f888c-105">Send the message specified in the request body using either JSON or MIME format.</span></span>

<span data-ttu-id="f888c-106">使用 JSON 格式时，可以在同一 **sendMail** 操作调用中包含 [文件附件](../resources/fileattachment.md)。</span><span class="sxs-lookup"><span data-stu-id="f888c-106">When using JSON format you can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

<span data-ttu-id="f888c-107">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="f888c-107">When using MIME format:</span></span>
- <span data-ttu-id="f888c-108">提供适用的 [Internet 邮件头](https://tools.ietf.org/html/rfc2076) 和 [MIME 内容](https://tools.ietf.org/html/rfc2045)，所有内容在请求正文中都通过 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="f888c-108">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="f888c-109">向 MIME 内容添加任何附件和 S/MIME 属性。</span><span class="sxs-lookup"><span data-stu-id="f888c-109">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="f888c-110">此方法将邮件保存在 **“已发送邮件”** 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="f888c-110">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="f888c-111">或者，[创建草稿邮件](../api/user-post-messages.md)稍后发送。</span><span class="sxs-lookup"><span data-stu-id="f888c-111">Alternatively, [create a draft message](../api/user-post-messages.md) to send later.</span></span>

## <a name="permissions"></a><span data-ttu-id="f888c-112">权限</span><span class="sxs-lookup"><span data-stu-id="f888c-112">Permissions</span></span>
<span data-ttu-id="f888c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f888c-p101">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f888c-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="f888c-115">Permission type</span></span>      | <span data-ttu-id="f888c-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f888c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f888c-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f888c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f888c-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f888c-118">Mail.Send</span></span>    |
|<span data-ttu-id="f888c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f888c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f888c-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f888c-120">Mail.Send</span></span>    |
|<span data-ttu-id="f888c-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="f888c-121">Application</span></span> | <span data-ttu-id="f888c-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f888c-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="f888c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f888c-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```

## <a name="request-headers"></a><span data-ttu-id="f888c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="f888c-124">Request headers</span></span>
| <span data-ttu-id="f888c-125">名称</span><span class="sxs-lookup"><span data-stu-id="f888c-125">Name</span></span>       | <span data-ttu-id="f888c-126">类型</span><span class="sxs-lookup"><span data-stu-id="f888c-126">Type</span></span> | <span data-ttu-id="f888c-127">说明</span><span class="sxs-lookup"><span data-stu-id="f888c-127">Description</span></span>| 
|:---------------|:--------|:----------
| <span data-ttu-id="f888c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f888c-128">Authorization</span></span>  | <span data-ttu-id="f888c-129">string</span><span class="sxs-lookup"><span data-stu-id="f888c-129">string</span></span>  | <span data-ttu-id="f888c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f888c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f888c-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f888c-132">Content-Type</span></span> | <span data-ttu-id="f888c-133">string</span><span class="sxs-lookup"><span data-stu-id="f888c-133">string</span></span>  | <span data-ttu-id="f888c-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="f888c-p103">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="f888c-136">对 JSON 对象使用 `application/json`，对 MIME 内容使用 `text/plain`。</span><span class="sxs-lookup"><span data-stu-id="f888c-136">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f888c-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="f888c-137">Request body</span></span>
<span data-ttu-id="f888c-138">使用 JSON 格式时，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f888c-138">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f888c-139">参数</span><span class="sxs-lookup"><span data-stu-id="f888c-139">Parameter</span></span>    | <span data-ttu-id="f888c-140">类型</span><span class="sxs-lookup"><span data-stu-id="f888c-140">Type</span></span>   |<span data-ttu-id="f888c-141">描述</span><span class="sxs-lookup"><span data-stu-id="f888c-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f888c-142">message</span><span class="sxs-lookup"><span data-stu-id="f888c-142">message</span></span>|[<span data-ttu-id="f888c-143">Message</span><span class="sxs-lookup"><span data-stu-id="f888c-143">Message</span></span>](../resources/message.md)|<span data-ttu-id="f888c-p104">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="f888c-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="f888c-146">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="f888c-146">saveToSentItems</span></span>|<span data-ttu-id="f888c-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="f888c-147">Boolean</span></span>|<span data-ttu-id="f888c-p105">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="f888c-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

<span data-ttu-id="f888c-151">当指定 MIME 格式的正文时，请在请求正文中提供 MIME 内容为 **base64 编码的字符串**。</span><span class="sxs-lookup"><span data-stu-id="f888c-151">When specifying the body in MIME format, provide the MIME content as **a base64-encoded string** in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="f888c-152">响应</span><span class="sxs-lookup"><span data-stu-id="f888c-152">Response</span></span>

<span data-ttu-id="f888c-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f888c-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="f888c-155">如果请求正文包含错误的 MIME 内容，此方法将返回 `400 Bad request` 和以下错误消息：“无效的 base64 字符串 MIME 内容”。</span><span class="sxs-lookup"><span data-stu-id="f888c-155">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="f888c-156">示例</span><span class="sxs-lookup"><span data-stu-id="f888c-156">Examples</span></span>
### <a name="example-1-send-a-new-email-using-json-format"></a><span data-ttu-id="f888c-157">示例 1：使用 JSON 格式发送新电子邮件</span><span class="sxs-lookup"><span data-stu-id="f888c-157">Example 1: Send a new email using JSON format</span></span>
<span data-ttu-id="f888c-158">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f888c-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f888c-159">请求</span><span class="sxs-lookup"><span data-stu-id="f888c-159">Request</span></span>
<span data-ttu-id="f888c-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f888c-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f888c-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="f888c-161">HTTP</span></span>](#tab/http)

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
# <a name="c"></a>[<span data-ttu-id="f888c-162">C#</span><span class="sxs-lookup"><span data-stu-id="f888c-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f888c-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f888c-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f888c-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f888c-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f888c-165">Java</span><span class="sxs-lookup"><span data-stu-id="f888c-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f888c-166">响应</span><span class="sxs-lookup"><span data-stu-id="f888c-166">Response</span></span>
<span data-ttu-id="f888c-167">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f888c-167">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-create-a-message-with-custom-internet-message-headers-and-send-the-message"></a><span data-ttu-id="f888c-168">示例 2：创建带自定义 Internet 邮件头的邮件并发送邮件</span><span class="sxs-lookup"><span data-stu-id="f888c-168">Example 2: Create a message with custom Internet message headers and send the message</span></span>
#### <a name="request"></a><span data-ttu-id="f888c-169">请求</span><span class="sxs-lookup"><span data-stu-id="f888c-169">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f888c-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="f888c-170">HTTP</span></span>](#tab/http)

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
# <a name="c"></a>[<span data-ttu-id="f888c-171">C#</span><span class="sxs-lookup"><span data-stu-id="f888c-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f888c-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f888c-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f888c-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f888c-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f888c-174">Java</span><span class="sxs-lookup"><span data-stu-id="f888c-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f888c-175">响应</span><span class="sxs-lookup"><span data-stu-id="f888c-175">Response</span></span>
<span data-ttu-id="f888c-176">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f888c-176">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-3--create-a-message-with-a-file-attachment-and-send-the-message"></a><span data-ttu-id="f888c-177">示例 3：创建带文件附件的邮件并发送邮件</span><span class="sxs-lookup"><span data-stu-id="f888c-177">Example 3:  Create a message with a file attachment and send the message</span></span>
#### <a name="request"></a><span data-ttu-id="f888c-178">请求</span><span class="sxs-lookup"><span data-stu-id="f888c-178">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f888c-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="f888c-179">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f888c-180">C#</span><span class="sxs-lookup"><span data-stu-id="f888c-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f888c-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f888c-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f888c-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f888c-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f888c-183">Java</span><span class="sxs-lookup"><span data-stu-id="f888c-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f888c-184">响应</span><span class="sxs-lookup"><span data-stu-id="f888c-184">Response</span></span>
<span data-ttu-id="f888c-185">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f888c-185">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-4-send-a-new-message-using-mime-format"></a><span data-ttu-id="f888c-186">示例 4：使用 MIME 格式发送新邮件</span><span class="sxs-lookup"><span data-stu-id="f888c-186">Example 4: Send a new message using MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="f888c-187">请求</span><span class="sxs-lookup"><span data-stu-id="f888c-187">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_send_mime_beta"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/sendMail
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

#### <a name="response"></a><span data-ttu-id="f888c-188">响应</span><span class="sxs-lookup"><span data-stu-id="f888c-188">Response</span></span>
<span data-ttu-id="f888c-189">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f888c-189">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="f888c-190">如果请求正文包含错误的 MIME 内容，此方法返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="f888c-190">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
