---
title: 邮件：转发
description: '转发邮件、 将注释添加或修改任何可更新的属性  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 18394c29d57c090811bca9a70371c451b090fb26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971485"
---
# <a name="message-forward"></a><span data-ttu-id="2f4f2-103">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="2f4f2-103">message: forward</span></span>

> <span data-ttu-id="2f4f2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f4f2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f4f2-106">转发邮件、 将注释添加或修改任何可更新的属性</span><span class="sxs-lookup"><span data-stu-id="2f4f2-106">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="2f4f2-107">全部位于一个**转接**呼叫。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-107">all in one **forward** call.</span></span> <span data-ttu-id="2f4f2-108">该邮件将保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-108">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="2f4f2-109">此外，您可以第一个[创建草稿转发邮件](../api/message-createforward.md)包含评论或更新任何消息属性，然后[发送](../api/message-send.md)邮件草稿。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-109">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="2f4f2-110">**注意**</span><span class="sxs-lookup"><span data-stu-id="2f4f2-110">**Note**</span></span>

- <span data-ttu-id="2f4f2-111">您可以指定注释或的**body**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-111">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="2f4f2-112">如果同时指定将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-112">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="2f4f2-113">必须指定`toRecipients`参数或**toRecipients**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-113">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="2f4f2-114">指定这两个或指定都不将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-114">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f4f2-115">权限</span><span class="sxs-lookup"><span data-stu-id="2f4f2-115">Permissions</span></span>
<span data-ttu-id="2f4f2-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f4f2-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f4f2-118">Permission type</span></span>      | <span data-ttu-id="2f4f2-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f4f2-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f4f2-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f4f2-120">Delegated (work or school account)</span></span> | <span data-ttu-id="2f4f2-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="2f4f2-121">Mail.Send</span></span>    |
|<span data-ttu-id="2f4f2-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f4f2-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f4f2-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="2f4f2-123">Mail.Send</span></span>    |
|<span data-ttu-id="2f4f2-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f4f2-124">Application</span></span> | <span data-ttu-id="2f4f2-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="2f4f2-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f4f2-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f4f2-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="2f4f2-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f4f2-127">Request headers</span></span>
| <span data-ttu-id="2f4f2-128">名称</span><span class="sxs-lookup"><span data-stu-id="2f4f2-128">Name</span></span>       | <span data-ttu-id="2f4f2-129">类型</span><span class="sxs-lookup"><span data-stu-id="2f4f2-129">Type</span></span> | <span data-ttu-id="2f4f2-130">说明</span><span class="sxs-lookup"><span data-stu-id="2f4f2-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f4f2-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f4f2-131">Authorization</span></span>  | <span data-ttu-id="2f4f2-132">string</span><span class="sxs-lookup"><span data-stu-id="2f4f2-132">string</span></span>  | <span data-ttu-id="2f4f2-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f4f2-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f4f2-135">Content-Type</span></span> | <span data-ttu-id="2f4f2-136">string</span><span class="sxs-lookup"><span data-stu-id="2f4f2-136">string</span></span>  | <span data-ttu-id="2f4f2-p107">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f4f2-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f4f2-139">Request body</span></span>
<span data-ttu-id="2f4f2-140">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f4f2-141">参数</span><span class="sxs-lookup"><span data-stu-id="2f4f2-141">Parameter</span></span>    | <span data-ttu-id="2f4f2-142">类型</span><span class="sxs-lookup"><span data-stu-id="2f4f2-142">Type</span></span>   |<span data-ttu-id="2f4f2-143">说明</span><span class="sxs-lookup"><span data-stu-id="2f4f2-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f4f2-144">注释</span><span class="sxs-lookup"><span data-stu-id="2f4f2-144">comment</span></span>|<span data-ttu-id="2f4f2-145">String</span><span class="sxs-lookup"><span data-stu-id="2f4f2-145">String</span></span>|<span data-ttu-id="2f4f2-p108">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="2f4f2-148">toRecipients</span><span class="sxs-lookup"><span data-stu-id="2f4f2-148">toRecipients</span></span>|<span data-ttu-id="2f4f2-149">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="2f4f2-149">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="2f4f2-150">收件人列表</span><span class="sxs-lookup"><span data-stu-id="2f4f2-150">The list of recipients.</span></span>|
|<span data-ttu-id="2f4f2-151">message</span><span class="sxs-lookup"><span data-stu-id="2f4f2-151">message</span></span>|[<span data-ttu-id="2f4f2-152">message</span><span class="sxs-lookup"><span data-stu-id="2f4f2-152">message</span></span>](../resources/message.md)|<span data-ttu-id="2f4f2-153">若要在答复邮件更新任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-153">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="2f4f2-154">响应</span><span class="sxs-lookup"><span data-stu-id="2f4f2-154">Response</span></span>

<span data-ttu-id="2f4f2-p109">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-p109">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f4f2-157">示例</span><span class="sxs-lookup"><span data-stu-id="2f4f2-157">Example</span></span>
<span data-ttu-id="2f4f2-158">下面的示例将**isDeliveryReceiptRequested**属性设置为 true，添加一个批注和将邮件转发。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-158">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="2f4f2-159">请求</span><span class="sxs-lookup"><span data-stu-id="2f4f2-159">Request</span></span>
<span data-ttu-id="2f4f2-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-160">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2f4f2-161">响应</span><span class="sxs-lookup"><span data-stu-id="2f4f2-161">Response</span></span>
<span data-ttu-id="2f4f2-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2f4f2-162">Here is an example of the response.</span></span>
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
