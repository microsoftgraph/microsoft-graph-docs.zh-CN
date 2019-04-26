---
title: 消息：答复
description: '全部在一个 **reply** 调用中回复邮件的发件人、添加注释或修改任意可更新的属性。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c745cfaab60aae9395e2b8d720852a1d2b2b2a39
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333196"
---
# <a name="message-reply"></a><span data-ttu-id="32d0c-103">消息：答复</span><span class="sxs-lookup"><span data-stu-id="32d0c-103">message: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32d0c-p101">全部在一个 **reply** 调用中回复邮件的发件人、添加注释或修改任意可更新的属性。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="32d0c-p101">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call. The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="32d0c-106">或者, 您可以先[创建草稿答复邮件](../api/message-createreply.md)以包含注释或更新任何邮件属性, 然后[发送](../api/message-send.md)回复。</span><span class="sxs-lookup"><span data-stu-id="32d0c-106">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="32d0c-107">**备注**</span><span class="sxs-lookup"><span data-stu-id="32d0c-107">**Note**</span></span>

- <span data-ttu-id="32d0c-108">您可以指定`message`参数的注释或**body**属性。</span><span class="sxs-lookup"><span data-stu-id="32d0c-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="32d0c-109">同时指定这两个将返回 HTTP 400 错误的请求错误。</span><span class="sxs-lookup"><span data-stu-id="32d0c-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="32d0c-110">如果在原始邮件中指定了**replyTo**属性 (根据 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822))), 则应将答复发送给**replyTo**中的收件人, 而不是发**件**人属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="32d0c-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="32d0c-111">权限</span><span class="sxs-lookup"><span data-stu-id="32d0c-111">Permissions</span></span>
<span data-ttu-id="32d0c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32d0c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32d0c-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="32d0c-114">Permission type</span></span>      | <span data-ttu-id="32d0c-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32d0c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32d0c-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32d0c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="32d0c-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="32d0c-117">Mail.Send</span></span>    |
|<span data-ttu-id="32d0c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32d0c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32d0c-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="32d0c-119">Mail.Send</span></span>    |
|<span data-ttu-id="32d0c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="32d0c-120">Application</span></span> | <span data-ttu-id="32d0c-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="32d0c-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="32d0c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32d0c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="32d0c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="32d0c-123">Request headers</span></span>
| <span data-ttu-id="32d0c-124">名称</span><span class="sxs-lookup"><span data-stu-id="32d0c-124">Name</span></span>       | <span data-ttu-id="32d0c-125">类型</span><span class="sxs-lookup"><span data-stu-id="32d0c-125">Type</span></span> | <span data-ttu-id="32d0c-126">说明</span><span class="sxs-lookup"><span data-stu-id="32d0c-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="32d0c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="32d0c-127">Authorization</span></span>  | <span data-ttu-id="32d0c-128">string</span><span class="sxs-lookup"><span data-stu-id="32d0c-128">string</span></span>  | <span data-ttu-id="32d0c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32d0c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32d0c-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32d0c-131">Content-Type</span></span> | <span data-ttu-id="32d0c-132">string</span><span class="sxs-lookup"><span data-stu-id="32d0c-132">string</span></span>  | <span data-ttu-id="32d0c-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="32d0c-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32d0c-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="32d0c-135">Request body</span></span>
<span data-ttu-id="32d0c-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="32d0c-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="32d0c-137">参数</span><span class="sxs-lookup"><span data-stu-id="32d0c-137">Parameter</span></span>    | <span data-ttu-id="32d0c-138">类型</span><span class="sxs-lookup"><span data-stu-id="32d0c-138">Type</span></span>   |<span data-ttu-id="32d0c-139">说明</span><span class="sxs-lookup"><span data-stu-id="32d0c-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32d0c-140">注释</span><span class="sxs-lookup"><span data-stu-id="32d0c-140">comment</span></span>|<span data-ttu-id="32d0c-141">String</span><span class="sxs-lookup"><span data-stu-id="32d0c-141">String</span></span>|<span data-ttu-id="32d0c-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="32d0c-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="32d0c-144">message</span><span class="sxs-lookup"><span data-stu-id="32d0c-144">message</span></span>|[<span data-ttu-id="32d0c-145">邮件</span><span class="sxs-lookup"><span data-stu-id="32d0c-145">message</span></span>](../resources/message.md)|<span data-ttu-id="32d0c-146">答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="32d0c-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="32d0c-147">响应</span><span class="sxs-lookup"><span data-stu-id="32d0c-147">Response</span></span>

<span data-ttu-id="32d0c-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="32d0c-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32d0c-150">示例</span><span class="sxs-lookup"><span data-stu-id="32d0c-150">Example</span></span>
<span data-ttu-id="32d0c-151">下面的示例包含注释并将收件人添加到回复邮件中。</span><span class="sxs-lookup"><span data-stu-id="32d0c-151">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="32d0c-152">请求</span><span class="sxs-lookup"><span data-stu-id="32d0c-152">Request</span></span>
<span data-ttu-id="32d0c-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32d0c-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="32d0c-154">响应</span><span class="sxs-lookup"><span data-stu-id="32d0c-154">Response</span></span>
<span data-ttu-id="32d0c-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="32d0c-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
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
  "suppressions": []
}
-->
