---
title: 消息：replyAll
description: '通过指定注释并修改任何可更新的属性来答复邮件的所有收件人 '
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2e0ad862a656b6b26d4de20bb4e0a31b45656a2d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981055"
---
# <a name="message-replyall"></a><span data-ttu-id="76405-103">消息：replyAll</span><span class="sxs-lookup"><span data-stu-id="76405-103">message: replyAll</span></span>

<span data-ttu-id="76405-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76405-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76405-105">通过使用 **replyAll** 方法指定注释并修改所有可更新的答复属性来答复邮件的所有收件人。</span><span class="sxs-lookup"><span data-stu-id="76405-105">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="76405-106">然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="76405-106">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="76405-107">或者，您可以先 [创建草稿的 "全部答复" 邮件](../api/message-createreplyall.md) ，以包含注释或更新任何邮件属性，然后 [发送](../api/message-send.md) 答复。</span><span class="sxs-lookup"><span data-stu-id="76405-107">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="76405-108">**注意**</span><span class="sxs-lookup"><span data-stu-id="76405-108">**Note**</span></span>

- <span data-ttu-id="76405-109">您可以指定参数的注释或 **body** 属性 `message` 。</span><span class="sxs-lookup"><span data-stu-id="76405-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="76405-110">同时指定这两个将返回 HTTP 400 错误的请求错误。</span><span class="sxs-lookup"><span data-stu-id="76405-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="76405-111">如果在原始邮件中指定了 **replyTo** 属性（按 Internet 邮件格式 ( [RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ，则应将答复发送给收件人</span><span class="sxs-lookup"><span data-stu-id="76405-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="76405-112">**replyTo** 和 **toRecipients** 属性，而不是 **from** 和 **toRecipients** 属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="76405-112">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="76405-113">权限</span><span class="sxs-lookup"><span data-stu-id="76405-113">Permissions</span></span>
<span data-ttu-id="76405-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76405-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76405-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="76405-116">Permission type</span></span>      | <span data-ttu-id="76405-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76405-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76405-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76405-118">Delegated (work or school account)</span></span> | <span data-ttu-id="76405-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="76405-119">Mail.Send</span></span>    |
|<span data-ttu-id="76405-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76405-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76405-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="76405-121">Mail.Send</span></span>    |
|<span data-ttu-id="76405-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="76405-122">Application</span></span> | <span data-ttu-id="76405-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="76405-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="76405-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76405-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="76405-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="76405-125">Request headers</span></span>
| <span data-ttu-id="76405-126">名称</span><span class="sxs-lookup"><span data-stu-id="76405-126">Name</span></span>       | <span data-ttu-id="76405-127">类型</span><span class="sxs-lookup"><span data-stu-id="76405-127">Type</span></span> | <span data-ttu-id="76405-128">说明</span><span class="sxs-lookup"><span data-stu-id="76405-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="76405-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="76405-129">Authorization</span></span>  | <span data-ttu-id="76405-130">string</span><span class="sxs-lookup"><span data-stu-id="76405-130">string</span></span>  | <span data-ttu-id="76405-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76405-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76405-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76405-133">Content-Type</span></span> | <span data-ttu-id="76405-134">string</span><span class="sxs-lookup"><span data-stu-id="76405-134">string</span></span>  | <span data-ttu-id="76405-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="76405-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76405-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="76405-137">Request body</span></span>
<span data-ttu-id="76405-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="76405-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="76405-139">参数</span><span class="sxs-lookup"><span data-stu-id="76405-139">Parameter</span></span>    | <span data-ttu-id="76405-140">类型</span><span class="sxs-lookup"><span data-stu-id="76405-140">Type</span></span>   |<span data-ttu-id="76405-141">说明</span><span class="sxs-lookup"><span data-stu-id="76405-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76405-142">注释</span><span class="sxs-lookup"><span data-stu-id="76405-142">comment</span></span>|<span data-ttu-id="76405-143">String</span><span class="sxs-lookup"><span data-stu-id="76405-143">String</span></span>|<span data-ttu-id="76405-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="76405-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="76405-146">message</span><span class="sxs-lookup"><span data-stu-id="76405-146">message</span></span>|[<span data-ttu-id="76405-147">message</span><span class="sxs-lookup"><span data-stu-id="76405-147">message</span></span>](../resources/message.md)|<span data-ttu-id="76405-148">答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="76405-148">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="76405-149">响应</span><span class="sxs-lookup"><span data-stu-id="76405-149">Response</span></span>

<span data-ttu-id="76405-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="76405-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76405-152">示例</span><span class="sxs-lookup"><span data-stu-id="76405-152">Example</span></span>
<span data-ttu-id="76405-153">以下示例包含注释并将附件添加到全部答复邮件中。</span><span class="sxs-lookup"><span data-stu-id="76405-153">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="76405-154">请求</span><span class="sxs-lookup"><span data-stu-id="76405-154">Request</span></span>
<span data-ttu-id="76405-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76405-155">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="76405-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="76405-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="76405-157">C#</span><span class="sxs-lookup"><span data-stu-id="76405-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76405-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76405-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76405-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76405-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="76405-160">Java</span><span class="sxs-lookup"><span data-stu-id="76405-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="76405-161">响应</span><span class="sxs-lookup"><span data-stu-id="76405-161">Response</span></span>
<span data-ttu-id="76405-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="76405-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


