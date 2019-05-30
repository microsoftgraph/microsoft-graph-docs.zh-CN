---
title: 消息：replyAll
description: '通过指定注释并修改任何可更新的属性来答复邮件的所有收件人 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5215af70332977d1c7aef70ad9418287f7c0b46f
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536986"
---
# <a name="message-replyall"></a><span data-ttu-id="fc568-103">消息：replyAll</span><span class="sxs-lookup"><span data-stu-id="fc568-103">message: replyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc568-104">通过使用**replyAll**方法指定注释并修改所有可更新的答复属性来答复邮件的所有收件人。</span><span class="sxs-lookup"><span data-stu-id="fc568-104">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="fc568-105">然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="fc568-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="fc568-106">或者, 您可以先[创建草稿的 "全部答复" 邮件](../api/message-createreplyall.md), 以包含注释或更新任何邮件属性, 然后[发送](../api/message-send.md)答复。</span><span class="sxs-lookup"><span data-stu-id="fc568-106">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="fc568-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="fc568-107">**Note**</span></span>

- <span data-ttu-id="fc568-108">您可以指定`message`参数的注释或**body**属性。</span><span class="sxs-lookup"><span data-stu-id="fc568-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="fc568-109">同时指定这两个将返回 HTTP 400 错误的请求错误。</span><span class="sxs-lookup"><span data-stu-id="fc568-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="fc568-110">如果在原始邮件中指定了**replyTo**属性 (根据 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822))), 则应将答复发送给收件人</span><span class="sxs-lookup"><span data-stu-id="fc568-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="fc568-111">**replyTo**和**toRecipients**属性, 而不是**from**和**toRecipients**属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="fc568-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="fc568-112">权限</span><span class="sxs-lookup"><span data-stu-id="fc568-112">Permissions</span></span>
<span data-ttu-id="fc568-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc568-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc568-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc568-115">Permission type</span></span>      | <span data-ttu-id="fc568-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc568-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc568-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc568-117">Delegated (work or school account)</span></span> | <span data-ttu-id="fc568-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fc568-118">Mail.Send</span></span>    |
|<span data-ttu-id="fc568-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc568-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc568-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fc568-120">Mail.Send</span></span>    |
|<span data-ttu-id="fc568-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc568-121">Application</span></span> | <span data-ttu-id="fc568-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fc568-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc568-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc568-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="fc568-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc568-124">Request headers</span></span>
| <span data-ttu-id="fc568-125">名称</span><span class="sxs-lookup"><span data-stu-id="fc568-125">Name</span></span>       | <span data-ttu-id="fc568-126">类型</span><span class="sxs-lookup"><span data-stu-id="fc568-126">Type</span></span> | <span data-ttu-id="fc568-127">说明</span><span class="sxs-lookup"><span data-stu-id="fc568-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc568-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc568-128">Authorization</span></span>  | <span data-ttu-id="fc568-129">string</span><span class="sxs-lookup"><span data-stu-id="fc568-129">string</span></span>  | <span data-ttu-id="fc568-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc568-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc568-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc568-132">Content-Type</span></span> | <span data-ttu-id="fc568-133">string</span><span class="sxs-lookup"><span data-stu-id="fc568-133">string</span></span>  | <span data-ttu-id="fc568-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="fc568-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc568-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc568-136">Request body</span></span>
<span data-ttu-id="fc568-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fc568-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc568-138">参数</span><span class="sxs-lookup"><span data-stu-id="fc568-138">Parameter</span></span>    | <span data-ttu-id="fc568-139">类型</span><span class="sxs-lookup"><span data-stu-id="fc568-139">Type</span></span>   |<span data-ttu-id="fc568-140">说明</span><span class="sxs-lookup"><span data-stu-id="fc568-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc568-141">注释</span><span class="sxs-lookup"><span data-stu-id="fc568-141">comment</span></span>|<span data-ttu-id="fc568-142">String</span><span class="sxs-lookup"><span data-stu-id="fc568-142">String</span></span>|<span data-ttu-id="fc568-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="fc568-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="fc568-145">message</span><span class="sxs-lookup"><span data-stu-id="fc568-145">message</span></span>|[<span data-ttu-id="fc568-146">message</span><span class="sxs-lookup"><span data-stu-id="fc568-146">message</span></span>](../resources/message.md)|<span data-ttu-id="fc568-147">答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="fc568-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="fc568-148">响应</span><span class="sxs-lookup"><span data-stu-id="fc568-148">Response</span></span>

<span data-ttu-id="fc568-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fc568-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc568-151">示例</span><span class="sxs-lookup"><span data-stu-id="fc568-151">Example</span></span>
<span data-ttu-id="fc568-152">以下示例包含注释并将附件添加到全部答复邮件中。</span><span class="sxs-lookup"><span data-stu-id="fc568-152">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="fc568-153">请求</span><span class="sxs-lookup"><span data-stu-id="fc568-153">Request</span></span>
<span data-ttu-id="fc568-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc568-154">Here is an example of the request.</span></span>
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


##### <a name="response"></a><span data-ttu-id="fc568-155">响应</span><span class="sxs-lookup"><span data-stu-id="fc568-155">Response</span></span>
<span data-ttu-id="fc568-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fc568-156">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fc568-157">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="fc568-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fc568-158">C#</span><span class="sxs-lookup"><span data-stu-id="fc568-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_replyall-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc568-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc568-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_replyall-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/message-replyall.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-replyall.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
