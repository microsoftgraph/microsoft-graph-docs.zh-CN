---
title: 'message: createForward'
description: '创建草稿转发邮件以包含注释或更新任何邮件属性  '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: aeb456327d6a1828dd389787d080539ab06f6636
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266561"
---
# <a name="message-createforward"></a><span data-ttu-id="c64d5-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="c64d5-103">message: createForward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c64d5-104">创建草稿转发邮件以包含注释或更新任何邮件属性</span><span class="sxs-lookup"><span data-stu-id="c64d5-104">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="c64d5-105">全部在一个**createForward**调用中。</span><span class="sxs-lookup"><span data-stu-id="c64d5-105">all in one **createForward** call.</span></span> <span data-ttu-id="c64d5-106">然后, 您可以[发送](../api/message-send.md)草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="c64d5-106">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="c64d5-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="c64d5-107">**Note**</span></span>

- <span data-ttu-id="c64d5-108">您可以指定`message`参数的注释或**body**属性。</span><span class="sxs-lookup"><span data-stu-id="c64d5-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="c64d5-109">同时指定这两个将返回 HTTP 400 错误的请求错误。</span><span class="sxs-lookup"><span data-stu-id="c64d5-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="c64d5-110">您必须指定`toRecipients`参数或`message`参数的**toRecipients**属性。</span><span class="sxs-lookup"><span data-stu-id="c64d5-110">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="c64d5-111">同时指定或指定两者均不会返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="c64d5-111">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="c64d5-112">权限</span><span class="sxs-lookup"><span data-stu-id="c64d5-112">Permissions</span></span>
<span data-ttu-id="c64d5-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c64d5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c64d5-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="c64d5-115">Permission type</span></span>      | <span data-ttu-id="c64d5-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c64d5-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c64d5-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c64d5-117">Delegated (work or school account)</span></span> | <span data-ttu-id="c64d5-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c64d5-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c64d5-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c64d5-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c64d5-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c64d5-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c64d5-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="c64d5-121">Application</span></span> | <span data-ttu-id="c64d5-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c64d5-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c64d5-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c64d5-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="c64d5-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="c64d5-124">Request headers</span></span>
| <span data-ttu-id="c64d5-125">名称</span><span class="sxs-lookup"><span data-stu-id="c64d5-125">Name</span></span>       | <span data-ttu-id="c64d5-126">类型</span><span class="sxs-lookup"><span data-stu-id="c64d5-126">Type</span></span> | <span data-ttu-id="c64d5-127">说明</span><span class="sxs-lookup"><span data-stu-id="c64d5-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c64d5-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c64d5-128">Authorization</span></span>  | <span data-ttu-id="c64d5-129">string</span><span class="sxs-lookup"><span data-stu-id="c64d5-129">string</span></span>  | <span data-ttu-id="c64d5-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c64d5-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c64d5-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c64d5-132">Content-Type</span></span> | <span data-ttu-id="c64d5-133">string</span><span class="sxs-lookup"><span data-stu-id="c64d5-133">string</span></span>  | <span data-ttu-id="c64d5-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="c64d5-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c64d5-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="c64d5-136">Request body</span></span>
<span data-ttu-id="c64d5-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c64d5-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c64d5-138">参数</span><span class="sxs-lookup"><span data-stu-id="c64d5-138">Parameter</span></span>    | <span data-ttu-id="c64d5-139">类型</span><span class="sxs-lookup"><span data-stu-id="c64d5-139">Type</span></span>   |<span data-ttu-id="c64d5-140">说明</span><span class="sxs-lookup"><span data-stu-id="c64d5-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c64d5-141">注释</span><span class="sxs-lookup"><span data-stu-id="c64d5-141">comment</span></span>|<span data-ttu-id="c64d5-142">String</span><span class="sxs-lookup"><span data-stu-id="c64d5-142">String</span></span>|<span data-ttu-id="c64d5-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="c64d5-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="c64d5-145">toRecipients</span><span class="sxs-lookup"><span data-stu-id="c64d5-145">toRecipients</span></span>|<span data-ttu-id="c64d5-146">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="c64d5-146">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="c64d5-147">收件人列表</span><span class="sxs-lookup"><span data-stu-id="c64d5-147">The list of recipients.</span></span>|
|<span data-ttu-id="c64d5-148">message</span><span class="sxs-lookup"><span data-stu-id="c64d5-148">message</span></span>|[<span data-ttu-id="c64d5-149">邮件</span><span class="sxs-lookup"><span data-stu-id="c64d5-149">message</span></span>](../resources/message.md)|<span data-ttu-id="c64d5-150">答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="c64d5-150">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="c64d5-151">响应</span><span class="sxs-lookup"><span data-stu-id="c64d5-151">Response</span></span>

<span data-ttu-id="c64d5-152">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c64d5-152">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c64d5-153">示例</span><span class="sxs-lookup"><span data-stu-id="c64d5-153">Example</span></span>
<span data-ttu-id="c64d5-154">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c64d5-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c64d5-155">请求</span><span class="sxs-lookup"><span data-stu-id="c64d5-155">Request</span></span>
<span data-ttu-id="c64d5-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c64d5-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c64d5-157">响应</span><span class="sxs-lookup"><span data-stu-id="c64d5-157">Response</span></span>
<span data-ttu-id="c64d5-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c64d5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c64d5-161">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c64d5-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c64d5-162">C#</span><span class="sxs-lookup"><span data-stu-id="c64d5-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_createforward-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c64d5-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="c64d5-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_createforward-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c64d5-164">目标-C</span><span class="sxs-lookup"><span data-stu-id="c64d5-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_createforward-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-createforward.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-createforward.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-createforward.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
