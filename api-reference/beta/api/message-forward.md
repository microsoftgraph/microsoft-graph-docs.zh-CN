---
title: 邮件：转发
description: '转发邮件、 将注释添加或修改任何可更新的属性  '
localization_priority: Normal
ms.openlocfilehash: b601ea1152e9f5b0c5796779967393b956fd2da0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864678"
---
# <a name="message-forward"></a><span data-ttu-id="f3955-103">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="f3955-103">message: forward</span></span>

> <span data-ttu-id="f3955-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f3955-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3955-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f3955-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3955-106">转发邮件、 将注释添加或修改任何可更新的属性</span><span class="sxs-lookup"><span data-stu-id="f3955-106">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="f3955-107">全部位于一个**转接**呼叫。</span><span class="sxs-lookup"><span data-stu-id="f3955-107">all in one **forward** call.</span></span> <span data-ttu-id="f3955-108">该邮件将保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="f3955-108">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="f3955-109">此外，您可以第一个[创建草稿转发邮件](../api/message-createforward.md)包含评论或更新任何消息属性，然后[发送](../api/message-send.md)邮件草稿。</span><span class="sxs-lookup"><span data-stu-id="f3955-109">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="f3955-110">**注意**</span><span class="sxs-lookup"><span data-stu-id="f3955-110">**Note**</span></span>

- <span data-ttu-id="f3955-111">您可以指定注释或的**body**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="f3955-111">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="f3955-112">如果同时指定将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="f3955-112">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="f3955-113">必须指定`toRecipients`参数或**toRecipients**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="f3955-113">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="f3955-114">指定这两个或指定都不将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="f3955-114">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3955-115">权限</span><span class="sxs-lookup"><span data-stu-id="f3955-115">Permissions</span></span>
<span data-ttu-id="f3955-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3955-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3955-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3955-118">Permission type</span></span>      | <span data-ttu-id="f3955-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3955-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3955-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3955-120">Delegated (work or school account)</span></span> | <span data-ttu-id="f3955-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f3955-121">Mail.Send</span></span>    |
|<span data-ttu-id="f3955-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3955-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3955-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f3955-123">Mail.Send</span></span>    |
|<span data-ttu-id="f3955-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3955-124">Application</span></span> | <span data-ttu-id="f3955-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f3955-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3955-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3955-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="f3955-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3955-127">Request headers</span></span>
| <span data-ttu-id="f3955-128">名称</span><span class="sxs-lookup"><span data-stu-id="f3955-128">Name</span></span>       | <span data-ttu-id="f3955-129">类型</span><span class="sxs-lookup"><span data-stu-id="f3955-129">Type</span></span> | <span data-ttu-id="f3955-130">说明</span><span class="sxs-lookup"><span data-stu-id="f3955-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f3955-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3955-131">Authorization</span></span>  | <span data-ttu-id="f3955-132">string</span><span class="sxs-lookup"><span data-stu-id="f3955-132">string</span></span>  | <span data-ttu-id="f3955-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f3955-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3955-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f3955-135">Content-Type</span></span> | <span data-ttu-id="f3955-136">string</span><span class="sxs-lookup"><span data-stu-id="f3955-136">string</span></span>  | <span data-ttu-id="f3955-p107">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="f3955-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3955-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3955-139">Request body</span></span>
<span data-ttu-id="f3955-140">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f3955-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f3955-141">参数</span><span class="sxs-lookup"><span data-stu-id="f3955-141">Parameter</span></span>    | <span data-ttu-id="f3955-142">类型</span><span class="sxs-lookup"><span data-stu-id="f3955-142">Type</span></span>   |<span data-ttu-id="f3955-143">说明</span><span class="sxs-lookup"><span data-stu-id="f3955-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3955-144">注释</span><span class="sxs-lookup"><span data-stu-id="f3955-144">comment</span></span>|<span data-ttu-id="f3955-145">String</span><span class="sxs-lookup"><span data-stu-id="f3955-145">String</span></span>|<span data-ttu-id="f3955-p108">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="f3955-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="f3955-148">toRecipients</span><span class="sxs-lookup"><span data-stu-id="f3955-148">toRecipients</span></span>|<span data-ttu-id="f3955-149">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="f3955-149">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="f3955-150">收件人列表</span><span class="sxs-lookup"><span data-stu-id="f3955-150">The list of recipients.</span></span>|
|<span data-ttu-id="f3955-151">message</span><span class="sxs-lookup"><span data-stu-id="f3955-151">message</span></span>|[<span data-ttu-id="f3955-152">message</span><span class="sxs-lookup"><span data-stu-id="f3955-152">message</span></span>](../resources/message.md)|<span data-ttu-id="f3955-153">若要在答复邮件更新任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="f3955-153">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="f3955-154">响应</span><span class="sxs-lookup"><span data-stu-id="f3955-154">Response</span></span>

<span data-ttu-id="f3955-p109">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f3955-p109">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3955-157">示例</span><span class="sxs-lookup"><span data-stu-id="f3955-157">Example</span></span>
<span data-ttu-id="f3955-158">下面的示例将**isDeliveryReceiptRequested**属性设置为 true，添加一个批注和将邮件转发。</span><span class="sxs-lookup"><span data-stu-id="f3955-158">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="f3955-159">请求</span><span class="sxs-lookup"><span data-stu-id="f3955-159">Request</span></span>
<span data-ttu-id="f3955-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f3955-160">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f3955-161">响应</span><span class="sxs-lookup"><span data-stu-id="f3955-161">Response</span></span>
<span data-ttu-id="f3955-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f3955-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
