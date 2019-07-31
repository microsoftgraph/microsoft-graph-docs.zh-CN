---
title: 'message: createReplyAll'
description: '创建 "全部答复" 邮件的草稿, 以包含注释或更新任何邮件属性。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 38c61608f080e336b239685476bf3b3d354643c8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983918"
---
# <a name="message-createreplyall"></a><span data-ttu-id="46985-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="46985-103">message: createReplyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46985-p101">创建回复全部邮件草稿以全部在一个 createReplyAll 调用中添加注释或更新任意邮件属性。然后，你可以更新或发送草稿。</span><span class="sxs-lookup"><span data-stu-id="46985-p101">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="46985-106">**注意**</span><span class="sxs-lookup"><span data-stu-id="46985-106">**Note**</span></span>

- <span data-ttu-id="46985-107">您可以指定`message`参数的注释或**body**属性。</span><span class="sxs-lookup"><span data-stu-id="46985-107">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="46985-108">同时指定这两个将返回 HTTP 400 错误的请求错误。</span><span class="sxs-lookup"><span data-stu-id="46985-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="46985-109">如果在原始邮件中指定了**replyTo**属性 (根据 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822))), 则应将答复发送给收件人</span><span class="sxs-lookup"><span data-stu-id="46985-109">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="46985-110">**replyTo**和**toRecipients**属性, 而不是**from**和**toRecipients**属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="46985-110">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="46985-111">权限</span><span class="sxs-lookup"><span data-stu-id="46985-111">Permissions</span></span>
<span data-ttu-id="46985-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46985-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46985-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="46985-114">Permission type</span></span>      | <span data-ttu-id="46985-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46985-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46985-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46985-116">Delegated (work or school account)</span></span> | <span data-ttu-id="46985-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46985-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="46985-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46985-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46985-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46985-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="46985-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="46985-120">Application</span></span> | <span data-ttu-id="46985-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46985-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="46985-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46985-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="46985-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="46985-123">Request headers</span></span>
| <span data-ttu-id="46985-124">名称</span><span class="sxs-lookup"><span data-stu-id="46985-124">Name</span></span>       | <span data-ttu-id="46985-125">类型</span><span class="sxs-lookup"><span data-stu-id="46985-125">Type</span></span> | <span data-ttu-id="46985-126">说明</span><span class="sxs-lookup"><span data-stu-id="46985-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46985-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="46985-127">Authorization</span></span>  | <span data-ttu-id="46985-128">string</span><span class="sxs-lookup"><span data-stu-id="46985-128">string</span></span>  | <span data-ttu-id="46985-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46985-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46985-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46985-131">Content-Type</span></span> | <span data-ttu-id="46985-132">string</span><span class="sxs-lookup"><span data-stu-id="46985-132">string</span></span>  | <span data-ttu-id="46985-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="46985-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46985-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="46985-135">Request body</span></span>
<span data-ttu-id="46985-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="46985-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="46985-137">参数</span><span class="sxs-lookup"><span data-stu-id="46985-137">Parameter</span></span>    | <span data-ttu-id="46985-138">类型</span><span class="sxs-lookup"><span data-stu-id="46985-138">Type</span></span>   |<span data-ttu-id="46985-139">说明</span><span class="sxs-lookup"><span data-stu-id="46985-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46985-140">注释</span><span class="sxs-lookup"><span data-stu-id="46985-140">comment</span></span>|<span data-ttu-id="46985-141">String</span><span class="sxs-lookup"><span data-stu-id="46985-141">String</span></span>|<span data-ttu-id="46985-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="46985-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="46985-144">message</span><span class="sxs-lookup"><span data-stu-id="46985-144">message</span></span>|[<span data-ttu-id="46985-145">邮件</span><span class="sxs-lookup"><span data-stu-id="46985-145">message</span></span>](../resources/message.md)|<span data-ttu-id="46985-146">全部在答复邮件中更新的可写属性。</span><span class="sxs-lookup"><span data-stu-id="46985-146">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="46985-147">响应</span><span class="sxs-lookup"><span data-stu-id="46985-147">Response</span></span>

<span data-ttu-id="46985-148">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46985-148">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46985-149">示例</span><span class="sxs-lookup"><span data-stu-id="46985-149">Example</span></span>
<span data-ttu-id="46985-150">下面的示例创建一个草稿以全部答复, 并在一个**createReplyAll**调用中添加附件和批注。</span><span class="sxs-lookup"><span data-stu-id="46985-150">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="46985-151">请求</span><span class="sxs-lookup"><span data-stu-id="46985-151">Request</span></span>
<span data-ttu-id="46985-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46985-152">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46985-153">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="46985-153">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="46985-154">C#</span><span class="sxs-lookup"><span data-stu-id="46985-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46985-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="46985-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46985-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="46985-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="46985-157">Java</span><span class="sxs-lookup"><span data-stu-id="46985-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="46985-158">响应</span><span class="sxs-lookup"><span data-stu-id="46985-158">Response</span></span>
<span data-ttu-id="46985-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46985-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
