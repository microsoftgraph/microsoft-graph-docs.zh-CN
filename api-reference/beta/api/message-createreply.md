---
title: 'message: createReply'
description: '创建答复邮件的草稿以包含注释或更新任何邮件属性 '
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: de6a65d1497007d4d2d9f9f5dd29d5b638c6633f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027634"
---
# <a name="message-createreply"></a><span data-ttu-id="ba6e9-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="ba6e9-103">message: createReply</span></span>

<span data-ttu-id="ba6e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba6e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba6e9-p101">创建回复邮件草稿以全部在一个 createReply 调用中添加注释或更新任意邮件属性。然后，你可以更新或发送草稿。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-p101">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="ba6e9-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="ba6e9-107">**Note**</span></span>

- <span data-ttu-id="ba6e9-108">您可以指定参数的注释或 **body** 属性 `message` 。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="ba6e9-109">同时指定这两个将返回 HTTP 400 错误的请求错误。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="ba6e9-110">如果在原始邮件中指定了 **replyTo** （根据 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) 的 Internet 邮件格式），则应将答复发送到 **replyTo**中的收件人，而不是 **发件**人中的收件人。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-110">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ba6e9-111">权限</span><span class="sxs-lookup"><span data-stu-id="ba6e9-111">Permissions</span></span>
<span data-ttu-id="ba6e9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba6e9-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba6e9-114">Permission type</span></span>      | <span data-ttu-id="ba6e9-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba6e9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba6e9-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba6e9-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ba6e9-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba6e9-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ba6e9-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba6e9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba6e9-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba6e9-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ba6e9-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba6e9-120">Application</span></span> | <span data-ttu-id="ba6e9-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba6e9-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba6e9-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba6e9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="ba6e9-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba6e9-123">Request headers</span></span>
| <span data-ttu-id="ba6e9-124">名称</span><span class="sxs-lookup"><span data-stu-id="ba6e9-124">Name</span></span>       | <span data-ttu-id="ba6e9-125">类型</span><span class="sxs-lookup"><span data-stu-id="ba6e9-125">Type</span></span> | <span data-ttu-id="ba6e9-126">说明</span><span class="sxs-lookup"><span data-stu-id="ba6e9-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba6e9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba6e9-127">Authorization</span></span>  | <span data-ttu-id="ba6e9-128">string</span><span class="sxs-lookup"><span data-stu-id="ba6e9-128">string</span></span>  | <span data-ttu-id="ba6e9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba6e9-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba6e9-131">Content-Type</span></span> | <span data-ttu-id="ba6e9-132">string</span><span class="sxs-lookup"><span data-stu-id="ba6e9-132">string</span></span>  | <span data-ttu-id="ba6e9-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba6e9-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba6e9-135">Request body</span></span>
<span data-ttu-id="ba6e9-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ba6e9-137">参数</span><span class="sxs-lookup"><span data-stu-id="ba6e9-137">Parameter</span></span>    | <span data-ttu-id="ba6e9-138">类型</span><span class="sxs-lookup"><span data-stu-id="ba6e9-138">Type</span></span>   |<span data-ttu-id="ba6e9-139">说明</span><span class="sxs-lookup"><span data-stu-id="ba6e9-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba6e9-140">注释</span><span class="sxs-lookup"><span data-stu-id="ba6e9-140">comment</span></span>|<span data-ttu-id="ba6e9-141">String</span><span class="sxs-lookup"><span data-stu-id="ba6e9-141">String</span></span>|<span data-ttu-id="ba6e9-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ba6e9-144">message</span><span class="sxs-lookup"><span data-stu-id="ba6e9-144">message</span></span>|[<span data-ttu-id="ba6e9-145">邮件</span><span class="sxs-lookup"><span data-stu-id="ba6e9-145">message</span></span>](../resources/message.md)|<span data-ttu-id="ba6e9-146">答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="ba6e9-147">响应</span><span class="sxs-lookup"><span data-stu-id="ba6e9-147">Response</span></span>

<span data-ttu-id="ba6e9-148">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-148">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba6e9-149">示例</span><span class="sxs-lookup"><span data-stu-id="ba6e9-149">Example</span></span>
<span data-ttu-id="ba6e9-150">下面的示例创建一个 "答复草稿"，在请求正文中添加注释和收件人。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-150">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="ba6e9-151">请求</span><span class="sxs-lookup"><span data-stu-id="ba6e9-151">Request</span></span>
<span data-ttu-id="ba6e9-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-152">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ba6e9-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba6e9-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ba6e9-154">C#</span><span class="sxs-lookup"><span data-stu-id="ba6e9-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba6e9-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba6e9-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba6e9-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba6e9-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ba6e9-157">响应</span><span class="sxs-lookup"><span data-stu-id="ba6e9-157">Response</span></span>
<span data-ttu-id="ba6e9-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ba6e9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->


