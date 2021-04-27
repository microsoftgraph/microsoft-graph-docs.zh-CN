---
title: 'message: createForward'
description: '创建转发邮件草稿以包含注释或更新任何邮件属性  '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: dd0802fa9443067fe4db9edd53783b800d81ce8c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052171"
---
# <a name="message-createforward"></a><span data-ttu-id="ceeee-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="ceeee-103">message: createForward</span></span>

<span data-ttu-id="ceeee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceeee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceeee-105">创建转发邮件草稿以包含注释或更新任何邮件属性</span><span class="sxs-lookup"><span data-stu-id="ceeee-105">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="ceeee-106">全部在一 **个 createForward 调用** 中。</span><span class="sxs-lookup"><span data-stu-id="ceeee-106">all in one **createForward** call.</span></span> <span data-ttu-id="ceeee-107">然后， [您可以发送](../api/message-send.md) 草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="ceeee-107">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="ceeee-108">**注意**</span><span class="sxs-lookup"><span data-stu-id="ceeee-108">**Note**</span></span>

- <span data-ttu-id="ceeee-109">可以指定参数的 comment 或 **body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="ceeee-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="ceeee-110">指定这两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="ceeee-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="ceeee-111">必须指定 参数 `toRecipients` 或 **参数的 toRecipients** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="ceeee-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="ceeee-112">指定两者或同时指定两者都将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="ceeee-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="ceeee-113">权限</span><span class="sxs-lookup"><span data-stu-id="ceeee-113">Permissions</span></span>
<span data-ttu-id="ceeee-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ceeee-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceeee-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="ceeee-116">Permission type</span></span>      | <span data-ttu-id="ceeee-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ceeee-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ceeee-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ceeee-118">Delegated (work or school account)</span></span> | <span data-ttu-id="ceeee-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ceeee-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ceeee-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ceeee-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceeee-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ceeee-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ceeee-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="ceeee-122">Application</span></span> | <span data-ttu-id="ceeee-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ceeee-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ceeee-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ceeee-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="ceeee-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="ceeee-125">Request headers</span></span>
| <span data-ttu-id="ceeee-126">名称</span><span class="sxs-lookup"><span data-stu-id="ceeee-126">Name</span></span>       | <span data-ttu-id="ceeee-127">类型</span><span class="sxs-lookup"><span data-stu-id="ceeee-127">Type</span></span> | <span data-ttu-id="ceeee-128">说明</span><span class="sxs-lookup"><span data-stu-id="ceeee-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ceeee-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ceeee-129">Authorization</span></span>  | <span data-ttu-id="ceeee-130">string</span><span class="sxs-lookup"><span data-stu-id="ceeee-130">string</span></span>  | <span data-ttu-id="ceeee-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ceeee-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ceeee-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ceeee-133">Content-Type</span></span> | <span data-ttu-id="ceeee-134">string</span><span class="sxs-lookup"><span data-stu-id="ceeee-134">string</span></span>  | <span data-ttu-id="ceeee-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="ceeee-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ceeee-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="ceeee-137">Request body</span></span>
<span data-ttu-id="ceeee-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ceeee-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ceeee-139">参数</span><span class="sxs-lookup"><span data-stu-id="ceeee-139">Parameter</span></span>    | <span data-ttu-id="ceeee-140">类型</span><span class="sxs-lookup"><span data-stu-id="ceeee-140">Type</span></span>   |<span data-ttu-id="ceeee-141">说明</span><span class="sxs-lookup"><span data-stu-id="ceeee-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ceeee-142">注释</span><span class="sxs-lookup"><span data-stu-id="ceeee-142">comment</span></span>|<span data-ttu-id="ceeee-143">String</span><span class="sxs-lookup"><span data-stu-id="ceeee-143">String</span></span>|<span data-ttu-id="ceeee-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="ceeee-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ceeee-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="ceeee-146">toRecipients</span></span>|<span data-ttu-id="ceeee-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="ceeee-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="ceeee-148">收件人列表</span><span class="sxs-lookup"><span data-stu-id="ceeee-148">The list of recipients.</span></span>|
|<span data-ttu-id="ceeee-149">message</span><span class="sxs-lookup"><span data-stu-id="ceeee-149">message</span></span>|[<span data-ttu-id="ceeee-150">message</span><span class="sxs-lookup"><span data-stu-id="ceeee-150">message</span></span>](../resources/message.md)|<span data-ttu-id="ceeee-151">回复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="ceeee-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="ceeee-152">响应</span><span class="sxs-lookup"><span data-stu-id="ceeee-152">Response</span></span>

<span data-ttu-id="ceeee-153">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ceeee-153">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceeee-154">示例</span><span class="sxs-lookup"><span data-stu-id="ceeee-154">Example</span></span>
<span data-ttu-id="ceeee-155">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ceeee-155">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ceeee-156">请求</span><span class="sxs-lookup"><span data-stu-id="ceeee-156">Request</span></span>
<span data-ttu-id="ceeee-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ceeee-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ceeee-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="ceeee-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ceeee-159">C#</span><span class="sxs-lookup"><span data-stu-id="ceeee-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ceeee-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ceeee-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ceeee-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ceeee-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ceeee-162">Java</span><span class="sxs-lookup"><span data-stu-id="ceeee-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createforward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ceeee-163">响应</span><span class="sxs-lookup"><span data-stu-id="ceeee-163">Response</span></span>
<span data-ttu-id="ceeee-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ceeee-164">Here is an example of the response.</span></span> <span data-ttu-id="ceeee-165">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ceeee-165">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


