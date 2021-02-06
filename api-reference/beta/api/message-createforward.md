---
title: 'message: createForward'
description: '创建草稿转发邮件以包含注释或更新任何邮件属性  '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e36487e3e25e4eac30c4c05987082b26b31601f3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136715"
---
# <a name="message-createforward"></a><span data-ttu-id="57fdb-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="57fdb-103">message: createForward</span></span>

<span data-ttu-id="57fdb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57fdb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57fdb-105">创建草稿转发邮件以包含注释或更新任何邮件属性</span><span class="sxs-lookup"><span data-stu-id="57fdb-105">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="57fdb-106">全部在一 **个 createForward 调用** 中。</span><span class="sxs-lookup"><span data-stu-id="57fdb-106">all in one **createForward** call.</span></span> <span data-ttu-id="57fdb-107">然后， [您可以发送](../api/message-send.md) 草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="57fdb-107">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="57fdb-108">**注意**</span><span class="sxs-lookup"><span data-stu-id="57fdb-108">**Note**</span></span>

- <span data-ttu-id="57fdb-109">可以指定参数的注释 **或 body** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="57fdb-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="57fdb-110">指定两者将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="57fdb-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="57fdb-111">必须指定参数 `toRecipients` 的参数或参数的 **toRecipients** `message` 属性。</span><span class="sxs-lookup"><span data-stu-id="57fdb-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="57fdb-112">如果同时指定两者或两者均不指定，将返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="57fdb-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="57fdb-113">权限</span><span class="sxs-lookup"><span data-stu-id="57fdb-113">Permissions</span></span>
<span data-ttu-id="57fdb-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57fdb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57fdb-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="57fdb-116">Permission type</span></span>      | <span data-ttu-id="57fdb-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57fdb-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57fdb-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57fdb-118">Delegated (work or school account)</span></span> | <span data-ttu-id="57fdb-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57fdb-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="57fdb-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57fdb-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57fdb-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57fdb-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="57fdb-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="57fdb-122">Application</span></span> | <span data-ttu-id="57fdb-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57fdb-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="57fdb-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57fdb-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="57fdb-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="57fdb-125">Request headers</span></span>
| <span data-ttu-id="57fdb-126">名称</span><span class="sxs-lookup"><span data-stu-id="57fdb-126">Name</span></span>       | <span data-ttu-id="57fdb-127">类型</span><span class="sxs-lookup"><span data-stu-id="57fdb-127">Type</span></span> | <span data-ttu-id="57fdb-128">说明</span><span class="sxs-lookup"><span data-stu-id="57fdb-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="57fdb-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="57fdb-129">Authorization</span></span>  | <span data-ttu-id="57fdb-130">string</span><span class="sxs-lookup"><span data-stu-id="57fdb-130">string</span></span>  | <span data-ttu-id="57fdb-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="57fdb-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57fdb-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57fdb-133">Content-Type</span></span> | <span data-ttu-id="57fdb-134">string</span><span class="sxs-lookup"><span data-stu-id="57fdb-134">string</span></span>  | <span data-ttu-id="57fdb-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="57fdb-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57fdb-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="57fdb-137">Request body</span></span>
<span data-ttu-id="57fdb-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="57fdb-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="57fdb-139">参数</span><span class="sxs-lookup"><span data-stu-id="57fdb-139">Parameter</span></span>    | <span data-ttu-id="57fdb-140">类型</span><span class="sxs-lookup"><span data-stu-id="57fdb-140">Type</span></span>   |<span data-ttu-id="57fdb-141">说明</span><span class="sxs-lookup"><span data-stu-id="57fdb-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57fdb-142">注释</span><span class="sxs-lookup"><span data-stu-id="57fdb-142">comment</span></span>|<span data-ttu-id="57fdb-143">String</span><span class="sxs-lookup"><span data-stu-id="57fdb-143">String</span></span>|<span data-ttu-id="57fdb-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="57fdb-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="57fdb-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="57fdb-146">toRecipients</span></span>|<span data-ttu-id="57fdb-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="57fdb-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="57fdb-148">收件人列表</span><span class="sxs-lookup"><span data-stu-id="57fdb-148">The list of recipients.</span></span>|
|<span data-ttu-id="57fdb-149">message</span><span class="sxs-lookup"><span data-stu-id="57fdb-149">message</span></span>|[<span data-ttu-id="57fdb-150">邮件</span><span class="sxs-lookup"><span data-stu-id="57fdb-150">message</span></span>](../resources/message.md)|<span data-ttu-id="57fdb-151">回复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="57fdb-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="57fdb-152">响应</span><span class="sxs-lookup"><span data-stu-id="57fdb-152">Response</span></span>

<span data-ttu-id="57fdb-153">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57fdb-153">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57fdb-154">示例</span><span class="sxs-lookup"><span data-stu-id="57fdb-154">Example</span></span>
<span data-ttu-id="57fdb-155">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="57fdb-155">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="57fdb-156">请求</span><span class="sxs-lookup"><span data-stu-id="57fdb-156">Request</span></span>
<span data-ttu-id="57fdb-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57fdb-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57fdb-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="57fdb-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="57fdb-159">C#</span><span class="sxs-lookup"><span data-stu-id="57fdb-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57fdb-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57fdb-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57fdb-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57fdb-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57fdb-162">Java</span><span class="sxs-lookup"><span data-stu-id="57fdb-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createforward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="57fdb-163">响应</span><span class="sxs-lookup"><span data-stu-id="57fdb-163">Response</span></span>
<span data-ttu-id="57fdb-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="57fdb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


