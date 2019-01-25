---
title: 邮件：转发
description: '转发邮件、 将注释添加或修改任何可更新的属性  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ed3d51c28e6fe0404b5cb26fb17f6d8ed3bba212
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508886"
---
# <a name="message-forward"></a><span data-ttu-id="07a13-103">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="07a13-103">message: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07a13-104">转发邮件、 将注释添加或修改任何可更新的属性</span><span class="sxs-lookup"><span data-stu-id="07a13-104">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="07a13-105">全部位于一个**转接**呼叫。</span><span class="sxs-lookup"><span data-stu-id="07a13-105">all in one **forward** call.</span></span> <span data-ttu-id="07a13-106">该邮件将保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="07a13-106">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="07a13-107">此外，您可以第一个[创建草稿转发邮件](../api/message-createforward.md)包含评论或更新任何消息属性，然后[发送](../api/message-send.md)邮件草稿。</span><span class="sxs-lookup"><span data-stu-id="07a13-107">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="07a13-108">**注意**</span><span class="sxs-lookup"><span data-stu-id="07a13-108">**Note**</span></span>

- <span data-ttu-id="07a13-109">您可以指定注释或的**body**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="07a13-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="07a13-110">如果同时指定将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="07a13-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="07a13-111">必须指定`toRecipients`参数或**toRecipients**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="07a13-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="07a13-112">指定这两个或指定都不将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="07a13-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="07a13-113">权限</span><span class="sxs-lookup"><span data-stu-id="07a13-113">Permissions</span></span>
<span data-ttu-id="07a13-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07a13-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07a13-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="07a13-116">Permission type</span></span>      | <span data-ttu-id="07a13-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07a13-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07a13-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07a13-118">Delegated (work or school account)</span></span> | <span data-ttu-id="07a13-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="07a13-119">Mail.Send</span></span>    |
|<span data-ttu-id="07a13-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07a13-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07a13-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="07a13-121">Mail.Send</span></span>    |
|<span data-ttu-id="07a13-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="07a13-122">Application</span></span> | <span data-ttu-id="07a13-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="07a13-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="07a13-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07a13-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="07a13-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="07a13-125">Request headers</span></span>
| <span data-ttu-id="07a13-126">名称</span><span class="sxs-lookup"><span data-stu-id="07a13-126">Name</span></span>       | <span data-ttu-id="07a13-127">类型</span><span class="sxs-lookup"><span data-stu-id="07a13-127">Type</span></span> | <span data-ttu-id="07a13-128">说明</span><span class="sxs-lookup"><span data-stu-id="07a13-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="07a13-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="07a13-129">Authorization</span></span>  | <span data-ttu-id="07a13-130">string</span><span class="sxs-lookup"><span data-stu-id="07a13-130">string</span></span>  | <span data-ttu-id="07a13-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07a13-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="07a13-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="07a13-133">Content-Type</span></span> | <span data-ttu-id="07a13-134">string</span><span class="sxs-lookup"><span data-stu-id="07a13-134">string</span></span>  | <span data-ttu-id="07a13-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="07a13-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07a13-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="07a13-137">Request body</span></span>
<span data-ttu-id="07a13-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="07a13-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="07a13-139">参数</span><span class="sxs-lookup"><span data-stu-id="07a13-139">Parameter</span></span>    | <span data-ttu-id="07a13-140">类型</span><span class="sxs-lookup"><span data-stu-id="07a13-140">Type</span></span>   |<span data-ttu-id="07a13-141">说明</span><span class="sxs-lookup"><span data-stu-id="07a13-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07a13-142">注释</span><span class="sxs-lookup"><span data-stu-id="07a13-142">comment</span></span>|<span data-ttu-id="07a13-143">String</span><span class="sxs-lookup"><span data-stu-id="07a13-143">String</span></span>|<span data-ttu-id="07a13-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="07a13-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="07a13-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="07a13-146">toRecipients</span></span>|<span data-ttu-id="07a13-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="07a13-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="07a13-148">收件人列表</span><span class="sxs-lookup"><span data-stu-id="07a13-148">The list of recipients.</span></span>|
|<span data-ttu-id="07a13-149">message</span><span class="sxs-lookup"><span data-stu-id="07a13-149">message</span></span>|[<span data-ttu-id="07a13-150">message</span><span class="sxs-lookup"><span data-stu-id="07a13-150">message</span></span>](../resources/message.md)|<span data-ttu-id="07a13-151">若要在答复邮件更新任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="07a13-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="07a13-152">响应</span><span class="sxs-lookup"><span data-stu-id="07a13-152">Response</span></span>

<span data-ttu-id="07a13-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="07a13-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07a13-155">示例</span><span class="sxs-lookup"><span data-stu-id="07a13-155">Example</span></span>
<span data-ttu-id="07a13-156">下面的示例将**isDeliveryReceiptRequested**属性设置为 true，添加一个批注和将邮件转发。</span><span class="sxs-lookup"><span data-stu-id="07a13-156">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="07a13-157">请求</span><span class="sxs-lookup"><span data-stu-id="07a13-157">Request</span></span>
<span data-ttu-id="07a13-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07a13-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="07a13-159">响应</span><span class="sxs-lookup"><span data-stu-id="07a13-159">Response</span></span>
<span data-ttu-id="07a13-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="07a13-160">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/message-forward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
