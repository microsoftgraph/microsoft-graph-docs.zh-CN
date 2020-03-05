---
title: 邮件：转发
description: '转发邮件、添加注释或修改任何可更新的属性  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f30b10cefc0ca4ff8f4f59c2b25cb5e91637e453
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456906"
---
# <a name="message-forward"></a><span data-ttu-id="ac78c-103">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="ac78c-103">message: forward</span></span>

<span data-ttu-id="ac78c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ac78c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac78c-105">转发邮件、添加注释或修改任何可更新的属性</span><span class="sxs-lookup"><span data-stu-id="ac78c-105">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="ac78c-106">一个**正向**调用中的全部。</span><span class="sxs-lookup"><span data-stu-id="ac78c-106">all in one **forward** call.</span></span> <span data-ttu-id="ac78c-107">邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="ac78c-107">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="ac78c-108">或者，您可以先[创建一个草稿转发邮件](../api/message-createforward.md)，以包含注释或更新任何邮件属性，然后[发送](../api/message-send.md)草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="ac78c-108">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="ac78c-109">**注意**</span><span class="sxs-lookup"><span data-stu-id="ac78c-109">**Note**</span></span>

- <span data-ttu-id="ac78c-110">您可以指定`message`参数的注释或**body**属性。</span><span class="sxs-lookup"><span data-stu-id="ac78c-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="ac78c-111">同时指定这两个将返回 HTTP 400 错误的请求错误。</span><span class="sxs-lookup"><span data-stu-id="ac78c-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="ac78c-112">您必须指定`toRecipients`参数或`message`参数的**toRecipients**属性。</span><span class="sxs-lookup"><span data-stu-id="ac78c-112">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="ac78c-113">同时指定或指定两者均不会返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="ac78c-113">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac78c-114">权限</span><span class="sxs-lookup"><span data-stu-id="ac78c-114">Permissions</span></span>
<span data-ttu-id="ac78c-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac78c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac78c-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac78c-117">Permission type</span></span>      | <span data-ttu-id="ac78c-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac78c-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac78c-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac78c-119">Delegated (work or school account)</span></span> | <span data-ttu-id="ac78c-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ac78c-120">Mail.Send</span></span>    |
|<span data-ttu-id="ac78c-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac78c-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac78c-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ac78c-122">Mail.Send</span></span>    |
|<span data-ttu-id="ac78c-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac78c-123">Application</span></span> | <span data-ttu-id="ac78c-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ac78c-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac78c-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac78c-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="ac78c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac78c-126">Request headers</span></span>
| <span data-ttu-id="ac78c-127">名称</span><span class="sxs-lookup"><span data-stu-id="ac78c-127">Name</span></span>       | <span data-ttu-id="ac78c-128">类型</span><span class="sxs-lookup"><span data-stu-id="ac78c-128">Type</span></span> | <span data-ttu-id="ac78c-129">说明</span><span class="sxs-lookup"><span data-stu-id="ac78c-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ac78c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac78c-130">Authorization</span></span>  | <span data-ttu-id="ac78c-131">string</span><span class="sxs-lookup"><span data-stu-id="ac78c-131">string</span></span>  | <span data-ttu-id="ac78c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac78c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac78c-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac78c-134">Content-Type</span></span> | <span data-ttu-id="ac78c-135">string</span><span class="sxs-lookup"><span data-stu-id="ac78c-135">string</span></span>  | <span data-ttu-id="ac78c-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="ac78c-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac78c-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac78c-138">Request body</span></span>
<span data-ttu-id="ac78c-139">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ac78c-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ac78c-140">参数</span><span class="sxs-lookup"><span data-stu-id="ac78c-140">Parameter</span></span>    | <span data-ttu-id="ac78c-141">类型</span><span class="sxs-lookup"><span data-stu-id="ac78c-141">Type</span></span>   |<span data-ttu-id="ac78c-142">说明</span><span class="sxs-lookup"><span data-stu-id="ac78c-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac78c-143">注释</span><span class="sxs-lookup"><span data-stu-id="ac78c-143">comment</span></span>|<span data-ttu-id="ac78c-144">String</span><span class="sxs-lookup"><span data-stu-id="ac78c-144">String</span></span>|<span data-ttu-id="ac78c-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="ac78c-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ac78c-147">toRecipients</span><span class="sxs-lookup"><span data-stu-id="ac78c-147">toRecipients</span></span>|<span data-ttu-id="ac78c-148">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="ac78c-148">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="ac78c-149">收件人列表</span><span class="sxs-lookup"><span data-stu-id="ac78c-149">The list of recipients.</span></span>|
|<span data-ttu-id="ac78c-150">message</span><span class="sxs-lookup"><span data-stu-id="ac78c-150">message</span></span>|[<span data-ttu-id="ac78c-151">邮件</span><span class="sxs-lookup"><span data-stu-id="ac78c-151">message</span></span>](../resources/message.md)|<span data-ttu-id="ac78c-152">答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="ac78c-152">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="ac78c-153">响应</span><span class="sxs-lookup"><span data-stu-id="ac78c-153">Response</span></span>

<span data-ttu-id="ac78c-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ac78c-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac78c-156">示例</span><span class="sxs-lookup"><span data-stu-id="ac78c-156">Example</span></span>
<span data-ttu-id="ac78c-157">下面的示例将**isDeliveryReceiptRequested**属性设置为 true，添加注释并转发邮件。</span><span class="sxs-lookup"><span data-stu-id="ac78c-157">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="ac78c-158">请求</span><span class="sxs-lookup"><span data-stu-id="ac78c-158">Request</span></span>
<span data-ttu-id="ac78c-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac78c-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac78c-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac78c-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
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
  "comment": "Dana, just want to make sure you get this." 
}
```
# <a name="c"></a>[<span data-ttu-id="ac78c-161">C#</span><span class="sxs-lookup"><span data-stu-id="ac78c-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac78c-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac78c-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac78c-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac78c-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ac78c-164">响应</span><span class="sxs-lookup"><span data-stu-id="ac78c-164">Response</span></span>
<span data-ttu-id="ac78c-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ac78c-165">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
