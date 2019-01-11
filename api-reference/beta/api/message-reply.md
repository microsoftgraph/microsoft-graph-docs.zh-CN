---
title: 消息：答复
description: '答复邮件发件人、 将注释添加或修改任何可更新一个**答复**呼叫中的所有属性。 '
localization_priority: Normal
ms.openlocfilehash: 3844969c8c4bbec9026aee8477db968d5a3b0e52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827459"
---
# <a name="message-reply"></a><span data-ttu-id="08beb-103">消息：答复</span><span class="sxs-lookup"><span data-stu-id="08beb-103">message: reply</span></span>

> <span data-ttu-id="08beb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="08beb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08beb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="08beb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08beb-p102">全部在一个 **reply** 调用中回复邮件的发件人、添加注释或修改任意可更新的属性。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="08beb-p102">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call. The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="08beb-108">此外，您可以第一个[创建草稿答复邮件](../api/message-createreply.md)包含评论或更新任何消息属性，然后[发送](../api/message-send.md)答复。</span><span class="sxs-lookup"><span data-stu-id="08beb-108">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="08beb-109">**注意**</span><span class="sxs-lookup"><span data-stu-id="08beb-109">**Note**</span></span>

- <span data-ttu-id="08beb-110">您可以指定注释或的**body**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="08beb-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="08beb-111">如果同时指定将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="08beb-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="08beb-112">如果**回复**属性指定在原始邮件中，每个 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822))，您应在**回复**并不**从**属性中的收件人发送对收件人的答复。</span><span class="sxs-lookup"><span data-stu-id="08beb-112">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="08beb-113">权限</span><span class="sxs-lookup"><span data-stu-id="08beb-113">Permissions</span></span>
<span data-ttu-id="08beb-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08beb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08beb-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="08beb-116">Permission type</span></span>      | <span data-ttu-id="08beb-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08beb-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08beb-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08beb-118">Delegated (work or school account)</span></span> | <span data-ttu-id="08beb-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="08beb-119">Mail.Send</span></span>    |
|<span data-ttu-id="08beb-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08beb-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08beb-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="08beb-121">Mail.Send</span></span>    |
|<span data-ttu-id="08beb-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="08beb-122">Application</span></span> | <span data-ttu-id="08beb-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="08beb-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="08beb-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08beb-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="08beb-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="08beb-125">Request headers</span></span>
| <span data-ttu-id="08beb-126">名称</span><span class="sxs-lookup"><span data-stu-id="08beb-126">Name</span></span>       | <span data-ttu-id="08beb-127">类型</span><span class="sxs-lookup"><span data-stu-id="08beb-127">Type</span></span> | <span data-ttu-id="08beb-128">说明</span><span class="sxs-lookup"><span data-stu-id="08beb-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08beb-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="08beb-129">Authorization</span></span>  | <span data-ttu-id="08beb-130">string</span><span class="sxs-lookup"><span data-stu-id="08beb-130">string</span></span>  | <span data-ttu-id="08beb-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08beb-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08beb-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08beb-133">Content-Type</span></span> | <span data-ttu-id="08beb-134">string</span><span class="sxs-lookup"><span data-stu-id="08beb-134">string</span></span>  | <span data-ttu-id="08beb-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="08beb-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08beb-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="08beb-137">Request body</span></span>
<span data-ttu-id="08beb-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="08beb-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08beb-139">参数</span><span class="sxs-lookup"><span data-stu-id="08beb-139">Parameter</span></span>    | <span data-ttu-id="08beb-140">类型</span><span class="sxs-lookup"><span data-stu-id="08beb-140">Type</span></span>   |<span data-ttu-id="08beb-141">说明</span><span class="sxs-lookup"><span data-stu-id="08beb-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08beb-142">注释</span><span class="sxs-lookup"><span data-stu-id="08beb-142">comment</span></span>|<span data-ttu-id="08beb-143">String</span><span class="sxs-lookup"><span data-stu-id="08beb-143">String</span></span>|<span data-ttu-id="08beb-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="08beb-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="08beb-146">message</span><span class="sxs-lookup"><span data-stu-id="08beb-146">message</span></span>|[<span data-ttu-id="08beb-147">message</span><span class="sxs-lookup"><span data-stu-id="08beb-147">message</span></span>](../resources/message.md)|<span data-ttu-id="08beb-148">若要在答复邮件更新任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="08beb-148">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="08beb-149">响应</span><span class="sxs-lookup"><span data-stu-id="08beb-149">Response</span></span>

<span data-ttu-id="08beb-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="08beb-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08beb-152">示例</span><span class="sxs-lookup"><span data-stu-id="08beb-152">Example</span></span>
<span data-ttu-id="08beb-153">下面的示例包括一条注释，并将收件人添加到答复消息。</span><span class="sxs-lookup"><span data-stu-id="08beb-153">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="08beb-154">请求</span><span class="sxs-lookup"><span data-stu-id="08beb-154">Request</span></span>
<span data-ttu-id="08beb-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08beb-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
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

##### <a name="response"></a><span data-ttu-id="08beb-156">响应</span><span class="sxs-lookup"><span data-stu-id="08beb-156">Response</span></span>
<span data-ttu-id="08beb-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="08beb-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
