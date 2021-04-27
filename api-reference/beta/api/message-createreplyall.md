---
title: 'message: createReplyAll'
description: '创建全部答复邮件的草稿以包含注释或更新任何邮件属性， '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ac0e9047933d51773601d64aff8970758f36a171
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052157"
---
# <a name="message-createreplyall"></a><span data-ttu-id="5f33c-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="5f33c-103">message: createReplyAll</span></span>

<span data-ttu-id="5f33c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f33c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f33c-p101">创建回复全部邮件草稿以全部在一个 createReplyAll 调用中添加注释或更新任意邮件属性。然后，你可以更新或发送草稿。</span><span class="sxs-lookup"><span data-stu-id="5f33c-p101">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="5f33c-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="5f33c-107">**Note**</span></span>

- <span data-ttu-id="5f33c-108">可以指定参数的 comment 或 **body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="5f33c-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="5f33c-109">指定这两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="5f33c-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="5f33c-110">如果在原始邮件中指定了 **replyTo** 属性，则根据 [RFC 2822](https://www.rfc-editor.org/info/rfc2822) (Internet 邮件格式) ，您应将答复发送给</span><span class="sxs-lookup"><span data-stu-id="5f33c-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="5f33c-111">**replyTo** 和 **toRecipients** 属性，而不是 **from** 和 **toRecipients 属性中的** 收件人。</span><span class="sxs-lookup"><span data-stu-id="5f33c-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="5f33c-112">权限</span><span class="sxs-lookup"><span data-stu-id="5f33c-112">Permissions</span></span>
<span data-ttu-id="5f33c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f33c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f33c-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f33c-115">Permission type</span></span>      | <span data-ttu-id="5f33c-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f33c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f33c-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f33c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="5f33c-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f33c-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f33c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f33c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f33c-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f33c-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f33c-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f33c-121">Application</span></span> | <span data-ttu-id="5f33c-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f33c-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f33c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f33c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="5f33c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f33c-124">Request headers</span></span>
| <span data-ttu-id="5f33c-125">名称</span><span class="sxs-lookup"><span data-stu-id="5f33c-125">Name</span></span>       | <span data-ttu-id="5f33c-126">类型</span><span class="sxs-lookup"><span data-stu-id="5f33c-126">Type</span></span> | <span data-ttu-id="5f33c-127">说明</span><span class="sxs-lookup"><span data-stu-id="5f33c-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5f33c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f33c-128">Authorization</span></span>  | <span data-ttu-id="5f33c-129">string</span><span class="sxs-lookup"><span data-stu-id="5f33c-129">string</span></span>  | <span data-ttu-id="5f33c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f33c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f33c-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f33c-132">Content-Type</span></span> | <span data-ttu-id="5f33c-133">string</span><span class="sxs-lookup"><span data-stu-id="5f33c-133">string</span></span>  | <span data-ttu-id="5f33c-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="5f33c-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f33c-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f33c-136">Request body</span></span>
<span data-ttu-id="5f33c-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5f33c-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5f33c-138">参数</span><span class="sxs-lookup"><span data-stu-id="5f33c-138">Parameter</span></span>    | <span data-ttu-id="5f33c-139">类型</span><span class="sxs-lookup"><span data-stu-id="5f33c-139">Type</span></span>   |<span data-ttu-id="5f33c-140">说明</span><span class="sxs-lookup"><span data-stu-id="5f33c-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f33c-141">注释</span><span class="sxs-lookup"><span data-stu-id="5f33c-141">comment</span></span>|<span data-ttu-id="5f33c-142">String</span><span class="sxs-lookup"><span data-stu-id="5f33c-142">String</span></span>|<span data-ttu-id="5f33c-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="5f33c-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="5f33c-145">message</span><span class="sxs-lookup"><span data-stu-id="5f33c-145">message</span></span>|[<span data-ttu-id="5f33c-146">message</span><span class="sxs-lookup"><span data-stu-id="5f33c-146">message</span></span>](../resources/message.md)|<span data-ttu-id="5f33c-147">在全部答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="5f33c-147">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="5f33c-148">响应</span><span class="sxs-lookup"><span data-stu-id="5f33c-148">Response</span></span>

<span data-ttu-id="5f33c-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5f33c-149">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f33c-150">示例</span><span class="sxs-lookup"><span data-stu-id="5f33c-150">Example</span></span>
<span data-ttu-id="5f33c-151">以下示例创建一个草稿以全部答复，并将附件和注释全部添加到一个 **createReplyAll** 调用中。</span><span class="sxs-lookup"><span data-stu-id="5f33c-151">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="5f33c-152">请求</span><span class="sxs-lookup"><span data-stu-id="5f33c-152">Request</span></span>
<span data-ttu-id="5f33c-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f33c-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5f33c-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f33c-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5f33c-155">C#</span><span class="sxs-lookup"><span data-stu-id="5f33c-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f33c-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f33c-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f33c-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f33c-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f33c-158">Java</span><span class="sxs-lookup"><span data-stu-id="5f33c-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5f33c-159">响应</span><span class="sxs-lookup"><span data-stu-id="5f33c-159">Response</span></span>
<span data-ttu-id="5f33c-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5f33c-160">Here is an example of the response.</span></span> <span data-ttu-id="5f33c-161">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5f33c-161">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


