---
title: 消息：答复
description: '全部在一个 **reply** 调用中回复邮件的发件人、添加注释或修改任意可更新的属性。 '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 39d03daf5a26d5617e4eca31ae7ba3799a5159c9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131138"
---
# <a name="message-reply"></a><span data-ttu-id="16453-103">消息：答复</span><span class="sxs-lookup"><span data-stu-id="16453-103">message: reply</span></span>

<span data-ttu-id="16453-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16453-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16453-p101">全部在一个 **reply** 调用中回复邮件的发件人、添加注释或修改任意可更新的属性。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="16453-p101">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call. The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="16453-107">或者，您可以先创建草稿答复 [邮件](../api/message-createreply.md) 以包含注释或更新任何邮件属性，然后 [发送](../api/message-send.md) 答复。</span><span class="sxs-lookup"><span data-stu-id="16453-107">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="16453-108">**注意**</span><span class="sxs-lookup"><span data-stu-id="16453-108">**Note**</span></span>

- <span data-ttu-id="16453-109">可以指定参数的注释 **或 body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="16453-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="16453-110">指定两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="16453-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="16453-111">如果在原始邮件中指定了 **replyTo** 属性，则根据 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ，您应该将答复发送给 **replyTo** 中的收件人，而不是 **from** 属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="16453-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="16453-112">权限</span><span class="sxs-lookup"><span data-stu-id="16453-112">Permissions</span></span>
<span data-ttu-id="16453-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16453-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16453-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="16453-115">Permission type</span></span>      | <span data-ttu-id="16453-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16453-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16453-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16453-117">Delegated (work or school account)</span></span> | <span data-ttu-id="16453-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="16453-118">Mail.Send</span></span>    |
|<span data-ttu-id="16453-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16453-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16453-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="16453-120">Mail.Send</span></span>    |
|<span data-ttu-id="16453-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="16453-121">Application</span></span> | <span data-ttu-id="16453-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="16453-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="16453-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16453-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="16453-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="16453-124">Request headers</span></span>
| <span data-ttu-id="16453-125">名称</span><span class="sxs-lookup"><span data-stu-id="16453-125">Name</span></span>       | <span data-ttu-id="16453-126">类型</span><span class="sxs-lookup"><span data-stu-id="16453-126">Type</span></span> | <span data-ttu-id="16453-127">说明</span><span class="sxs-lookup"><span data-stu-id="16453-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16453-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="16453-128">Authorization</span></span>  | <span data-ttu-id="16453-129">string</span><span class="sxs-lookup"><span data-stu-id="16453-129">string</span></span>  | <span data-ttu-id="16453-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16453-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16453-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16453-132">Content-Type</span></span> | <span data-ttu-id="16453-133">string</span><span class="sxs-lookup"><span data-stu-id="16453-133">string</span></span>  | <span data-ttu-id="16453-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="16453-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16453-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="16453-136">Request body</span></span>
<span data-ttu-id="16453-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="16453-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="16453-138">参数</span><span class="sxs-lookup"><span data-stu-id="16453-138">Parameter</span></span>    | <span data-ttu-id="16453-139">类型</span><span class="sxs-lookup"><span data-stu-id="16453-139">Type</span></span>   |<span data-ttu-id="16453-140">说明</span><span class="sxs-lookup"><span data-stu-id="16453-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16453-141">注释</span><span class="sxs-lookup"><span data-stu-id="16453-141">comment</span></span>|<span data-ttu-id="16453-142">String</span><span class="sxs-lookup"><span data-stu-id="16453-142">String</span></span>|<span data-ttu-id="16453-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="16453-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="16453-145">message</span><span class="sxs-lookup"><span data-stu-id="16453-145">message</span></span>|[<span data-ttu-id="16453-146">邮件</span><span class="sxs-lookup"><span data-stu-id="16453-146">message</span></span>](../resources/message.md)|<span data-ttu-id="16453-147">回复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="16453-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="16453-148">响应</span><span class="sxs-lookup"><span data-stu-id="16453-148">Response</span></span>

<span data-ttu-id="16453-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="16453-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16453-151">示例</span><span class="sxs-lookup"><span data-stu-id="16453-151">Example</span></span>
<span data-ttu-id="16453-152">下面的示例包括一个注释，并将收件人添加到回复邮件。</span><span class="sxs-lookup"><span data-stu-id="16453-152">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="16453-153">请求</span><span class="sxs-lookup"><span data-stu-id="16453-153">Request</span></span>
<span data-ttu-id="16453-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16453-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16453-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="16453-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_reply_beta",
  "sampleKeys": ["AAMkADA1MTAAAAqldOAAA="]
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group please?" 
}
```
# <a name="c"></a>[<span data-ttu-id="16453-156">C#</span><span class="sxs-lookup"><span data-stu-id="16453-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16453-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16453-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16453-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16453-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16453-159">Java</span><span class="sxs-lookup"><span data-stu-id="16453-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="16453-160">响应</span><span class="sxs-lookup"><span data-stu-id="16453-160">Response</span></span>
<span data-ttu-id="16453-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16453-161">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


