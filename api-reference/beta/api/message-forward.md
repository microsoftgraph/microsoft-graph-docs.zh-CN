---
title: 邮件：转发
description: '转发邮件、添加注释或修改任何可更新的属性  '
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5302533908c99244602704d3e1c6314b7d1d0967
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978568"
---
# <a name="message-forward"></a><span data-ttu-id="43fa7-103">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="43fa7-103">message: forward</span></span>

<span data-ttu-id="43fa7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43fa7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43fa7-105">转发邮件、添加注释或修改任何可更新的属性</span><span class="sxs-lookup"><span data-stu-id="43fa7-105">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="43fa7-106">一个 **正向** 调用中的全部。</span><span class="sxs-lookup"><span data-stu-id="43fa7-106">all in one **forward** call.</span></span> <span data-ttu-id="43fa7-107">邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="43fa7-107">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="43fa7-108">或者，您可以先 [创建一个草稿转发邮件](../api/message-createforward.md) ，以包含注释或更新任何邮件属性，然后 [发送](../api/message-send.md) 草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="43fa7-108">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="43fa7-109">**注意**</span><span class="sxs-lookup"><span data-stu-id="43fa7-109">**Note**</span></span>

- <span data-ttu-id="43fa7-110">您可以指定参数的注释或 **body** 属性 `message` 。</span><span class="sxs-lookup"><span data-stu-id="43fa7-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="43fa7-111">同时指定这两个将返回 HTTP 400 错误的请求错误。</span><span class="sxs-lookup"><span data-stu-id="43fa7-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="43fa7-112">您必须指定参数 `toRecipients` 或参数的 **toRecipients** 属性 `message` 。</span><span class="sxs-lookup"><span data-stu-id="43fa7-112">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="43fa7-113">同时指定或指定两者均不会返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="43fa7-113">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="43fa7-114">权限</span><span class="sxs-lookup"><span data-stu-id="43fa7-114">Permissions</span></span>
<span data-ttu-id="43fa7-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43fa7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43fa7-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="43fa7-117">Permission type</span></span>      | <span data-ttu-id="43fa7-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43fa7-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43fa7-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43fa7-119">Delegated (work or school account)</span></span> | <span data-ttu-id="43fa7-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="43fa7-120">Mail.Send</span></span>    |
|<span data-ttu-id="43fa7-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43fa7-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43fa7-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="43fa7-122">Mail.Send</span></span>    |
|<span data-ttu-id="43fa7-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="43fa7-123">Application</span></span> | <span data-ttu-id="43fa7-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="43fa7-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="43fa7-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43fa7-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="43fa7-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="43fa7-126">Request headers</span></span>
| <span data-ttu-id="43fa7-127">名称</span><span class="sxs-lookup"><span data-stu-id="43fa7-127">Name</span></span>       | <span data-ttu-id="43fa7-128">类型</span><span class="sxs-lookup"><span data-stu-id="43fa7-128">Type</span></span> | <span data-ttu-id="43fa7-129">说明</span><span class="sxs-lookup"><span data-stu-id="43fa7-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="43fa7-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="43fa7-130">Authorization</span></span>  | <span data-ttu-id="43fa7-131">string</span><span class="sxs-lookup"><span data-stu-id="43fa7-131">string</span></span>  | <span data-ttu-id="43fa7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="43fa7-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="43fa7-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43fa7-134">Content-Type</span></span> | <span data-ttu-id="43fa7-135">string</span><span class="sxs-lookup"><span data-stu-id="43fa7-135">string</span></span>  | <span data-ttu-id="43fa7-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="43fa7-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43fa7-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="43fa7-138">Request body</span></span>
<span data-ttu-id="43fa7-139">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="43fa7-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="43fa7-140">参数</span><span class="sxs-lookup"><span data-stu-id="43fa7-140">Parameter</span></span>    | <span data-ttu-id="43fa7-141">类型</span><span class="sxs-lookup"><span data-stu-id="43fa7-141">Type</span></span>   |<span data-ttu-id="43fa7-142">说明</span><span class="sxs-lookup"><span data-stu-id="43fa7-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43fa7-143">注释</span><span class="sxs-lookup"><span data-stu-id="43fa7-143">comment</span></span>|<span data-ttu-id="43fa7-144">String</span><span class="sxs-lookup"><span data-stu-id="43fa7-144">String</span></span>|<span data-ttu-id="43fa7-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="43fa7-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="43fa7-147">toRecipients</span><span class="sxs-lookup"><span data-stu-id="43fa7-147">toRecipients</span></span>|<span data-ttu-id="43fa7-148">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="43fa7-148">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="43fa7-149">收件人列表</span><span class="sxs-lookup"><span data-stu-id="43fa7-149">The list of recipients.</span></span>|
|<span data-ttu-id="43fa7-150">message</span><span class="sxs-lookup"><span data-stu-id="43fa7-150">message</span></span>|[<span data-ttu-id="43fa7-151">message</span><span class="sxs-lookup"><span data-stu-id="43fa7-151">message</span></span>](../resources/message.md)|<span data-ttu-id="43fa7-152">答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="43fa7-152">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="43fa7-153">响应</span><span class="sxs-lookup"><span data-stu-id="43fa7-153">Response</span></span>

<span data-ttu-id="43fa7-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="43fa7-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43fa7-156">示例</span><span class="sxs-lookup"><span data-stu-id="43fa7-156">Example</span></span>
<span data-ttu-id="43fa7-157">下面的示例将 **isDeliveryReceiptRequested** 属性设置为 true，添加注释并转发邮件。</span><span class="sxs-lookup"><span data-stu-id="43fa7-157">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="43fa7-158">请求</span><span class="sxs-lookup"><span data-stu-id="43fa7-158">Request</span></span>
<span data-ttu-id="43fa7-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43fa7-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="43fa7-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="43fa7-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="43fa7-161">C#</span><span class="sxs-lookup"><span data-stu-id="43fa7-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43fa7-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43fa7-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43fa7-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43fa7-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43fa7-164">Java</span><span class="sxs-lookup"><span data-stu-id="43fa7-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="43fa7-165">响应</span><span class="sxs-lookup"><span data-stu-id="43fa7-165">Response</span></span>
<span data-ttu-id="43fa7-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="43fa7-166">Here is an example of the response.</span></span>
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


