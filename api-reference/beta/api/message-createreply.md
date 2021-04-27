---
title: 'message: createReply'
description: '创建回复邮件草稿以包含注释或更新任何邮件属性 '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f952621dce25b4aa1525b4a7fafb21ca231259fa
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052164"
---
# <a name="message-createreply"></a><span data-ttu-id="46418-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="46418-103">message: createReply</span></span>

<span data-ttu-id="46418-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46418-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46418-p101">创建回复邮件草稿以全部在一个 createReply 调用中添加注释或更新任意邮件属性。然后，你可以更新或发送草稿。</span><span class="sxs-lookup"><span data-stu-id="46418-p101">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="46418-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="46418-107">**Note**</span></span>

- <span data-ttu-id="46418-108">可以指定参数的 comment 或 **body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="46418-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="46418-109">指定这两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="46418-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="46418-110">如果在原始邮件中指定了 **replyTo，** 则根据 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ，您应该将答复发送给 **replyTo** 中的收件人，而不是 中的 **收件人**。</span><span class="sxs-lookup"><span data-stu-id="46418-110">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="46418-111">权限</span><span class="sxs-lookup"><span data-stu-id="46418-111">Permissions</span></span>
<span data-ttu-id="46418-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46418-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46418-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="46418-114">Permission type</span></span>      | <span data-ttu-id="46418-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46418-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46418-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46418-116">Delegated (work or school account)</span></span> | <span data-ttu-id="46418-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46418-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="46418-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46418-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46418-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46418-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="46418-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="46418-120">Application</span></span> | <span data-ttu-id="46418-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46418-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="46418-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46418-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="46418-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="46418-123">Request headers</span></span>
| <span data-ttu-id="46418-124">名称</span><span class="sxs-lookup"><span data-stu-id="46418-124">Name</span></span>       | <span data-ttu-id="46418-125">类型</span><span class="sxs-lookup"><span data-stu-id="46418-125">Type</span></span> | <span data-ttu-id="46418-126">说明</span><span class="sxs-lookup"><span data-stu-id="46418-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46418-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="46418-127">Authorization</span></span>  | <span data-ttu-id="46418-128">string</span><span class="sxs-lookup"><span data-stu-id="46418-128">string</span></span>  | <span data-ttu-id="46418-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46418-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46418-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46418-131">Content-Type</span></span> | <span data-ttu-id="46418-132">string</span><span class="sxs-lookup"><span data-stu-id="46418-132">string</span></span>  | <span data-ttu-id="46418-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="46418-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46418-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="46418-135">Request body</span></span>
<span data-ttu-id="46418-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="46418-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="46418-137">参数</span><span class="sxs-lookup"><span data-stu-id="46418-137">Parameter</span></span>    | <span data-ttu-id="46418-138">类型</span><span class="sxs-lookup"><span data-stu-id="46418-138">Type</span></span>   |<span data-ttu-id="46418-139">说明</span><span class="sxs-lookup"><span data-stu-id="46418-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46418-140">注释</span><span class="sxs-lookup"><span data-stu-id="46418-140">comment</span></span>|<span data-ttu-id="46418-141">String</span><span class="sxs-lookup"><span data-stu-id="46418-141">String</span></span>|<span data-ttu-id="46418-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="46418-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="46418-144">message</span><span class="sxs-lookup"><span data-stu-id="46418-144">message</span></span>|[<span data-ttu-id="46418-145">message</span><span class="sxs-lookup"><span data-stu-id="46418-145">message</span></span>](../resources/message.md)|<span data-ttu-id="46418-146">回复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="46418-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="46418-147">响应</span><span class="sxs-lookup"><span data-stu-id="46418-147">Response</span></span>

<span data-ttu-id="46418-148">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46418-148">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46418-149">示例</span><span class="sxs-lookup"><span data-stu-id="46418-149">Example</span></span>
<span data-ttu-id="46418-150">以下示例创建答复草稿，在请求正文中添加注释和收件人。</span><span class="sxs-lookup"><span data-stu-id="46418-150">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="46418-151">请求</span><span class="sxs-lookup"><span data-stu-id="46418-151">Request</span></span>
<span data-ttu-id="46418-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46418-152">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46418-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="46418-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="46418-154">C#</span><span class="sxs-lookup"><span data-stu-id="46418-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46418-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46418-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46418-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46418-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46418-157">Java</span><span class="sxs-lookup"><span data-stu-id="46418-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="46418-158">响应</span><span class="sxs-lookup"><span data-stu-id="46418-158">Response</span></span>
<span data-ttu-id="46418-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="46418-159">Here is an example of the response.</span></span> <span data-ttu-id="46418-160">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="46418-160">Note: The response object shown here might be shortened for readability.</span></span>
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


