---
title: 邮件：转发
description: 使用 JSON 或 MIME 格式转发邮件
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 021d17d930e76a7696ab8e4484d1f43c20c84fd4
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870631"
---
# <a name="message-forward"></a><span data-ttu-id="3a976-103">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="3a976-103">message: forward</span></span>

<span data-ttu-id="3a976-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a976-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a976-105">使用 JSON 或 MIME 格式转发邮件。</span><span class="sxs-lookup"><span data-stu-id="3a976-105">Forward a message using either JSON or MIME format.</span></span>

<span data-ttu-id="3a976-106">使用 JSON 格式时，可以：</span><span class="sxs-lookup"><span data-stu-id="3a976-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="3a976-107">指定参数的 comment 或 **body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="3a976-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="3a976-108">指定这两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="3a976-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="3a976-109">指定参数 `toRecipients` 的参数或 **toRecipients** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="3a976-109">Specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="3a976-110">指定两者或同时指定两者都将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="3a976-110">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

<span data-ttu-id="3a976-111">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="3a976-111">When using MIME format:</span></span>
- <span data-ttu-id="3a976-112">提供适用的 [Internet 邮件头](https://tools.ietf.org/html/rfc2076) 和 [MIME 内容](https://tools.ietf.org/html/rfc2045)，所有内容在请求正文中都通过 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="3a976-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="3a976-113">向 MIME 内容添加任何附件和 S/MIME 属性。</span><span class="sxs-lookup"><span data-stu-id="3a976-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="3a976-114">此方法将邮件保存在 **“已发送邮件”** 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="3a976-114">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="3a976-115">或者，[创建转发邮件的草稿，](../api/message-createforward.md)[并稍后](../api/message-send.md)发送。</span><span class="sxs-lookup"><span data-stu-id="3a976-115">Alternatively, [create a draft to forward a message](../api/message-createforward.md), and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a976-116">权限</span><span class="sxs-lookup"><span data-stu-id="3a976-116">Permissions</span></span>
<span data-ttu-id="3a976-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a976-p103">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a976-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a976-119">Permission type</span></span>      | <span data-ttu-id="3a976-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a976-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a976-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a976-121">Delegated (work or school account)</span></span> | <span data-ttu-id="3a976-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3a976-122">Mail.Send</span></span>    |
|<span data-ttu-id="3a976-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a976-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a976-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3a976-124">Mail.Send</span></span>    |
|<span data-ttu-id="3a976-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a976-125">Application</span></span> | <span data-ttu-id="3a976-126">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3a976-126">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a976-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a976-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="3a976-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a976-128">Request headers</span></span>
| <span data-ttu-id="3a976-129">名称</span><span class="sxs-lookup"><span data-stu-id="3a976-129">Name</span></span>       | <span data-ttu-id="3a976-130">类型</span><span class="sxs-lookup"><span data-stu-id="3a976-130">Type</span></span> | <span data-ttu-id="3a976-131">说明</span><span class="sxs-lookup"><span data-stu-id="3a976-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3a976-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a976-132">Authorization</span></span>  | <span data-ttu-id="3a976-133">string</span><span class="sxs-lookup"><span data-stu-id="3a976-133">string</span></span>  | <span data-ttu-id="3a976-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3a976-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a976-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a976-136">Content-Type</span></span> | <span data-ttu-id="3a976-137">string</span><span class="sxs-lookup"><span data-stu-id="3a976-137">string</span></span>  | <span data-ttu-id="3a976-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="3a976-p105">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="3a976-140">对 JSON 对象使用 `application/json`，对 MIME 内容使用 `text/plain`。</span><span class="sxs-lookup"><span data-stu-id="3a976-140">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a976-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a976-141">Request body</span></span>
<span data-ttu-id="3a976-142">使用 JSON 格式时，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3a976-142">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a976-143">参数</span><span class="sxs-lookup"><span data-stu-id="3a976-143">Parameter</span></span>    | <span data-ttu-id="3a976-144">类型</span><span class="sxs-lookup"><span data-stu-id="3a976-144">Type</span></span>   |<span data-ttu-id="3a976-145">说明</span><span class="sxs-lookup"><span data-stu-id="3a976-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a976-146">注释</span><span class="sxs-lookup"><span data-stu-id="3a976-146">comment</span></span>|<span data-ttu-id="3a976-147">String</span><span class="sxs-lookup"><span data-stu-id="3a976-147">String</span></span>|<span data-ttu-id="3a976-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="3a976-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="3a976-150">toRecipients</span><span class="sxs-lookup"><span data-stu-id="3a976-150">toRecipients</span></span>|<span data-ttu-id="3a976-151">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="3a976-151">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="3a976-152">收件人列表</span><span class="sxs-lookup"><span data-stu-id="3a976-152">The list of recipients.</span></span>|
|<span data-ttu-id="3a976-153">message</span><span class="sxs-lookup"><span data-stu-id="3a976-153">message</span></span>|[<span data-ttu-id="3a976-154">message</span><span class="sxs-lookup"><span data-stu-id="3a976-154">message</span></span>](../resources/message.md)|<span data-ttu-id="3a976-155">回复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="3a976-155">Any writeable properties to update in the reply message.</span></span>|

<span data-ttu-id="3a976-156">当指定 MIME 格式的正文时，请提供 MIME 内容与适用的 Internet 邮件头（“收件人”、“抄送”、“密件抄送”、“主题”）所有内容在请求正文中编码为 **base64** 格式。</span><span class="sxs-lookup"><span data-stu-id="3a976-156">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="3a976-157">响应</span><span class="sxs-lookup"><span data-stu-id="3a976-157">Response</span></span>

<span data-ttu-id="3a976-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3a976-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="3a976-160">如果请求正文包含错误的 MIME 内容，此方法将返回 `400 Bad request` 和以下错误消息：“无效的 base64 字符串 MIME 内容”。</span><span class="sxs-lookup"><span data-stu-id="3a976-160">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="3a976-161">示例</span><span class="sxs-lookup"><span data-stu-id="3a976-161">Examples</span></span>
### <a name="example-1-forward-a-message-using-json-format"></a><span data-ttu-id="3a976-162">示例 1：使用 JSON 格式转发邮件</span><span class="sxs-lookup"><span data-stu-id="3a976-162">Example 1: Forward a message using JSON format</span></span>
<span data-ttu-id="3a976-163">以下示例将 **isDeliveryReceiptRequested** 属性设置为 true，添加注释并转发邮件。</span><span class="sxs-lookup"><span data-stu-id="3a976-163">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="3a976-164">请求</span><span class="sxs-lookup"><span data-stu-id="3a976-164">Request</span></span>
<span data-ttu-id="3a976-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3a976-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a976-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a976-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this." 
}
```
# <a name="c"></a>[<span data-ttu-id="3a976-167">C#</span><span class="sxs-lookup"><span data-stu-id="3a976-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a976-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a976-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a976-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a976-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a976-170">Java</span><span class="sxs-lookup"><span data-stu-id="3a976-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3a976-171">响应</span><span class="sxs-lookup"><span data-stu-id="3a976-171">Response</span></span>
<span data-ttu-id="3a976-172">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3a976-172">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-forward-a-message-using-mime-format"></a><span data-ttu-id="3a976-173">示例 2：使用 MIME 格式转发邮件</span><span class="sxs-lookup"><span data-stu-id="3a976-173">Example 2: Forward a message using MIME format</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_forward_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
Content-Type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np...

```


##### <a name="response"></a><span data-ttu-id="3a976-174">响应</span><span class="sxs-lookup"><span data-stu-id="3a976-174">Response</span></span>
<span data-ttu-id="3a976-175">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3a976-175">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted

```

<span data-ttu-id="3a976-176">如果请求正文包含错误的 MIME 内容，此方法返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="3a976-176">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
