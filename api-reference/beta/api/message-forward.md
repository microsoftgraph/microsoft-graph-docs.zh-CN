---
title: 邮件：转发
description: '转发邮件、添加注释或修改任何可更新的属性  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e94f79ef5dfa45aa9a398b3261e6bc14091b2bed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992897"
---
# <a name="message-forward"></a><span data-ttu-id="19255-103">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="19255-103">message: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19255-104">转发邮件、添加注释或修改任何可更新的属性</span><span class="sxs-lookup"><span data-stu-id="19255-104">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="19255-105">一个**正向**调用中的全部。</span><span class="sxs-lookup"><span data-stu-id="19255-105">all in one **forward** call.</span></span> <span data-ttu-id="19255-106">邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="19255-106">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="19255-107">或者, 您可以先[创建一个草稿转发邮件](../api/message-createforward.md), 以包含注释或更新任何邮件属性, 然后[发送](../api/message-send.md)草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="19255-107">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="19255-108">**注意**</span><span class="sxs-lookup"><span data-stu-id="19255-108">**Note**</span></span>

- <span data-ttu-id="19255-109">您可以指定`message`参数的注释或**body**属性。</span><span class="sxs-lookup"><span data-stu-id="19255-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="19255-110">同时指定这两个将返回 HTTP 400 错误的请求错误。</span><span class="sxs-lookup"><span data-stu-id="19255-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="19255-111">您必须指定`toRecipients`参数或`message`参数的**toRecipients**属性。</span><span class="sxs-lookup"><span data-stu-id="19255-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="19255-112">同时指定或指定两者均不会返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="19255-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="19255-113">权限</span><span class="sxs-lookup"><span data-stu-id="19255-113">Permissions</span></span>
<span data-ttu-id="19255-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19255-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19255-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="19255-116">Permission type</span></span>      | <span data-ttu-id="19255-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19255-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19255-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19255-118">Delegated (work or school account)</span></span> | <span data-ttu-id="19255-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="19255-119">Mail.Send</span></span>    |
|<span data-ttu-id="19255-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19255-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19255-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="19255-121">Mail.Send</span></span>    |
|<span data-ttu-id="19255-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="19255-122">Application</span></span> | <span data-ttu-id="19255-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="19255-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="19255-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19255-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="19255-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="19255-125">Request headers</span></span>
| <span data-ttu-id="19255-126">名称</span><span class="sxs-lookup"><span data-stu-id="19255-126">Name</span></span>       | <span data-ttu-id="19255-127">类型</span><span class="sxs-lookup"><span data-stu-id="19255-127">Type</span></span> | <span data-ttu-id="19255-128">说明</span><span class="sxs-lookup"><span data-stu-id="19255-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="19255-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="19255-129">Authorization</span></span>  | <span data-ttu-id="19255-130">string</span><span class="sxs-lookup"><span data-stu-id="19255-130">string</span></span>  | <span data-ttu-id="19255-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19255-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19255-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19255-133">Content-Type</span></span> | <span data-ttu-id="19255-134">string</span><span class="sxs-lookup"><span data-stu-id="19255-134">string</span></span>  | <span data-ttu-id="19255-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="19255-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19255-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="19255-137">Request body</span></span>
<span data-ttu-id="19255-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="19255-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19255-139">参数</span><span class="sxs-lookup"><span data-stu-id="19255-139">Parameter</span></span>    | <span data-ttu-id="19255-140">类型</span><span class="sxs-lookup"><span data-stu-id="19255-140">Type</span></span>   |<span data-ttu-id="19255-141">说明</span><span class="sxs-lookup"><span data-stu-id="19255-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19255-142">注释</span><span class="sxs-lookup"><span data-stu-id="19255-142">comment</span></span>|<span data-ttu-id="19255-143">String</span><span class="sxs-lookup"><span data-stu-id="19255-143">String</span></span>|<span data-ttu-id="19255-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="19255-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="19255-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="19255-146">toRecipients</span></span>|<span data-ttu-id="19255-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="19255-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="19255-148">收件人列表</span><span class="sxs-lookup"><span data-stu-id="19255-148">The list of recipients.</span></span>|
|<span data-ttu-id="19255-149">message</span><span class="sxs-lookup"><span data-stu-id="19255-149">message</span></span>|[<span data-ttu-id="19255-150">邮件</span><span class="sxs-lookup"><span data-stu-id="19255-150">message</span></span>](../resources/message.md)|<span data-ttu-id="19255-151">答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="19255-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="19255-152">响应</span><span class="sxs-lookup"><span data-stu-id="19255-152">Response</span></span>

<span data-ttu-id="19255-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="19255-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19255-155">示例</span><span class="sxs-lookup"><span data-stu-id="19255-155">Example</span></span>
<span data-ttu-id="19255-156">下面的示例将**isDeliveryReceiptRequested**属性设置为 true, 添加注释并转发邮件。</span><span class="sxs-lookup"><span data-stu-id="19255-156">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="19255-157">请求</span><span class="sxs-lookup"><span data-stu-id="19255-157">Request</span></span>
<span data-ttu-id="19255-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19255-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="19255-159">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="19255-159">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="19255-160">C#</span><span class="sxs-lookup"><span data-stu-id="19255-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19255-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="19255-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19255-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="19255-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19255-163">Java</span><span class="sxs-lookup"><span data-stu-id="19255-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19255-164">响应</span><span class="sxs-lookup"><span data-stu-id="19255-164">Response</span></span>
<span data-ttu-id="19255-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="19255-165">Here is an example of the response.</span></span>
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
