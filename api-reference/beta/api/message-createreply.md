---
title: 'message: createReply'
description: '创建包含评论或更新任何邮件属性的答复邮件草稿 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 112db29116625da1c154783eee840c7a69b5ebfc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526835"
---
# <a name="message-createreply"></a><span data-ttu-id="43be0-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="43be0-103">message: createReply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43be0-p101">创建回复邮件草稿以全部在一个 createReply 调用中添加注释或更新任意邮件属性。然后，你可以更新或发送草稿。</span><span class="sxs-lookup"><span data-stu-id="43be0-p101">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="43be0-106">**注意**</span><span class="sxs-lookup"><span data-stu-id="43be0-106">**Note**</span></span>

- <span data-ttu-id="43be0-107">您可以指定注释或的**body**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="43be0-107">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="43be0-108">如果同时指定将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="43be0-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="43be0-109">如果**回复**指定在原始邮件中，每个 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822))，您应**从**中发送对**回复**中的收件人和不收件人的答复。</span><span class="sxs-lookup"><span data-stu-id="43be0-109">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="43be0-110">权限</span><span class="sxs-lookup"><span data-stu-id="43be0-110">Permissions</span></span>
<span data-ttu-id="43be0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43be0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43be0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="43be0-113">Permission type</span></span>      | <span data-ttu-id="43be0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43be0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43be0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43be0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="43be0-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43be0-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="43be0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43be0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43be0-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43be0-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="43be0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="43be0-119">Application</span></span> | <span data-ttu-id="43be0-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43be0-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="43be0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43be0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="43be0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="43be0-122">Request headers</span></span>
| <span data-ttu-id="43be0-123">名称</span><span class="sxs-lookup"><span data-stu-id="43be0-123">Name</span></span>       | <span data-ttu-id="43be0-124">类型</span><span class="sxs-lookup"><span data-stu-id="43be0-124">Type</span></span> | <span data-ttu-id="43be0-125">说明</span><span class="sxs-lookup"><span data-stu-id="43be0-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="43be0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="43be0-126">Authorization</span></span>  | <span data-ttu-id="43be0-127">string</span><span class="sxs-lookup"><span data-stu-id="43be0-127">string</span></span>  | <span data-ttu-id="43be0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="43be0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="43be0-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43be0-130">Content-Type</span></span> | <span data-ttu-id="43be0-131">string</span><span class="sxs-lookup"><span data-stu-id="43be0-131">string</span></span>  | <span data-ttu-id="43be0-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="43be0-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43be0-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="43be0-134">Request body</span></span>
<span data-ttu-id="43be0-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="43be0-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="43be0-136">参数</span><span class="sxs-lookup"><span data-stu-id="43be0-136">Parameter</span></span>    | <span data-ttu-id="43be0-137">类型</span><span class="sxs-lookup"><span data-stu-id="43be0-137">Type</span></span>   |<span data-ttu-id="43be0-138">说明</span><span class="sxs-lookup"><span data-stu-id="43be0-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43be0-139">注释</span><span class="sxs-lookup"><span data-stu-id="43be0-139">comment</span></span>|<span data-ttu-id="43be0-140">String</span><span class="sxs-lookup"><span data-stu-id="43be0-140">String</span></span>|<span data-ttu-id="43be0-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="43be0-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="43be0-143">message</span><span class="sxs-lookup"><span data-stu-id="43be0-143">message</span></span>|[<span data-ttu-id="43be0-144">message</span><span class="sxs-lookup"><span data-stu-id="43be0-144">message</span></span>](../resources/message.md)|<span data-ttu-id="43be0-145">若要在答复邮件更新任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="43be0-145">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="43be0-146">响应</span><span class="sxs-lookup"><span data-stu-id="43be0-146">Response</span></span>

<span data-ttu-id="43be0-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43be0-147">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43be0-148">示例</span><span class="sxs-lookup"><span data-stu-id="43be0-148">Example</span></span>
<span data-ttu-id="43be0-149">下面的示例创建答复草稿，在请求正文中添加注释和收件人。</span><span class="sxs-lookup"><span data-stu-id="43be0-149">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="43be0-150">请求</span><span class="sxs-lookup"><span data-stu-id="43be0-150">Request</span></span>
<span data-ttu-id="43be0-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43be0-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="43be0-152">响应</span><span class="sxs-lookup"><span data-stu-id="43be0-152">Response</span></span>
<span data-ttu-id="43be0-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43be0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-createreply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
