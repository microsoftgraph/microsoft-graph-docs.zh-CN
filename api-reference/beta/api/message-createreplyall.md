---
title: 'message: createReplyAll'
description: '创建包含评论或更新任何消息属性的全部答复邮件草稿 '
ms.openlocfilehash: 85cdef106fcd84764fe0d5f86d24ecef6b6ed29e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045411"
---
# <a name="message-createreplyall"></a><span data-ttu-id="624d4-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="624d4-103">message: createReplyAll</span></span>

> <span data-ttu-id="624d4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="624d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="624d4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="624d4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="624d4-p102">创建回复全部邮件草稿以全部在一个 **createReplyAll** 调用中添加注释或更新任意邮件属性。然后，你可以[更新](../api/message-update.md)或[发送](../api/message-send.md)草稿。</span><span class="sxs-lookup"><span data-stu-id="624d4-p102">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="624d4-108">**注意**</span><span class="sxs-lookup"><span data-stu-id="624d4-108">**Note**</span></span>

- <span data-ttu-id="624d4-109">您可以指定注释或的**body**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="624d4-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="624d4-110">如果同时指定将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="624d4-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="624d4-111">如果**回复**属性指定在原始邮件中，每个 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822))，您应发送给收件人的答复</span><span class="sxs-lookup"><span data-stu-id="624d4-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="624d4-112">**回复**和**toRecipients**属性，并不**从**和**toRecipients**属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="624d4-112">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="624d4-113">权限</span><span class="sxs-lookup"><span data-stu-id="624d4-113">Permissions</span></span>
<span data-ttu-id="624d4-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="624d4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="624d4-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="624d4-116">Permission type</span></span>      | <span data-ttu-id="624d4-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="624d4-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="624d4-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="624d4-118">Delegated (work or school account)</span></span> | <span data-ttu-id="624d4-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="624d4-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="624d4-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="624d4-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="624d4-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="624d4-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="624d4-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="624d4-122">Application</span></span> | <span data-ttu-id="624d4-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="624d4-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="624d4-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="624d4-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="624d4-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="624d4-125">Request headers</span></span>
| <span data-ttu-id="624d4-126">名称</span><span class="sxs-lookup"><span data-stu-id="624d4-126">Name</span></span>       | <span data-ttu-id="624d4-127">类型</span><span class="sxs-lookup"><span data-stu-id="624d4-127">Type</span></span> | <span data-ttu-id="624d4-128">说明</span><span class="sxs-lookup"><span data-stu-id="624d4-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="624d4-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="624d4-129">Authorization</span></span>  | <span data-ttu-id="624d4-130">string</span><span class="sxs-lookup"><span data-stu-id="624d4-130">string</span></span>  | <span data-ttu-id="624d4-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="624d4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="624d4-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="624d4-133">Content-Type</span></span> | <span data-ttu-id="624d4-134">string</span><span class="sxs-lookup"><span data-stu-id="624d4-134">string</span></span>  | <span data-ttu-id="624d4-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="624d4-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="624d4-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="624d4-137">Request body</span></span>
<span data-ttu-id="624d4-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="624d4-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="624d4-139">参数</span><span class="sxs-lookup"><span data-stu-id="624d4-139">Parameter</span></span>    | <span data-ttu-id="624d4-140">类型</span><span class="sxs-lookup"><span data-stu-id="624d4-140">Type</span></span>   |<span data-ttu-id="624d4-141">说明</span><span class="sxs-lookup"><span data-stu-id="624d4-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="624d4-142">注释</span><span class="sxs-lookup"><span data-stu-id="624d4-142">comment</span></span>|<span data-ttu-id="624d4-143">String</span><span class="sxs-lookup"><span data-stu-id="624d4-143">String</span></span>|<span data-ttu-id="624d4-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="624d4-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="624d4-146">message</span><span class="sxs-lookup"><span data-stu-id="624d4-146">message</span></span>|[<span data-ttu-id="624d4-147">message</span><span class="sxs-lookup"><span data-stu-id="624d4-147">message</span></span>](../resources/message.md)|<span data-ttu-id="624d4-148">全部答复邮件中更新任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="624d4-148">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="624d4-149">响应</span><span class="sxs-lookup"><span data-stu-id="624d4-149">Response</span></span>

<span data-ttu-id="624d4-150">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="624d4-150">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="624d4-151">示例</span><span class="sxs-lookup"><span data-stu-id="624d4-151">Example</span></span>
<span data-ttu-id="624d4-152">下面的示例草稿答复所有，并将附件和批注添加一个**createReplyAll**呼叫中的所有。</span><span class="sxs-lookup"><span data-stu-id="624d4-152">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="624d4-153">请求</span><span class="sxs-lookup"><span data-stu-id="624d4-153">Request</span></span>
<span data-ttu-id="624d4-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="624d4-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/createReplyAll
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
    "comment": "if the project gets approved, please take a look at the attached guidelines before you decide on the name." 
}
```

##### <a name="response"></a><span data-ttu-id="624d4-155">响应</span><span class="sxs-lookup"><span data-stu-id="624d4-155">Response</span></span>
<span data-ttu-id="624d4-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="624d4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKpAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DP\"",
  "id": "AAMkADA1MTAAAH5JKpAAA=",
  "subject": "RE: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body dir=\"ltr\">\r\nif the project gets approved, please take a look at the attached guidelines before you decide on the name.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:36:32 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group\r\n<div>Samantha, Randi, would you name the group please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n</body>\r\n</html>"
  },
  "sender": {
    "emailAddress": {
      "name": "Admin",
      "address": "admin@contoso.onmicrosoft.com"
    }
  },
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress": {
        "name": "Randi Welch",
        "address": "randiw@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
