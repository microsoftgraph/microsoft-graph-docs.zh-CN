---
title: 'message: createReply'
description: '创建包含评论或更新任何邮件属性的答复邮件草稿 '
ms.openlocfilehash: 40bdd5792e9d7a018fc8c7b1aca2d5955a8ef807
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048632"
---
# <a name="message-createreply"></a><span data-ttu-id="8dbdb-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="8dbdb-103">message: createReply</span></span>

> <span data-ttu-id="8dbdb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8dbdb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8dbdb-p102">创建回复邮件草稿以全部在一个 **createReply** 调用中添加注释或更新任意邮件属性。然后，你可以[更新](../api/message-update.md)或[发送](../api/message-send.md)草稿。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-p102">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="8dbdb-108">**注意**</span><span class="sxs-lookup"><span data-stu-id="8dbdb-108">**Note**</span></span>

- <span data-ttu-id="8dbdb-109">您可以指定注释或的**body**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="8dbdb-110">如果同时指定将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="8dbdb-111">如果**回复**指定在原始邮件中，每个 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822))，您应**从**中发送对**回复**中的收件人和不收件人的答复。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-111">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8dbdb-112">权限</span><span class="sxs-lookup"><span data-stu-id="8dbdb-112">Permissions</span></span>
<span data-ttu-id="8dbdb-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dbdb-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="8dbdb-115">Permission type</span></span>      | <span data-ttu-id="8dbdb-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8dbdb-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dbdb-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8dbdb-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8dbdb-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8dbdb-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8dbdb-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8dbdb-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dbdb-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8dbdb-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8dbdb-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="8dbdb-121">Application</span></span> | <span data-ttu-id="8dbdb-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8dbdb-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dbdb-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8dbdb-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="8dbdb-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="8dbdb-124">Request headers</span></span>
| <span data-ttu-id="8dbdb-125">名称</span><span class="sxs-lookup"><span data-stu-id="8dbdb-125">Name</span></span>       | <span data-ttu-id="8dbdb-126">类型</span><span class="sxs-lookup"><span data-stu-id="8dbdb-126">Type</span></span> | <span data-ttu-id="8dbdb-127">说明</span><span class="sxs-lookup"><span data-stu-id="8dbdb-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8dbdb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dbdb-128">Authorization</span></span>  | <span data-ttu-id="8dbdb-129">string</span><span class="sxs-lookup"><span data-stu-id="8dbdb-129">string</span></span>  | <span data-ttu-id="8dbdb-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8dbdb-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8dbdb-132">Content-Type</span></span> | <span data-ttu-id="8dbdb-133">string</span><span class="sxs-lookup"><span data-stu-id="8dbdb-133">string</span></span>  | <span data-ttu-id="8dbdb-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dbdb-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="8dbdb-136">Request body</span></span>
<span data-ttu-id="8dbdb-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8dbdb-138">参数</span><span class="sxs-lookup"><span data-stu-id="8dbdb-138">Parameter</span></span>    | <span data-ttu-id="8dbdb-139">类型</span><span class="sxs-lookup"><span data-stu-id="8dbdb-139">Type</span></span>   |<span data-ttu-id="8dbdb-140">说明</span><span class="sxs-lookup"><span data-stu-id="8dbdb-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dbdb-141">注释</span><span class="sxs-lookup"><span data-stu-id="8dbdb-141">comment</span></span>|<span data-ttu-id="8dbdb-142">String</span><span class="sxs-lookup"><span data-stu-id="8dbdb-142">String</span></span>|<span data-ttu-id="8dbdb-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="8dbdb-145">message</span><span class="sxs-lookup"><span data-stu-id="8dbdb-145">message</span></span>|[<span data-ttu-id="8dbdb-146">message</span><span class="sxs-lookup"><span data-stu-id="8dbdb-146">message</span></span>](../resources/message.md)|<span data-ttu-id="8dbdb-147">若要在答复邮件更新任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="8dbdb-148">响应</span><span class="sxs-lookup"><span data-stu-id="8dbdb-148">Response</span></span>

<span data-ttu-id="8dbdb-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-149">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dbdb-150">示例</span><span class="sxs-lookup"><span data-stu-id="8dbdb-150">Example</span></span>
<span data-ttu-id="8dbdb-151">下面的示例创建答复草稿，在请求正文中添加注释和收件人。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-151">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="8dbdb-152">请求</span><span class="sxs-lookup"><span data-stu-id="8dbdb-152">Request</span></span>
<span data-ttu-id="8dbdb-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply
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
  "comment": "Samantha, Randi, would you name the group if the project is approved, please?" 
}
```

##### <a name="response"></a><span data-ttu-id="8dbdb-154">响应</span><span class="sxs-lookup"><span data-stu-id="8dbdb-154">Response</span></span>
<span data-ttu-id="8dbdb-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8dbdb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKoAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DO\"",
  "id": "AAMkADA1MTAAAH5JKoAAA=",
  "subject": "RE: Let's start a group",
  "Body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>Samantha, Randi, would you name the group if the project is approved, please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n<p>That's a great idea!<br>\r\n</body>\r\n</html>"
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
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
