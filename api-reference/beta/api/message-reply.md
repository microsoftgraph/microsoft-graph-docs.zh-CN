---
title: 消息：答复
description: '答复邮件发件人、 将注释添加或修改任何可更新一个**答复**呼叫中的所有属性。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6461d9735459ff9cf956820b00bb61a4d42d1ec0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519008"
---
# <a name="message-reply"></a><span data-ttu-id="1a06e-103">消息：答复</span><span class="sxs-lookup"><span data-stu-id="1a06e-103">message: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a06e-p101">全部在一个 reply 调用中回复邮件的发件人、添加注释或修改任意可更新的属性。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="1a06e-p101">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call. The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="1a06e-106">此外，您可以第一个[创建草稿答复邮件](../api/message-createreply.md)包含评论或更新任何消息属性，然后[发送](../api/message-send.md)答复。</span><span class="sxs-lookup"><span data-stu-id="1a06e-106">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="1a06e-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="1a06e-107">**Note**</span></span>

- <span data-ttu-id="1a06e-108">您可以指定注释或的**body**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="1a06e-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="1a06e-109">如果同时指定将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="1a06e-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="1a06e-110">如果**回复**属性指定在原始邮件中，每个 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822))，您应在**回复**并不**从**属性中的收件人发送对收件人的答复。</span><span class="sxs-lookup"><span data-stu-id="1a06e-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="1a06e-111">权限</span><span class="sxs-lookup"><span data-stu-id="1a06e-111">Permissions</span></span>
<span data-ttu-id="1a06e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a06e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a06e-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a06e-114">Permission type</span></span>      | <span data-ttu-id="1a06e-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a06e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a06e-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a06e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="1a06e-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1a06e-117">Mail.Send</span></span>    |
|<span data-ttu-id="1a06e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a06e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a06e-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1a06e-119">Mail.Send</span></span>    |
|<span data-ttu-id="1a06e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a06e-120">Application</span></span> | <span data-ttu-id="1a06e-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1a06e-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a06e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a06e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="1a06e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a06e-123">Request headers</span></span>
| <span data-ttu-id="1a06e-124">名称</span><span class="sxs-lookup"><span data-stu-id="1a06e-124">Name</span></span>       | <span data-ttu-id="1a06e-125">类型</span><span class="sxs-lookup"><span data-stu-id="1a06e-125">Type</span></span> | <span data-ttu-id="1a06e-126">说明</span><span class="sxs-lookup"><span data-stu-id="1a06e-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1a06e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a06e-127">Authorization</span></span>  | <span data-ttu-id="1a06e-128">string</span><span class="sxs-lookup"><span data-stu-id="1a06e-128">string</span></span>  | <span data-ttu-id="1a06e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a06e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a06e-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a06e-131">Content-Type</span></span> | <span data-ttu-id="1a06e-132">string</span><span class="sxs-lookup"><span data-stu-id="1a06e-132">string</span></span>  | <span data-ttu-id="1a06e-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="1a06e-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a06e-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a06e-135">Request body</span></span>
<span data-ttu-id="1a06e-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1a06e-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a06e-137">参数</span><span class="sxs-lookup"><span data-stu-id="1a06e-137">Parameter</span></span>    | <span data-ttu-id="1a06e-138">类型</span><span class="sxs-lookup"><span data-stu-id="1a06e-138">Type</span></span>   |<span data-ttu-id="1a06e-139">说明</span><span class="sxs-lookup"><span data-stu-id="1a06e-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a06e-140">注释</span><span class="sxs-lookup"><span data-stu-id="1a06e-140">comment</span></span>|<span data-ttu-id="1a06e-141">String</span><span class="sxs-lookup"><span data-stu-id="1a06e-141">String</span></span>|<span data-ttu-id="1a06e-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="1a06e-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="1a06e-144">message</span><span class="sxs-lookup"><span data-stu-id="1a06e-144">message</span></span>|[<span data-ttu-id="1a06e-145">message</span><span class="sxs-lookup"><span data-stu-id="1a06e-145">message</span></span>](../resources/message.md)|<span data-ttu-id="1a06e-146">若要在答复邮件更新任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="1a06e-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="1a06e-147">响应</span><span class="sxs-lookup"><span data-stu-id="1a06e-147">Response</span></span>

<span data-ttu-id="1a06e-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1a06e-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a06e-150">示例</span><span class="sxs-lookup"><span data-stu-id="1a06e-150">Example</span></span>
<span data-ttu-id="1a06e-151">下面的示例包括一条注释，并将收件人添加到答复消息。</span><span class="sxs-lookup"><span data-stu-id="1a06e-151">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="1a06e-152">请求</span><span class="sxs-lookup"><span data-stu-id="1a06e-152">Request</span></span>
<span data-ttu-id="1a06e-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a06e-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1a06e-154">响应</span><span class="sxs-lookup"><span data-stu-id="1a06e-154">Response</span></span>
<span data-ttu-id="1a06e-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a06e-155">Here is an example of the response.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/message-reply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
