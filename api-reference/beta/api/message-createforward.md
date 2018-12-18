---
title: 'message: createForward'
description: '创建正向邮件草稿包含评论或更新任何消息属性  '
author: angelgolfer-ms
ms.openlocfilehash: 6630bf8486f3fdbc53106ef334aeb23aa36f93dd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329776"
---
# <a name="message-createforward"></a><span data-ttu-id="aff5b-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="aff5b-103">message: createForward</span></span>

> <span data-ttu-id="aff5b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aff5b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aff5b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aff5b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aff5b-106">创建正向邮件草稿包含评论或更新任何消息属性</span><span class="sxs-lookup"><span data-stu-id="aff5b-106">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="aff5b-107">一个**createForward**中的所有呼叫。</span><span class="sxs-lookup"><span data-stu-id="aff5b-107">all in one **createForward** call.</span></span> <span data-ttu-id="aff5b-108">您然后可以[发送](../api/message-send.md)的邮件草稿。</span><span class="sxs-lookup"><span data-stu-id="aff5b-108">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="aff5b-109">**注意**</span><span class="sxs-lookup"><span data-stu-id="aff5b-109">**Note**</span></span>

- <span data-ttu-id="aff5b-110">您可以指定注释或的**body**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="aff5b-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="aff5b-111">如果同时指定将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="aff5b-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="aff5b-112">必须指定`toRecipients`参数或**toRecipients**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="aff5b-112">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="aff5b-113">指定这两个或指定都不将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="aff5b-113">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="aff5b-114">权限</span><span class="sxs-lookup"><span data-stu-id="aff5b-114">Permissions</span></span>
<span data-ttu-id="aff5b-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aff5b-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aff5b-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="aff5b-117">Permission type</span></span>      | <span data-ttu-id="aff5b-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aff5b-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aff5b-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aff5b-119">Delegated (work or school account)</span></span> | <span data-ttu-id="aff5b-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aff5b-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aff5b-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aff5b-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aff5b-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aff5b-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aff5b-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="aff5b-123">Application</span></span> | <span data-ttu-id="aff5b-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aff5b-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aff5b-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aff5b-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="aff5b-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="aff5b-126">Request headers</span></span>
| <span data-ttu-id="aff5b-127">Name</span><span class="sxs-lookup"><span data-stu-id="aff5b-127">Name</span></span>       | <span data-ttu-id="aff5b-128">类型</span><span class="sxs-lookup"><span data-stu-id="aff5b-128">Type</span></span> | <span data-ttu-id="aff5b-129">说明</span><span class="sxs-lookup"><span data-stu-id="aff5b-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aff5b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="aff5b-130">Authorization</span></span>  | <span data-ttu-id="aff5b-131">string</span><span class="sxs-lookup"><span data-stu-id="aff5b-131">string</span></span>  | <span data-ttu-id="aff5b-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aff5b-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aff5b-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aff5b-134">Content-Type</span></span> | <span data-ttu-id="aff5b-135">string</span><span class="sxs-lookup"><span data-stu-id="aff5b-135">string</span></span>  | <span data-ttu-id="aff5b-p107">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="aff5b-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aff5b-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="aff5b-138">Request body</span></span>
<span data-ttu-id="aff5b-139">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="aff5b-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aff5b-140">参数</span><span class="sxs-lookup"><span data-stu-id="aff5b-140">Parameter</span></span>    | <span data-ttu-id="aff5b-141">Type</span><span class="sxs-lookup"><span data-stu-id="aff5b-141">Type</span></span>   |<span data-ttu-id="aff5b-142">说明</span><span class="sxs-lookup"><span data-stu-id="aff5b-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aff5b-143">注释</span><span class="sxs-lookup"><span data-stu-id="aff5b-143">comment</span></span>|<span data-ttu-id="aff5b-144">String</span><span class="sxs-lookup"><span data-stu-id="aff5b-144">String</span></span>|<span data-ttu-id="aff5b-p108">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="aff5b-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="aff5b-147">toRecipients</span><span class="sxs-lookup"><span data-stu-id="aff5b-147">toRecipients</span></span>|<span data-ttu-id="aff5b-148">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="aff5b-148">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="aff5b-149">收件人列表</span><span class="sxs-lookup"><span data-stu-id="aff5b-149">The list of recipients.</span></span>|
|<span data-ttu-id="aff5b-150">message</span><span class="sxs-lookup"><span data-stu-id="aff5b-150">message</span></span>|[<span data-ttu-id="aff5b-151">message</span><span class="sxs-lookup"><span data-stu-id="aff5b-151">message</span></span>](../resources/message.md)|<span data-ttu-id="aff5b-152">若要在答复邮件更新任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="aff5b-152">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="aff5b-153">响应</span><span class="sxs-lookup"><span data-stu-id="aff5b-153">Response</span></span>

<span data-ttu-id="aff5b-154">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aff5b-154">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aff5b-155">示例</span><span class="sxs-lookup"><span data-stu-id="aff5b-155">Example</span></span>
<span data-ttu-id="aff5b-156">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="aff5b-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aff5b-157">请求</span><span class="sxs-lookup"><span data-stu-id="aff5b-157">Request</span></span>
<span data-ttu-id="aff5b-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aff5b-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this; you'll need this if the project gets approved." 
}
```

##### <a name="response"></a><span data-ttu-id="aff5b-159">响应</span><span class="sxs-lookup"><span data-stu-id="aff5b-159">Response</span></span>
<span data-ttu-id="aff5b-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aff5b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKqAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DQ\"",
  "id": "AAMkADA1MTAAAH5JKqAAA=",
  "subject": "FW: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>\r\nDana, just want to make sure you get this; you'll need this if the project gets approved.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:47:54 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group</body>\r\n</html>\r\n"
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
        "name": "Dana Swope",
        "address": "danas@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->