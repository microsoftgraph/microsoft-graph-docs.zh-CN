---
title: 消息：答复
description: '全部在一个 **reply** 调用中回复邮件的发件人、添加注释或修改任意可更新的属性。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 16c7cc0c052266249e5fcaf78189dc6344953f20
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37427859"
---
# <a name="message-reply"></a><span data-ttu-id="0e683-103">消息：答复</span><span class="sxs-lookup"><span data-stu-id="0e683-103">message: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e683-p101">全部在一个 **reply** 调用中回复邮件的发件人、添加注释或修改任意可更新的属性。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="0e683-p101">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call. The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="0e683-106">或者，您可以先[创建草稿答复邮件](../api/message-createreply.md)以包含注释或更新任何邮件属性，然后[发送](../api/message-send.md)回复。</span><span class="sxs-lookup"><span data-stu-id="0e683-106">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="0e683-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="0e683-107">**Note**</span></span>

- <span data-ttu-id="0e683-108">您可以指定`message`参数的注释或**body**属性。</span><span class="sxs-lookup"><span data-stu-id="0e683-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="0e683-109">同时指定这两个将返回 HTTP 400 错误的请求错误。</span><span class="sxs-lookup"><span data-stu-id="0e683-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="0e683-110">如果在原始邮件中指定了**replyTo**属性（根据 Internet 邮件格式（[RFC 2822](https://www.rfc-editor.org/info/rfc2822)）），则应将答复发送给**replyTo**中的收件人，而不是发**件**人属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="0e683-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="0e683-111">权限</span><span class="sxs-lookup"><span data-stu-id="0e683-111">Permissions</span></span>
<span data-ttu-id="0e683-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e683-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e683-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e683-114">Permission type</span></span>      | <span data-ttu-id="0e683-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e683-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e683-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e683-116">Delegated (work or school account)</span></span> | <span data-ttu-id="0e683-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0e683-117">Mail.Send</span></span>    |
|<span data-ttu-id="0e683-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e683-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e683-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0e683-119">Mail.Send</span></span>    |
|<span data-ttu-id="0e683-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e683-120">Application</span></span> | <span data-ttu-id="0e683-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0e683-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e683-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e683-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="0e683-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e683-123">Request headers</span></span>
| <span data-ttu-id="0e683-124">名称</span><span class="sxs-lookup"><span data-stu-id="0e683-124">Name</span></span>       | <span data-ttu-id="0e683-125">类型</span><span class="sxs-lookup"><span data-stu-id="0e683-125">Type</span></span> | <span data-ttu-id="0e683-126">说明</span><span class="sxs-lookup"><span data-stu-id="0e683-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0e683-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e683-127">Authorization</span></span>  | <span data-ttu-id="0e683-128">string</span><span class="sxs-lookup"><span data-stu-id="0e683-128">string</span></span>  | <span data-ttu-id="0e683-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e683-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e683-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e683-131">Content-Type</span></span> | <span data-ttu-id="0e683-132">string</span><span class="sxs-lookup"><span data-stu-id="0e683-132">string</span></span>  | <span data-ttu-id="0e683-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="0e683-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e683-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e683-135">Request body</span></span>
<span data-ttu-id="0e683-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0e683-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0e683-137">参数</span><span class="sxs-lookup"><span data-stu-id="0e683-137">Parameter</span></span>    | <span data-ttu-id="0e683-138">类型</span><span class="sxs-lookup"><span data-stu-id="0e683-138">Type</span></span>   |<span data-ttu-id="0e683-139">说明</span><span class="sxs-lookup"><span data-stu-id="0e683-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e683-140">注释</span><span class="sxs-lookup"><span data-stu-id="0e683-140">comment</span></span>|<span data-ttu-id="0e683-141">String</span><span class="sxs-lookup"><span data-stu-id="0e683-141">String</span></span>|<span data-ttu-id="0e683-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="0e683-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="0e683-144">message</span><span class="sxs-lookup"><span data-stu-id="0e683-144">message</span></span>|[<span data-ttu-id="0e683-145">邮件</span><span class="sxs-lookup"><span data-stu-id="0e683-145">message</span></span>](../resources/message.md)|<span data-ttu-id="0e683-146">答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="0e683-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="0e683-147">响应</span><span class="sxs-lookup"><span data-stu-id="0e683-147">Response</span></span>

<span data-ttu-id="0e683-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0e683-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e683-150">示例</span><span class="sxs-lookup"><span data-stu-id="0e683-150">Example</span></span>
<span data-ttu-id="0e683-151">下面的示例包含注释并将收件人添加到回复邮件中。</span><span class="sxs-lookup"><span data-stu-id="0e683-151">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="0e683-152">请求</span><span class="sxs-lookup"><span data-stu-id="0e683-152">Request</span></span>
<span data-ttu-id="0e683-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e683-153">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0e683-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e683-154">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0e683-155">C#</span><span class="sxs-lookup"><span data-stu-id="0e683-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e683-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e683-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0e683-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e683-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0e683-158">响应</span><span class="sxs-lookup"><span data-stu-id="0e683-158">Response</span></span>
<span data-ttu-id="0e683-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0e683-159">Here is an example of the response.</span></span>
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
