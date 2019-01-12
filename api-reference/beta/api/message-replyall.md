---
title: 消息：replyAll
description: '通过指定注释和修改任何可更新属性回复邮件的所有收件人 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1abbf271350c6bbbd10af1f17c6c7d3069c3cf22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976364"
---
# <a name="message-replyall"></a><span data-ttu-id="aa752-103">消息：replyAll</span><span class="sxs-lookup"><span data-stu-id="aa752-103">message: replyAll</span></span>

> <span data-ttu-id="aa752-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aa752-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa752-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa752-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa752-106">通过指定注释和所有使用**replyAll**方法修改的回复，任何可更新属性回复邮件的所有收件人。</span><span class="sxs-lookup"><span data-stu-id="aa752-106">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="aa752-107">然后在已发送邮件文件夹中保存邮件。</span><span class="sxs-lookup"><span data-stu-id="aa752-107">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="aa752-108">此外，您可以第一个[创建草稿全部答复邮件](../api/message-createreplyall.md)包含评论或更新任何消息属性，然后[发送](../api/message-send.md)答复。</span><span class="sxs-lookup"><span data-stu-id="aa752-108">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="aa752-109">**注意**</span><span class="sxs-lookup"><span data-stu-id="aa752-109">**Note**</span></span>

- <span data-ttu-id="aa752-110">您可以指定注释或的**body**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="aa752-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="aa752-111">如果同时指定将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="aa752-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="aa752-112">如果**回复**属性指定在原始邮件中，每个 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822))，您应发送给收件人的答复</span><span class="sxs-lookup"><span data-stu-id="aa752-112">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="aa752-113">**回复**和**toRecipients**属性，并不**从**和**toRecipients**属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="aa752-113">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="aa752-114">权限</span><span class="sxs-lookup"><span data-stu-id="aa752-114">Permissions</span></span>
<span data-ttu-id="aa752-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa752-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa752-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa752-117">Permission type</span></span>      | <span data-ttu-id="aa752-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa752-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa752-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa752-119">Delegated (work or school account)</span></span> | <span data-ttu-id="aa752-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="aa752-120">Mail.Send</span></span>    |
|<span data-ttu-id="aa752-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa752-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa752-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="aa752-122">Mail.Send</span></span>    |
|<span data-ttu-id="aa752-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa752-123">Application</span></span> | <span data-ttu-id="aa752-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="aa752-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa752-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa752-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="aa752-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa752-126">Request headers</span></span>
| <span data-ttu-id="aa752-127">名称</span><span class="sxs-lookup"><span data-stu-id="aa752-127">Name</span></span>       | <span data-ttu-id="aa752-128">类型</span><span class="sxs-lookup"><span data-stu-id="aa752-128">Type</span></span> | <span data-ttu-id="aa752-129">说明</span><span class="sxs-lookup"><span data-stu-id="aa752-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa752-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa752-130">Authorization</span></span>  | <span data-ttu-id="aa752-131">string</span><span class="sxs-lookup"><span data-stu-id="aa752-131">string</span></span>  | <span data-ttu-id="aa752-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa752-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa752-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa752-134">Content-Type</span></span> | <span data-ttu-id="aa752-135">string</span><span class="sxs-lookup"><span data-stu-id="aa752-135">string</span></span>  | <span data-ttu-id="aa752-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="aa752-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa752-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa752-138">Request body</span></span>
<span data-ttu-id="aa752-139">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="aa752-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aa752-140">参数</span><span class="sxs-lookup"><span data-stu-id="aa752-140">Parameter</span></span>    | <span data-ttu-id="aa752-141">类型</span><span class="sxs-lookup"><span data-stu-id="aa752-141">Type</span></span>   |<span data-ttu-id="aa752-142">说明</span><span class="sxs-lookup"><span data-stu-id="aa752-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa752-143">注释</span><span class="sxs-lookup"><span data-stu-id="aa752-143">comment</span></span>|<span data-ttu-id="aa752-144">String</span><span class="sxs-lookup"><span data-stu-id="aa752-144">String</span></span>|<span data-ttu-id="aa752-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="aa752-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="aa752-147">message</span><span class="sxs-lookup"><span data-stu-id="aa752-147">message</span></span>|[<span data-ttu-id="aa752-148">message</span><span class="sxs-lookup"><span data-stu-id="aa752-148">message</span></span>](../resources/message.md)|<span data-ttu-id="aa752-149">若要在答复邮件更新任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="aa752-149">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="aa752-150">响应</span><span class="sxs-lookup"><span data-stu-id="aa752-150">Response</span></span>

<span data-ttu-id="aa752-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="aa752-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa752-153">示例</span><span class="sxs-lookup"><span data-stu-id="aa752-153">Example</span></span>
<span data-ttu-id="aa752-154">下面的示例包括一条注释，并将添加到全部答复邮件附件。</span><span class="sxs-lookup"><span data-stu-id="aa752-154">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="aa752-155">请求</span><span class="sxs-lookup"><span data-stu-id="aa752-155">Request</span></span>
<span data-ttu-id="aa752-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa752-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```


##### <a name="response"></a><span data-ttu-id="aa752-157">响应</span><span class="sxs-lookup"><span data-stu-id="aa752-157">Response</span></span>
<span data-ttu-id="aa752-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aa752-158">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
