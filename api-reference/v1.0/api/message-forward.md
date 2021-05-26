---
title: 邮件：转发
description: 使用 JSON 或 MIME 格式转发邮件。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a787aeaa213732dc1a527a3889fb1a37ce9ad325
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645498"
---
# <a name="message-forward"></a><span data-ttu-id="9145c-103">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="9145c-103">message: forward</span></span>

<span data-ttu-id="9145c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9145c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9145c-105">使用 JSON 或 MIME 格式转发邮件。</span><span class="sxs-lookup"><span data-stu-id="9145c-105">Forward a message using either JSON or MIME format.</span></span>

<span data-ttu-id="9145c-106">使用 JSON 格式时，可以：</span><span class="sxs-lookup"><span data-stu-id="9145c-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="9145c-107">指定参数的 comment 或 **body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="9145c-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="9145c-108">指定这两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="9145c-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="9145c-109">指定参数 `toRecipients` 的参数或 **toRecipients** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="9145c-109">Specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="9145c-110">指定两者或同时指定两者都将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="9145c-110">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

<span data-ttu-id="9145c-111">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="9145c-111">When using MIME format:</span></span>
- <span data-ttu-id="9145c-112">在请求正文中提供适用的 [Internet](https://tools.ietf.org/html/rfc2076) 邮件头和 [MIME](https://tools.ietf.org/html/rfc2045)内容，这些内容均以 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="9145c-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="9145c-113">将任何附件和 S/MIME 属性添加到 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="9145c-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="9145c-114">此方法将邮件保存在"已发送 **的项目"** 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="9145c-114">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="9145c-115">或者，[创建转发邮件的草稿，](../api/message-createforward.md)[并稍后](../api/message-send.md)发送。</span><span class="sxs-lookup"><span data-stu-id="9145c-115">Alternatively, [create a draft to forward a message](../api/message-createforward.md), and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="9145c-116">权限</span><span class="sxs-lookup"><span data-stu-id="9145c-116">Permissions</span></span>
<span data-ttu-id="9145c-117">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="9145c-117">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="9145c-118">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9145c-118">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9145c-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="9145c-119">Permission type</span></span>      | <span data-ttu-id="9145c-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9145c-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9145c-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9145c-121">Delegated (work or school account)</span></span> | <span data-ttu-id="9145c-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9145c-122">Mail.Send</span></span>    |
|<span data-ttu-id="9145c-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9145c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9145c-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9145c-124">Mail.Send</span></span>    |
|<span data-ttu-id="9145c-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="9145c-125">Application</span></span> | <span data-ttu-id="9145c-126">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9145c-126">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="9145c-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9145c-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="9145c-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="9145c-128">Request headers</span></span>
| <span data-ttu-id="9145c-129">名称</span><span class="sxs-lookup"><span data-stu-id="9145c-129">Name</span></span>       | <span data-ttu-id="9145c-130">类型</span><span class="sxs-lookup"><span data-stu-id="9145c-130">Type</span></span> | <span data-ttu-id="9145c-131">说明</span><span class="sxs-lookup"><span data-stu-id="9145c-131">Description</span></span>| 
|:---------------|:--------|:----------|
| <span data-ttu-id="9145c-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="9145c-132">Authorization</span></span>  | <span data-ttu-id="9145c-133">string</span><span class="sxs-lookup"><span data-stu-id="9145c-133">string</span></span>  | <span data-ttu-id="9145c-134">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="9145c-134">Bearer {token}.</span></span> <span data-ttu-id="9145c-135">必需</span><span class="sxs-lookup"><span data-stu-id="9145c-135">Required</span></span> |
| <span data-ttu-id="9145c-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9145c-136">Content-Type</span></span> | <span data-ttu-id="9145c-137">string</span><span class="sxs-lookup"><span data-stu-id="9145c-137">string</span></span>  | <span data-ttu-id="9145c-138">实体正文中的数据性质。</span><span class="sxs-lookup"><span data-stu-id="9145c-138">Nature of the data in the body of an entity.</span></span>  <span data-ttu-id="9145c-139">必需。</span><span class="sxs-lookup"><span data-stu-id="9145c-139">Required.</span></span> <br/> <span data-ttu-id="9145c-140">用于 `application/json` JSON 对象和 `text/plain` MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="9145c-140">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9145c-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="9145c-141">Request body</span></span>
<span data-ttu-id="9145c-142">使用 JSON 格式时，在请求正文中提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9145c-142">When using JSON format, provide a JSON object in the request body with the following parameters.</span></span>

| <span data-ttu-id="9145c-143">参数</span><span class="sxs-lookup"><span data-stu-id="9145c-143">Parameter</span></span>    | <span data-ttu-id="9145c-144">类型</span><span class="sxs-lookup"><span data-stu-id="9145c-144">Type</span></span>   |<span data-ttu-id="9145c-145">说明</span><span class="sxs-lookup"><span data-stu-id="9145c-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9145c-146">注释</span><span class="sxs-lookup"><span data-stu-id="9145c-146">comment</span></span>|<span data-ttu-id="9145c-147">String</span><span class="sxs-lookup"><span data-stu-id="9145c-147">String</span></span>|<span data-ttu-id="9145c-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="9145c-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="9145c-150">toRecipients</span><span class="sxs-lookup"><span data-stu-id="9145c-150">toRecipients</span></span>|<span data-ttu-id="9145c-151">[Recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="9145c-151">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="9145c-152">收件人列表</span><span class="sxs-lookup"><span data-stu-id="9145c-152">The list of recipients.</span></span>|

<span data-ttu-id="9145c-153">指定 MIME 格式的正文时，向 MIME 内容提供适用的 Internet 邮件头 ("收件人"、"抄送"、"密件抄送"、"主题") ，请求正文中均以 **base64** 格式编码。</span><span class="sxs-lookup"><span data-stu-id="9145c-153">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="9145c-154">响应</span><span class="sxs-lookup"><span data-stu-id="9145c-154">Response</span></span>

<span data-ttu-id="9145c-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9145c-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="9145c-157">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息："MIME 内容的 `400 Bad request` base64 字符串无效"。</span><span class="sxs-lookup"><span data-stu-id="9145c-157">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="9145c-158">示例</span><span class="sxs-lookup"><span data-stu-id="9145c-158">Examples</span></span>
### <a name="example-1-forward-a-message-using-json-format"></a><span data-ttu-id="9145c-159">示例 1：使用 JSON 格式转发邮件</span><span class="sxs-lookup"><span data-stu-id="9145c-159">Example 1: Forward a message using JSON format</span></span>
<span data-ttu-id="9145c-160">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9145c-160">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9145c-161">请求</span><span class="sxs-lookup"><span data-stu-id="9145c-161">Request</span></span>
<span data-ttu-id="9145c-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9145c-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9145c-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="9145c-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9145c-164">C#</span><span class="sxs-lookup"><span data-stu-id="9145c-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9145c-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9145c-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9145c-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9145c-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9145c-167">Java</span><span class="sxs-lookup"><span data-stu-id="9145c-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9145c-168">响应</span><span class="sxs-lookup"><span data-stu-id="9145c-168">Response</span></span>
<span data-ttu-id="9145c-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9145c-169">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

### <a name="example-2-forward-a-message-using-mime-content"></a><span data-ttu-id="9145c-170">示例 2：使用 MIME 内容转发邮件</span><span class="sxs-lookup"><span data-stu-id="9145c-170">Example 2: Forward a message using MIME content</span></span>
##### <a name="request"></a><span data-ttu-id="9145c-171">请求</span><span class="sxs-lookup"><span data-stu-id="9145c-171">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/forward
Content-type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np
```
##### <a name="response"></a><span data-ttu-id="9145c-172">响应</span><span class="sxs-lookup"><span data-stu-id="9145c-172">Response</span></span>
<span data-ttu-id="9145c-173">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9145c-173">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="9145c-174">如果请求正文包含格式错误的 MIME 内容，此方法将返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="9145c-174">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

